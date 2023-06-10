# Comparing `tmp/csle_system_identification-0.2.8.tar.gz` & `tmp/csle_system_identification-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_system_identification-0.2.8.tar", last modified: Sun Jun  4 08:48:46 2023, max compression
+gzip compressed data, was "csle_system_identification-0.2.9.tar", last modified: Sun Jun  4 09:09:07 2023, max compression
```

## Comparing `csle_system_identification-0.2.8.tar` & `csle_system_identification-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.999965 csle_system_identification-0.2.8/
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-06-04 08:48:45.999965 csle_system_identification-0.2.8/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4235 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      686 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1340 2023-06-04 08:48:45.999965 csle_system_identification-0.2.8/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.995965 csle_system_identification-0.2.8/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.995965 csle_system_identification-0.2.8/src/csle_system_identification/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 08:47:59.000000 csle_system_identification-0.2.8/src/csle_system_identification/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.995965 csle_system_identification-0.2.8/src/csle_system_identification/base/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2074 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/base/base_system_identification_algorithm.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.995965 csle_system_identification-0.2.8/src/csle_system_identification/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      688 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.995965 csle_system_identification-0.2.8/src/csle_system_identification/empirical/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/empirical/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7249 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/empirical/empirical_algorithm.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17108 2023-04-18 12:43:31.000000 csle_system_identification-0.2.8/src/csle_system_identification/emulator.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.995965 csle_system_identification-0.2.8/src/csle_system_identification/expectation_maximization/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/expectation_maximization/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7494 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.999965 csle_system_identification-0.2.8/src/csle_system_identification/gp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/gp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9801 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/gp/gp_regression_algorithm.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      555 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.999965 csle_system_identification-0.2.8/src/csle_system_identification/job_controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/job_controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2159 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/job_controllers/data_collection_job_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2212 2023-03-28 14:03:22.000000 csle_system_identification-0.2.8/src/csle_system_identification/job_controllers/system_identification_job_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:45.995965 csle_system_identification-0.2.8/src/csle_system_identification.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-06-04 08:48:45.000000 csle_system_identification-0.2.8/src/csle_system_identification.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1412 2023-06-04 08:48:45.000000 csle_system_identification-0.2.8/src/csle_system_identification.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 08:48:45.000000 csle_system_identification-0.2.8/src/csle_system_identification.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:14.000000 csle_system_identification-0.2.8/src/csle_system_identification.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      257 2023-06-04 08:48:45.000000 csle_system_identification-0.2.8/src/csle_system_identification.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       27 2023-06-04 08:48:45.000000 csle_system_identification-0.2.8/src/csle_system_identification.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4235 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      686 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1340 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 09:08:20.000000 csle_system_identification-0.2.9/src/csle_system_identification/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2074 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/base/base_system_identification_algorithm.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      688 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification/empirical/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/empirical/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7249 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/empirical/empirical_algorithm.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17108 2023-04-18 12:43:31.000000 csle_system_identification-0.2.9/src/csle_system_identification/emulator.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification/expectation_maximization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/expectation_maximization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7494 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification/gp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/gp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9801 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/gp/gp_regression_algorithm.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      555 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2159 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/job_controllers/data_collection_job_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2212 2023-03-28 14:03:22.000000 csle_system_identification-0.2.9/src/csle_system_identification/job_controllers/system_identification_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:07.145795 csle_system_identification-0.2.9/src/csle_system_identification.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-06-04 09:09:06.000000 csle_system_identification-0.2.9/src/csle_system_identification.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1412 2023-06-04 09:09:07.000000 csle_system_identification-0.2.9/src/csle_system_identification.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 09:09:06.000000 csle_system_identification-0.2.9/src/csle_system_identification.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:14.000000 csle_system_identification-0.2.9/src/csle_system_identification.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      257 2023-06-04 09:09:07.000000 csle_system_identification-0.2.9/src/csle_system_identification.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       27 2023-06-04 09:09:07.000000 csle_system_identification-0.2.9/src/csle_system_identification.egg-info/top_level.txt
```

### Comparing `csle_system_identification-0.2.8/PKG-INFO` & `csle_system_identification-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_system_identification
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.2.8/README.md` & `csle_system_identification-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/pyproject.toml` & `csle_system_identification-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/setup.cfg` & `csle_system_identification-0.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.8
-	csle-collector>=0.2.8
-	csle-attacker>=0.2.8
-	csle-defender>=0.2.8
+	csle-common>=0.2.9
+	csle-collector>=0.2.9
+	csle-attacker>=0.2.9
+	csle-defender>=0.2.9
 	gpytorch>=1.9.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
```

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/base/base_system_identification_algorithm.py` & `csle_system_identification-0.2.9/src/csle_system_identification/base/base_system_identification_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/constants/constants.py` & `csle_system_identification-0.2.9/src/csle_system_identification/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/empirical/empirical_algorithm.py` & `csle_system_identification-0.2.9/src/csle_system_identification/empirical/empirical_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/emulator.py` & `csle_system_identification-0.2.9/src/csle_system_identification/emulator.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py` & `csle_system_identification-0.2.9/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/gp/gp_regression_algorithm.py` & `csle_system_identification-0.2.9/src/csle_system_identification/gp/gp_regression_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py` & `csle_system_identification-0.2.9/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/job_controllers/data_collection_job_manager.py` & `csle_system_identification-0.2.9/src/csle_system_identification/job_controllers/data_collection_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification/job_controllers/system_identification_job_manager.py` & `csle_system_identification-0.2.9/src/csle_system_identification/job_controllers/system_identification_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification.egg-info/PKG-INFO` & `csle_system_identification-0.2.9/src/csle_system_identification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-system-identification
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.2.8/src/csle_system_identification.egg-info/SOURCES.txt` & `csle_system_identification-0.2.9/src/csle_system_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

