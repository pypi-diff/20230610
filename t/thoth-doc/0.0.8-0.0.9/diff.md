# Comparing `tmp/thoth_doc-0.0.8.tar.gz` & `tmp/thoth_doc-0.0.9.tar.gz`

## Comparing `thoth_doc-0.0.8.tar` & `thoth_doc-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.env
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/Makefile
--rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/Thoth.svg.png
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/vscode.env
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/__init__.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/main.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/parsers.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/utils.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/compiled_docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/tests/test_generator.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/tests/test_parsers.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/LICENSE
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.env
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/Makefile
+-rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/Thoth.svg.png
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/vscode.env
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/__init__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/main.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/parsers.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/tests/test_generator.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/tests/test_parsers.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/PKG-INFO
```

### Comparing `thoth_doc-0.0.8/Thoth.svg.png` & `thoth_doc-0.0.9/Thoth.svg.png`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.8/src/thoth_doc/main.py` & `thoth_doc-0.0.9/src/thoth_doc/main.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.8/src/thoth_doc/parsers.py` & `thoth_doc-0.0.9/src/thoth_doc/parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,13 @@
 import os
 import re
 
 from thoth_doc.utils import get_docstring, remove_whitespaces
 
 
-def add_image_host_to_image_links(generator, line):
-    ''' Adds image host to image links. you need to set image_host attribute on generator instance. '''
-
-    host = getattr(generator, 'image_host', None)
-    matches = re.findall(r'(!\[.*?\]\((.*?)\))', line)
-    if matches and host:
-        for match in matches:
-            line = line.replace(match[1], f'{host}/{match[1]}')
-        return line
-    return line
-
-
 def code_reference_parser(_, line):
     ''' Parses [@code/main.py#Class.method] syntax. Extacts docstring. '''
 
     matches = re.findall(r'(\[@(.+?)\])', line)
     if matches:
         for match in matches:
             mod, name = match[1].split('#')
```

### Comparing `thoth_doc-0.0.8/src/thoth_doc/utils.py` & `thoth_doc-0.0.9/src/thoth_doc/utils.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.8/LICENSE` & `thoth_doc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.8/README.md` & `thoth_doc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.8/pyproject.toml` & `thoth_doc-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thoth_doc"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Lev", email="smj510black@gmail.com" },
 ]
 description = "Dependency-free, lightweight docstring parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thoth_doc-0.0.8/PKG-INFO` & `thoth_doc-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoth_doc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dependency-free, lightweight docstring parser
 Project-URL: Homepage, https://github.com/mariownyou/thoth-doc
 Project-URL: Bug Tracker, https://github.com/mariownyou/thoth-doc/issues
 Author-email: Lev <smj510black@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

