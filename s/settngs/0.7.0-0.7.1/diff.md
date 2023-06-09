# Comparing `tmp/settngs-0.7.0.tar.gz` & `tmp/settngs-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settngs-0.7.0.tar", last modified: Fri Jun  9 06:04:07 2023, max compression
+gzip compressed data, was "settngs-0.7.1.tar", last modified: Fri Jun  9 22:56:10 2023, max compression
```

## Comparing `settngs-0.7.0.tar` & `settngs-0.7.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.426365 settngs-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.418365 settngs-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-09 06:03:46.000000 settngs-0.7.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-09 06:03:46.000000 settngs-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-09 06:03:46.000000 settngs-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-09 06:03:46.000000 settngs-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 06:04:07.426365 settngs-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-09 06:03:46.000000 settngs-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-09 06:03:46.000000 settngs-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:03:46.000000 settngs-0.7.0/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/settngs/
--rw-r--r--   0 runner    (1001) docker     (123)    33397 2023-06-09 06:03:46.000000 settngs-0.7.0/settngs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 06:03:46.000000 settngs-0.7.0/settngs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:03:46.000000 settngs-0.7.0/settngs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/settngs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-09 06:04:07.426365 settngs-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 06:03:46.000000 settngs-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:03:46.000000 settngs-0.7.0/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-06-09 06:03:46.000000 settngs-0.7.0/testing/settngs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.426365 settngs-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:03:46.000000 settngs-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-06-09 06:03:46.000000 settngs-0.7.0/tests/settngs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.426365 settngs-0.7.0/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-09 06:03:46.000000 settngs-0.7.0/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-09 06:03:46.000000 settngs-0.7.0/workflows/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.301996 settngs-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.297995 settngs-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.297995 settngs-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-09 22:55:49.000000 settngs-0.7.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-09 22:55:49.000000 settngs-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-09 22:55:49.000000 settngs-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-09 22:55:49.000000 settngs-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 22:56:10.301996 settngs-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-09 22:55:49.000000 settngs-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-09 22:55:49.000000 settngs-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 22:55:49.000000 settngs-0.7.1/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.301996 settngs-0.7.1/settngs/
+-rw-r--r--   0 runner    (1001) docker     (123)    33804 2023-06-09 22:55:49.000000 settngs-0.7.1/settngs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 22:55:49.000000 settngs-0.7.1/settngs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 22:55:49.000000 settngs-0.7.1/settngs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.301996 settngs-0.7.1/settngs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 22:56:10.000000 settngs-0.7.1/settngs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-09 22:56:10.000000 settngs-0.7.1/settngs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:56:10.000000 settngs-0.7.1/settngs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 22:56:10.000000 settngs-0.7.1/settngs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 22:56:10.000000 settngs-0.7.1/settngs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-09 22:56:10.301996 settngs-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 22:55:49.000000 settngs-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.301996 settngs-0.7.1/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 22:55:49.000000 settngs-0.7.1/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-06-09 22:55:49.000000 settngs-0.7.1/testing/settngs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.301996 settngs-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 22:55:49.000000 settngs-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-06-09 22:55:49.000000 settngs-0.7.1/tests/settngs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:56:10.301996 settngs-0.7.1/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-09 22:55:49.000000 settngs-0.7.1/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-09 22:55:49.000000 settngs-0.7.1/workflows/package.yaml
```

### Comparing `settngs-0.7.0/.github/workflows/build.yaml` & `settngs-0.7.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/.gitignore` & `settngs-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/.pre-commit-config.yaml` & `settngs-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/LICENSE` & `settngs-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/PKG-INFO` & `settngs-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.7.0/README.md` & `settngs-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/settngs/__init__.py` & `settngs-0.7.1/settngs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,16 @@
         if not isinstance(other, Setting):
             return NotImplemented
         return self.__dict__ == other.__dict__
 
     def _guess_type(self) -> type | Literal['Any'] | None:
         if self.type is None and self.action is None:
             if self.cmdline:
+                if self.nargs in ('+', '*') or isinstance(self.nargs, int) and self.nargs > 1:
+                    return List[str]
                 return str
             else:
                 if not self.cmdline and self.default is not None:
                     return type(self.default)
                 return 'Any'
 
         if isinstance(self.type, type):
@@ -251,48 +253,53 @@
     def filter_argparse_kwargs(self) -> dict[str, Any]:
         return {k: v for k, v in self.argparse_kwargs.items() if v is not None}
 
     def to_argparse(self) -> tuple[Sequence[str], dict[str, Any]]:
         return self.argparse_args, self.filter_argparse_kwargs()
 
 
+class TypedNS:
+    def __init__(self) -> None:
+        raise TypeError('TypedNS cannot be instantiated')
+
+
 class Group(NamedTuple):
     persistent: bool
     v: dict[str, Setting]
 
 
 Values = Dict[str, Dict[str, Any]]
 Definitions = Dict[str, Group]
 
-T = TypeVar('T', Values, Namespace)
+T = TypeVar('T', bound=Union[Values, Namespace, TypedNS])
 
 
 class Config(NamedTuple, Generic[T]):
     values: T
     definitions: Definitions
 
 
 if TYPE_CHECKING:
     ArgParser = Union[argparse._MutuallyExclusiveGroup, argparse._ArgumentGroup, argparse.ArgumentParser]
-    ns = Namespace | Config[T] | None
+    ns = Namespace | TypedNS | Config[T] | None
 
 
 def generate_ns(definitions: Definitions) -> str:
     imports = ['from __future__ import annotations', 'import typing', 'import settngs']
-    ns = 'class settngs_namespace(settngs.Namespace):\n'
+    ns = 'class settngs_namespace(settngs.TypedNS):\n'
     types = []
     for group_name, group in definitions.items():
         for setting_name, setting in group.v.items():
             t = setting._guess_type()
             if t is None:
                 continue
             type_name = 'Any'
             if isinstance(t, str):
                 type_name = t
-            elif type(t) == types_GenericAlias:
+            elif isinstance(t, types_GenericAlias):
                 type_name = str(t)
             elif isinstance(t, type):
                 type_name = t.__name__
                 if t.__module__ != 'builtins':
                     imports.append(f'import {t.__module__}')
                     type_name = t.__module__ + '.' + type_name
             if type_name == 'Any':
@@ -309,15 +316,15 @@
     return '\n'.join(imports) + '\n\n' + ns + '\n'.join(types)
 
 
 def sanitize_name(name: str) -> str:
     return re.sub('[' + re.escape(' -_,.!@#$%^&*(){}[]\',."<>;:') + ']+', '_', name).strip('_')
 
 
-def get_option(options: Values | Namespace, setting: Setting) -> tuple[Any, bool]:
+def get_option(options: Values | Namespace | TypedNS, setting: Setting) -> tuple[Any, bool]:
     """
     Helper function to retrieve the value for a setting and if the current value is the default value
 
     Args:
         options: Dictionary or namespace of options
         setting: The setting object describing the value to retrieve
     """
@@ -333,15 +340,15 @@
     Helper function to retrieve all of the values for a group. Only to be used on persistent groups.
 
     Args:
         config: Dictionary or namespace of options
         group: The name of the group to retrieve
     """
     if isinstance(config[0], dict):
-        values = config[0].get(group, {}).copy()
+        values: dict[str, Any] = config[0].get(group, {}).copy()
     else:
         internal_names = {x.internal_name: x for x in config[1][group].v.values()}
         values = {}
         v = vars(config[0])
         for name, value in v.items():
             if name.startswith(f'{group}_'):
                 if name in internal_names:
@@ -466,19 +473,22 @@
         default: Include default values in the returned Config object
         persistent: Include unknown keys in persistent groups
     """
 
     if not file and not cmdline:
         raise ValueError('Invalid parameters: you must set either file or cmdline to True')
 
-    if isinstance(config.values, Namespace):
+    options: Values
+    definitions: Definitions
+    if isinstance(config.values, dict):
+        options = config.values
+        definitions = config.definitions
+    else:
         cfg = normalize_config(config, file=file, cmdline=cmdline, default=default, persistent=persistent)
         options, definitions = cfg
-    else:
-        options, definitions = config
     namespace = Namespace()
     for group_name, group in definitions.items():
 
         group_options = get_options(config, group_name)
         if group.persistent and persistent:
             for name, value in group_options.items():
                 if name in group.v:
@@ -569,22 +579,23 @@
     Args:
         definitions: A set of setting definitions. See `Config.definitions` and `Manager.definitions`
         description: Passed to argparse.ArgumentParser
         epilog: Passed to argparse.ArgumentParser
         args: Passed to argparse.ArgumentParser.parse_args
         config: The Config or Namespace object to use as a Namespace passed to argparse.ArgumentParser.parse_args
     """
-    namespace = None
+    namespace: Namespace | TypedNS | None = None
     if isinstance(config, Config):
         if isinstance(config.values, Namespace):
             namespace = config.values
         else:
             namespace = get_namespace(config, file=True, cmdline=True, default=False)[0]
     else:
         namespace = config
+
     argparser = create_argparser(definitions, description, epilog)
     ns = argparser.parse_args(args, namespace=namespace)
 
     return normalize_config(Config(ns, definitions), cmdline=True, file=True)
 
 
 def parse_config(
```

### Comparing `settngs-0.7.0/settngs.egg-info/PKG-INFO` & `settngs-0.7.1/settngs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.7.0/setup.cfg` & `settngs-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/testing/settngs.py` & `settngs-0.7.1/testing/settngs.py`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/tests/settngs_test.py` & `settngs-0.7.1/tests/settngs_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from testing.settngs import example
 from testing.settngs import failure
 from testing.settngs import success
 
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import List
-else:
+else:  # pragma: no cover
     List = list
 
 
 @pytest.fixture
 def settngs_manager() -> Generator[settngs.Manager, None, None]:
     manager = settngs.Manager()
     yield manager
@@ -537,15 +537,15 @@
 from __future__ import annotations
 import typing
 import settngs
 '''
     if typ == 'tests.settngs_test.test_type':
         src += 'import tests.settngs_test\n'
     src += '''
-class settngs_namespace(settngs.Namespace):
+class settngs_namespace(settngs.TypedNS):
 '''
     if typ is None:
         src += '    ...\n'
     else:
         src += f'    {settngs_manager.definitions["test"].v["test"].internal_name}: {typ}\n'
 
     generated_src = settngs_manager.generate_ns()
```

### Comparing `settngs-0.7.0/workflows/build.yaml` & `settngs-0.7.1/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `settngs-0.7.0/workflows/package.yaml` & `settngs-0.7.1/workflows/package.yaml`

 * *Files identical despite different names*

