# Comparing `tmp/basaran-0.18.1.tar.gz` & `tmp/basaran-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.18.1.tar", last modified: Fri Jun  2 04:51:04 2023, max compression
+gzip compressed data, was "basaran-0.19.0.tar", last modified: Sat Jun 10 04:46:31 2023, max compression
```

## Comparing `basaran-0.18.1.tar` & `basaran-0.19.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.066489 basaran-0.18.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-02 04:48:11.000000 basaran-0.18.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 04:48:11.000000 basaran-0.18.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-02 04:51:04.066489 basaran-0.18.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-02 04:48:11.000000 basaran-0.18.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.058489 basaran-0.18.1/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.058489 basaran-0.18.1/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.062489 basaran-0.18.1/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/templates/default.chat.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.058489 basaran-0.18.1/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:51:04.066489 basaran-0.18.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-02 04:48:11.000000 basaran-0.18.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.062489 basaran-0.18.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-02 04:48:11.000000 basaran-0.18.1/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-02 04:48:11.000000 basaran-0.18.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-02 04:48:11.000000 basaran-0.18.1/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.062489 basaran-0.18.1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-02 04:48:11.000000 basaran-0.18.1/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-02 04:48:11.000000 basaran-0.18.1/utils/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-10 04:44:14.000000 basaran-0.19.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 04:44:14.000000 basaran-0.19.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-10 04:46:31.040270 basaran-0.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-10 04:44:14.000000 basaran-0.19.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.036270 basaran-0.19.0/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.036270 basaran-0.19.0/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/templates/default.chat.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.036270 basaran-0.19.0/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 04:46:31.040270 basaran-0.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-10 04:44:14.000000 basaran-0.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-10 04:44:14.000000 basaran-0.19.0/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-10 04:44:14.000000 basaran-0.19.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-10 04:44:14.000000 basaran-0.19.0/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-10 04:44:14.000000 basaran-0.19.0/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-10 04:44:14.000000 basaran-0.19.0/utils/render.py
```

### Comparing `basaran-0.18.1/LICENSE` & `basaran-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/PKG-INFO` & `basaran-0.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.18.1
+Version: 0.19.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.18.1/README.md` & `basaran-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/basaran/__init__.py` & `basaran-0.19.0/basaran/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 HOST = os.getenv("HOST", "0.0.0.0")
 PORT = int(os.getenv("PORT", "80"))
 
 # Model-related arguments:
 MODEL_REVISION = os.getenv("MODEL_REVISION", "")
 MODEL_CACHE_DIR = os.getenv("MODEL_CACHE_DIR", "models")
 MODEL_LOAD_IN_8BIT = is_true(os.getenv("MODEL_LOAD_IN_8BIT", ""))
+MODEL_LOAD_IN_4BIT = is_true(os.getenv("MODEL_LOAD_IN_4BIT", ""))
 MODEL_LOCAL_FILES_ONLY = is_true(os.getenv("MODEL_LOCAL_FILES_ONLY", ""))
 MODEL_TRUST_REMOTE_CODE = is_true(os.getenv("MODEL_TRUST_REMOTE_CODE", ""))
 MODEL_HALF_PRECISION = is_true(os.getenv("MODEL_HALF_PRECISION", ""))
 
 # Server-related arguments:
 # https://docs.pylonsproject.org/projects/waitress/en/stable/arguments.html
 SERVER_THREADS = int(os.getenv("SERVER_THREADS", "32"))
```

### Comparing `basaran-0.18.1/basaran/__main__.py` & `basaran-0.19.0/basaran/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # Configurations from environment variables.
 from . import MODEL
 from . import HOST
 from . import PORT
 from . import MODEL_REVISION
 from . import MODEL_CACHE_DIR
 from . import MODEL_LOAD_IN_8BIT
+from . import MODEL_LOAD_IN_4BIT
 from . import MODEL_LOCAL_FILES_ONLY
 from . import MODEL_TRUST_REMOTE_CODE
 from . import MODEL_HALF_PRECISION
 from . import SERVER_THREADS
 from . import SERVER_IDENTITY
 from . import SERVER_CONNECTION_LIMIT
 from . import SERVER_CHANNEL_TIMEOUT
@@ -38,14 +39,15 @@
 
 # Load the language model to be served.
 stream_model = load_model(
     name_or_path=MODEL,
     revision=MODEL_REVISION,
     cache_dir=MODEL_CACHE_DIR,
     load_in_8bit=MODEL_LOAD_IN_8BIT,
+    load_in_4bit=MODEL_LOAD_IN_4BIT,
     local_files_only=MODEL_LOCAL_FILES_ONLY,
     trust_remote_code=MODEL_TRUST_REMOTE_CODE,
     half_precision=MODEL_HALF_PRECISION,
 )
 
 # Create and configure application.
 app = Flask(__name__)
```

### Comparing `basaran-0.18.1/basaran/choice.py` & `basaran-0.19.0/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/basaran/model.py` & `basaran-0.19.0/basaran/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,15 @@
 
 
 def load_model(
     name_or_path,
     revision=None,
     cache_dir=None,
     load_in_8bit=False,
+    load_in_4bit=False,
     local_files_only=False,
     trust_remote_code=False,
     half_precision=False,
 ):
     """Load a text generation model and make it stream-able."""
     kwargs = {
         "local_files_only": local_files_only,
@@ -318,17 +319,18 @@
     tokenizer = AutoTokenizer.from_pretrained(name_or_path, **kwargs)
 
     # Set device mapping and quantization options if CUDA is available.
     if torch.cuda.is_available():
         kwargs = kwargs.copy()
         kwargs["device_map"] = "auto"
         kwargs["load_in_8bit"] = load_in_8bit
+        kwargs["load_in_4bit"] = load_in_4bit
 
         # Cast all parameters to float16 if quantization is enabled.
-        if half_precision or load_in_8bit:
+        if half_precision or load_in_8bit or load_in_4bit:
             kwargs["torch_dtype"] = torch.float16
 
     # Support both decoder-only and encoder-decoder models.
     try:
         model = AutoModelForCausalLM.from_pretrained(name_or_path, **kwargs)
     except ValueError:
         model = AutoModelForSeq2SeqLM.from_pretrained(name_or_path, **kwargs)
```

### Comparing `basaran-0.18.1/basaran/static/playground.css` & `basaran-0.19.0/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/basaran/static/playground.js` & `basaran-0.19.0/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/basaran/static/presets.json` & `basaran-0.19.0/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/basaran/templates/playground.html` & `basaran-0.19.0/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/basaran/tokenizer.py` & `basaran-0.19.0/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/basaran.egg-info/PKG-INFO` & `basaran-0.19.0/basaran.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.18.1
+Version: 0.19.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.18.1/basaran.egg-info/SOURCES.txt` & `basaran-0.19.0/basaran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/setup.py` & `basaran-0.19.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.18.1"
+VERSION = "0.19.0"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
```

### Comparing `basaran-0.18.1/tests/test_choice.py` & `basaran-0.19.0/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/tests/test_model.py` & `basaran-0.19.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/tests/test_tokenizer.py` & `basaran-0.19.0/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/utils/download.py` & `basaran-0.19.0/utils/download.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.1/utils/render.py` & `basaran-0.19.0/utils/render.py`

 * *Files identical despite different names*

