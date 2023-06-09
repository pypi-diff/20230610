# Comparing `tmp/mongoclasses-0.1.0.tar.gz` & `tmp/mongoclasses-0.2.0.tar.gz`

## Comparing `mongoclasses-0.1.0.tar` & `mongoclasses-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/src/mongoclasses/__about__.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/src/mongoclasses/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/tests/test_mongoclasses.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/.python-version
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/src/mongoclasses/__about__.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/src/mongoclasses/__init__.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/tests/test_fromdict.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/tests/test_mongoclass.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/tests/test_mongoclass_instances.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/PKG-INFO
```

### Comparing `mongoclasses-0.1.0/src/mongoclasses/__init__.py` & `mongoclasses-0.2.0/src/mongoclasses/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,91 @@
-from collections.abc import Callable, Iterable
 from dataclasses import asdict, dataclass, fields, is_dataclass
 import inspect
+from typing import (
+    Any, Callable, Dict, List, Optional, Type, TypeVar, Union
+)
 
 from motor.motor_asyncio import AsyncIOMotorCursor, AsyncIOMotorDatabase
 from pymongo.results import DeleteResult, InsertOneResult, UpdateResult
 
 
 __all__ = [
     "fromdict",
-    "include",
     "mongoclass",
     "is_mongoclass",
     "insert_one",
     "update_one",
     "delete_one",
     "find_one",
-    "find"
+    "find",
 ]
 
+
+T = TypeVar("T")
+
+
 _COLLECTION = "__mongoclasses_collection__"
 
 
-def fromdict(cls, data: dict):
+def fromdict(cls: Type[T], data: Dict[str, Any]) -> T:
     """
     Attempts to create a dataclass instance from a dictionary.
     """
     if not is_dataclass(cls):
         raise TypeError("Object must be a dataclass type.")
 
     if not inspect.isclass(cls):
         raise TypeError("Object must be a dataclass type.")
 
+    # initialize object.
     sig = inspect.signature(cls)
-    param_names = (param for param in sig.parameters)
-    init_kwargs = {param: data[param] for param in param_names if param in data}
-    obj = cls(**init_kwargs)
-
-    field_names = set(f.name for f in fields(cls))
-    non_init_fields = field_names.difference(param_names)
-
-    for field in non_init_fields:
-        if field not in data:
-            continue
-        setattr(obj, field, data[field])
+    init_data = {p: data[p] for p in sig.parameters if p in data}
+    ba = sig.bind(**init_data)
+    obj = cls(*ba.args, **ba.kwargs)
+
+    # Add remaining fields (if any) using setattr.
+    non_init_fields = (f.name for f in fields(cls) if f.name not in sig.parameters)
+    non_init_data = ((f, data[f]) for f in non_init_fields if f in data)
+    for field, value in non_init_data:
+        setattr(obj, field, value)
 
     return obj
 
 
-def include(fields: Iterable[str]) -> Callable[[Iterable], dict]:
-    """
-    Returns a dict_factory that will include the fields.
-    """
-
-    def include_dict_factory(iterable: Iterable) -> dict:
-        return {k: v for k, v in iterable if k in fields}
-
-    return include_dict_factory
-
-
 def mongoclass(
-    cls=None,
-    /,
+    cls: Optional[Type[T]] = None,
     *,
-    db: AsyncIOMotorDatabase | None = None,
+    db: Optional[AsyncIOMotorDatabase] = None,
     collection_name: str = "",
-    **kwargs,
-):
-    def wrap(cls):
+    **kwargs: Any,
+) -> Union[Type[T], Callable[[Type[T]], Type[T]]]:
+    def wrap(cls: Type[T]) -> Type[T]:
         return _process_class(cls, db, collection_name, kwargs)
 
     # See if we're being called as @dataclass or @dataclass().
     if cls is None:
         # We're called with parens.
         return wrap
 
     # We're called as @dataclass without parens.
     return wrap(cls)
 
 
-def _process_class(cls, db, collection_name, dataclass_kwargs):
+def _process_class(
+    cls: Type[T],
+    db: AsyncIOMotorDatabase,
+    collection_name: str,
+    dataclass_kwargs: Dict[str, Any],
+) -> Type[T]:
     # If the class is not a dataclass, make it a dataclass.
     if not is_dataclass(cls):
         cls = dataclass(**dataclass_kwargs)(cls)
 
     if not any(f.name == "_id" for f in fields(cls)):
-        raise AttributeError("Missing '_id' field.")
+        raise AttributeError("Missing required field '_id'.")
 
     # get parent db if db is None.
     if db is None:
         for base in reversed(cls.mro()):
             if not _is_mongoclass_type(base):
                 continue
             db = getattr(base, _COLLECTION).database
@@ -98,83 +95,89 @@
 
     collection_name = collection_name or cls.__name__.lower()
     collection = db[collection_name]
     setattr(cls, _COLLECTION, collection)
     return cls
 
 
-def is_mongoclass(obj):
+def is_mongoclass(obj) -> bool:
     """
     Returns True if the obj is a a mongoclass or an instance of
     a mongoclass.
     """
     cls = obj if inspect.isclass(obj) else type(obj)
     return hasattr(cls, _COLLECTION)
 
 
-def _is_mongoclass_type(obj):
+def _is_mongoclass_type(obj) -> bool:
     return hasattr(obj, _COLLECTION) and inspect.isclass(obj)
 
 
-def _is_mongoclass_instance(obj):
+def _is_mongoclass_instance(obj) -> bool:
     """
     Returns True if the obj is an instance of a mongoclass.
     """
     return hasattr(type(obj), _COLLECTION)
 
 
-async def insert_one(obj, /) -> InsertOneResult:
+async def insert_one(obj) -> InsertOneResult:
     if not _is_mongoclass_instance(obj):
         raise TypeError("Object must be a mongoclass instance.")
 
     document = asdict(obj)
     if document["_id"] is None:
         del document["_id"]
 
     collection = getattr(obj, _COLLECTION)
-    result = await collection.insert_one(document)
+    result: InsertOneResult = await collection.insert_one(document)
     obj._id = result.inserted_id
     return result
 
 
-async def update_one(obj, /, fields: Iterable[str] | None = None) -> UpdateResult:
+async def update_one(obj, fields: Optional[List[str]] = None) -> UpdateResult:
     if not _is_mongoclass_instance(obj):
         raise TypeError("Object must be a mongoclass instance.")
 
-    dict_factory = include(fields) if fields else dict
-    document = asdict(obj, dict_factory=dict_factory)
+    document = asdict(obj)
+    if fields is not None:
+        document = {k: v for k, v in document.items() if k in fields}
+
     collection = getattr(obj, _COLLECTION)
     return await collection.update_one(
         filter={"_id": obj._id}, update={"$set": document}
     )
 
 
-async def delete_one(obj, /) -> DeleteResult:
+async def delete_one(obj) -> DeleteResult:
     if not _is_mongoclass_instance(obj):
         raise TypeError("Object must be a mongoclass instance.")
 
     collection = getattr(obj, _COLLECTION)
     return await collection.delete_one({"_id": obj._id})
 
 
-async def find_one(cls, query):
+async def find_one(
+    cls: Type[T],
+    query: Dict[str, Any],
+    fromdict: Callable[[Type[T], Dict[str, Any]], T] = fromdict
+) -> Optional[T]:
     """
     Return a single instance that matches the query on the mongoclass or None.
     """
     if not _is_mongoclass_type(cls):
         raise TypeError("Must be called with a mongoclass type.")
 
     collection = getattr(cls, _COLLECTION)
     document = await collection.find_one(query)
     if document is None:
         return None
     return fromdict(cls, document)
 
 
-def find(cls, query) -> AsyncIOMotorCursor:
+def find(cls: Type[T], query: Dict[str, Any]) -> AsyncIOMotorCursor:
     """
     Performs a query on the mongoclass.
     Returns a DocumentCursor.
     """
     if not _is_mongoclass_type(cls):
         raise TypeError("Must be called with a mongoclass type.")
```

### Comparing `mongoclasses-0.1.0/tests/test_mongoclasses.py` & `mongoclasses-0.2.0/tests/test_mongoclass_instances.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,82 @@
-from dataclasses import dataclass, asdict
+from dataclasses import asdict
+from typing import Optional
 
 from bson import ObjectId
 import pytest
 import pytest_asyncio
 from motor.motor_asyncio import AsyncIOMotorClient
 
 from mongoclasses import (
-    mongoclass, insert_one, update_one, delete_one, find_one, find, fromdict
+    delete_one, find, find_one, fromdict, insert_one, mongoclass, update_one
 )
 
 
 @pytest_asyncio.fixture
 async def database():
     client = AsyncIOMotorClient()
     await client.drop_database('test')
     return client['test']
 
 
 @pytest.fixture
 def Foo(database):
     @mongoclass(db=database)
     class Foo:
-        _id: ObjectId | None = None
+        _id: Optional[ObjectId] = None
         name: str = ""
+        description: str = ""
 
     return Foo
 
 
-def test_mongoclass_creation(database):
-    # Missing a database.
-    with pytest.raises(RuntimeError):
-        @mongoclass
-        class Foo:
-            _id: ObjectId | None = None
-
-    # Missing an _id field.
-    with pytest.raises(AttributeError):
-        @mongoclass(db=database)
-        class Foo:
-            ...
-
-    # Valid mongoclass
-    @mongoclass(db=database)
-    class Foo:
-        _id: ObjectId | None = None
-    
-    assert Foo.__mongoclasses_collection__.database == database
-    assert Foo.__mongoclasses_collection__.name == 'foo'
-
-    # Mongoclass being created from an already existing dataclass.
-    @dataclass
-    class Foo:
-        _id: ObjectId | None = None
-    
-    Foo = mongoclass(db=database)(Foo)
-    
-    assert Foo.__mongoclasses_collection__.database == database
-    assert Foo.__mongoclasses_collection__.name == 'foo'
-
-
-def test_mongoclass_collection_name(database):
-    @mongoclass(db=database, collection_name='foobar')
-    class Foo:
-        _id: ObjectId | None = None
-    
-    assert Foo.__mongoclasses_collection__.name == 'foobar'
-
-
-def test_database_inheritance(database):
-
-    @mongoclass(db=database)
-    class Foo:
-        _id: ObjectId | None = None
-
-    @mongoclass
-    class Bar(Foo):
-        ...
+@pytest.mark.asyncio
+async def test_insert_one_without_id(Foo, database):    
+    f = Foo()
+    await insert_one(f)
 
-    assert Foo.__mongoclasses_collection__.database == database
-    assert Bar.__mongoclasses_collection__.database == database
+    assert f._id is not None
+    assert await database['foo'].find_one({'_id': f._id}) is not None
 
 
 @pytest.mark.asyncio
-async def test_insert_one(Foo, database):    
-    f = Foo()
+async def test_insert_one_with_id(Foo, database):  
+    # test scenario where an _id is generated before insertion.  
+    object_id = ObjectId()
+    f = Foo(_id=object_id)
     await insert_one(f)
 
-    assert f._id is not None
+    assert f._id == object_id
     assert await database['foo'].find_one({'_id': f._id}) is not None
 
 
 @pytest.mark.asyncio
 async def test_update_one(Foo, database):    
     f = Foo()
     await insert_one(f)
 
     f.name = "Fred"
     await update_one(f)
     
     doc = await database['foo'].find_one({"_id": f._id})
     assert doc["name"] == "Fred"
+
+
+@pytest.mark.asyncio
+async def test_update_one_with_fields(Foo, database):    
+    f = Foo()
+    await insert_one(f)
+
+    f.name = "Fred"
+    f.description = "foobar"
+    await update_one(f, fields=["description"])
+    
+    doc = await database['foo'].find_one({"_id": f._id})
+    assert doc["name"] == ""
+    assert doc["description"] == "foobar"
     
 
 @pytest.mark.asyncio
 async def test_delete_one(Foo, database):    
     f = Foo()
     await insert_one(f)
     await delete_one(f)
@@ -133,19 +106,16 @@
     f2 = Foo(name="Bob")
     await insert_one(f2)
 
     f3 = Foo(name="Charlie")
     await insert_one(f3)
 
     cursor = find(Foo, {})
-    l = []
-    async for foo in cursor:
-        l.append(foo)
-
-    assert len(l) == 3
+    objects = [foo async for foo in cursor]
+    assert len(objects) == 3
 
 
 @pytest.mark.asyncio
 async def test_fromdict(Foo):
     f1 = Foo()
     f2 = fromdict(Foo, asdict(f1))
     assert f1 == f2
```

### Comparing `mongoclasses-0.1.0/.gitignore` & `mongoclasses-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.1.0/LICENSE.txt` & `mongoclasses-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.1.0/pyproject.toml` & `mongoclasses-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "mongoclasses"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Ryan Kroon", email = "rykroon.tech@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  # "Programming Language :: Python :: 3.7",
-  # "Programming Language :: Python :: 3.8",
-  # "Programming Language :: Python :: 3.9",
-  # "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "motor==3.1.*"
 ]
@@ -51,15 +51,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.11"]
+python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 [tool.coverage.run]
 source_pkgs = ["mongoclasses", "tests"]
 branch = true
 parallel = true
 omit = [
   "src/mongoclasses/__about__.py",
```

### Comparing `mongoclasses-0.1.0/PKG-INFO` & `mongoclasses-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: mongoclasses
-Version: 0.1.0
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/rykroon/mongoclasses#readme
 Project-URL: Issues, https://github.com/rykroon/mongoclasses/issues
 Project-URL: Source, https://github.com/rykroon/mongoclasses
 Author-email: Ryan Kroon <rykroon.tech@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Requires-Dist: motor==3.1.*
 Description-Content-Type: text/markdown
 
 # mongoclasses
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mongoclasses.svg)](https://pypi.org/project/mongoclasses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mongoclasses.svg)](https://pypi.org/project/mongoclasses)
```

