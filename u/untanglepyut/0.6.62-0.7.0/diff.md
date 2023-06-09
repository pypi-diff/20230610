# Comparing `tmp/untanglepyut-0.6.62.tar.gz` & `tmp/untanglepyut-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untanglepyut-0.6.62.tar", last modified: Tue May 16 19:53:12 2023, max compression
+gzip compressed data, was "untanglepyut-0.7.0.tar", last modified: Fri Jun  9 22:03:56 2023, max compression
```

## Comparing `untanglepyut-0.6.62.tar` & `untanglepyut-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 19:53:12.659412 untanglepyut-0.6.62/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-0.6.62/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-16 19:53:12.659286 untanglepyut-0.6.62/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3226 2023-04-13 20:32:39.000000 untanglepyut-0.6.62/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-16 19:53:12.659483 untanglepyut-0.6.62/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      821 2023-05-16 18:45:49.000000 untanglepyut-0.6.62/setup.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 19:53:12.658537 untanglepyut-0.6.62/untanglepyut/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-0.6.62/untanglepyut/BaseUnTangle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-0.6.62/untanglepyut/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-0.6.62/untanglepyut/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15843 2023-03-19 16:02:08.000000 untanglepyut-0.6.62/untanglepyut/UnTangleOglLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14445 2023-05-08 16:55:26.000000 untanglepyut-0.6.62/untanglepyut/UnTanglePyut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-0.6.62/untanglepyut/UnTangleUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13009 2023-05-10 17:16:32.000000 untanglepyut-0.6.62/untanglepyut/UnTangler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3918 2023-01-31 19:27:38.000000 untanglepyut-0.6.62/untanglepyut/UntangleSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-05-15 00:32:46.000000 untanglepyut-0.6.62/untanglepyut/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       28 2023-05-16 18:48:12.000000 untanglepyut-0.6.62/untanglepyut/_version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-0.6.62/untanglepyut/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 19:53:12.659147 untanglepyut-0.6.62/untanglepyut.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-16 19:53:12.000000 untanglepyut-0.6.62/untanglepyut.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      518 2023-05-16 19:53:12.000000 untanglepyut-0.6.62/untanglepyut.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-16 19:53:12.000000 untanglepyut-0.6.62/untanglepyut.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       84 2023-05-16 19:53:12.000000 untanglepyut-0.6.62/untanglepyut.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-05-16 19:53:12.000000 untanglepyut-0.6.62/untanglepyut.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:03:56.235884 untanglepyut-0.7.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-0.7.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3477 2023-06-09 22:03:56.235774 untanglepyut-0.7.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3226 2023-04-13 20:32:39.000000 untanglepyut-0.7.0/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 22:03:56.235914 untanglepyut-0.7.0/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      821 2023-06-09 21:53:23.000000 untanglepyut-0.7.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:03:56.235046 untanglepyut-0.7.0/untanglepyut/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-0.7.0/untanglepyut/BaseUnTangle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-0.7.0/untanglepyut/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-0.7.0/untanglepyut/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15843 2023-03-19 16:02:08.000000 untanglepyut-0.7.0/untanglepyut/UnTangleOglLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14445 2023-05-08 16:55:26.000000 untanglepyut-0.7.0/untanglepyut/UnTanglePyut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-0.7.0/untanglepyut/UnTangleUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13009 2023-05-10 17:16:32.000000 untanglepyut-0.7.0/untanglepyut/UnTangler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3918 2023-01-31 19:27:38.000000 untanglepyut-0.7.0/untanglepyut/UntangleSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-05-15 00:32:46.000000 untanglepyut-0.7.0/untanglepyut/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-06-09 20:48:03.000000 untanglepyut-0.7.0/untanglepyut/_version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-0.7.0/untanglepyut/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:03:56.235612 untanglepyut-0.7.0/untanglepyut.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3477 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      518 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       84 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/top_level.txt
```

### Comparing `untanglepyut-0.6.62/LICENSE` & `untanglepyut-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/PKG-INFO` & `untanglepyut-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 0.6.62
+Version: 0.7.0
 Summary: XML to Ogl Object Model
 Home-page: https://github.com/hasii2011/untanglepyut
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./docs/agpl-license-web-badge-version-2-256x48.png"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 0.6.62 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 0.7.0 Summary: XML to Ogl
 Object Model Home-page: https://github.com/hasii2011/untanglepyut Author-email:
 Humberto.A.Sanchez.II@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/
 master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/
 hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-
 window=last-30-days&insights-snapshot=true) [![CircleCI](https://
```

### Comparing `untanglepyut-0.6.62/README.md` & `untanglepyut-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/setup.py` & `untanglepyut-0.7.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     packages=[
         'untanglepyut'
     ],
     package_data={
         'untanglepyut': ['py.typed'],
     },
 
-    install_requires=['hasiihelper~=0.2.0', 'hasiicommon~=0.2.2', 'pyutmodel~=1.4.3', 'ogl==0.70.40', 'untangle==1.2.1'],
+    install_requires=['hasiihelper==0.2.1', 'hasiicommon==0.3.1', 'pyutmodel~=1.4.4', 'ogl==0.70.52', 'untangle==1.2.1'],
 )
```

### Comparing `untanglepyut-0.6.62/untanglepyut/BaseUnTangle.py` & `untanglepyut-0.7.0/untanglepyut/BaseUnTangle.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut/Common.py` & `untanglepyut-0.7.0/untanglepyut/Common.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut/Types.py` & `untanglepyut-0.7.0/untanglepyut/Types.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut/UnTangleOglLinks.py` & `untanglepyut-0.7.0/untanglepyut/UnTangleOglLinks.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut/UnTanglePyut.py` & `untanglepyut-0.7.0/untanglepyut/UnTanglePyut.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut/UnTangleUseCaseDiagram.py` & `untanglepyut-0.7.0/untanglepyut/UnTangleUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut/UnTangler.py` & `untanglepyut-0.7.0/untanglepyut/UnTangler.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut/UntangleSequenceDiagram.py` & `untanglepyut-0.7.0/untanglepyut/UntangleSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.62/untanglepyut.egg-info/PKG-INFO` & `untanglepyut-0.7.0/untanglepyut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 0.6.62
+Version: 0.7.0
 Summary: XML to Ogl Object Model
 Home-page: https://github.com/hasii2011/untanglepyut
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./docs/agpl-license-web-badge-version-2-256x48.png"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 0.6.62 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 0.7.0 Summary: XML to Ogl
 Object Model Home-page: https://github.com/hasii2011/untanglepyut Author-email:
 Humberto.A.Sanchez.II@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/
 master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/
 hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-
 window=last-30-days&insights-snapshot=true) [![CircleCI](https://
```

### Comparing `untanglepyut-0.6.62/untanglepyut.egg-info/SOURCES.txt` & `untanglepyut-0.7.0/untanglepyut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

