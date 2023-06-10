# Comparing `tmp/fastapi_xray-0.1.0.tar.gz` & `tmp/fastapi_xray-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xray-0.1.0.tar", last modified: Wed May 31 17:37:57 2023, max compression
+gzip compressed data, was "fastapi_xray-0.1.1.tar", last modified: Sat Jun 10 09:00:36 2023, max compression
```

## Comparing `fastapi_xray-0.1.0.tar` & `fastapi_xray-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.629109 fastapi_xray-0.1.0/
--rw-r--r--   0 ropali    (1000) ropali    (1000)     2214 2023-05-31 17:37:57.629109 fastapi_xray-0.1.0/PKG-INFO
--rw-r--r--   0 ropali    (1000) ropali    (1000)     1837 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/README.md
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.625776 fastapi_xray-0.1.0/fastapi_xray/
--rw-r--r--   0 ropali    (1000) ropali    (1000)       37 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/__init__.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     1009 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/cli.py
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.625776 fastapi_xray-0.1.0/fastapi_xray/commons/
--rw-r--r--   0 ropali    (1000) ropali    (1000)        0 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/commons/__init__.py
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.625776 fastapi_xray-0.1.0/fastapi_xray/commons/logger/
--rw-r--r--   0 ropali    (1000) ropali    (1000)      514 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/commons/logger/__init__.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     1071 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/schemas.py
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.629109 fastapi_xray-0.1.0/fastapi_xray/server/
--rw-r--r--   0 ropali    (1000) ropali    (1000)      425 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/server/__init__.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     1709 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/server/receiver.py
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.629109 fastapi_xray-0.1.0/fastapi_xray/ui/
--rw-r--r--   0 ropali    (1000) ropali    (1000)        0 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/__init__.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     3402 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/app.py
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.629109 fastapi_xray-0.1.0/fastapi_xray/ui/components/
--rw-r--r--   0 ropali    (1000) ropali    (1000)        0 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/components/__init__.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     4946 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/components/panel_factory.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     3037 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/components/panels.py
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.629109 fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/
--rw-r--r--   0 ropali    (1000) ropali    (1000)      343 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/__init__.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     1564 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/list.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)      783 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/panels.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)      924 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/text.py
--rw-r--r--   0 ropali    (1000) ropali    (1000)     1304 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/ui/main.css
--rw-r--r--   0 ropali    (1000) ropali    (1000)     6425 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/fastapi_xray/xray.py
-drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-05-31 17:37:57.625776 fastapi_xray-0.1.0/fastapi_xray.egg-info/
--rw-r--r--   0 ropali    (1000) ropali    (1000)     2214 2023-05-31 17:37:57.000000 fastapi_xray-0.1.0/fastapi_xray.egg-info/PKG-INFO
--rw-r--r--   0 ropali    (1000) ropali    (1000)      860 2023-05-31 17:37:57.000000 fastapi_xray-0.1.0/fastapi_xray.egg-info/SOURCES.txt
--rw-r--r--   0 ropali    (1000) ropali    (1000)        1 2023-05-31 17:37:57.000000 fastapi_xray-0.1.0/fastapi_xray.egg-info/dependency_links.txt
--rw-r--r--   0 ropali    (1000) ropali    (1000)       54 2023-05-31 17:37:57.000000 fastapi_xray-0.1.0/fastapi_xray.egg-info/entry_points.txt
--rw-r--r--   0 ropali    (1000) ropali    (1000)       94 2023-05-31 17:37:57.000000 fastapi_xray-0.1.0/fastapi_xray.egg-info/requires.txt
--rw-r--r--   0 ropali    (1000) ropali    (1000)       13 2023-05-31 17:37:57.000000 fastapi_xray-0.1.0/fastapi_xray.egg-info/top_level.txt
--rw-r--r--   0 ropali    (1000) ropali    (1000)      838 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/pyproject.toml
--rw-r--r--   0 ropali    (1000) ropali    (1000)       94 2023-05-28 09:01:08.000000 fastapi_xray-0.1.0/requirements.txt
--rw-r--r--   0 ropali    (1000) ropali    (1000)       38 2023-05-31 17:37:57.629109 fastapi_xray-0.1.0/setup.cfg
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.073497 fastapi_xray-0.1.1/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     2214 2023-06-10 09:00:36.073497 fastapi_xray-0.1.1/PKG-INFO
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     1837 2023-06-10 08:53:00.000000 fastapi_xray-0.1.1/README.md
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.070164 fastapi_xray-0.1.1/fastapi_xray/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)       37 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/__init__.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     1009 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/cli.py
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.070164 fastapi_xray-0.1.1/fastapi_xray/commons/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)        0 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/commons/__init__.py
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.070164 fastapi_xray-0.1.1/fastapi_xray/commons/logger/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)      514 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/commons/logger/__init__.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     1071 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/schemas.py
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.070164 fastapi_xray-0.1.1/fastapi_xray/server/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)      425 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/server/__init__.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     1709 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/server/receiver.py
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.073497 fastapi_xray-0.1.1/fastapi_xray/ui/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)        0 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/__init__.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     3402 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/app.py
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.073497 fastapi_xray-0.1.1/fastapi_xray/ui/components/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)        0 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/components/__init__.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     4946 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/components/panel_factory.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     3037 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/components/panels.py
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.073497 fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)      343 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/__init__.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     1564 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/list.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)      783 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/panels.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)      924 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/text.py
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     1304 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/ui/main.css
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     6881 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/fastapi_xray/xray.py
+drwxr-xr-x   0 ropali    (1000) ropali    (1000)        0 2023-06-10 09:00:36.070164 fastapi_xray-0.1.1/fastapi_xray.egg-info/
+-rw-r--r--   0 ropali    (1000) ropali    (1000)     2214 2023-06-10 09:00:36.000000 fastapi_xray-0.1.1/fastapi_xray.egg-info/PKG-INFO
+-rw-r--r--   0 ropali    (1000) ropali    (1000)      860 2023-06-10 09:00:36.000000 fastapi_xray-0.1.1/fastapi_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 ropali    (1000) ropali    (1000)        1 2023-06-10 09:00:36.000000 fastapi_xray-0.1.1/fastapi_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 ropali    (1000) ropali    (1000)       54 2023-06-10 09:00:36.000000 fastapi_xray-0.1.1/fastapi_xray.egg-info/entry_points.txt
+-rw-r--r--   0 ropali    (1000) ropali    (1000)       94 2023-06-10 09:00:36.000000 fastapi_xray-0.1.1/fastapi_xray.egg-info/requires.txt
+-rw-r--r--   0 ropali    (1000) ropali    (1000)       13 2023-06-10 09:00:36.000000 fastapi_xray-0.1.1/fastapi_xray.egg-info/top_level.txt
+-rw-r--r--   0 ropali    (1000) ropali    (1000)      838 2023-06-10 09:00:21.000000 fastapi_xray-0.1.1/pyproject.toml
+-rw-r--r--   0 ropali    (1000) ropali    (1000)       94 2023-06-10 08:52:01.000000 fastapi_xray-0.1.1/requirements.txt
+-rw-r--r--   0 ropali    (1000) ropali    (1000)       38 2023-06-10 09:00:36.073497 fastapi_xray-0.1.1/setup.cfg
```

### Comparing `fastapi_xray-0.1.0/PKG-INFO` & `fastapi_xray-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_xray
-Version: 0.1.0
+Version: 0.1.1
 Summary: A FastAPI debug tool to look into request/response
 Author-email: Ropali Munshi <ropali68@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 ![image](https://github.com/ropali/fastapi_xray/assets/31515245/504a8da8-f366-4f1c-ba56-cd798cb70a91)
 
 ![image](https://github.com/ropali/fastapi_xray/assets/31515245/cc1fb459-f4b3-45ff-ae66-1c5a48316f6c)
 
 ## Installation
 Install this package from pypi using this command.
 ```
-pip install fastapi_xray
+pip install fastapi-xray
 ```
 
 ## Usage
 It is very easy to use. Call the `start_xray` function to start intercepting all the request and response.
 
 ```
 from fastapi import FastAPI
```

### Comparing `fastapi_xray-0.1.0/README.md` & `fastapi_xray-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ![image](https://github.com/ropali/fastapi_xray/assets/31515245/504a8da8-f366-4f1c-ba56-cd798cb70a91)
 
 ![image](https://github.com/ropali/fastapi_xray/assets/31515245/cc1fb459-f4b3-45ff-ae66-1c5a48316f6c)
 
 ## Installation
 Install this package from pypi using this command.
 ```
-pip install fastapi_xray
+pip install fastapi-xray
 ```
 
 ## Usage
 It is very easy to use. Call the `start_xray` function to start intercepting all the request and response.
 
 ```
 from fastapi import FastAPI
```

### Comparing `fastapi_xray-0.1.0/fastapi_xray/cli.py` & `fastapi_xray-0.1.1/fastapi_xray/cli.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/commons/logger/__init__.py` & `fastapi_xray-0.1.1/fastapi_xray/commons/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/schemas.py` & `fastapi_xray-0.1.1/fastapi_xray/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/server/receiver.py` & `fastapi_xray-0.1.1/fastapi_xray/server/receiver.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/ui/app.py` & `fastapi_xray-0.1.1/fastapi_xray/ui/app.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/ui/components/panel_factory.py` & `fastapi_xray-0.1.1/fastapi_xray/ui/components/panel_factory.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/ui/components/panels.py` & `fastapi_xray-0.1.1/fastapi_xray/ui/components/panels.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/list.py` & `fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/list.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/panels.py` & `fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/panels.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/ui/components/widgets/text.py` & `fastapi_xray-0.1.1/fastapi_xray/ui/components/widgets/text.py`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/ui/main.css` & `fastapi_xray-0.1.1/fastapi_xray/ui/main.css`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/fastapi_xray/xray.py` & `fastapi_xray-0.1.1/fastapi_xray/xray.py`

 * *Files 7% similar despite different names*

```diff
@@ -181,15 +181,27 @@
 
 async def extract_body(body: bytes, request: Request) -> bytes:
     if request.headers.get("Content-Type") == "application/json":
         # This is workaround to get request body in the middleware
         # https://stackoverflow.com/a/74778485/6832201
         await set_body(request, await request.body())
         body = await request.json()
+    elif request.headers.get("Content-Type") == "application/x-www-form-urlencoded":
+        await set_body(request, await request.body())
+        form_data = await form_to_json(request)
+        return form_data
     return body
 
+async def form_to_json(request: Request):
+        form_data = await request.form()
+        form_items = form_data.items()
+        form_body = {}
+        for item in form_items:
+            form_body[item[0]] = item[1]
+        return form_body
+
 
 def send_debug_info(debug_info: Dict):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as out_sock:
         out_sock.connect((HOST, OUT_PORT))
         out_sock.sendall(json.dumps(debug_info).encode("utf-8"))
         logger.info("Sent data to receiver")
```

### Comparing `fastapi_xray-0.1.0/fastapi_xray.egg-info/PKG-INFO` & `fastapi_xray-0.1.1/fastapi_xray.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-xray
-Version: 0.1.0
+Version: 0.1.1
 Summary: A FastAPI debug tool to look into request/response
 Author-email: Ropali Munshi <ropali68@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 ![image](https://github.com/ropali/fastapi_xray/assets/31515245/504a8da8-f366-4f1c-ba56-cd798cb70a91)
 
 ![image](https://github.com/ropali/fastapi_xray/assets/31515245/cc1fb459-f4b3-45ff-ae66-1c5a48316f6c)
 
 ## Installation
 Install this package from pypi using this command.
 ```
-pip install fastapi_xray
+pip install fastapi-xray
 ```
 
 ## Usage
 It is very easy to use. Call the `start_xray` function to start intercepting all the request and response.
 
 ```
 from fastapi import FastAPI
```

### Comparing `fastapi_xray-0.1.0/fastapi_xray.egg-info/SOURCES.txt` & `fastapi_xray-0.1.1/fastapi_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_xray-0.1.0/pyproject.toml` & `fastapi_xray-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fastapi_xray"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Ropali Munshi", email = "ropali68@example.com" },
 ]
 
 description = "A FastAPI debug tool to look into request/response"
 readme = "README.md"
 requires-python = ">=3.8"
```

