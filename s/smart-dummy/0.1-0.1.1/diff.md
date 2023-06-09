# Comparing `tmp/smart_dummy-0.1.tar.gz` & `tmp/smart_dummy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_dummy-0.1.tar", last modified: Fri Jun  9 23:24:03 2023, max compression
+gzip compressed data, was "smart_dummy-0.1.1.tar", last modified: Fri Jun  9 23:29:36 2023, max compression
```

## Comparing `smart_dummy-0.1.tar` & `smart_dummy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 23:24:03.809224 smart_dummy-0.1/
--rw-rw-rw-   0        0        0     1105 2023-06-09 23:14:45.000000 smart_dummy-0.1/LICENSE
--rw-rw-rw-   0        0        0     2632 2023-06-09 23:24:03.809224 smart_dummy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1622 2023-06-09 23:14:45.000000 smart_dummy-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 23:24:03.810224 smart_dummy-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-06-09 23:23:56.000000 smart_dummy-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 23:24:03.790217 smart_dummy-0.1/smart_dummy/
--rw-rw-rw-   0        0        0      284 2023-06-09 23:14:45.000000 smart_dummy-0.1/smart_dummy/__init__.py
--rw-rw-rw-   0        0        0      661 2023-06-09 23:14:45.000000 smart_dummy-0.1/smart_dummy/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 23:24:03.808224 smart_dummy-0.1/smart_dummy.egg-info/
--rw-rw-rw-   0        0        0     2632 2023-06-09 23:24:03.000000 smart_dummy-0.1/smart_dummy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-09 23:24:03.000000 smart_dummy-0.1/smart_dummy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 23:24:03.000000 smart_dummy-0.1/smart_dummy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-09 23:24:03.000000 smart_dummy-0.1/smart_dummy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 23:24:03.000000 smart_dummy-0.1/smart_dummy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 23:29:36.967117 smart_dummy-0.1.1/
+-rw-rw-rw-   0        0        0     1105 2023-06-09 23:14:45.000000 smart_dummy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2634 2023-06-09 23:29:36.966065 smart_dummy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1622 2023-06-09 23:14:45.000000 smart_dummy-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 23:29:36.967117 smart_dummy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2023-06-09 23:29:26.000000 smart_dummy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 23:29:36.954060 smart_dummy-0.1.1/smart_dummy/
+-rw-rw-rw-   0        0        0      284 2023-06-09 23:14:45.000000 smart_dummy-0.1.1/smart_dummy/__init__.py
+-rw-rw-rw-   0        0        0      661 2023-06-09 23:14:45.000000 smart_dummy-0.1.1/smart_dummy/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 23:29:36.965064 smart_dummy-0.1.1/smart_dummy.egg-info/
+-rw-rw-rw-   0        0        0     2634 2023-06-09 23:29:36.000000 smart_dummy-0.1.1/smart_dummy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-09 23:29:36.000000 smart_dummy-0.1.1/smart_dummy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 23:29:36.000000 smart_dummy-0.1.1/smart_dummy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-09 23:29:36.000000 smart_dummy-0.1.1/smart_dummy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 23:29:36.000000 smart_dummy-0.1.1/smart_dummy.egg-info/top_level.txt
```

### Comparing `smart_dummy-0.1/LICENSE` & `smart_dummy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_dummy-0.1/PKG-INFO` & `smart_dummy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_dummy
-Version: 0.1
+Version: 0.1.1
 Summary: A smart and easy replacement to pandas.get_dummies() 
 Home-page: https://github.com/emmalzhang/smart_dummy
 Author: Muriel Grobler, Emma Zhang
 Author-email: muriel.grobler@gmail.com, emma.lzhang@gmail.com
 License: UNKNOWN
 Description: # smart_dummy
```

### Comparing `smart_dummy-0.1/README.md` & `smart_dummy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `smart_dummy-0.1/setup.py` & `smart_dummy-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 def parse_requirements(filename):
     """Load requirements from a pip requirements file."""
     with open(filename) as f:
         lineiter = (line.strip() for line in f)
         return [line for line in lineiter if line and not line.startswith("#")]
 
 
-reqs = parse_requirements('requirements.txt')
+reqs = parse_requirements('requires.txt')
 
 setup(
     name="smart_dummy",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=reqs,
     author="Muriel Grobler, Emma Zhang",
     author_email="muriel.grobler@gmail.com, emma.lzhang@gmail.com",
     description="A smart and easy replacement to pandas.get_dummies() ",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `smart_dummy-0.1/smart_dummy/main.py` & `smart_dummy-0.1.1/smart_dummy/main.py`

 * *Files identical despite different names*

### Comparing `smart_dummy-0.1/smart_dummy.egg-info/PKG-INFO` & `smart_dummy-0.1.1/smart_dummy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-dummy
-Version: 0.1
+Version: 0.1.1
 Summary: A smart and easy replacement to pandas.get_dummies() 
 Home-page: https://github.com/emmalzhang/smart_dummy
 Author: Muriel Grobler, Emma Zhang
 Author-email: muriel.grobler@gmail.com, emma.lzhang@gmail.com
 License: UNKNOWN
 Description: # smart_dummy
```

