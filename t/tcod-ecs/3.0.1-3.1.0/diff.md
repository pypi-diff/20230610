# Comparing `tmp/tcod_ecs-3.0.1.tar.gz` & `tmp/tcod_ecs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-3.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-3.0.1.tar` & `tcod_ecs-3.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/LICENSE
--rw-r--r--   0        0        0     8627 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/README.md
--rw-r--r--   0        0        0     3688 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/pyproject.toml
--rw-r--r--   0        0        0    35784 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/tcod/ecs/__init__.py
--rw-r--r--   0        0        0      160 2023-06-04 11:34:26.389237 tcod_ecs-3.0.1/tcod/ecs/_version.py
--rw-r--r--   0        0        0        0 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/tcod/ecs/py.typed
--rw-r--r--   0        0        0     9822 1970-01-01 00:00:00.000000 tcod_ecs-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-10 15:18:27.842121 tcod_ecs-3.1.0/LICENSE
+-rw-r--r--   0        0        0     8465 2023-06-10 15:18:27.842121 tcod_ecs-3.1.0/README.md
+-rw-r--r--   0        0        0     3708 2023-06-10 15:18:27.842121 tcod_ecs-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    37039 2023-06-10 15:18:27.846121 tcod_ecs-3.1.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-10 15:18:39.870181 tcod_ecs-3.1.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0        0 2023-06-10 15:18:27.846121 tcod_ecs-3.1.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     9660 1970-01-01 00:00:00.000000 tcod_ecs-3.1.0/PKG-INFO
```

### Comparing `tcod_ecs-3.0.1/LICENSE` & `tcod_ecs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.0.1/README.md` & `tcod_ecs-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,15 @@
 >>> @attrs.define
 ... class Vector2:
 ...     x: int = 0
 ...     y: int = 0
 >>> entity.components[Vector2] = Vector2(1, 2)
 >>> entity.components[Vector2]
 Vector2(x=1, y=2)
->>> entity.components.set(Vector2(3, 4))  # Shorter syntax derives the type from the value when assigning a component.
->>> entity.components[Vector2]
-Vector2(x=3, y=4)
->>> entity.components.update_values([11, Vector2(0, 0)])  # Multiple values can be assigned without keys.
+>>> entity.components.update({int: 11, Vector2: Vector2(0, 0)})  # Multiple values can be assigned like a dict.
 >>> entity.components[int]
 11
 >>> entity.components[Vector2]
 Vector2(x=0, y=0)
 
 # Queries can be made on all entities of a world with matching components.
 >>> for e in world.Q.all_of(components=[Vector2]):
```

### Comparing `tcod_ecs-3.0.1/pyproject.toml` & `tcod_ecs-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 warn_return_any = true
 no_implicit_reexport = true
 strict_equality = true
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 required_plugins = ["pytest-cov>=4.0.0", "pytest-benchmark>=4.0.0"]
-addopts = "--doctest-modules --cov=tcod --cov-report=term-missing --doctest-glob=*.md"
+addopts = "--doctest-modules --cov=tcod --cov-report=term-missing --doctest-glob=*.md --benchmark-disable"
 testpaths = ["."]
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html
 exclude_lines = ['^\s*\.\.\.', "if TYPE_CHECKING:"]
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules/
```

### Comparing `tcod_ecs-3.0.1/tcod/ecs/__init__.py` & `tcod_ecs-3.1.0/tcod/ecs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,24 @@
 _T4 = TypeVar("_T4")
 _T5 = TypeVar("_T5")
 _ComponentKey = Union[Type[T], Tuple[object, Type[T]]]
 """ComponentKey is plain `type` or tuple `(tag, type)`."""
 
 
 def abstract_component(cls: type[T]) -> type[T]:
-    """Register class `cls` as an abstract component and return it."""
+    """Register class `cls` as an abstract component and return it.
+
+    .. deprecated:: 3.1
+        This decorator is deprecated since abstract components should always be explicit.
+    """
+    warnings.warn(
+        "This decorator is deprecated since abstract components should always be explicit.",
+        FutureWarning,
+        stacklevel=2,
+    )
     cls._TCOD_BASE_COMPONENT = cls  # type: ignore[attr-defined]
     return cls
 
 
 _entity_table: WeakKeyDictionary[World, WeakValueDictionary[object, Entity]] = WeakKeyDictionary()
 """A weak table of worlds and unique identifiers to entity objects.
 
@@ -61,17 +70,19 @@
 
 class Entity:
     """A unique entity in a world.
 
     Example::
 
         >>> import tcod.ecs
-        >>> world = tcod.ecs.World()  # Create a new world.
-        >>> entity = world.new_entity(name="entity")  # Create a new entity, name is optional.
-        >>> other_entity = world.new_entity(name="other_entity")
+        >>> world = tcod.ecs.World()  # Create a new world
+        >>> world.new_entity()  # Create a new entity
+        <Entity(uid=object at ...)>
+        >>> entity = world["entity"]  # Get an entity from a specific identifier
+        >>> other_entity = world["other"]
     """  # Changes here should be reflected in conftest.py.
 
     __slots__ = ("world", "uid", "__weakref__")
 
     world: Final[World]  # type:ignore[misc]  # https://github.com/python/mypy/issues/5774
     """The :any:`World` this entity belongs to."""
     uid: Final[object]  # type:ignore[misc]
@@ -121,31 +132,31 @@
             >>> entity.components[str] = "foo"  # Assign component.
             >>> entity.components[("name", str)] = "my_name" # Assign named component.
             >>> ("name", str) in entity.components
             True
             >>> {str, ("name", str)}.issubset(entity.components.keys())
             True
             >>> list(world.Q.all_of(components=[str]))  # Query components.
-            [<Entity name='entity'>]
+            [<Entity(uid='entity')>]
             >>> list(world.Q[tcod.ecs.Entity, str, ("name", str)])  # Query zip components.
-            [(<Entity name='entity'>, 'foo', 'my_name')]
+            [(<Entity(uid='entity')>, 'foo', 'my_name')]
         """
         return EntityComponents(self)
 
     @property
     def tags(self) -> EntityTags:
         """Access an entities tags.
 
         Example::
 
             >>> entity.tags.add("tag") # Add tag.
             >>> "tag" in entity.tags  # Check tag.
             True
             >>> list(world.Q.all_of(tags=["tag"]))  # Query tags.
-            [<Entity name='entity'>]
+            [<Entity(uid='entity')>]
             >>> entity.tags.discard("tag")
         """
         return EntityTags(self)
 
     @property
     def relation_components(self) -> EntityComponentRelations:
         """Access an entities relation components.
@@ -153,82 +164,91 @@
         Example::
 
             >>> entity.relation_components[str][other_entity] = "foo" # Assign component to relation.
             >>> entity.relation_components[("distance", int)][other_entity] = 42 # Also works for named components.
             >>> other_entity in entity.relation_components[str]
             True
             >>> list(world.Q.all_of(relations=[(str, other_entity)]))
-            [<Entity name='entity'>]
+            [<Entity(uid='entity')>]
             >>> list(world.Q.all_of(relations=[(str, ...)]))
-            [<Entity name='entity'>]
+            [<Entity(uid='entity')>]
             >>> list(world.Q.all_of(relations=[(entity, str, None)]))
-            [<Entity name='other_entity'>]
+            [<Entity(uid='other')>]
             >>> list(world.Q.all_of(relations=[(..., str, None)]))
-            [<Entity name='other_entity'>]
+            [<Entity(uid='other')>]
         """
         return EntityComponentRelations(self)
 
     @property
     def relation_tags(self) -> EntityRelationsExclusive:
         """Access an entities exclusive relations.
 
         Example::
 
             >>> entity.relation_tags["ChildOf"] = other_entity  # Assign relation.
             >>> list(world.Q.all_of(relations=[("ChildOf", other_entity)]))  # Get children of other_entity.
-            [<Entity name='entity'>]
+            [<Entity(uid='entity')>]
             >>> list(world.Q.all_of(relations=[(entity, "ChildOf", None)]))  # Get parents of entity.
-            [<Entity name='other_entity'>]
+            [<Entity(uid='other')>]
             >>> del entity.relation_tags["ChildOf"]
         """
         return EntityRelationsExclusive(self)
 
     @property
     def relation_tags_many(self) -> EntityRelations:
         """Access an entities many-to-many relations.
 
         Example::
 
             >>> entity.relation_tags_many["KnownBy"].add(other_entity)  # Assign relation.
         """
         return EntityRelations(self)
 
-    @property
-    def name(self) -> object:
-        """The unique name of this entity or None.
-
-        You may assign a new name, but if an entity of the world already has that name then it will lose it.
-        """
-        return self.world._names_by_entity.get(self)
-
-    @name.setter
-    def name(self, value: object) -> None:
+    def _set_name(self, value: object, stacklevel: int = 1) -> None:
+        warnings.warn(
+            "The name feature has been deprecated and will be removed.",
+            FutureWarning,
+            stacklevel=stacklevel + 1,
+        )
         old_name = self.name
         if old_name is not None:  # Remove self from names.
             del self.world._names_by_name[old_name]
             del self.world._names_by_entity[self]
 
         if value is not None:  # Add self to names.
             old_entity = self.world._names_by_name.get(value)
             if old_entity is not None:  # Remove entity with old name, name will be overwritten.
                 del self.world._names_by_entity[old_entity]
             self.world._names_by_name[value] = self
             self.world._names_by_entity[self] = value
 
+    @property
+    def name(self) -> object:
+        """The unique name of this entity or None.
+
+        You may assign a new name, but if an entity of the world already has that name then it will lose it.
+
+        .. deprecated:: 3.1
+            This feature has been deprecated.
+        """
+        return self.world._names_by_entity.get(self)
+
+    @name.setter
+    def name(self, value: object) -> None:
+        self._set_name(value, stacklevel=2)
+
     def __repr__(self) -> str:
         """Return a representation of this entity.
 
         Example::
 
             >>> world.new_entity()
             <Entity(uid=object at ...)>
             >>> world["foo"]
             <Entity(uid='foo')>
-            >>> world.new_entity(name="foo")
-            <Entity name='foo'>
         """
         uid_str = f"object at 0x{id(self.uid):X}" if self.uid.__class__ == object else repr(self.uid)
         items = [f"{self.__class__.__name__}(uid={uid_str})"]
         name = self.name
         if name is not None:  # Switch to older style.
             items = [self.__class__.__name__, f"name={name!r}"]
         return f"<{' '.join(items)}>"
@@ -254,16 +274,25 @@
 
     __slots__ = ("entity",)
 
     def __init__(self, entity: Entity) -> None:
         """Initialize this attribute for the given entity."""
         self.entity: Final = entity
 
-    def set(self, value: object) -> None:
-        """Assign or overwrite a component, automatically deriving the key."""
+    def set(self, value: object, *, _stacklevel: int = 1) -> None:
+        """Assign or overwrite a component, automatically deriving the key.
+
+        .. deprecated:: 3.1
+            Setting values without an explicit key has been deprecated.
+        """
+        warnings.warn(
+            "Setting values without an explicit key has been deprecated.",
+            FutureWarning,
+            stacklevel=_stacklevel + 1,
+        )
         key = getattr(value, "_TCOD_BASE_COMPONENT", value.__class__)
         self[key] = value
 
     @staticmethod
     def __assert_key(key: _ComponentKey[Any]) -> bool:
         """Verify that abstract classes are accessed correctly."""
         if isinstance(key, tuple):
@@ -304,31 +333,32 @@
         """Iterate over the component types belonging to this entity."""
         return iter(self.entity.world._components_by_entity.get(self.entity, ()))
 
     def __len__(self) -> int:
         """Return the number of components belonging to this entity."""
         return len(self.entity.world._components_by_entity.get(self.entity, ()))
 
-    def update_values(self, values: Iterable[object]) -> None:
-        """Add or overwrite multiple components inplace, deriving the keys from the values."""
+    def update_values(self, values: Iterable[object], *, _stacklevel: int = 1) -> None:
+        """Add or overwrite multiple components inplace, deriving the keys from the values.
+
+        .. deprecated:: 3.1
+            Setting values without an explicit key has been deprecated.
+        """
         for value in values:
-            self.set(value)
+            self.set(value, _stacklevel=_stacklevel + 1)
 
     def by_name_type(self, name_type: type[_T1], component_type: type[_T2]) -> Iterator[tuple[_T1, type[_T2]]]:
         """Iterate over all of an entities component keys with a specific (name_type, component_type) combination.
 
-        .. versionadded:: 3.0.0
+        .. versionadded:: 3.0
 
-        Example::
-
-            >>> entity.components["A", int] = 1
-            >>> entity.components["B", int] = 2
-            >>> sorted(entity.components.by_name_type(str, int))
-            [('A', <class 'int'>), ('B', <class 'int'>)]
+        .. deprecated:: 3.1
+            This method has been deprecated. Iterate over items instead.
         """
+        warnings.warn("This method has been deprecated. Iterate over items instead.", FutureWarning, stacklevel=2)
         # Naive implementation until I feel like optimizing it.
         for key in self:
             if not isinstance(key, tuple):
                 continue
             key_name, key_component = key
             if key_component is component_type and isinstance(key_name, name_type):
                 yield key_name, key_component
@@ -759,42 +789,55 @@
         assert uid is not object, "This is reserved."
         return Entity(self, uid)
 
     @property
     def named(self) -> Mapping[object, Entity]:
         """A view into this worlds named entities.
 
-        Example::
-
-            >>> entity = world.new_entity(name="MyEntity")  # Name is optional and can be any hashable, not just str.
-            >>> entity
-            <Entity name='MyEntity'>
-            >>> entity.world is world  # Worlds can always be accessed from their entity.
-            True
-            >>> world.named["MyEntity"]  # Named entities can be accessed with `World.named`.
-            <Entity name='MyEntity'>
-            >>> world.named.get("Missing") is None  # `World.named` acts like a dictionary, including assignment and `.get()`.
-            True
+        .. deprecated:: 3.1
+            This feature has been deprecated.
         """
         return self._names_by_name
 
     def new_entity(
         self,
-        components: Iterable[object] = (),
+        components: Iterable[object] | Mapping[_ComponentKey[object], object] = (),
         *,
         name: object = None,
         tags: Iterable[Any] = (),
     ) -> Entity:
-        """Create and return a new entity."""
+        """Create and return a new entity.
+
+        .. versionchanged:: 3.1
+            `components` can now take a mapping.
+
+        Example::
+
+            >>> entity = world.new_entity(
+            ...     components={
+            ...         ("name", str): "my name",
+            ...         ("hp", int): 10,
+            ...     },
+            ...     tags=["Actor"],
+            ... )
+            >>> entity.components[("name", str)]
+            'my name'
+            >>> "Actor" in entity.tags
+            True
+        """
         entity = Entity(self)
-        entity.components.update_values(components)
+        if isinstance(components, Mapping):
+            entity.components.update(components)
+        elif components:
+            entity.components.update_values(components, _stacklevel=2)
         entity_tags = entity.tags
         for tag in tags:
             entity_tags.add(tag)
-        entity.name = name
+        if name is not None:
+            entity._set_name(name, stacklevel=2)
         return entity
 
     @property
     def Q(self) -> Query:
         """Start a new Query for this world.
 
         Alias for ``tcod.ecs.Query(world)``.
```

### Comparing `tcod_ecs-3.0.1/PKG-INFO` & `tcod_ecs-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 3.0.1
+Version: 3.1.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -129,18 +129,15 @@
 >>> @attrs.define
 ... class Vector2:
 ...     x: int = 0
 ...     y: int = 0
 >>> entity.components[Vector2] = Vector2(1, 2)
 >>> entity.components[Vector2]
 Vector2(x=1, y=2)
->>> entity.components.set(Vector2(3, 4))  # Shorter syntax derives the type from the value when assigning a component.
->>> entity.components[Vector2]
-Vector2(x=3, y=4)
->>> entity.components.update_values([11, Vector2(0, 0)])  # Multiple values can be assigned without keys.
+>>> entity.components.update({int: 11, Vector2: Vector2(0, 0)})  # Multiple values can be assigned like a dict.
 >>> entity.components[int]
 11
 >>> entity.components[Vector2]
 Vector2(x=0, y=0)
 
 # Queries can be made on all entities of a world with matching components.
 >>> for e in world.Q.all_of(components=[Vector2]):
```

