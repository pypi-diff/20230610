# Comparing `tmp/counterplots-0.0.1.tar.gz` & `tmp/counterplots-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "counterplots-0.0.1.tar", last modified: Sat Jun 10 15:46:10 2023, max compression
+gzip compressed data, was "counterplots-0.0.2.tar", last modified: Sat Jun 10 16:46:13 2023, max compression
```

## Comparing `counterplots-0.0.1.tar` & `counterplots-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 15:46:10.250805 counterplots-0.0.1/
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     1067 2023-06-10 15:01:31.000000 counterplots-0.0.1/LICENSE.txt
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     1585 2023-06-10 15:46:10.250805 counterplots-0.0.1/PKG-INFO
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     1036 2023-06-10 15:14:15.000000 counterplots-0.0.1/README.md
-drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 15:46:10.246804 counterplots-0.0.1/counterplots/
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     7742 2023-06-08 13:25:54.000000 counterplots-0.0.1/counterplots/__init__.py
-drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 15:46:10.246804 counterplots-0.0.1/counterplots/utils/
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-08 12:29:34.000000 counterplots-0.0.1/counterplots/utils/__init__.py
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)    10947 2023-06-10 12:25:27.000000 counterplots-0.0.1/counterplots/utils/plots.py
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     8868 2023-06-10 12:25:34.000000 counterplots-0.0.1/counterplots/utils/process.py
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     1631 2023-06-10 12:25:46.000000 counterplots-0.0.1/counterplots/utils/verification.py
-drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 15:46:10.246804 counterplots-0.0.1/counterplots.egg-info/
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     1585 2023-06-10 15:46:10.000000 counterplots-0.0.1/counterplots.egg-info/PKG-INFO
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)      493 2023-06-10 15:46:10.000000 counterplots-0.0.1/counterplots.egg-info/SOURCES.txt
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)        1 2023-06-10 15:46:10.000000 counterplots-0.0.1/counterplots.egg-info/dependency_links.txt
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)       17 2023-06-10 15:46:10.000000 counterplots-0.0.1/counterplots.egg-info/requires.txt
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)       19 2023-06-10 15:46:10.000000 counterplots-0.0.1/counterplots.egg-info/top_level.txt
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)       38 2023-06-10 15:46:10.250805 counterplots-0.0.1/setup.cfg
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)      998 2023-06-10 15:19:20.000000 counterplots-0.0.1/setup.py
-drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 15:46:10.246804 counterplots-0.0.1/tests/
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     4530 2023-06-10 12:29:17.000000 counterplots-0.0.1/tests/test____init__.py
-drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 15:46:10.250805 counterplots-0.0.1/tests/utils/
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-08 12:24:10.000000 counterplots-0.0.1/tests/utils/__init__.py
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     3095 2023-06-10 12:40:22.000000 counterplots-0.0.1/tests/utils/test_plots.py
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     5550 2023-06-10 12:29:50.000000 counterplots-0.0.1/tests/utils/test_process.py
--rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     2868 2023-06-10 12:30:25.000000 counterplots-0.0.1/tests/utils/test_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:46:13.713659 counterplots-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-10 16:45:35.000000 counterplots-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-10 16:46:13.713659 counterplots-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-10 16:45:35.000000 counterplots-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:46:13.713659 counterplots-0.0.2/counterplots/
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-10 16:45:35.000000 counterplots-0.0.2/counterplots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:46:13.713659 counterplots-0.0.2/counterplots/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:45:35.000000 counterplots-0.0.2/counterplots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-10 16:45:35.000000 counterplots-0.0.2/counterplots/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-10 16:45:35.000000 counterplots-0.0.2/counterplots/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-10 16:45:35.000000 counterplots-0.0.2/counterplots/utils/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:46:13.713659 counterplots-0.0.2/counterplots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-10 16:46:13.000000 counterplots-0.0.2/counterplots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-10 16:46:13.000000 counterplots-0.0.2/counterplots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:46:13.000000 counterplots-0.0.2/counterplots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-10 16:46:13.000000 counterplots-0.0.2/counterplots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 16:46:13.000000 counterplots-0.0.2/counterplots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:46:13.713659 counterplots-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-10 16:45:35.000000 counterplots-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:46:13.709658 counterplots-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:46:13.713659 counterplots-0.0.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:45:35.000000 counterplots-0.0.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-10 16:45:35.000000 counterplots-0.0.2/tests/utils/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-10 16:45:35.000000 counterplots-0.0.2/tests/utils/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-10 16:45:35.000000 counterplots-0.0.2/tests/utils/test_verification.py
```

### Comparing `counterplots-0.0.1/LICENSE.txt` & `counterplots-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.1/counterplots/__init__.py` & `counterplots-0.0.2/counterplots/__init__.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.1/counterplots/utils/plots.py` & `counterplots-0.0.2/counterplots/utils/plots.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.1/counterplots/utils/process.py` & `counterplots-0.0.2/counterplots/utils/process.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.1/counterplots/utils/verification.py` & `counterplots-0.0.2/counterplots/utils/verification.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.1/setup.py` & `counterplots-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     LICENSE = f.read()
 
 with open('HISTORY.md') as f:
     HISTORY = f.read()
 
 setup_args = dict(
     name='counterplots',
-    version='0.0.1',
+    version='0.0.2',
     description='Plotting tool for counterfactual explanations',
     long_description_content_type='text/markdown',
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(exclude=('tests', 'exp_notebooks', '_static')),
     author='Raphael Mazzine Barbosa de Oliveira, Bjorge Meulemeester',
     keywords=['Counterfactual Explanations', 'Visualization', 'Plotting', 'Explainable Artificial Intelligence', 'XAI', 'Machine Learning'],
```

### Comparing `counterplots-0.0.1/tests/utils/test_plots.py` & `counterplots-0.0.2/tests/utils/test_plots.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.1/tests/utils/test_process.py` & `counterplots-0.0.2/tests/utils/test_process.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.1/tests/utils/test_verification.py` & `counterplots-0.0.2/tests/utils/test_verification.py`

 * *Files identical despite different names*

