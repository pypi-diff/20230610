# Comparing `tmp/nfonistaxx-0.1.tar.gz` & `tmp/nfonistaxx-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nfonistaxx-0.1.tar", last modified: Sat Jun 10 12:08:16 2023, max compression
+gzip compressed data, was "nfonistaxx-0.4.tar", last modified: Sat Jun 10 13:54:08 2023, max compression
```

## Comparing `nfonistaxx-0.1.tar` & `nfonistaxx-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:08:16.793259 nfonistaxx-0.1/
--rw-rw----   0 root         (0) everybody  (9997)       30 2023-06-07 05:27:20.000000 nfonistaxx-0.1/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 12:08:16.781259 nfonistaxx-0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      213 2023-06-08 06:55:58.000000 nfonistaxx-0.1/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-10 12:08:16.793259 nfonistaxx-0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      938 2023-06-10 12:06:56.000000 nfonistaxx-0.1/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:08:16.625259 nfonistaxx-0.1/src/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:08:16.681259 nfonistaxx-0.1/src/nfonistaxx/
--rw-rw----   0 root         (0) everybody  (9997)       25 2023-06-10 12:07:58.000000 nfonistaxx-0.1/src/nfonistaxx/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)   204938 2023-06-07 05:26:20.000000 nfonistaxx-0.1/src/nfonistaxx/nfonistaxx.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:08:16.753259 nfonistaxx-0.1/src/nfonistaxx.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 12:08:16.000000 nfonistaxx-0.1/src/nfonistaxx.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      238 2023-06-10 12:08:16.000000 nfonistaxx-0.1/src/nfonistaxx.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-10 12:08:16.000000 nfonistaxx-0.1/src/nfonistaxx.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-10 12:08:16.000000 nfonistaxx-0.1/src/nfonistaxx.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 13:54:08.101436 nfonistaxx-0.4/
+-rw-rw----   0 root         (0) everybody  (9997)       30 2023-06-07 05:27:20.000000 nfonistaxx-0.4/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 13:54:08.093436 nfonistaxx-0.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      213 2023-06-08 06:55:58.000000 nfonistaxx-0.4/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-10 13:54:08.101436 nfonistaxx-0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      938 2023-06-10 13:53:16.000000 nfonistaxx-0.4/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 13:54:07.933436 nfonistaxx-0.4/src/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 13:54:08.021436 nfonistaxx-0.4/src/nfonistaxx/
+-rw-rw----   0 root         (0) everybody  (9997)       26 2023-06-10 13:50:49.000000 nfonistaxx-0.4/src/nfonistaxx/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    47610 2023-06-10 13:50:30.000000 nfonistaxx-0.4/src/nfonistaxx/nfonistaxx.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 13:54:08.081436 nfonistaxx-0.4/src/nfonistaxx.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      669 2023-06-10 13:54:07.000000 nfonistaxx-0.4/src/nfonistaxx.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      238 2023-06-10 13:54:07.000000 nfonistaxx-0.4/src/nfonistaxx.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-10 13:54:07.000000 nfonistaxx-0.4/src/nfonistaxx.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-10 13:54:07.000000 nfonistaxx-0.4/src/nfonistaxx.egg-info/top_level.txt
```

### Comparing `nfonistaxx-0.1/PKG-INFO` & `nfonistaxx-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfonistaxx
-Version: 0.1
+Version: 0.4
 Summary: • instagram profile info
 Home-page: 
 Author: Alaa
 Author-email: Alaaposhnaq@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nfonistaxx-0.1/setup.py` & `nfonistaxx-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('instaloder\nuser_agent\nrequests\nuuid')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="nfonistaxx",
-    version="0.1",
+    version="0.4",
     author="Alaa",
     author_email="Alaaposhnaq@gmail.com",
     description="• instagram profile info",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `nfonistaxx-0.1/src/nfonistaxx.egg-info/PKG-INFO` & `nfonistaxx-0.4/src/nfonistaxx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfonistaxx
-Version: 0.1
+Version: 0.4
 Summary: • instagram profile info
 Home-page: 
 Author: Alaa
 Author-email: Alaaposhnaq@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

