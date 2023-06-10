# Comparing `tmp/blockchain-apis-0.1.2.tar.gz` & `tmp/blockchain-apis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain-apis-0.1.2.tar", last modified: Fri Jun  9 15:30:14 2023, max compression
+gzip compressed data, was "blockchain-apis-0.1.3.tar", last modified: Sat Jun 10 14:24:29 2023, max compression
```

## Comparing `blockchain-apis-0.1.2.tar` & `blockchain-apis-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.1.2/LICENSE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 15:30:18.000000 blockchain-apis-0.1.2/README.md
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-09 15:21:30.000000 blockchain-apis-0.1.2/setup.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.933297 blockchain-apis-0.1.2/src/
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.937297 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1718 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/top_level.txt
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.937297 blockchain-apis-0.1.2/src/blockchainapis/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    25822 2023-06-09 15:27:18.000000 blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    25217 2023-06-09 15:27:15.000000 blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIsSync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      622 2023-06-09 15:21:23.000000 blockchain-apis-0.1.2/src/blockchainapis/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.937297 blockchain-apis-0.1.2/src/blockchainapis/exceptions/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/BlockchainAPIsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      681 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      674 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      771 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/InvalidPageException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/PairNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      773 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/TokenNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      708 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/TooManyRequestsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      691 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/UnauthorizedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      922 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/src/blockchainapis/models/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      859 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/AmountIn.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      870 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/AmountOut.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      579 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Blockchain.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      547 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Exchange.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      863 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      677 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Pair.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      933 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Reserve.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      760 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1826 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1475 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/tests/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_in.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_in_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_out.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_out_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_blockchains.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_blockchains_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_decimals.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_decimals_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_exchanges_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_info.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_info_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_pairs_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_reserves.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_reserves_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_tokens_sync.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-10 14:24:29.588269 blockchain-apis-0.1.3/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.1.3/LICENSE
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-10 14:24:29.588269 blockchain-apis-0.1.3/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 15:30:18.000000 blockchain-apis-0.1.3/README.md
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-10 14:24:29.588269 blockchain-apis-0.1.3/setup.cfg
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-10 14:14:06.000000 blockchain-apis-0.1.3/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-10 14:24:29.580269 blockchain-apis-0.1.3/src/
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-10 14:24:29.580269 blockchain-apis-0.1.3/src/blockchain_apis.egg-info/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-10 14:24:29.000000 blockchain-apis-0.1.3/src/blockchain_apis.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1718 2023-06-10 14:24:29.000000 blockchain-apis-0.1.3/src/blockchain_apis.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-10 14:24:29.000000 blockchain-apis-0.1.3/src/blockchain_apis.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-10 14:24:29.000000 blockchain-apis-0.1.3/src/blockchain_apis.egg-info/requires.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-10 14:24:29.000000 blockchain-apis-0.1.3/src/blockchain_apis.egg-info/top_level.txt
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-10 14:24:29.580269 blockchain-apis-0.1.3/src/blockchainapis/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    26306 2023-06-10 14:13:46.000000 blockchain-apis-0.1.3/src/blockchainapis/BlockchainAPIs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    25217 2023-06-10 14:13:53.000000 blockchain-apis-0.1.3/src/blockchainapis/BlockchainAPIsSync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      622 2023-06-10 14:13:21.000000 blockchain-apis-0.1.3/src/blockchainapis/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-10 14:24:29.584269 blockchain-apis-0.1.3/src/blockchainapis/exceptions/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/BlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      681 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      674 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      771 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/InvalidPageException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/PairNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      773 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/TokenNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      708 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/TooManyRequestsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      691 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/UnauthorizedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      922 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/exceptions/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-10 14:24:29.584269 blockchain-apis-0.1.3/src/blockchainapis/models/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      859 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/AmountIn.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      870 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/AmountOut.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      579 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Blockchain.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      547 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Exchange.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      863 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      677 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Pair.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      933 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Reserve.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      760 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Token.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1826 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/Tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1475 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/src/blockchainapis/models/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-10 14:24:29.588269 blockchain-apis-0.1.3/tests/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_amount_in.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_amount_in_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_amount_out.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_amount_out_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_blockchains.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_blockchains_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_decimals.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_decimals_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_exchanges_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_info.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_info_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_pairs_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_reserves.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_reserves_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-10 14:12:58.000000 blockchain-apis-0.1.3/tests/test_tokens_sync.py
```

### Comparing `blockchain-apis-0.1.2/LICENSE` & `blockchain-apis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/PKG-INFO` & `blockchain-apis-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.1.2/README.md` & `blockchain-apis-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/setup.py` & `blockchain-apis-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name = "blockchain-apis",
-    version = "0.1.2",
+    version = "0.1.3",
     author = "Clarensia",
     author_email = "contact@blockchainapis.io",
     description = "Fastest and easiest way to access decentralized finance data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://www.blockchainapis.io",
     license="MIT",
```

### Comparing `blockchain-apis-0.1.2/src/blockchain_apis.egg-info/PKG-INFO` & `blockchain-apis-0.1.3/src/blockchain_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.1.2/src/blockchain_apis.egg-info/SOURCES.txt` & `blockchain-apis-0.1.3/src/blockchain_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIs.py` & `blockchain-apis-0.1.3/src/blockchainapis/BlockchainAPIs.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,33 @@
         """Close the async session object.
         
         You must call this method at the end of your program or when you have finished
         working with BlockchainAPIs.
         """
         await self._session.close()
 
+    async def __aenter__(self):
+        """Called when you use `async with`.
+        
+        For example:
+        async with BlockchainAPIs() as blockchain_apis:
+            # do some stuff
+            pass
+
+        :return: self
+        :rtype: self
+        """
+        return self
+
+    async def __aexit__(self, *_):
+        """Called at the end of the `async with` statement in order
+        to free the resources used by the API instance.
+        """
+        await self.close()
+
     async def _do_request(self, path: str, params: Dict[str, Any] | None = None) -> Dict[str, Any]:
         """Make raw API request (that return the json result).
         
         This method additionaly adds the user API key to the request if it is present.
 
         :param path: The path to the request
         :type path: str
```

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIsSync.py` & `blockchain-apis-0.1.3/src/blockchainapis/BlockchainAPIsSync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/__init__.py` & `blockchain-apis-0.1.3/src/blockchainapis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 you can use the BlockchainAPIsSync class.
 
 """
 
 # Clarensia: https://www.clarensia.com is the company behind
 # the development of https://www.blockchainapis.io
 __author__ = "Clarensia"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 from .BlockchainAPIs import BlockchainAPIs
 from .BlockchainAPIsSync import BlockchainAPIsSync
 
 __all__ = ['BlockchainAPIs']
```

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/BlockchainNotSupportedException.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/BlockchainNotSupportedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/ExchangeNotSupportedException.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/ExchangeNotSupportedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/InvalidPageException.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/InvalidPageException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/PairNotFoundException.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/PairNotFoundException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/TokenNotFoundException.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/TokenNotFoundException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/TooManyRequestsException.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/TooManyRequestsException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/UnauthorizedException.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/UnauthorizedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/exceptions/__init__.py` & `blockchain-apis-0.1.3/src/blockchainapis/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/AmountIn.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/AmountIn.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/AmountOut.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/AmountOut.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Blockchain.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Blockchain.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Exchange.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Exchange.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Exchanges.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Pair.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Pair.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Pairs.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Reserve.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Reserve.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Token.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Token.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/Tokens.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/Tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/src/blockchainapis/models/__init__.py` & `blockchain-apis-0.1.3/src/blockchainapis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_amount_in.py` & `blockchain-apis-0.1.3/tests/test_amount_in.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_amount_in_sync.py` & `blockchain-apis-0.1.3/tests/test_amount_in_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_amount_out.py` & `blockchain-apis-0.1.3/tests/test_amount_out.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_amount_out_sync.py` & `blockchain-apis-0.1.3/tests/test_amount_out_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_decimals.py` & `blockchain-apis-0.1.3/tests/test_decimals.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_decimals_sync.py` & `blockchain-apis-0.1.3/tests/test_decimals_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_exchanges.py` & `blockchain-apis-0.1.3/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_exchanges_sync.py` & `blockchain-apis-0.1.3/tests/test_exchanges_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_info.py` & `blockchain-apis-0.1.3/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_info_sync.py` & `blockchain-apis-0.1.3/tests/test_info_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_pairs.py` & `blockchain-apis-0.1.3/tests/test_pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_pairs_sync.py` & `blockchain-apis-0.1.3/tests/test_pairs_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_reserves.py` & `blockchain-apis-0.1.3/tests/test_reserves.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_reserves_sync.py` & `blockchain-apis-0.1.3/tests/test_reserves_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_tokens.py` & `blockchain-apis-0.1.3/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.2/tests/test_tokens_sync.py` & `blockchain-apis-0.1.3/tests/test_tokens_sync.py`

 * *Files identical despite different names*

