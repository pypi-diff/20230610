# Comparing `tmp/psychicapi-0.7.1.tar.gz` & `tmp/psychicapi-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.7.1.tar", last modified: Wed Jun  7 02:42:11 2023, max compression
+gzip compressed data, was "psychicapi-0.7.2.tar", last modified: Sat Jun 10 02:01:32 2023, max compression
```

## Comparing `psychicapi-0.7.1.tar` & `psychicapi-0.7.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:42:11.441211 psychicapi-0.7.1/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1776 2023-06-07 02:42:11.441073 psychicapi-0.7.1/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-29 20:05:07.000000 psychicapi-0.7.1/README.md
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:42:11.439919 psychicapi-0.7.1/psychicapi/
--rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.7.1/psychicapi/__init__.py
--rw-r--r--   0 jasonfan   (501) staff       (20)     2563 2023-06-07 02:41:01.000000 psychicapi-0.7.1/psychicapi/psychic.py
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:42:11.440861 psychicapi-0.7.1/psychicapi.egg-info/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1776 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/requires.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-06-07 02:42:11.441275 psychicapi-0.7.1/setup.cfg
--rw-r--r--   0 jasonfan   (501) staff       (20)      666 2023-06-07 02:42:07.000000 psychicapi-0.7.1/setup.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-10 02:01:32.073785 psychicapi-0.7.2/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1842 2023-06-10 02:01:32.073650 psychicapi-0.7.2/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1575 2023-06-07 19:40:18.000000 psychicapi-0.7.2/README.md
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-10 02:01:32.072607 psychicapi-0.7.2/psychicapi/
+-rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.7.2/psychicapi/__init__.py
+-rw-r--r--   0 jasonfan   (501) staff       (20)     2940 2023-06-10 02:01:10.000000 psychicapi-0.7.2/psychicapi/psychic.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-10 02:01:32.073421 psychicapi-0.7.2/psychicapi.egg-info/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1842 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-06-10 02:01:32.073831 psychicapi-0.7.2/setup.cfg
+-rw-r--r--   0 jasonfan   (501) staff       (20)      666 2023-06-10 02:01:27.000000 psychicapi-0.7.2/setup.py
```

### Comparing `psychicapi-0.7.1/PKG-INFO` & `psychicapi-0.7.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
 
@@ -13,15 +13,15 @@
 ## What is Psychic?
 
 Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
 
 ## Quick start
 
 1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps. Or, use the [playground](https://dashboard.psychic.dev/playground) to connect your own data sources.
 3. Use `psychicapi` to retrieve documents from your active connections.
 
 ## Usage 
 
 ### Initialization
 
 ```
@@ -29,15 +29,15 @@
 psychic = Psychic(secret_key="secret-key")
 ```
 
 ### Get active connections
 
 ```
 # Get all active connections and optionally filter by connector id and/or account id
-connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
+connections = psychic.get_connections(account_id="account_id")
 ```
 
 ### Retrieve documents from a connection
 
 ```
-docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
+docs = psychic.get_documents(account_id="account_id")
 ```
```

### Comparing `psychicapi-0.7.1/README.md` & `psychicapi-0.7.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## What is Psychic?
 
 Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
 
 ## Quick start
 
 1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps. Or, use the [playground](https://dashboard.psychic.dev/playground) to connect your own data sources.
 3. Use `psychicapi` to retrieve documents from your active connections.
 
 ## Usage 
 
 ### Initialization
 
 ```
@@ -21,15 +21,15 @@
 psychic = Psychic(secret_key="secret-key")
 ```
 
 ### Get active connections
 
 ```
 # Get all active connections and optionally filter by connector id and/or account id
-connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
+connections = psychic.get_connections(account_id="account_id")
 ```
 
 ### Retrieve documents from a connection
 
 ```
-docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
+docs = psychic.get_documents(account_id="account_id")
 ```
```

### Comparing `psychicapi-0.7.1/psychicapi/psychic.py` & `psychicapi-0.7.2/psychicapi/psychic.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,20 +10,26 @@
     slack = "slack"
 
 class Psychic:
     def __init__(self, secret_key: str):
         self.api_url = "https://api.psychic.dev/"
         self.secret_key = secret_key
 
-    def get_documents(self, *, account_id: str, connector_id: Optional[ConnectorId] = None):
+    def get_documents(self, *, account_id: str, connector_id: Optional[ConnectorId] = None, pre_chunked: Optional[bool] = False, min_chunk_size: Optional[int] = None, max_chunk_size: Optional[int] = None):
         body = {
             "account_id": account_id
         }
         if connector_id is not None:
             body["connector_id"] = connector_id.value
+        if pre_chunked is not None:
+            body["pre_chunked"] = pre_chunked
+        if min_chunk_size is not None:
+            body["min_chunk_size"] = min_chunk_size
+        if max_chunk_size is not None:
+            body["max_chunk_size"] = max_chunk_size
         response = requests.post(
             self.api_url + "get-documents",
             json=body,
             headers={
                 'Authorization': 'Bearer ' + self.secret_key,
                 'Accept': 'application/json'
             }
```

### Comparing `psychicapi-0.7.1/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.7.2/psychicapi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
 
@@ -13,15 +13,15 @@
 ## What is Psychic?
 
 Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
 
 ## Quick start
 
 1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps. Or, use the [playground](https://dashboard.psychic.dev/playground) to connect your own data sources.
 3. Use `psychicapi` to retrieve documents from your active connections.
 
 ## Usage 
 
 ### Initialization
 
 ```
@@ -29,15 +29,15 @@
 psychic = Psychic(secret_key="secret-key")
 ```
 
 ### Get active connections
 
 ```
 # Get all active connections and optionally filter by connector id and/or account id
-connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
+connections = psychic.get_connections(account_id="account_id")
 ```
 
 ### Retrieve documents from a connection
 
 ```
-docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
+docs = psychic.get_documents(account_id="account_id")
 ```
```

### Comparing `psychicapi-0.7.1/setup.py` & `psychicapi-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.7.1',
+    version='0.7.2',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

