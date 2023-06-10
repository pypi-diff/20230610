# Comparing `tmp/chatdocs-0.2.3.tar.gz` & `tmp/chatdocs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.2.3.tar", last modified: Sat Jun 10 08:52:05 2023, max compression
+gzip compressed data, was "chatdocs-0.2.4.tar", last modified: Sat Jun 10 21:49:34 2023, max compression
```

## Comparing `chatdocs-0.2.3.tar` & `chatdocs-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9764 2023-06-10 08:52:05.323495 chatdocs-0.2.3/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6708 2023-06-10 08:08:07.000000 chatdocs-0.2.3/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.3/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.3/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5675 2023-06-10 08:41:19.000000 chatdocs-0.2.3/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.3/chatdocs/chains.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1376 2023-06-07 13:32:32.000000 chatdocs-0.2.3/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.3/chatdocs/config.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/chatdocs/data/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      639 2023-06-07 13:37:27.000000 chatdocs-0.2.3/chatdocs/data/chatdocs.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4272 2023-06-04 20:29:35.000000 chatdocs-0.2.3/chatdocs/data/index.html
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-07 19:32:55.000000 chatdocs-0.2.3/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.3/chatdocs/embeddings.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2668 2023-06-07 19:29:24.000000 chatdocs-0.2.3/chatdocs/llms.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.3/chatdocs/main.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.3/chatdocs/ui.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      219 2023-06-07 13:30:29.000000 chatdocs-0.2.3/chatdocs/utils.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.3/chatdocs/vectorstores.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9764 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      445 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-10 08:52:05.323495 chatdocs-0.2.3/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2247 2023-06-10 08:42:20.000000 chatdocs-0.2.3/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-10 21:49:34.126123 chatdocs-0.2.4/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6766 2023-06-10 21:30:46.000000 chatdocs-0.2.4/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.4/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.4/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5675 2023-06-10 08:41:19.000000 chatdocs-0.2.4/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.4/chatdocs/chains.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1376 2023-06-07 13:32:32.000000 chatdocs-0.2.4/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.4/chatdocs/config.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/chatdocs/data/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      697 2023-06-10 21:23:28.000000 chatdocs-0.2.4/chatdocs/data/chatdocs.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4297 2023-06-10 21:28:38.000000 chatdocs-0.2.4/chatdocs/data/index.html
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-07 19:32:55.000000 chatdocs-0.2.4/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.4/chatdocs/embeddings.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2668 2023-06-07 19:29:24.000000 chatdocs-0.2.4/chatdocs/llms.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.4/chatdocs/main.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.4/chatdocs/ui.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      219 2023-06-07 13:30:29.000000 chatdocs-0.2.4/chatdocs/utils.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.4/chatdocs/vectorstores.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      445 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-10 21:49:34.126123 chatdocs-0.2.4/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2247 2023-06-10 21:43:44.000000 chatdocs-0.2.4/setup.py
```

### Comparing `chatdocs-0.2.3/PKG-INFO` & `chatdocs-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.3
+Version: 0.2.4
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
         
@@ -114,14 +114,15 @@
         ### C Transformers
         
         To change the C Transformers GGML model, add and change the following in your `chatdocs.yml`:
         
         ```yml
         ctransformers:
           model: TheBloke/Wizard-Vicuna-7B-Uncensored-GGML
+          model_file: Wizard-Vicuna-7B-Uncensored.ggmlv3.q4_0.bin
           model_type: llama
         ```
         
         > **Note:** When you add a new model for the first time, run `chatdocs download` to download the model before using it.
         
         You can also use an existing local model file:
```

### Comparing `chatdocs-0.2.3/README.md` & `chatdocs-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 ### C Transformers
 
 To change the C Transformers GGML model, add and change the following in your `chatdocs.yml`:
 
 ```yml
 ctransformers:
   model: TheBloke/Wizard-Vicuna-7B-Uncensored-GGML
+  model_file: Wizard-Vicuna-7B-Uncensored.ggmlv3.q4_0.bin
   model_type: llama
 ```
 
 > **Note:** When you add a new model for the first time, run `chatdocs download` to download the model before using it.
 
 You can also use an existing local model file:
```

### Comparing `chatdocs-0.2.3/chatdocs/add.py` & `chatdocs-0.2.4/chatdocs/add.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs/chains.py` & `chatdocs-0.2.4/chatdocs/chains.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs/chat.py` & `chatdocs-0.2.4/chatdocs/chat.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs/config.py` & `chatdocs-0.2.4/chatdocs/config.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs/data/chatdocs.yml` & `chatdocs-0.2.4/chatdocs/data/chatdocs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 embeddings:
   model: hkunlp/instructor-large
 
 llm: ctransformers
 
 ctransformers:
   model: TheBloke/Wizard-Vicuna-7B-Uncensored-GGML
+  model_file: Wizard-Vicuna-7B-Uncensored.ggmlv3.q4_0.bin
   model_type: llama
   config:
     context_length: 1024
 
 huggingface:
   model: TheBloke/Wizard-Vicuna-7B-Uncensored-HF
   pipeline_kwargs:
```

### Comparing `chatdocs-0.2.3/chatdocs/data/index.html` & `chatdocs-0.2.4/chatdocs/data/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<title>ChatDocs</title>
+
 <script>
   const ws = new WebSocket(`ws://${location.host}/ws`);
 
   ws.addEventListener('message', (event) => {
     data = JSON.parse(event.data);
     onReceive(data);
   });
```

### Comparing `chatdocs-0.2.3/chatdocs/llms.py` & `chatdocs-0.2.4/chatdocs/llms.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs/main.py` & `chatdocs-0.2.4/chatdocs/main.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs/ui.py` & `chatdocs-0.2.4/chatdocs/ui.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs/vectorstores.py` & `chatdocs-0.2.4/chatdocs/vectorstores.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/chatdocs.egg-info/PKG-INFO` & `chatdocs-0.2.4/chatdocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.3
+Version: 0.2.4
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
         
@@ -114,14 +114,15 @@
         ### C Transformers
         
         To change the C Transformers GGML model, add and change the following in your `chatdocs.yml`:
         
         ```yml
         ctransformers:
           model: TheBloke/Wizard-Vicuna-7B-Uncensored-GGML
+          model_file: Wizard-Vicuna-7B-Uncensored.ggmlv3.q4_0.bin
           model_type: llama
         ```
         
         > **Note:** When you add a new model for the first time, run `chatdocs download` to download the model before using it.
         
         You can also use an existing local model file:
```

### Comparing `chatdocs-0.2.3/chatdocs.egg-info/SOURCES.txt` & `chatdocs-0.2.4/chatdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.3/setup.py` & `chatdocs-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.2.3",
+    version="0.2.4",
     description="Chat with your documents offline using AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
```

