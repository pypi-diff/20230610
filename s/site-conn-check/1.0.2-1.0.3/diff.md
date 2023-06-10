# Comparing `tmp/site_conn_check-1.0.2.tar.gz` & `tmp/site_conn_check-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "site_conn_check-1.0.2.tar", last modified: Fri Jun  9 20:43:55 2023, max compression
+gzip compressed data, was "site_conn_check-1.0.3.tar", last modified: Fri Jun  9 20:45:55 2023, max compression
```

## Comparing `site_conn_check-1.0.2.tar` & `site_conn_check-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:43:55.827567 site_conn_check-1.0.2/
--rw-rw-rw-   0        0        0     1088 2023-06-09 17:42:27.000000 site_conn_check-1.0.2/LICENCE
--rw-rw-rw-   0        0        0     1886 2023-06-09 20:43:55.826567 site_conn_check-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1435 2023-06-09 20:35:05.000000 site_conn_check-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 20:43:55.828565 site_conn_check-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1326 2023-06-09 20:43:34.000000 site_conn_check-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:43:55.769719 site_conn_check-1.0.2/site_conn_check/
--rw-rw-rw-   0        0        0        0 2023-06-09 18:03:41.000000 site_conn_check-1.0.2/site_conn_check/__init__.py
--rw-rw-rw-   0        0        0      715 2023-06-09 19:42:55.000000 site_conn_check-1.0.2/site_conn_check/conn_check.py
--rw-rw-rw-   0        0        0     3568 2023-06-09 17:24:19.000000 site_conn_check-1.0.2/site_conn_check/main.py
--rw-rw-rw-   0        0        0     3685 2023-06-09 19:17:47.000000 site_conn_check-1.0.2/site_conn_check/sites_db.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:43:55.824577 site_conn_check-1.0.2/site_conn_check.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-06-09 20:43:55.000000 site_conn_check-1.0.2/site_conn_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-06-09 20:43:55.000000 site_conn_check-1.0.2/site_conn_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:43:55.000000 site_conn_check-1.0.2/site_conn_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-09 20:43:55.000000 site_conn_check-1.0.2/site_conn_check.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-09 20:43:55.000000 site_conn_check-1.0.2/site_conn_check.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      214 2023-06-09 20:43:55.000000 site_conn_check-1.0.2/site_conn_check.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 20:43:55.000000 site_conn_check-1.0.2/site_conn_check.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 20:45:55.783221 site_conn_check-1.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-06-09 17:42:27.000000 site_conn_check-1.0.3/LICENCE
+-rw-rw-rw-   0        0        0     1940 2023-06-09 20:45:55.782224 site_conn_check-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1435 2023-06-09 20:35:05.000000 site_conn_check-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 20:45:55.783221 site_conn_check-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1380 2023-06-09 20:45:44.000000 site_conn_check-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:45:55.733356 site_conn_check-1.0.3/site_conn_check/
+-rw-rw-rw-   0        0        0        0 2023-06-09 18:03:41.000000 site_conn_check-1.0.3/site_conn_check/__init__.py
+-rw-rw-rw-   0        0        0      715 2023-06-09 19:42:55.000000 site_conn_check-1.0.3/site_conn_check/conn_check.py
+-rw-rw-rw-   0        0        0     3568 2023-06-09 17:24:19.000000 site_conn_check-1.0.3/site_conn_check/main.py
+-rw-rw-rw-   0        0        0     3685 2023-06-09 19:17:47.000000 site_conn_check-1.0.3/site_conn_check/sites_db.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:45:55.779234 site_conn_check-1.0.3/site_conn_check.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-09 20:45:55.000000 site_conn_check-1.0.3/site_conn_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-06-09 20:45:55.000000 site_conn_check-1.0.3/site_conn_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:45:55.000000 site_conn_check-1.0.3/site_conn_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-09 20:45:55.000000 site_conn_check-1.0.3/site_conn_check.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-09 20:45:55.000000 site_conn_check-1.0.3/site_conn_check.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      214 2023-06-09 20:45:55.000000 site_conn_check-1.0.3/site_conn_check.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 20:45:55.000000 site_conn_check-1.0.3/site_conn_check.egg-info/top_level.txt
```

### Comparing `site_conn_check-1.0.2/LICENCE` & `site_conn_check-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `site_conn_check-1.0.2/PKG-INFO` & `site_conn_check-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: site_conn_check
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package to check status code and response time of websites
+Home-page: https://github.com/rxxyxd/site-conn-check
 Author: Joshua Abbey
 Author-email: Joshuaabbey2022@gmail.com
 License: LICENCE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `site_conn_check-1.0.2/README.md` & `site_conn_check-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `site_conn_check-1.0.2/setup.py` & `site_conn_check-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='site_conn_check',
-    version='1.0.2',
+    version='1.0.3',
         zip_safe=False,
     author="Joshua Abbey",
     author_email="Joshuaabbey2022@gmail.com",
     description="Package to check status code and response time of websites",
+    url="https://github.com/rxxyxd/site-conn-check",
     long_description=long_description,
     long_description_content_type ='text/markdown',
     packages=["site_conn_check"],
     install_requires=[
         'certifi==2023.5.7',
         'charset-normalizer==3.1.0',
         'decorator==5.1.1',
```

### Comparing `site_conn_check-1.0.2/site_conn_check/conn_check.py` & `site_conn_check-1.0.3/site_conn_check/conn_check.py`

 * *Files identical despite different names*

### Comparing `site_conn_check-1.0.2/site_conn_check/main.py` & `site_conn_check-1.0.3/site_conn_check/main.py`

 * *Files identical despite different names*

### Comparing `site_conn_check-1.0.2/site_conn_check/sites_db.py` & `site_conn_check-1.0.3/site_conn_check/sites_db.py`

 * *Files identical despite different names*

### Comparing `site_conn_check-1.0.2/site_conn_check.egg-info/PKG-INFO` & `site_conn_check-1.0.3/site_conn_check.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: site-conn-check
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package to check status code and response time of websites
+Home-page: https://github.com/rxxyxd/site-conn-check
 Author: Joshua Abbey
 Author-email: Joshuaabbey2022@gmail.com
 License: LICENCE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

