# Comparing `tmp/supreme_task-0.1.0.tar.gz` & `tmp/supreme_task-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supreme_task-0.1.0.tar", max compression
+gzip compressed data, was "supreme_task-0.1.1.tar", max compression
```

## Comparing `supreme_task-0.1.0.tar` & `supreme_task-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2357 2023-06-10 10:53:34.047859 supreme_task-0.1.0/README.md
--rw-r--r--   0        0        0     1280 2023-06-09 21:27:21.505866 supreme_task-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-09 21:13:13.262078 supreme_task-0.1.0/src/supreme_task/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 15:17:49.254434 supreme_task-0.1.0/src/supreme_task/py.typed
--rw-r--r--   0        0        0    13897 2023-06-10 10:38:27.913532 supreme_task-0.1.0/src/supreme_task/tasks.py
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 supreme_task-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2357 2023-06-10 10:53:34.047859 supreme_task-0.1.1/README.md
+-rw-r--r--   0        0        0     1554 2023-06-10 11:07:03.773613 supreme_task-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-06-09 21:13:13.262078 supreme_task-0.1.1/src/supreme_task/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:17:49.254434 supreme_task-0.1.1/src/supreme_task/py.typed
+-rw-r--r--   0        0        0    13897 2023-06-10 10:38:27.913532 supreme_task-0.1.1/src/supreme_task/tasks.py
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 supreme_task-0.1.1/PKG-INFO
```

### Comparing `supreme_task-0.1.0/README.md` & `supreme_task-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `supreme_task-0.1.0/pyproject.toml` & `supreme_task-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 [tool.poetry]
 name = "supreme_task"
-version = "0.1.0"
+version = "0.1.1"
 description = "Prefect tasks plus added functionality to enforce type checking and help in debugging helping to reduce negative engineering!"
 packages = [{ include = "supreme_task", from = "src" }]
 authors = []
 
 readme = "README.md"
-include = ["README.md", "LICENSE.txt", "src/aws_parquet/py.typed"]
-exclude = ["*.so", "*.pyc", "*~", "#*", ".git*", ".coverage*", "DS_Store", "__pycache__"]
+include = ["README.md", "LICENSE.txt", "src/supreme_task/py.typed"]
+exclude = [
+    "*.so",
+    "*.pyc",
+    "*~",
+    "#*",
+    ".git*",
+    ".coverage*",
+    "DS_Store",
+    "__pycache__",
+]
+
+homepage = "https://github.com/marwan116/supreme-task/"
+repository = "https://github.com/marwan116/supreme-task/"
+documentation = "https://github.com/marwan116/supreme-task/"
+
+keywords = ["prefect", "tasks", "workflow", "orchestration"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 prefect = "^2.0.0"
 typeguard = "^4.0.0"
```

### Comparing `supreme_task-0.1.0/src/supreme_task/tasks.py` & `supreme_task-0.1.1/src/supreme_task/tasks.py`

 * *Files identical despite different names*

### Comparing `supreme_task-0.1.0/PKG-INFO` & `supreme_task-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: supreme-task
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prefect tasks plus added functionality to enforce type checking and help in debugging helping to reduce negative engineering!
+Home-page: https://github.com/marwan116/supreme-task/
+Keywords: prefect,tasks,workflow,orchestration
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: prefect (>=2.0.0,<3.0.0)
 Requires-Dist: typeguard (>=4.0.0,<5.0.0)
+Project-URL: Documentation, https://github.com/marwan116/supreme-task/
+Project-URL: Repository, https://github.com/marwan116/supreme-task/
 Description-Content-Type: text/markdown
 
 # A prefect extension giving prefect tasks super powers
 
 ## Motivation
 Prefect tasks plus added functionality to enforce type checking and help in debugging helping to reduce negative engineering!
```

