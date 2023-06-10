# Comparing `tmp/reqto-0.1.6.tar.gz` & `tmp/reqto-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\reqto-0.1.6.tar", last modified: Fri Mar 18 03:41:19 2022, max compression
+gzip compressed data, was "reqto-0.1.7.tar", last modified: Sat Jun 10 17:24:36 2023, max compression
```

## Comparing `reqto-0.1.6.tar` & `reqto-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-03-18 03:41:19.000000 reqto-0.1.6/
--rw-rw-rw-   0        0        0      487 2022-03-18 03:41:19.000000 reqto-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-03-18 03:06:27.000000 reqto-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto/
--rw-rw-rw-   0        0        0      115 2022-03-18 03:40:58.000000 reqto-0.1.6/reqto/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto/core/
--rw-rw-rw-   0        0        0        0 2022-03-18 03:36:26.000000 reqto-0.1.6/reqto/core/__init__.py
--rw-rw-rw-   0        0        0     4240 2022-03-18 03:03:14.000000 reqto-0.1.6/reqto/core/reqto.py
--rw-rw-rw-   0        0        0      439 2022-03-18 03:13:53.000000 reqto-0.1.6/reqto/example.py
-drwxrwxrwx   0        0        0        0 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto.egg-info/
--rw-rw-rw-   0        0        0      487 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-03-18 03:41:19.000000 reqto-0.1.6/reqto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-18 03:41:19.000000 reqto-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      755 2022-03-18 03:41:18.000000 reqto-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:24:36.608153 reqto-0.1.7/
+-rw-rw-rw-   0        0        0     1090 2022-03-18 03:43:56.000000 reqto-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1629 2023-06-10 17:24:36.607156 reqto-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-06-10 17:24:04.000000 reqto-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 17:24:36.586212 reqto-0.1.7/reqto/
+-rw-rw-rw-   0        0        0      115 2022-03-18 03:40:58.000000 reqto-0.1.7/reqto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:24:36.607156 reqto-0.1.7/reqto/core/
+-rw-rw-rw-   0        0        0        0 2022-03-18 03:36:26.000000 reqto-0.1.7/reqto/core/__init__.py
+-rw-rw-rw-   0        0        0     4206 2023-06-10 17:14:41.000000 reqto-0.1.7/reqto/core/reqto.py
+-rw-rw-rw-   0        0        0      471 2022-03-18 03:45:01.000000 reqto-0.1.7/reqto/example.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:24:36.605162 reqto-0.1.7/reqto.egg-info/
+-rw-rw-rw-   0        0        0     1629 2023-06-10 17:24:35.000000 reqto-0.1.7/reqto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-10 17:24:36.000000 reqto-0.1.7/reqto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 17:24:36.000000 reqto-0.1.7/reqto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-10 17:24:36.000000 reqto-0.1.7/reqto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-10 17:24:36.000000 reqto-0.1.7/reqto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 17:24:36.608153 reqto-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-10 17:24:32.000000 reqto-0.1.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `reqto-0.1.6/reqto/core/reqto.py` & `reqto-0.1.7/reqto/core/reqto.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,106 +12,100 @@
     try:
         if type(timeout)==list or type(timeout)==tuple:
             timeout=timeout[0]
         with eventlet.Timeout(timeout):
             arguments={**{"url":url},**kwargs}
             response = requests.get(**arguments)
         return(response)
-    except eventlet.timeout.Timeout:
+    except eventlet.timeout.Timeout as exc:
         if timeout_function is not None:
             if timeout_args is not None:
                 timeout_function(timeout_args)
             else:
                 timeout_function()
         else:
-            raise requests.exceptions.Timeout
-            
-            
+            raise requests.exceptions.Timeout from exc
+
 def post(url, data=None, json=None, timeout=None, timeout_function=None, timeout_args=None, **kwargs):
     try:
         if type(timeout)==list or type(timeout)==tuple:
             timeout=timeout[0]
         with eventlet.Timeout(timeout):
             arguments={**{"url":url, "data":data, "json":json},**kwargs}
             response = requests.post(**arguments)
         return(response)
-    except eventlet.timeout.Timeout:
+    except eventlet.timeout.Timeout as exc:
         if timeout_function is not None:
             if timeout_args is not None:
                 timeout_function(timeout_args)
             else:
                 timeout_function()
         else:
-            raise requests.exceptions.Timeout
-            
+            raise requests.exceptions.Timeout from exc
 
 def put(url, data=None, timeout=None, timeout_function=None, timeout_args=None, **kwargs):
     try:
         if type(timeout)==list or type(timeout)==tuple:
             timeout=timeout[0]
         with eventlet.Timeout(timeout):
             arguments={**{"url":url, "data":data},**kwargs}
             response = requests.put(**arguments)
         return(response)
-    except eventlet.timeout.Timeout:
+    except eventlet.timeout.Timeout as exc:
         if timeout_function is not None:
             if timeout_args is not None:
                 timeout_function(timeout_args)
             else:
                 timeout_function()
         else:
-            raise requests.exceptions.Timeout
-            
-            
+            raise requests.exceptions.Timeout from exc
+
 def patch(url, data=None, timeout=None, timeout_function=None, timeout_args=None, **kwargs):
     try:
         if type(timeout)==list or type(timeout)==tuple:
             timeout=timeout[0]
         with eventlet.Timeout(timeout):
             arguments={**{"url":url, "data":data},**kwargs}
             response = requests.patch(**arguments)
         return(response)
-    except eventlet.timeout.Timeout:
+    except eventlet.timeout.Timeout as exc:
         if timeout_function is not None:
             if timeout_args is not None:
                 timeout_function(timeout_args)
             else:
                 timeout_function()
         else:
-            raise requests.exceptions.Timeout
-            
-            
+            raise requests.exceptions.Timeout from exc
+
 def delete(url, timeout=None, timeout_function=None, timeout_args=None, **kwargs):
     try:
         if type(timeout)==list or type(timeout)==tuple:
             timeout=timeout[0]
         with eventlet.Timeout(timeout):
             arguments={**{"url":url},**kwargs}
             response = requests.delete(**arguments)
         return(response)
-    except eventlet.timeout.Timeout:
+    except eventlet.timeout.Timeout as exc:
         if timeout_function is not None:
             if timeout_args is not None:
                 timeout_function(timeout_args)
             else:
                 timeout_function()
         else:
-            raise requests.exceptions.Timeout
-            
-            
+            raise requests.exceptions.Timeout from exc
+
 def head(url, timeout=None, timeout_function=None, timeout_args=None, **kwargs):
     try:
         if type(timeout)==list or type(timeout)==tuple:
             timeout=timeout[0]
         with eventlet.Timeout(timeout):
             arguments={**{"url":url},**kwargs}
             response = requests.head(**arguments)
         return(response)
-    except eventlet.timeout.Timeout:
+    except eventlet.timeout.Timeout as exc:
         if timeout_function is not None:
             if timeout_args is not None:
                 timeout_function(timeout_args)
             else:
                 timeout_function()
         else:
-            raise requests.exceptions.Timeout
-            
+            raise requests.exceptions.Timeout from exc
```

### Comparing `reqto-0.1.6/setup.py` & `reqto-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='reqto',
-    version='0.1.6',
+    version='0.1.7',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A wrapper around requests to tackle unstable timeout issues',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/reqto',
     packages=setuptools.find_packages(),
```

