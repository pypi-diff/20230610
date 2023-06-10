# Comparing `tmp/progress-table-0.1.8.tar.gz` & `tmp/progress-table-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-0.1.8.tar", last modified: Sat Dec 10 15:35:19 2022, max compression
+gzip compressed data, was "progress-table-0.1.9.tar", last modified: Sat Dec 10 15:35:58 2022, max compression
```

## Comparing `progress-table-0.1.8.tar` & `progress-table-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 15:35:19.363072 progress-table-0.1.8/
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1052 2022-11-17 19:44:00.000000 progress-table-0.1.8/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)     5226 2022-12-10 15:35:19.363072 progress-table-0.1.8/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1001)     4486 2022-12-10 15:25:18.000000 progress-table-0.1.8/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 15:35:19.359739 progress-table-0.1.8/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1001)      108 2022-11-17 23:12:48.000000 progress-table-0.1.8/progress_table/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1234 2022-12-10 14:52:33.000000 progress-table-0.1.8/progress_table/devel.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)    14564 2022-12-09 16:31:28.000000 progress-table-0.1.8/progress_table/progress_table.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 15:35:19.363072 progress-table-0.1.8/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1001)     5226 2022-12-10 15:35:19.000000 progress-table-0.1.8/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1001)      328 2022-12-10 15:35:19.000000 progress-table-0.1.8/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)        1 2022-12-10 15:35:19.000000 progress-table-0.1.8/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)        9 2022-12-10 15:35:19.000000 progress-table-0.1.8/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)       15 2022-12-10 15:35:19.000000 progress-table-0.1.8/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)      188 2022-11-17 21:56:56.000000 progress-table-0.1.8/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1001)      105 2022-12-10 15:35:19.363072 progress-table-0.1.8/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1092 2022-12-10 15:35:13.000000 progress-table-0.1.8/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 15:35:58.444007 progress-table-0.1.9/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1052 2022-11-17 19:44:00.000000 progress-table-0.1.9/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5226 2022-12-10 15:35:58.444007 progress-table-0.1.9/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     4486 2022-12-10 15:25:18.000000 progress-table-0.1.9/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 15:35:58.444007 progress-table-0.1.9/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      108 2022-11-17 23:12:48.000000 progress-table-0.1.9/progress_table/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1234 2022-12-10 14:52:33.000000 progress-table-0.1.9/progress_table/devel.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)    14564 2022-12-09 16:31:28.000000 progress-table-0.1.9/progress_table/progress_table.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 15:35:58.444007 progress-table-0.1.9/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5226 2022-12-10 15:35:58.000000 progress-table-0.1.9/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      328 2022-12-10 15:35:58.000000 progress-table-0.1.9/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)        1 2022-12-10 15:35:58.000000 progress-table-0.1.9/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)        9 2022-12-10 15:35:58.000000 progress-table-0.1.9/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)       15 2022-12-10 15:35:58.000000 progress-table-0.1.9/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      188 2022-11-17 21:56:56.000000 progress-table-0.1.9/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      105 2022-12-10 15:35:58.444007 progress-table-0.1.9/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1092 2022-12-10 15:35:52.000000 progress-table-0.1.9/setup.py
```

### Comparing `progress-table-0.1.8/LICENSE.txt` & `progress-table-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-0.1.8/PKG-INFO` & `progress-table-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 0.1.8
+Version: 0.1.9
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-0.1.8/README.md` & `progress-table-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `progress-table-0.1.8/progress_table/devel.py` & `progress-table-0.1.9/progress_table/devel.py`

 * *Files identical despite different names*

### Comparing `progress-table-0.1.8/progress_table/progress_table.py` & `progress-table-0.1.9/progress_table/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-0.1.8/progress_table.egg-info/PKG-INFO` & `progress-table-0.1.9/progress_table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 0.1.8
+Version: 0.1.9
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-0.1.8/setup.py` & `progress-table-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="UTF-8")
 
 setup(
     name="progress-table",
-    version="0.1.8",
+    version="0.1.9",
     url="https://github.com/gahaalt/progress-table.git",
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
     description="Display progress as a pretty table in the command line.",
     packages=["progress_table"],
     python_requires=">=3.7",
```

