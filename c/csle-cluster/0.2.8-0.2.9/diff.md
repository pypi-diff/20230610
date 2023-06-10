# Comparing `tmp/csle_cluster-0.2.8.tar.gz` & `tmp/csle_cluster-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.2.8.tar", last modified: Sun Jun  4 08:49:54 2023, max compression
+gzip compressed data, was "csle_cluster-0.2.9.tar", last modified: Sun Jun  4 09:10:14 2023, max compression
```

## Comparing `csle_cluster-0.2.8.tar` & `csle_cluster-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/
--rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4256 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1406 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/src/csle_cluster/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/src/csle_cluster/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 08:47:59.000000 csle_cluster-0.2.8/src/csle_cluster/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   229454 2023-06-04 07:11:42.000000 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   269186 2023-05-03 08:18:28.000000 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   197343 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   349502 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   202990 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   188175 2023-04-18 12:48:07.000000 csle_cluster-0.2.8/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/src/csle_cluster/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/src/csle_cluster/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      375 2023-03-28 14:03:22.000000 csle_cluster-0.2.8/src/csle_cluster/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:54.716221 csle_cluster-0.2.8/src/csle_cluster.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-06-04 08:49:54.000000 csle_cluster-0.2.8/src/csle_cluster.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      805 2023-06-04 08:49:54.000000 csle_cluster-0.2.8/src/csle_cluster.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 08:49:54.000000 csle_cluster-0.2.8/src/csle_cluster.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.2.8/src/csle_cluster.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-06-04 08:49:54.000000 csle_cluster-0.2.8/src/csle_cluster.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       13 2023-06-04 08:49:54.000000 csle_cluster-0.2.8/src/csle_cluster.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:10:14.714904 csle_cluster-0.2.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-06-04 09:10:14.714904 csle_cluster-0.2.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4256 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1406 2023-06-04 09:10:14.714904 csle_cluster-0.2.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:10:14.710904 csle_cluster-0.2.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:10:14.710904 csle_cluster-0.2.9/src/csle_cluster/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/src/csle_cluster/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 09:08:20.000000 csle_cluster-0.2.9/src/csle_cluster/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:10:14.714904 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   229454 2023-06-04 07:11:42.000000 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   269186 2023-05-03 08:18:28.000000 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   197343 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   349502 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   202990 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   188175 2023-04-18 12:48:07.000000 csle_cluster-0.2.9/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:10:14.714904 csle_cluster-0.2.9/src/csle_cluster/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/src/csle_cluster/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      375 2023-03-28 14:03:22.000000 csle_cluster-0.2.9/src/csle_cluster/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:10:14.710904 csle_cluster-0.2.9/src/csle_cluster.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-06-04 09:10:14.000000 csle_cluster-0.2.9/src/csle_cluster.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      805 2023-06-04 09:10:14.000000 csle_cluster-0.2.9/src/csle_cluster.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 09:10:14.000000 csle_cluster-0.2.9/src/csle_cluster.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.2.9/src/csle_cluster.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-06-04 09:10:14.000000 csle_cluster-0.2.9/src/csle_cluster.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       13 2023-06-04 09:10:14.000000 csle_cluster-0.2.9/src/csle_cluster.egg-info/top_level.txt
```

### Comparing `csle_cluster-0.2.8/PKG-INFO` & `csle_cluster-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.8/README.md` & `csle_cluster-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/pyproject.toml` & `csle_cluster-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/setup.cfg` & `csle_cluster-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.27.2
 	grpcio-tools>=1.27.2
-	csle-collector>=0.2.8
-	csle-common>=0.2.8
-	csle-ryu>=0.2.8
+	csle-collector>=0.2.9
+	csle-common>=0.2.9
+	csle-ryu>=0.2.9
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.2.9/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.2.9/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.8/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.2.9/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.8/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.2.9/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

