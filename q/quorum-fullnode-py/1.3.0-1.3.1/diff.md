# Comparing `tmp/quorum_fullnode_py-1.3.0.tar.gz` & `tmp/quorum_fullnode_py-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_fullnode_py-1.3.0.tar", last modified: Fri May 19 12:27:53 2023, max compression
+gzip compressed data, was "quorum_fullnode_py-1.3.1.tar", last modified: Sat Jun 10 02:36:09 2023, max compression
```

## Comparing `quorum_fullnode_py-1.3.0.tar` & `quorum_fullnode_py-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.627620 quorum_fullnode_py-1.3.0/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:18.000000 quorum_fullnode_py-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     2522 2023-05-19 12:27:53.606482 quorum_fullnode_py-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1566 2023-04-03 04:33:04.000000 quorum_fullnode_py-1.3.0/README.md
--rw-rw-rw-   0        0        0      169 2023-02-23 03:21:16.000000 quorum_fullnode_py-1.3.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.572947 quorum_fullnode_py-1.3.0/quorum_fullnode_py/
--rw-rw-rw-   0        0        0      329 2023-05-19 08:07:50.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.595146 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/
--rw-rw-rw-   0        0        0      164 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/__init__.py
--rw-rw-rw-   0        0        0     6762 2023-05-19 08:38:21.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/base.py
--rw-rw-rw-   0        0        0    23454 2023-05-19 08:49:31.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/fullnode.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.601129 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/
--rw-rw-rw-   0        0        0      114 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/__init__.py
--rw-rw-rw-   0        0        0     1460 2023-04-06 03:32:26.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/_http.py
--rw-rw-rw-   0        0        0      871 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/fullnode.py
--rw-rw-rw-   0        0        0     1490 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.584914 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/
--rw-rw-rw-   0        0        0     2522 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 12:27:53.627620 quorum_fullnode_py-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-05-19 12:27:40.000000 quorum_fullnode_py-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.603124 quorum_fullnode_py-1.3.0/tests/
--rw-rw-rw-   0        0        0     2847 2023-03-27 06:09:37.000000 quorum_fullnode_py-1.3.0/tests/test_fullnode.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.742017 quorum_fullnode_py-1.3.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:18.000000 quorum_fullnode_py-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2522 2023-06-10 02:36:09.742017 quorum_fullnode_py-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-04-03 04:33:04.000000 quorum_fullnode_py-1.3.1/README.md
+-rw-rw-rw-   0        0        0      169 2023-02-23 03:21:16.000000 quorum_fullnode_py-1.3.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.697473 quorum_fullnode_py-1.3.1/quorum_fullnode_py/
+-rw-rw-rw-   0        0        0      329 2023-06-10 02:33:10.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.732045 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/
+-rw-rw-rw-   0        0        0      164 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     6762 2023-05-19 08:38:21.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/base.py
+-rw-rw-rw-   0        0        0    23960 2023-06-10 02:35:00.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/fullnode.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.738049 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/
+-rw-rw-rw-   0        0        0      114 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     1460 2023-04-06 03:32:26.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/_http.py
+-rw-rw-rw-   0        0        0      871 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/fullnode.py
+-rw-rw-rw-   0        0        0     1490 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.726073 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/
+-rw-rw-rw-   0        0        0     2522 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 02:36:09.743017 quorum_fullnode_py-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-06-10 02:33:10.000000 quorum_fullnode_py-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.739050 quorum_fullnode_py-1.3.1/tests/
+-rw-rw-rw-   0        0        0     2847 2023-03-27 06:09:37.000000 quorum_fullnode_py-1.3.1/tests/test_fullnode.py
```

### Comparing `quorum_fullnode_py-1.3.0/LICENSE` & `quorum_fullnode_py-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.0/PKG-INFO` & `quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum_fullnode_py
-Version: 1.3.0
+Name: quorum-fullnode-py
+Version: 1.3.1
 Summary: Python SDK for FullNode of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_fullnode_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_fullnode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_fullnode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_fullnode_py-1.3.0/README.md` & `quorum_fullnode_py-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/base.py` & `quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/base.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/fullnode.py` & `quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/fullnode.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,17 +261,21 @@
         }
         if start_trx:
             params["start_trx"] = start_trx
             params["include_start_trx"] = include_start_trx
         if senders:
             params["senders"] = senders
         trxs = []
-        for i in super()._get_content(group_id, params):
-            i["Data"] = json.loads(base64.b64decode(i["Data"]))
-            trxs.append(i)
+        for trx in super()._get_content(group_id, params):
+            # private group will return trx without Data
+            try:
+                trx["Data"] = json.loads(base64.b64decode(trx["Data"]))
+            except Exception as err:
+                logger.warning(f"decode trx data error: {err}\n{trx}")
+            trxs.append(trx)
         return trxs
 
     def trx(self, trx_id: str, group_id: str = None):
         """get trx data by trx_id"""
         trx = {}
         if not trx_id:
             return trx
@@ -555,15 +559,15 @@
 
     def get_consensus_current(self, group_id: str = None):
         group_id = self._check_group_id_as_required(group_id)
         return super()._get_consensus_current(group_id)
 
     def update_consensus(
         self,
-        start_from_epoch: int,
+        start_from_epoch: int = None,
         trx_epoch_tick: int = None,
         agreement_tick_length: int = None,
         agreement_tick_count=None,
         producer_pubkey: list = None,
         group_id: str = None,
     ):
         group_id = self._check_group_id_as_required(group_id)
@@ -597,14 +601,21 @@
             "agreement_tick_count": agreement_tick_count
             or _exist["agreement_tick_count"],
             "producer_pubkey": producer_pubkey or _exist["producer_pubkey"],
         }
 
         if payload == _exist:
             return {"message": "Nothing to update"}
+
+        if payload["trx_epoch_tick"] < payload["agreement_tick_Length"]:
+            logger.warning(
+                "trx_epoch_tick %s should be greater than agreement_tick_Length %s",
+                payload["trx_epoch_tick"],
+                payload["agreement_tick_Length"],
+            )
         return super()._update_consensus(payload)
 
     def update_user(self, payload: dict = None):
         return super()._update_user(payload)
 
     def get_announced_users(self, group_id: str = None):
         """get the announced users to approve(add or remove)"""
```

### Comparing `quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/_http.py` & `quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/fullnode.py` & `quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/fullnode.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.0/quorum_fullnode_py/exceptions.py` & `quorum_fullnode_py-1.3.1/quorum_fullnode_py/exceptions.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/PKG-INFO` & `quorum_fullnode_py-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum-fullnode-py
-Version: 1.3.0
+Name: quorum_fullnode_py
+Version: 1.3.1
 Summary: Python SDK for FullNode of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_fullnode_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_fullnode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_fullnode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/SOURCES.txt` & `quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.0/setup.py` & `quorum_fullnode_py-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_fullnode_py",
-    version="1.3.0",
+    version="1.3.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python SDK for FullNode of QuoRum",
     keywords=["quorum_fullnode_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_fullnode_py",
```

### Comparing `quorum_fullnode_py-1.3.0/tests/test_fullnode.py` & `quorum_fullnode_py-1.3.1/tests/test_fullnode.py`

 * *Files identical despite different names*

