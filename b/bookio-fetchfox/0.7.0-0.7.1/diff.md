# Comparing `tmp/bookio_fetchfox-0.7.0.tar.gz` & `tmp/bookio_fetchfox-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.7.0.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.7.1.tar", max compression
```

## Comparing `bookio_fetchfox-0.7.0.tar` & `bookio_fetchfox-0.7.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     3723 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1764 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      734 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1606 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      675 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4147 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2555 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     8307 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     2380 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    12461 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      666 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     9983 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      670 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      216 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2263 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3435 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      463 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1409 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      365 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1792 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1895 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2023-06-09 15:33:23.431378 bookio_fetchfox-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.0/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2140 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      596 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1349 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1764 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      592 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      734 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1606 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      675 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4147 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2555 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-10 14:51:16.333802 bookio_fetchfox-0.7.1/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     8295 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      504 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     2380 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    12449 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1061 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     9983 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      619 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0      670 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      154 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      216 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2263 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3435 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      463 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1591 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      365 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1974 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1895 2023-06-10 14:51:16.337803 bookio_fetchfox-0.7.1/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-10 14:51:16.349803 bookio_fetchfox-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.1/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.1/PKG-INFO
```

### Comparing `bookio_fetchfox-0.7.0/README.md` & `bookio_fetchfox-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.7.1/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid algorand address or nfdomain")
 
     def explorer_url(self, collection_id: str) -> str:
         return f"https://algoexplorer.io/address/{collection_id}"
 
     def marketplace_url(self, collection_id: str) -> str:
-        return f"https://www.randgallery.com/algo-collection/?address={collection_id}"
+        return f"https://randgallery.com/algo-collection/?address={collection_id}"
 
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         for asset_id in algonodecloud.get_assets(collection_id):
             if fetch_metadata:
                 yield self.get_asset(
@@ -147,15 +147,15 @@
                 asset_names=asset_names,
                 listing_id=listing["timestamp"],
                 marketplace=RANDGALLERY_COM,
                 price=listing["price"],
                 currency=ALGO,
                 listed_at=listed_at,
                 listed_by=listing["sellerAddress"],
-                marketplace_url=f"https://www.randgallery.com/algo-collection/?address={asset_id}",
+                marketplace_url=f"https://randgallery.com/algo-collection/?address={asset_id}",
             )
 
         listings = algoxnftcom.get_listings(collection_id)
 
         for listing in listings:
             asset_id = str(listing["asset_id"])
             asset_ids = [asset_id]
@@ -222,15 +222,15 @@
             ).replace(
                 tzinfo=pytz.UTC,
             )
 
             marketplace = venues[sale.get("venue")]
 
             if marketplace == RANDGALLERY_COM:
-                marketplace_url = f"https://www.randgallery.com/algo-collection/?address={asset_id}"
+                marketplace_url = f"https://randgallery.com/algo-collection/?address={asset_id}"
             elif marketplace == ALGOXNFT_COM:
                 marketplace_url = f"https://algoxnft.com/asset/{asset_id}"
             elif marketplace == SHUFL_APP:
                 marketplace_url = f"https://shufl.app/detail/{asset_id}"
             else:
                 marketplace_url = None
```

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid cardano address, stake key or ada handle")
 
     def explorer_url(self, collection_id: str) -> str:
         return f"https://cardanoscan.io/tokenPolicy/{collection_id}"
 
     def marketplace_url(self, collection_id: str) -> str:
-        return f"https://www.jpg.store/collection/{collection_id}"
+        return f"https://jpg.store/collection/{collection_id}"
 
     @lru_cache
     def get_stake_key(self, wallet: str) -> str:
         self.check_wallet(wallet)
 
         if utils.is_stake_key(wallet):
             return wallet
@@ -260,15 +260,15 @@
                 listing_id=listing["listing_id"],
                 marketplace=JPG_STORE,
                 price=int(listing["price_lovelace"]) // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=None,
                 tx_hash=listing["tx_hash"],
-                marketplace_url=f"https://www.jpg.store/asset/{asset_id}",
+                marketplace_url=f"https://jpg.store/asset/{asset_id}",
             )
 
     def get_floor(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> FloorDTO:
         self.check_collection_id(collection_id)
 
         floor = None
         count = 0
@@ -342,10 +342,10 @@
                 marketplace=JPG_STORE,
                 price=int(sale["amount_lovelace"]) // 10**6,
                 currency=self.currency,
                 confirmed_at=confirmed_at,
                 type=sale_type,
                 sold_by=seller,
                 bought_by=buyer,
-                marketplace_url=f"https://www.jpg.store/asset/{asset_id}",
+                marketplace_url=f"https://jpg.store/asset/{asset_id}",
                 explorer_url=f"https://cardanoscan.io/transaction/{tx_hash}",
             )
```

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/evm/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-0.7.1/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.7.1/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.7.1/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.7.1/fetchfox/dtos/listing.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,18 +30,26 @@
         self.currency: str = currency
         self.listed_at: datetime = listed_at
         self.listed_by: str = listed_by
         self.tx_hash: str = tx_hash
         self.marketplace_url: str = marketplace_url
 
     @property
+    def price_str(self) -> str:
+        return f"{self.price}:0.2f {self.currency}"
+
+    @property
     def usd(self) -> float:
         return self.price * coingeckocom.usd(self.currency)
 
     @property
+    def usd_str(self) -> str:
+        return f"{self.usd}:0.2f USD"
+
+    @property
     def first(self) -> str:
         return self.asset_ids[0]
 
     @property
     def is_bundle(self) -> bool:
         return len(self.asset_ids) > 1
```

### Comparing `bookio_fetchfox-0.7.0/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.7.1/fetchfox/dtos/sale.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,18 +44,26 @@
         self.sale_id: str = sale_id
         self.sold_by: str = sold_by
         self.bought_by: str = bought_by
         self.marketplace_url: str = marketplace_url
         self.explorer_url: str = explorer_url
 
     @property
+    def price_str(self) -> str:
+        return f"{self.price}:0.2f {self.currency}"
+
+    @property
     def usd(self) -> float:
         return self.price * coingeckocom.usd(self.currency)
 
     @property
+    def usd_str(self) -> str:
+        return f"{self.usd}:0.2f USD"
+
+    @property
     def first(self) -> str:
         return self.asset_ids[0]
 
     @property
     def is_bundle(self) -> bool:
         return len(self.asset_ids) > 1
```

### Comparing `bookio_fetchfox-0.7.0/fetchfox/rest.py` & `bookio_fetchfox-0.7.1/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.0/pyproject.toml` & `bookio_fetchfox-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.7.0"
+version = "0.7.1"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-0.7.0/setup.py` & `bookio_fetchfox-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.7.0/PKG-INFO` & `bookio_fetchfox-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.7.0
+Version: 0.7.1
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

