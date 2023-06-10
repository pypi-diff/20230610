# Comparing `tmp/custom_secrets_manager-1.0.8b0.tar.gz` & `tmp/custom_secrets_manager-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_secrets_manager-1.0.8b0.tar", last modified: Sat Jun 10 14:40:20 2023, max compression
+gzip compressed data, was "custom_secrets_manager-1.1.0.tar", last modified: Sat Jun 10 14:57:43 2023, max compression
```

## Comparing `custom_secrets_manager-1.0.8b0.tar` & `custom_secrets_manager-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:40:20.502818 custom_secrets_manager-1.0.8b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-10 14:40:20.502818 custom_secrets_manager-1.0.8b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:40:20.498818 custom_secrets_manager-1.0.8b0/custom_secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager/encryption_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager/secrets_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager/starter_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager/temp_log_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager/workflow_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:40:20.502818 custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-10 14:40:20.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-10 14:40:20.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:40:20.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-10 14:40:20.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 14:40:20.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-10 14:40:20.000000 custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 14:40:20.502818 custom_secrets_manager-1.0.8b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-10 14:40:03.000000 custom_secrets_manager-1.0.8b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:57:43.530628 custom_secrets_manager-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-10 14:57:43.530628 custom_secrets_manager-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:57:43.530628 custom_secrets_manager-1.1.0/custom_secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/custom_secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/custom_secrets_manager/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/custom_secrets_manager/encryption_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/custom_secrets_manager/secrets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/custom_secrets_manager/starter_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/custom_secrets_manager/temp_log_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/custom_secrets_manager/workflow_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:57:43.530628 custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-10 14:57:43.000000 custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-10 14:57:43.000000 custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:57:43.000000 custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-10 14:57:43.000000 custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 14:57:43.000000 custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-10 14:57:43.000000 custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 14:57:43.530628 custom_secrets_manager-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-10 14:57:27.000000 custom_secrets_manager-1.1.0/setup.py
```

### Comparing `custom_secrets_manager-1.0.8b0/LICENSE` & `custom_secrets_manager-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/PKG-INFO` & `custom_secrets_manager-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: custom_secrets_manager
-Version: 1.0.8b0
+Version: 1.1.0
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `custom_secrets_manager-1.0.8b0/README.md` & `custom_secrets_manager-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/custom_secrets_manager/encryption_helper.py` & `custom_secrets_manager-1.1.0/custom_secrets_manager/encryption_helper.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/custom_secrets_manager/secrets_loader.py` & `custom_secrets_manager-1.1.0/custom_secrets_manager/secrets_loader.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/custom_secrets_manager/starter_process.py` & `custom_secrets_manager-1.1.0/custom_secrets_manager/starter_process.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/custom_secrets_manager/temp_log_cleanup.py` & `custom_secrets_manager-1.1.0/custom_secrets_manager/temp_log_cleanup.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/custom_secrets_manager/workflow_helper.py` & `custom_secrets_manager-1.1.0/custom_secrets_manager/workflow_helper.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/PKG-INFO` & `custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: custom-secrets-manager
-Version: 1.0.8b0
+Version: 1.1.0
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `custom_secrets_manager-1.0.8b0/custom_secrets_manager.egg-info/SOURCES.txt` & `custom_secrets_manager-1.1.0/custom_secrets_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.8b0/setup.py` & `custom_secrets_manager-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     long_description_content_type="text/markdown",
     author=AUTHOR,
     license=LICENSE,
     url=URL,
     packages=find_packages(),
     install_requires=REQUIRES,
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

