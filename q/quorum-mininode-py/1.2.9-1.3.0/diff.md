# Comparing `tmp/quorum_mininode_py-1.2.9.tar.gz` & `tmp/quorum_mininode_py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_mininode_py-1.2.9.tar", last modified: Wed May 17 04:14:40 2023, max compression
+gzip compressed data, was "quorum_mininode_py-1.3.0.tar", last modified: Sat Jun 10 03:15:05 2023, max compression
```

## Comparing `quorum_mininode_py-1.2.9.tar` & `quorum_mininode_py-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.746090 quorum_mininode_py-1.2.9/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.9/LICENSE
--rw-rw-rw-   0        0        0     2440 2023-05-17 04:14:40.745092 quorum_mininode_py-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.626861 quorum_mininode_py-1.2.9/quorum_mininode_py/
--rw-rw-rw-   0        0        0      364 2023-05-17 04:13:41.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.675730 quorum_mininode_py-1.2.9/quorum_mininode_py/api/
--rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/api/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-05-17 04:12:51.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/api/base.py
--rw-rw-rw-   0        0        0     3812 2023-05-03 11:14:28.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/api/lightnode.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.682711 quorum_mininode_py-1.2.9/quorum_mininode_py/client/
--rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/client/__init__.py
--rw-rw-rw-   0        0        0     2815 2023-05-17 04:09:25.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/client/_http.py
--rw-rw-rw-   0        0        0     2636 2023-05-17 04:11:59.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/client/mininode.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.735120 quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/
--rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/__init__.py
--rw-rw-rw-   0        0        0     2361 2023-05-03 11:14:57.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/account.py
--rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/aes.py
--rw-rw-rw-   0        0        0     1824 2023-05-03 11:15:00.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/age.py
--rw-rw-rw-   0        0        0     3846 2023-05-03 11:36:39.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/trx.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.739109 quorum_mininode_py-1.2.9/quorum_mininode_py/proto/
--rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/proto/__init__.py
--rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/proto/quorum_pb2.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.743098 quorum_mininode_py-1.2.9/quorum_mininode_py/utils/
--rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/utils/__init__.py
--rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.9/quorum_mininode_py/utils/url.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:14:40.669748 quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/
--rw-rw-rw-   0        0        0     2440 2023-05-17 04:14:40.000000 quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-05-17 04:14:40.000000 quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 04:14:40.000000 quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-17 04:14:40.000000 quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-17 04:14:40.000000 quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 04:14:40.747089 quorum_mininode_py-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1308 2023-05-17 04:13:41.000000 quorum_mininode_py-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.128498 quorum_mininode_py-1.3.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2440 2023-06-10 03:15:05.127499 quorum_mininode_py-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.067971 quorum_mininode_py-1.3.0/quorum_mininode_py/
+-rw-rw-rw-   0        0        0      364 2023-06-07 09:26:23.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.083942 quorum_mininode_py-1.3.0/quorum_mininode_py/api/
+-rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     2547 2023-06-09 08:19:00.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/api/base.py
+-rw-rw-rw-   0        0        0     4154 2023-06-10 03:12:57.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/api/lightnode.py
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.090925 quorum_mininode_py-1.3.0/quorum_mininode_py/client/
+-rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     2921 2023-06-07 09:36:32.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/client/_http.py
+-rw-rw-rw-   0        0        0     2403 2023-06-09 08:19:00.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/client/mininode.py
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.101902 quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/
+-rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2414 2023-06-09 07:33:41.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/account.py
+-rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/aes.py
+-rw-rw-rw-   0        0        0     3065 2023-06-10 03:12:55.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/age.py
+-rw-rw-rw-   0        0        0     3573 2023-06-10 03:12:57.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/trx.py
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.105886 quorum_mininode_py-1.3.0/quorum_mininode_py/proto/
+-rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/proto/__init__.py
+-rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/proto/quorum_pb2.py
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.109904 quorum_mininode_py-1.3.0/quorum_mininode_py/utils/
+-rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/utils/__init__.py
+-rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.3.0/quorum_mininode_py/utils/url.py
+drwxrwxrwx   0        0        0        0 2023-06-10 03:15:05.078359 quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/
+-rw-rw-rw-   0        0        0     2440 2023-06-10 03:15:04.000000 quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-06-10 03:15:05.000000 quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 03:15:04.000000 quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-10 03:15:04.000000 quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-10 03:15:04.000000 quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 03:15:05.128498 quorum_mininode_py-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1308 2023-06-07 09:26:23.000000 quorum_mininode_py-1.3.0/setup.py
```

### Comparing `quorum_mininode_py-1.2.9/LICENSE` & `quorum_mininode_py-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.9/PKG-INFO` & `quorum_mininode_py-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_mininode_py
-Version: 1.2.9
+Version: 1.3.0
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.9/README.md` & `quorum_mininode_py-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/api/base.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,7 +63,11 @@
         return self._get(f"/api/v1/node/{self.group_id}/announced/producer")
 
     def _get_announced_user(self):
         return self._get(f"/api/v1/node/{self.group_id}/announced/user")
 
     def _post_announce(self, payload: dict):
         return self._post(f"/api/v1/node/{self.group_id}/announce", payload)
+
+    def _get_encrypt_pubkeys(self):
+        """get the age pubkeys of private group"""
+        return self._get(f"/api/v1/node/getencryptpubkeys/{self.group_id}")
```

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/api/lightnode.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/api/lightnode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,41 @@
 import logging
 
 from quorum_mininode_py.api.base import BaseAPI
 from quorum_mininode_py.crypto.account import check_pvtkey
-from quorum_mininode_py.crypto.trx import trx_decrypt, trx_encrypt
+from quorum_mininode_py.crypto.trx import get_announce_param, trx_decrypt, trx_encrypt
 
 logger = logging.getLogger(__name__)
 
 
 class LightNodeAPI(BaseAPI):
     """the light node api for quorum"""
 
     def post_content(
         self,
         data: dict,
         trx_id: str = None,
     ):
         """post content to group"""
-        if self._group.encryption_type == "public":
-            age_pubkey = None
-        else:
-            age_pubkey = self._account.age_pubkey
         trx = trx_encrypt(
             self.group_id,
             self._group.aes_key,
             data,
             check_pvtkey(self._account.pvtkey),
-            age_pubkey,
             trx_id,
         )
         return super()._post_content(trx)
 
     def get_trx(self, trx_id: str):
         """get encrpyted trx"""
         return super()._get_trx(trx_id)
 
     def trx(self, trx_id: str):
         """get decrypted trx"""
-        if self._group.encryption_type == "public":
-            age_priv_key = None
-        else:
-            age_priv_key = self._account.age_privkey
-
-        trx = trx_decrypt(self._group.aes_key, age_priv_key, self.get_trx(trx_id))
-        return trx
+        return trx_decrypt(self._group.aes_key, self.get_trx(trx_id))
 
     def get_content(
         self,
         start_trx: str = None,
         num: int = 20,
         reverse: bool = False,
         include_start_trx: bool = False,
@@ -60,26 +49,21 @@
         if start_trx:
             params["start_trx"] = start_trx
             params["include_start_trx"] = include_start_trx
         if senders:
             params["senders"] = senders
 
         encypted_trxs = super()._get_content(params)
-        if self._group.encryption_type.lower() == "public":
-            age_priv_key = None
-        else:
-            age_priv_key = self._account.age_privkey
-
         trxs = []
-        for i in encypted_trxs:
+        for trx in encypted_trxs:
             try:
-                i = trx_decrypt(self._group.aes_key, age_priv_key, i)
+                trx = trx_decrypt(self._group.aes_key, trx)
             except Exception as err:
                 logger.error(err)
-            trxs.append(i)
+            trxs.append(trx)
         return trxs
 
     def get_group_info(self):
         """get group info"""
         return super()._get_group()
 
     def get_encryptpubkeys(self):
@@ -117,10 +101,35 @@
         """get announced producer"""
         return super()._get_announced_producer()
 
     def get_announced_user(self):
         """get announced user"""
         return super()._get_announced_user()
 
-    def announce(self, payload: dict):  # TODO: to finish.
-        """post annonce to group"""
+    def announce(self, action: str, _type: str, memo: str = None):
+        """post annonce to group
+        action: str, one of [add, remove]
+        _type: str, one of [user, producer]
+        """
+        # only announce self as user will be success
+        payload = get_announce_param(
+            self._account.age_pubkey,
+            check_pvtkey(self._account.pvtkey),
+            self.group_id,
+            action,
+            _type,
+            memo or f"annonce as {_type}",
+        )
         return super()._post_announce(payload)
+
+    def announce_as_user(self):
+        """announce as user"""
+        return self.announce("add", "user")
+
+    def announce_as_producer(self):
+        """announce as producer"""
+        # lightnote can not announce as producer, return http 400
+        return self.announce("add", "producer")
+
+    def get_encrypt_pubkeys(self):
+        """get age pubkeys of private group"""
+        return super()._get_encryptpubkeys().get("keys")
```

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/client/_http.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/client/_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,24 +57,26 @@
                     response = self.session.request(
                         method=method,
                         url=url,
                         json=payload,
                         timeout=self.timeout,
                         headers=self.headers,
                     )
+                    logger.debug("payload %s", payload)
                     response.raise_for_status()
                     return response.json()
                 except requests.exceptions.RequestException as err:
                     logging.warning(
                         "HTTP request retry %s/%s: %s", i + 1, self.retries, err
                     )
         except requests.exceptions.RequestException as err:
             logging.warning(
                 "HTTP request error (endpoint %s}): %s", self.current_chain_url, err
             )
+            logger.debug("payload %s", payload)
             self.current_chain_url = (self.current_chain_url + 1) % len(self.chain_urls)
             return self._request(method, endpoint, payload)
         raise Exception("HTTP request error")
 
     def get(self, endpoint: str, payload: dict = None):
         return self._request("get", endpoint, payload)
```

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/client/mininode.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/client/mininode.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,38 +37,33 @@
 class RumAccount:
     pvtkey: str = None
     pubkey: str = None
     address: str = None
     age_pvtkey: str = None
     age_pubkey: str = None
 
-    def __init__(
-        self, pvtkey: str = None, age_pvtkey: str = None, encryption_type: str = None
-    ):
+    def __init__(self, pvtkey: str = None, age_pvtkey: str = None):
         self.pvtkey = pvtkey or eth_acc.create_pvtkey()
         self.pubkey = eth_acc.pvtkey_to_pubkey(self.pvtkey)
         self.address = eth_acc.pubkey_to_address(self.pubkey)
 
         if age_pvtkey:
             self.age_pvtkey = age_pvtkey
             self.age_pubkey = age_acc.age_pvtkey_to_pubkey(age_pvtkey)
-        elif (encryption_type or "").upper() == "PRIVATE":
-            self.age_pvtkey, self.age_pubkey = age_acc.create_age_keypair()
         else:
-            self.age_pvtkey = None
-            self.age_pubkey = None
+            self.age_pvtkey, self.age_pubkey = age_acc.create_age_keypair()
 
 
 class MiniNode:
     """python for quorum lightnode, without datastore, one MiniNode client for one group"""
 
     def __init__(self, seed_url: str, pvtkey=None, age_pvtkey=None):
         self.group = RumGroup(seed_url)
         self.http = HttpRequest(chain_urls=self.group.chain_urls or [])
-        self.account = RumAccount(pvtkey, age_pvtkey, self.group.encryption_type)
+        self.account = RumAccount(pvtkey, age_pvtkey)
         self.api = LightNodeAPI(self)
 
     def change_account(self, pvtkey, age_pvtkey=None):
         age_pvtkey = age_pvtkey or self.account.age_pvtkey
         if pvtkey != self.account.pvtkey or age_pvtkey != self.account.age_pvtkey:
-            self.account = RumAccount(pvtkey, age_pvtkey, self.group.encryption_type)
+            self.account = RumAccount(pvtkey, age_pvtkey)
             self.api = LightNodeAPI(self)
```

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/account.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import base64
 import logging
+import secrets
 from typing import Union
 
 import eth_keys
 from eth_account import Account
 from eth_utils.hexadecimal import encode_hex
 
 logger = logging.getLogger(__name__)
 
 
 def create_pvtkey() -> str:
     """create private key"""
-    acc = Account().create()
+    acc = Account().create(extra_entropy=secrets.token_bytes(32))
     private_key = encode_hex(acc.key)
     return private_key
 
 
 def check_pvtkey(private_key: Union[str, int, bytes]) -> bytes:
     """check private key"""
     if isinstance(private_key, int):
```

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/crypto/aes.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/proto/quorum_pb2.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/proto/quorum_pb2.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py/utils/url.py` & `quorum_mininode_py-1.3.0/quorum_mininode_py/utils/url.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/PKG-INFO` & `quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-mininode-py
-Version: 1.2.9
+Version: 1.3.0
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.9/quorum_mininode_py.egg-info/SOURCES.txt` & `quorum_mininode_py-1.3.0/quorum_mininode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.9/setup.py` & `quorum_mininode_py-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_mininode_py",
-    version="1.2.9",
+    version="1.3.0",
     author="liujuanjuan1984, zhangwm404",
     author_email="qiaoanlu@163.com",
     description="a mini python sdk for quorum lightnode with http/https requests to quorum fullnode",
     keywords=["rumsystem", "quorum", "lightnode", "sdk"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_mininode_py",
```

