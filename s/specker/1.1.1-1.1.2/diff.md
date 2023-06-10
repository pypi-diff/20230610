# Comparing `tmp/specker-1.1.1.tar.gz` & `tmp/specker-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specker-1.1.1.tar", last modified: Thu Jun  8 21:13:44 2023, max compression
+gzip compressed data, was "specker-1.1.2.tar", last modified: Sat Jun 10 20:42:51 2023, max compression
```

## Comparing `specker-1.1.1.tar` & `specker-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-02 06:34:14.000000 specker-1.1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.1/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.1/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.1/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-08 21:03:55.000000 specker-1.1.1/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.1/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-08 21:13:44.964403 specker-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.1/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.1/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.1/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-08 21:13:38.000000 specker-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 21:13:44.964403 specker-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.960403 specker-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/src/specker/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.1/src/specker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-06-08 21:07:15.000000 specker-1.1.1/src/specker/content.py
--rw-rw-rw-   0 root         (0) root         (0)     5945 2023-06-02 06:24:00.000000 specker-1.1.1/src/specker/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/src/specker/specs/
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-08 21:00:19.000000 specker-1.1.1/src/specker/specs/SPECFILES.md
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-08 21:00:19.000000 specker-1.1.1/src/specker/specs/specker.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/src/specker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.400125 specker-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-02 06:34:14.000000 specker-1.1.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.2/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.2/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.364125 specker-1.1.2/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.2/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-09 19:33:40.000000 specker-1.1.2/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.2/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-10 20:42:51.400125 specker-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.2/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.2/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.2/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-10 20:42:38.000000 specker-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 20:42:51.400125 specker-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.312125 specker-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.364125 specker-1.1.2/src/specker/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.2/src/specker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2023-06-09 19:33:40.000000 specker-1.1.2/src/specker/content.py
+-rw-rw-rw-   0 root         (0) root         (0)     5945 2023-06-02 06:24:00.000000 specker-1.1.2/src/specker/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.388125 specker-1.1.2/src/specker/specs/
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-08 21:00:19.000000 specker-1.1.2/src/specker/specs/SPECFILES.md
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-08 21:00:19.000000 specker-1.1.2/src/specker/specs/specker.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.368125 specker-1.1.2/src/specker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/top_level.txt
```

### Comparing `specker-1.1.1/.gitlab-ci.yml` & `specker-1.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/.pylintrc` & `specker-1.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/.vscode/extensions.json` & `specker-1.1.2/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/Doxyfile` & `specker-1.1.2/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "Specker JSON Specification Validator"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.1.1"
+PROJECT_NUMBER = "1.1.2"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `specker-1.1.1/LICENSE.md` & `specker-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/Makefile` & `specker-1.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/PKG-INFO` & `specker-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.1
+Version: 1.1.2
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `specker-1.1.1/README.md` & `specker-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/git-tags.sh` & `specker-1.1.2/git-tags.sh`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/icon.png` & `specker-1.1.2/icon.png`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/pyproject.toml` & `specker-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "specker"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "Specker JSON Specification Validator"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `specker-1.1.1/src/specker/__init__.py` & `specker-1.1.2/src/specker/__init__.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/src/specker/content.py` & `specker-1.1.2/src/specker/content.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,38 +39,40 @@
     }
 
     @property
     def type(self) -> object:
         """Get Spec Value Type
         @retval type Type specified from Spec
         """
+        if self._type not in self.__type_map.keys():
+            raise TypeError(f"Unknown Type: {str(self._type)}")
         return self.__type_map[self._type]
 
     def __init__(self,content:dict[str,typing.Any]) -> None:
         """Initializer
         @param dict[str,typing.Any] \c content Spec Content
         """
-        for k,v in content.items():
+        valid_attrs:list[str] = [ "required", "default", "comment", "example", "values" ]
+        attr_defaults:list[typing.Any] = [  False, None, "", "", [] ]
+
+        for k,v in content.items(): # Set Passed Attrs
             setattr(self,f"_{k}",v)
+
+        for i in range(0,len(valid_attrs),1): # Set Default Attrs
+            attr:str = valid_attrs[i]
+            default:typing.Any = attr_defaults[i]
+            if not hasattr(self,f"_{attr}"):
+                setattr(self,f"_{attr}",default)
+
         if not hasattr(self,"_name"):
             raise ValueError("Spec is missing required attribute: name")
         if not hasattr(self,"_type"):
             raise ValueError("Spec is missing required attribute: type")
         if self._type not in self.__type_map.keys():
-            raise ValueError("Spec has invalid type option. See Documentation for valid options for 'type'")
-        if not hasattr(self,"_required"):
-            self._required = False
-        if not hasattr(self,"_default"):
-            self._default = None
-        if not hasattr(self,"_comment"):
-            self._comment = ""
-        if not hasattr(self,"_example"):
-            self._example = ""
-        if not hasattr(self,"_values"):
-            self._values = []
+            raise TypeError("Spec has invalid type option. See Documentation for valid options for 'type'")
 
     def __str__(self) -> str:
         """To String Generator
         @retval str Markdown Formatted Data about Spec
         """
         default_str:str = ""
         if self._default is not None:
```

### Comparing `specker-1.1.1/src/specker/loader.py` & `specker-1.1.2/src/specker/loader.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/src/specker/specs/SPECFILES.md` & `specker-1.1.2/src/specker/specs/SPECFILES.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/src/specker/specs/specker.spec` & `specker-1.1.2/src/specker/specs/specker.spec`

 * *Files identical despite different names*

### Comparing `specker-1.1.1/src/specker.egg-info/PKG-INFO` & `specker-1.1.2/src/specker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.1
+Version: 1.1.2
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

