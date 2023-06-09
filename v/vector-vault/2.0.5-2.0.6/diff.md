# Comparing `tmp/vector_vault-2.0.5.tar.gz` & `tmp/vector_vault-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.5.tar", last modified: Fri Jun  9 20:04:21 2023, max compression
+gzip compressed data, was "vector_vault-2.0.6.tar", last modified: Fri Jun  9 23:05:34 2023, max compression
```

## Comparing `vector_vault-2.0.5.tar` & `vector_vault-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 20:04:21.536211 vector_vault-2.0.5/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-09 20:04:21.536071 vector_vault-2.0.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20080 2023-06-08 04:45:19.000000 vector_vault-2.0.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-09 20:04:21.536245 vector_vault-2.0.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-09 20:04:14.000000 vector_vault-2.0.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 20:04:21.532836 vector_vault-2.0.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 20:04:21.535655 vector_vault-2.0.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.0.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.5/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1954 2023-06-09 19:11:10.000000 vector_vault-2.0.5/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2398 2023-06-08 04:57:38.000000 vector_vault-2.0.5/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.5/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    30807 2023-06-09 19:58:53.000000 vector_vault-2.0.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.5/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 23:05:34.887707 vector_vault-2.0.6/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.6/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20846 2023-06-09 23:05:34.887574 vector_vault-2.0.6/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20121 2023-06-09 23:05:24.000000 vector_vault-2.0.6/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-09 23:05:34.887744 vector_vault-2.0.6/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-09 23:05:32.000000 vector_vault-2.0.6/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 23:05:34.884055 vector_vault-2.0.6/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20846 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 23:05:34.887255 vector_vault-2.0.6/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.0.6/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.6/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1954 2023-06-09 19:11:10.000000 vector_vault-2.0.6/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.6/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.6/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.6/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2398 2023-06-08 04:57:38.000000 vector_vault-2.0.6/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.6/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    30807 2023-06-09 19:58:53.000000 vector_vault-2.0.6/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.6/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.6/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.5/LICENSE` & `vector_vault-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/PKG-INFO` & `vector_vault-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.0.5
+Version: 2.0.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -249,15 +249,15 @@
 <br>
 <br>
 
 # Streaming:
 Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-![Alt text](https://github.com/John-Rood/VectorVault/blob/main/examples/Streaming%20Demo%20Offish.gif)
+![Alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/559fd0ea-8fa7-40a2-9260-c5b0f4b063b5/Streaming+Demo+Offish.gif)
 
 ## get_chat_stream():
 
 Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
 Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
 `cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
 `print_stream()` is for local console printing.
```

### Comparing `vector_vault-2.0.5/README.md` & `vector_vault-2.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 <br>
 <br>
 
 # Streaming:
 Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-![Alt text](https://github.com/John-Rood/VectorVault/blob/main/examples/Streaming%20Demo%20Offish.gif)
+![Alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/559fd0ea-8fa7-40a2-9260-c5b0f4b063b5/Streaming+Demo+Offish.gif)
 
 ## get_chat_stream():
 
 Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
 Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
 `cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
 `print_stream()` is for local console printing.
```

### Comparing `vector_vault-2.0.5/setup.py` & `vector_vault-2.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.5",
+    version="2.0.6",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.6/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.0.5
+Version: 2.0.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -249,15 +249,15 @@
 <br>
 <br>
 
 # Streaming:
 Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-![Alt text](https://github.com/John-Rood/VectorVault/blob/main/examples/Streaming%20Demo%20Offish.gif)
+![Alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/559fd0ea-8fa7-40a2-9260-c5b0f4b063b5/Streaming+Demo+Offish.gif)
 
 ## get_chat_stream():
 
 Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
 Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
 `cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
 `print_stream()` is for local console printing.
```

### Comparing `vector_vault-2.0.5/vectorvault/ai.py` & `vector_vault-2.0.6/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/cloud_api.py` & `vector_vault-2.0.6/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/cloudmanager.py` & `vector_vault-2.0.6/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/creds.py` & `vector_vault-2.0.6/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/download.py` & `vector_vault-2.0.6/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/itemize.py` & `vector_vault-2.0.6/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/tools_gpt.py` & `vector_vault-2.0.6/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/vault.py` & `vector_vault-2.0.6/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.5/vectorvault/vecreq.py` & `vector_vault-2.0.6/vectorvault/vecreq.py`

 * *Files identical despite different names*

