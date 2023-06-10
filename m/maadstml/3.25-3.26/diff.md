# Comparing `tmp/maadstml-3.25.tar.gz` & `tmp/maadstml-3.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.25.tar", last modified: Sat Jun 10 20:00:22 2023, max compression
+gzip compressed data, was "maadstml-3.26.tar", last modified: Sat Jun 10 20:23:25 2023, max compression
```

## Comparing `maadstml-3.25.tar` & `maadstml-3.26.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 20:00:22.092486 maadstml-3.25/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.25/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.25/MANIFEST.in
--rw-rw-rw-   0        0        0   171897 2023-06-10 20:00:22.092486 maadstml-3.25/PKG-INFO
--rw-rw-rw-   0        0        0   171300 2023-06-10 19:59:31.000000 maadstml-3.25/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 20:00:22.061183 maadstml-3.25/maadstml/
--rw-rw-rw-   0        0        0     2121 2023-06-10 19:55:10.000000 maadstml-3.25/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.25/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    65114 2023-06-10 19:54:10.000000 maadstml-3.25/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.25/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-10 20:00:22.092486 maadstml-3.25/maadstml.egg-info/
--rw-rw-rw-   0        0        0   171897 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-10 20:00:22.000000 maadstml-3.25/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:04.000000 maadstml-3.25/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 20:00:22.092486 maadstml-3.25/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-10 19:55:28.000000 maadstml-3.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:23:25.167508 maadstml-3.26/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.26/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.26/MANIFEST.in
+-rw-rw-rw-   0        0        0   171897 2023-06-10 20:23:25.167508 maadstml-3.26/PKG-INFO
+-rw-rw-rw-   0        0        0   171300 2023-06-10 19:59:31.000000 maadstml-3.26/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 20:23:25.140138 maadstml-3.26/maadstml/
+-rw-rw-rw-   0        0        0     2121 2023-06-10 19:55:10.000000 maadstml-3.26/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.26/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    65114 2023-06-10 19:54:10.000000 maadstml-3.26/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.26/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:23:25.163347 maadstml-3.26/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   171897 2023-06-10 20:23:25.000000 maadstml-3.26/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-10 20:23:25.000000 maadstml-3.26/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 20:23:25.000000 maadstml-3.26/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-06-10 20:23:25.000000 maadstml-3.26/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 20:23:25.000000 maadstml-3.26/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2021-02-05 16:13:04.000000 maadstml-3.26/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 20:23:25.167508 maadstml-3.26/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-10 20:23:20.000000 maadstml-3.26/setup.py
```

### Comparing `maadstml-3.25/LICENSE.txt` & `maadstml-3.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.25/PKG-INFO` & `maadstml-3.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.25
+Version: 3.26
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.25/README.md` & `maadstml-3.26/README.md`

 * *Files identical despite different names*

### Comparing `maadstml-3.25/maadstml/__init__.py` & `maadstml-3.26/maadstml/__init__.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.25/maadstml/readpdf.py` & `maadstml-3.26/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.25/maadstml/sendfiles.py` & `maadstml-3.26/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.25/maadstml/tmltextsummary.py` & `maadstml-3.26/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.25/maadstml.egg-info/PKG-INFO` & `maadstml-3.26/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.25
+Version: 3.26
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.25/setup.py` & `maadstml-3.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.25',
+    version='3.26',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

