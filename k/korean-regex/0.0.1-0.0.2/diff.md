# Comparing `tmp/korean_regex-0.0.1.tar.gz` & `tmp/korean_regex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "korean_regex-0.0.1.tar", last modified: Sat Jun 10 02:31:17 2023, max compression
+gzip compressed data, was "korean_regex-0.0.2.tar", last modified: Sat Jun 10 02:37:53 2023, max compression
```

## Comparing `korean_regex-0.0.1.tar` & `korean_regex-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 02:31:17.828073 korean_regex-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 korean_regex-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-10 02:05:20.000000 korean_regex-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6366 2023-06-10 02:31:17.827069 korean_regex-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5427 2023-06-10 02:18:18.000000 korean_regex-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 02:31:17.812805 korean_regex-0.0.1/ko_re/
--rw-rw-rw-   0        0        0       82 2023-06-10 02:07:32.000000 korean_regex-0.0.1/ko_re/__init__.py
--rw-rw-rw-   0        0        0    10476 2023-06-10 02:06:52.000000 korean_regex-0.0.1/ko_re/ko_re.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:31:17.826067 korean_regex-0.0.1/korean_regex.egg-info/
--rw-rw-rw-   0        0        0     6366 2023-06-10 02:31:17.000000 korean_regex-0.0.1/korean_regex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-06-10 02:31:17.000000 korean_regex-0.0.1/korean_regex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 02:31:17.000000 korean_regex-0.0.1/korean_regex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 02:31:17.000000 korean_regex-0.0.1/korean_regex.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-10 02:31:17.000000 korean_regex-0.0.1/korean_regex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 02:31:17.828073 korean_regex-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-06-10 02:29:56.000000 korean_regex-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:53.260485 korean_regex-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 korean_regex-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-10 02:05:20.000000 korean_regex-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6366 2023-06-10 02:37:53.259941 korean_regex-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5427 2023-06-10 02:18:18.000000 korean_regex-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:53.248903 korean_regex-0.0.2/ko_re/
+-rw-rw-rw-   0        0        0       84 2023-06-10 02:35:30.000000 korean_regex-0.0.2/ko_re/__init__.py
+-rw-rw-rw-   0        0        0    10476 2023-06-10 02:06:52.000000 korean_regex-0.0.2/ko_re/ko_re.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:53.258771 korean_regex-0.0.2/korean_regex.egg-info/
+-rw-rw-rw-   0        0        0     6366 2023-06-10 02:37:53.000000 korean_regex-0.0.2/korean_regex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-10 02:37:53.000000 korean_regex-0.0.2/korean_regex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 02:37:53.000000 korean_regex-0.0.2/korean_regex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-10 02:31:17.000000 korean_regex-0.0.2/korean_regex.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-10 02:37:53.000000 korean_regex-0.0.2/korean_regex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 02:37:53.260485 korean_regex-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-06-10 02:37:48.000000 korean_regex-0.0.2/setup.py
```

### Comparing `korean_regex-0.0.1/LICENSE` & `korean_regex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `korean_regex-0.0.1/PKG-INFO` & `korean_regex-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: korean_regex
-Version: 0.0.1
+Version: 0.0.2
 Summary: regex for Korean - Being free from ord/chr in Hangeul analysis.
 Home-page: https://github.com/ilotoki0804/ko_re
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: re,regex,korean regex,regular expression,정규표현식,hangeul,hangul,hangeul analysis
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `korean_regex-0.0.1/README.md` & `korean_regex-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `korean_regex-0.0.1/ko_re/ko_re.py` & `korean_regex-0.0.2/ko_re/ko_re.py`

 * *Files identical despite different names*

### Comparing `korean_regex-0.0.1/korean_regex.egg-info/PKG-INFO` & `korean_regex-0.0.2/korean_regex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: korean-regex
-Version: 0.0.1
+Version: 0.0.2
 Summary: regex for Korean - Being free from ord/chr in Hangeul analysis.
 Home-page: https://github.com/ilotoki0804/ko_re
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: re,regex,korean regex,regular expression,정규표현식,hangeul,hangul,hangeul analysis
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `korean_regex-0.0.1/setup.py` & `korean_regex-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='korean_regex',
-    version='0.0.1',
+    version='0.0.2',
     description='regex for Korean - Being free from ord/chr in Hangeul analysis.',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/ko_re',
```

