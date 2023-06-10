# Comparing `tmp/pycafe24-1.8.tar.gz` & `tmp/pycafe24-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycafe24-1.8.tar", last modified: Fri Aug 12 08:22:34 2022, max compression
+gzip compressed data, was "pycafe24-1.9.tar", last modified: Tue Aug 16 00:53:02 2022, max compression
```

## Comparing `pycafe24-1.8.tar` & `pycafe24-1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-08-12 08:22:34.293940 pycafe24-1.8/
--rw-r--r--   0 root         (0) staff       (20)     1069 2022-06-16 08:15:07.000000 pycafe24-1.8/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      160 2022-08-12 08:22:34.293681 pycafe24-1.8/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       11 2022-07-18 13:49:30.000000 pycafe24-1.8/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-08-12 08:22:34.291466 pycafe24-1.8/pycafe24/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-06-17 06:56:21.000000 pycafe24-1.8/pycafe24/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      742 2022-07-05 08:58:06.000000 pycafe24-1.8/pycafe24/cache.py
--rw-r--r--   0 root         (0) staff       (20)      400 2022-06-24 07:14:29.000000 pycafe24-1.8/pycafe24/exceptions.py
--rw-r--r--   0 root         (0) staff       (20)    11359 2022-08-12 08:01:38.000000 pycafe24-1.8/pycafe24/functions.py
--rw-r--r--   0 root         (0) staff       (20)     5142 2022-08-10 05:04:25.000000 pycafe24-1.8/pycafe24/oauth2.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-08-12 08:22:34.293304 pycafe24-1.8/pycafe24.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      160 2022-08-12 08:22:33.000000 pycafe24-1.8/pycafe24.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      288 2022-08-12 08:22:34.000000 pycafe24-1.8/pycafe24.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2022-08-12 08:22:33.000000 pycafe24-1.8/pycafe24.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2022-08-12 08:22:34.000000 pycafe24-1.8/pycafe24.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        9 2022-08-12 08:22:34.000000 pycafe24-1.8/pycafe24.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2022-08-12 08:22:34.294037 pycafe24-1.8/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      300 2022-08-10 05:05:03.000000 pycafe24-1.8/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2022-08-16 00:53:02.081777 pycafe24-1.9/
+-rw-r--r--   0 root         (0) staff       (20)     1069 2022-06-16 08:15:07.000000 pycafe24-1.9/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      160 2022-08-16 00:53:02.081520 pycafe24-1.9/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       11 2022-07-18 13:49:30.000000 pycafe24-1.9/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2022-08-16 00:53:02.079231 pycafe24-1.9/pycafe24/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-06-17 06:56:21.000000 pycafe24-1.9/pycafe24/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      742 2022-07-05 08:58:06.000000 pycafe24-1.9/pycafe24/cache.py
+-rw-r--r--   0 root         (0) staff       (20)      400 2022-06-24 07:14:29.000000 pycafe24-1.9/pycafe24/exceptions.py
+-rw-r--r--   0 root         (0) staff       (20)    11940 2022-08-16 00:35:32.000000 pycafe24-1.9/pycafe24/functions.py
+-rw-r--r--   0 root         (0) staff       (20)     5142 2022-08-10 05:04:25.000000 pycafe24-1.9/pycafe24/oauth2.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2022-08-16 00:53:02.081181 pycafe24-1.9/pycafe24.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      160 2022-08-16 00:53:01.000000 pycafe24-1.9/pycafe24.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      288 2022-08-16 00:53:02.000000 pycafe24-1.9/pycafe24.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2022-08-16 00:53:01.000000 pycafe24-1.9/pycafe24.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2022-08-16 00:53:01.000000 pycafe24-1.9/pycafe24.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        9 2022-08-16 00:53:01.000000 pycafe24-1.9/pycafe24.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2022-08-16 00:53:02.081873 pycafe24-1.9/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      300 2022-08-12 08:22:52.000000 pycafe24-1.9/setup.py
```

### Comparing `pycafe24-1.8/LICENSE` & `pycafe24-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycafe24-1.8/pycafe24/cache.py` & `pycafe24-1.9/pycafe24/cache.py`

 * *Files identical despite different names*

### Comparing `pycafe24-1.8/pycafe24/functions.py` & `pycafe24-1.9/pycafe24/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,30 @@
 			payload[key] = value
 
 		url = "https://{0}.cafe24api.com/api/v2/admin/orders".format(self.credentials_manager.mall_id)
 		response = self._get(url,payload=payload)
 		return response
 
 
+	def list_products(self,**rest):
+		payload = {}
+		for (key,value) in rest.items():
+			payload[key] = value
+		url = "https://{0}.cafe24api.com/api/v2/admin/products".format(self.credentials_manager.mall_id)
+		response = self._get(url,payload=payload)
+		return response
 
+	def retrieve_product(self, product_no, **rest):
+		payload = {}
+		for (key,value) in rest.items():
+			payload[key] = value
+		url = "https://{0}.cafe24api.com/api/v2/admin/products/{1}".format(self.credentials_manager.mall_id, product_no)
+		print(url)
+		response = self._get(url,payload=payload)
+		return response
 
 
 
 
 
 	def num_coupon(self):
 		payload = {}
```

### Comparing `pycafe24-1.8/pycafe24/oauth2.py` & `pycafe24-1.9/pycafe24/oauth2.py`

 * *Files identical despite different names*

