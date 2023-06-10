# Comparing `tmp/nfonistaxx-0.7.tar.gz` & `tmp/nfonistaxx-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nfonistaxx-0.7.tar", last modified: Sat Jun 10 14:21:53 2023, max compression
+gzip compressed data, was "nfonistaxx-0.9.tar", last modified: Sat Jun 10 15:01:00 2023, max compression
```

## Comparing `nfonistaxx-0.7.tar` & `nfonistaxx-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 14:21:53.813435 nfonistaxx-0.7/
--rw-rw----   0 root         (0) everybody  (9997)       30 2023-06-07 05:27:20.000000 nfonistaxx-0.7/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 14:21:53.801435 nfonistaxx-0.7/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      213 2023-06-08 06:55:58.000000 nfonistaxx-0.7/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-10 14:21:53.813435 nfonistaxx-0.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      938 2023-06-10 14:21:30.000000 nfonistaxx-0.7/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 14:21:53.665435 nfonistaxx-0.7/src/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 14:21:53.725435 nfonistaxx-0.7/src/nfonistaxx/
--rw-rw----   0 root         (0) everybody  (9997)       26 2023-06-10 13:50:49.000000 nfonistaxx-0.7/src/nfonistaxx/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    48922 2023-06-10 14:21:46.000000 nfonistaxx-0.7/src/nfonistaxx/nfonistaxx.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 14:21:53.789435 nfonistaxx-0.7/src/nfonistaxx.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 14:21:53.000000 nfonistaxx-0.7/src/nfonistaxx.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      238 2023-06-10 14:21:53.000000 nfonistaxx-0.7/src/nfonistaxx.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-10 14:21:53.000000 nfonistaxx-0.7/src/nfonistaxx.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-10 14:21:53.000000 nfonistaxx-0.7/src/nfonistaxx.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 15:01:00.104679 nfonistaxx-0.9/
+-rw-rw----   0 root         (0) everybody  (9997)       30 2023-06-07 05:27:20.000000 nfonistaxx-0.9/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 15:01:00.096680 nfonistaxx-0.9/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      213 2023-06-08 06:55:58.000000 nfonistaxx-0.9/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-10 15:01:00.108679 nfonistaxx-0.9/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      938 2023-06-10 15:00:54.000000 nfonistaxx-0.9/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 15:00:59.956679 nfonistaxx-0.9/src/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 15:01:00.044679 nfonistaxx-0.9/src/nfonistaxx/
+-rw-rw----   0 root         (0) everybody  (9997)       26 2023-06-10 13:50:49.000000 nfonistaxx-0.9/src/nfonistaxx/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)   126390 2023-06-10 15:00:21.000000 nfonistaxx-0.9/src/nfonistaxx/nfonistaxx.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 15:01:00.088679 nfonistaxx-0.9/src/nfonistaxx.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 15:00:59.000000 nfonistaxx-0.9/src/nfonistaxx.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      238 2023-06-10 15:00:59.000000 nfonistaxx-0.9/src/nfonistaxx.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-10 15:00:59.000000 nfonistaxx-0.9/src/nfonistaxx.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-10 15:00:59.000000 nfonistaxx-0.9/src/nfonistaxx.egg-info/top_level.txt
```

### Comparing `nfonistaxx-0.7/PKG-INFO` & `nfonistaxx-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfonistaxx
-Version: 0.7
+Version: 0.9
 Summary: • instagram profile info
 Home-page: 
 Author: Alaa
 Author-email: Alaaposhnaq@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nfonistaxx-0.7/setup.py` & `nfonistaxx-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('instaloder\nuser_agent\nrequests\nuuid')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="nfonistaxx",
-    version="0.7",
+    version="0.9",
     author="Alaa",
     author_email="Alaaposhnaq@gmail.com",
     description="• instagram profile info",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `nfonistaxx-0.7/src/nfonistaxx.egg-info/PKG-INFO` & `nfonistaxx-0.9/src/nfonistaxx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfonistaxx
-Version: 0.7
+Version: 0.9
 Summary: • instagram profile info
 Home-page: 
 Author: Alaa
 Author-email: Alaaposhnaq@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

