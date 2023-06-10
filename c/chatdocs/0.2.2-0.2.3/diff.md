# Comparing `tmp/chatdocs-0.2.2.tar.gz` & `tmp/chatdocs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.2.2.tar", last modified: Wed Jun  7 20:40:58 2023, max compression
+gzip compressed data, was "chatdocs-0.2.3.tar", last modified: Sat Jun 10 08:52:05 2023, max compression
```

## Comparing `chatdocs-0.2.2.tar` & `chatdocs-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.232766 chatdocs-0.2.2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-07 20:40:58.232766 chatdocs-0.2.2/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6774 2023-06-07 20:34:43.000000 chatdocs-0.2.2/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.222766 chatdocs-0.2.2/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.2/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.2/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5657 2023-06-04 03:56:33.000000 chatdocs-0.2.2/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.2/chatdocs/chains.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1376 2023-06-07 13:32:32.000000 chatdocs-0.2.2/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.2/chatdocs/config.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.232766 chatdocs-0.2.2/chatdocs/data/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      639 2023-06-07 13:37:27.000000 chatdocs-0.2.2/chatdocs/data/chatdocs.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4272 2023-06-04 20:29:35.000000 chatdocs-0.2.2/chatdocs/data/index.html
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-07 19:32:55.000000 chatdocs-0.2.2/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.2/chatdocs/embeddings.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2668 2023-06-07 19:29:24.000000 chatdocs-0.2.2/chatdocs/llms.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.2/chatdocs/main.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.2/chatdocs/ui.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      219 2023-06-07 13:30:29.000000 chatdocs-0.2.2/chatdocs/utils.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.2/chatdocs/vectorstores.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.222766 chatdocs-0.2.2/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      445 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-07 20:40:58.232766 chatdocs-0.2.2/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2247 2023-06-07 20:38:45.000000 chatdocs-0.2.2/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9764 2023-06-10 08:52:05.323495 chatdocs-0.2.3/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6708 2023-06-10 08:08:07.000000 chatdocs-0.2.3/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.3/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.3/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5675 2023-06-10 08:41:19.000000 chatdocs-0.2.3/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.3/chatdocs/chains.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1376 2023-06-07 13:32:32.000000 chatdocs-0.2.3/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.3/chatdocs/config.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/chatdocs/data/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      639 2023-06-07 13:37:27.000000 chatdocs-0.2.3/chatdocs/data/chatdocs.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4272 2023-06-04 20:29:35.000000 chatdocs-0.2.3/chatdocs/data/index.html
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-07 19:32:55.000000 chatdocs-0.2.3/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.3/chatdocs/embeddings.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2668 2023-06-07 19:29:24.000000 chatdocs-0.2.3/chatdocs/llms.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.3/chatdocs/main.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.3/chatdocs/ui.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      219 2023-06-07 13:30:29.000000 chatdocs-0.2.3/chatdocs/utils.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.3/chatdocs/vectorstores.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 08:52:05.323495 chatdocs-0.2.3/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9764 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      445 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-10 08:52:05.000000 chatdocs-0.2.3/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-10 08:52:05.323495 chatdocs-0.2.3/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2247 2023-06-10 08:42:20.000000 chatdocs-0.2.3/setup.py
```

### Comparing `chatdocs-0.2.2/PKG-INFO` & `chatdocs-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
         
@@ -149,15 +149,15 @@
         > **Note:** When you add a new model for the first time, run `chatdocs download` to download the model before using it.
         
         ### GPTQ
         
         To use GPTQ models, install the `auto-gptq` package using:
         
         ```sh
-        pip install git+https://github.com/PanQiWei/AutoGPTQ@v0.2.1
+        pip install chatdocs[gptq]
         ```
         
         and add the following to your `chatdocs.yml`:
         
         ```yml
         llm: gptq
         ```
@@ -248,15 +248,15 @@
         
         You may have to reinstall PyTorch with CUDA enabled by following the instructions [here](https://pytorch.org/get-started/locally/).
         
         After installing PyTorch with CUDA enabled, you should also reinstall the `auto-gptq` package:
         
         ```sh
         pip uninstall auto-gptq --yes
-        pip install git+https://github.com/PanQiWei/AutoGPTQ@v0.2.1
+        pip install chatdocs[gptq]
         ```
         
         ## License
         
         [MIT](https://github.com/marella/chatdocs/blob/main/LICENSE)
         
 Keywords: chatdocs ctransformers transformers langchain chroma ai llm
```

### Comparing `chatdocs-0.2.2/README.md` & `chatdocs-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 > **Note:** When you add a new model for the first time, run `chatdocs download` to download the model before using it.
 
 ### GPTQ
 
 To use GPTQ models, install the `auto-gptq` package using:
 
 ```sh
-pip install git+https://github.com/PanQiWei/AutoGPTQ@v0.2.1
+pip install chatdocs[gptq]
 ```
 
 and add the following to your `chatdocs.yml`:
 
 ```yml
 llm: gptq
 ```
@@ -240,13 +240,13 @@
 
 You may have to reinstall PyTorch with CUDA enabled by following the instructions [here](https://pytorch.org/get-started/locally/).
 
 After installing PyTorch with CUDA enabled, you should also reinstall the `auto-gptq` package:
 
 ```sh
 pip uninstall auto-gptq --yes
-pip install git+https://github.com/PanQiWei/AutoGPTQ@v0.2.1
+pip install chatdocs[gptq]
 ```
 
 ## License
 
 [MIT](https://github.com/marella/chatdocs/blob/main/LICENSE)
```

### Comparing `chatdocs-0.2.2/chatdocs/add.py` & `chatdocs-0.2.3/chatdocs/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             raise type(e)(f"{self.file_path}: {e}") from e
 
         return doc
 
 
 # Map file extensions to document loaders and their arguments
 LOADER_MAPPING = {
-    ".csv": (CSVLoader, {}),
+    ".csv": (CSVLoader, {"encoding": "utf8"}),
     # ".docx": (Docx2txtLoader, {}),
     ".doc": (UnstructuredWordDocumentLoader, {}),
     ".docx": (UnstructuredWordDocumentLoader, {}),
     ".enex": (EverNoteLoader, {}),
     ".eml": (MyElmLoader, {}),
     ".epub": (UnstructuredEPubLoader, {}),
     ".html": (UnstructuredHTMLLoader, {}),
```

### Comparing `chatdocs-0.2.2/chatdocs/chains.py` & `chatdocs-0.2.3/chatdocs/chains.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/chat.py` & `chatdocs-0.2.3/chatdocs/chat.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/config.py` & `chatdocs-0.2.3/chatdocs/config.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/data/chatdocs.yml` & `chatdocs-0.2.3/chatdocs/data/chatdocs.yml`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/data/index.html` & `chatdocs-0.2.3/chatdocs/data/index.html`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/llms.py` & `chatdocs-0.2.3/chatdocs/llms.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/main.py` & `chatdocs-0.2.3/chatdocs/main.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/ui.py` & `chatdocs-0.2.3/chatdocs/ui.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs/vectorstores.py` & `chatdocs-0.2.3/chatdocs/vectorstores.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/chatdocs.egg-info/PKG-INFO` & `chatdocs-0.2.3/chatdocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
         
@@ -149,15 +149,15 @@
         > **Note:** When you add a new model for the first time, run `chatdocs download` to download the model before using it.
         
         ### GPTQ
         
         To use GPTQ models, install the `auto-gptq` package using:
         
         ```sh
-        pip install git+https://github.com/PanQiWei/AutoGPTQ@v0.2.1
+        pip install chatdocs[gptq]
         ```
         
         and add the following to your `chatdocs.yml`:
         
         ```yml
         llm: gptq
         ```
@@ -248,15 +248,15 @@
         
         You may have to reinstall PyTorch with CUDA enabled by following the instructions [here](https://pytorch.org/get-started/locally/).
         
         After installing PyTorch with CUDA enabled, you should also reinstall the `auto-gptq` package:
         
         ```sh
         pip uninstall auto-gptq --yes
-        pip install git+https://github.com/PanQiWei/AutoGPTQ@v0.2.1
+        pip install chatdocs[gptq]
         ```
         
         ## License
         
         [MIT](https://github.com/marella/chatdocs/blob/main/LICENSE)
         
 Keywords: chatdocs ctransformers transformers langchain chroma ai llm
```

### Comparing `chatdocs-0.2.2/chatdocs.egg-info/SOURCES.txt` & `chatdocs-0.2.3/chatdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.2/setup.py` & `chatdocs-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.2.2",
+    version="0.2.3",
     description="Chat with your documents offline using AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
@@ -41,15 +41,15 @@
         "pdfminer.six==20221105",
         "unstructured>=0.6.0,<0.7.0",
         # Temporary fix for `rich`, `numpy` version conflicts.
         "argilla==1.8.0",
     ],
     extras_require={
         "gptq": [
-            "auto-gptq>=0.2.1,<0.3.0",
+            "auto-gptq>=0.2.2,<0.3.0",
         ],
         "tests": [
             "pytest",
         ],
     },
     zip_safe=False,
     classifiers=[
```

