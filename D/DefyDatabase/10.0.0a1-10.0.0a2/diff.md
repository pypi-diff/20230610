# Comparing `tmp/DefyDatabase-10.0.0a1.tar.gz` & `tmp/DefyDatabase-10.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a1.tar", last modified: Sat Jun 10 11:19:43 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0a2.tar", last modified: Sat Jun 10 11:26:24 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a1.tar` & `DefyDatabase-10.0.0a2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 11:19:43.250388 DefyDatabase-10.0.0a1/
-drwxrwxrwx   0        0        0        0 2023-06-10 11:19:43.240389 DefyDatabase-10.0.0a1/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      506 2023-06-10 11:19:43.000000 DefyDatabase-10.0.0a1/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-10 11:19:43.000000 DefyDatabase-10.0.0a1/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 11:19:43.000000 DefyDatabase-10.0.0a1/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-10 11:19:43.000000 DefyDatabase-10.0.0a1/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      506 2023-06-10 11:19:43.249388 DefyDatabase-10.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 11:19:43.244392 DefyDatabase-10.0.0a1/defy/
--rw-rw-rw-   0        0        0     5451 2023-06-10 11:19:01.000000 DefyDatabase-10.0.0a1/defy/__init__.py
--rw-rw-rw-   0        0        0     1558 2023-05-06 04:18:35.000000 DefyDatabase-10.0.0a1/defy/reader.py
--rw-rw-rw-   0        0        0       42 2023-06-10 11:19:43.250388 DefyDatabase-10.0.0a1/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-06-10 11:19:17.000000 DefyDatabase-10.0.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 11:26:24.006665 DefyDatabase-10.0.0a2/
+drwxrwxrwx   0        0        0        0 2023-06-10 11:26:23.999364 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      506 2023-06-10 11:26:24.004661 DefyDatabase-10.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a2/README.md
+-rw-rw-rw-   0        0        0     6986 2023-06-10 11:24:20.000000 DefyDatabase-10.0.0a2/defy.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 11:26:24.006665 DefyDatabase-10.0.0a2/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-06-10 11:25:17.000000 DefyDatabase-10.0.0a2/setup.py
```

### Comparing `DefyDatabase-10.0.0a1/setup.py` & `DefyDatabase-10.0.0a2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     name="DefyDatabase",
     version=defy.version,
     author="Defymen",
     author_email="vmuonline@126.com",
     description="Database for personal data based on SQLite",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
+    py_modules=['defy'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

