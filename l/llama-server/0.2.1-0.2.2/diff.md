# Comparing `tmp/llama-server-0.2.1.tar.gz` & `tmp/llama-server-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-server-0.2.1.tar", last modified: Sun Apr 30 17:13:17 2023, max compression
+gzip compressed data, was "llama-server-0.2.2.tar", last modified: Sat Jun 10 01:23:47 2023, max compression
```

## Comparing `llama-server-0.2.1.tar` & `llama-server-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 17:13:06.000000 llama-server-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 17:13:17.934796 llama-server-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-30 17:13:06.000000 llama-server-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/llama_server/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/llama_server/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/alpaca.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/chat-with-bob.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/dan.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/reason-act.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/llama_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-30 17:13:17.934796 llama-server-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-30 17:13:06.000000 llama-server-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:23:47.806622 llama-server-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-10 01:23:33.000000 llama-server-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-10 01:23:47.806622 llama-server-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-10 01:23:33.000000 llama-server-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:23:47.806622 llama-server-0.2.2/llama_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 01:23:33.000000 llama-server-0.2.2/llama_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:23:47.806622 llama-server-0.2.2/llama_server/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-10 01:23:33.000000 llama-server-0.2.2/llama_server/prompts/alpaca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-10 01:23:33.000000 llama-server-0.2.2/llama_server/prompts/chat-with-bob.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-10 01:23:33.000000 llama-server-0.2.2/llama_server/prompts/dan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-10 01:23:33.000000 llama-server-0.2.2/llama_server/prompts/reason-act.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-10 01:23:33.000000 llama-server-0.2.2/llama_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:23:47.806622 llama-server-0.2.2/llama_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-10 01:23:47.000000 llama-server-0.2.2/llama_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-10 01:23:47.000000 llama-server-0.2.2/llama_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:23:47.000000 llama-server-0.2.2/llama_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-10 01:23:47.000000 llama-server-0.2.2/llama_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-10 01:23:47.000000 llama-server-0.2.2/llama_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 01:23:47.000000 llama-server-0.2.2/llama_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-10 01:23:47.806622 llama-server-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-10 01:23:33.000000 llama-server-0.2.2/setup.py
```

### Comparing `llama-server-0.2.1/LICENSE` & `llama-server-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.1/PKG-INFO` & `llama-server-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-server
-Version: 0.2.1
+Version: 0.2.2
 Summary: LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.
 Home-page: https://github.com/nuance1979/llama-server
 Author: Yi Su
 Author-email: nuance@gmail.com
 License: MIT
 Keywords: llama llama.cpp chatbot-ui chatbot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `llama-server-0.2.1/README.md` & `llama-server-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.1/llama_server/prompts/dan.txt` & `llama-server-0.2.2/llama_server/prompts/dan.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.1/llama_server/prompts/reason-act.txt` & `llama-server-0.2.2/llama_server/prompts/reason-act.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.1/llama_server/server.py` & `llama-server-0.2.2/llama_server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         assert model_id in KNOWN_MODELS.models, f"Unknown model id: {model_id}"
     if model_path is None:
         model_path = Path(KNOWN_MODELS.models.get(model_id).path)
         if not model_path.is_absolute():
             model_path = Path(KNOWN_MODELS.model_home) / model_path
     globals()["model_id"] = model_id
     globals()["model"] = Model(
-        ggml_model=str(model_path),
+        model_path=str(model_path),
         n_ctx=512,
         prompt_context=PROMPT,
         prompt_prefix=REVERSE_PROMPT,
         prompt_suffix=REPLY_PREFIX,
     )
     globals()["logger"] = logging.getLogger(name=__name__)
     globals()["logger"].setLevel(log_level)
```

### Comparing `llama-server-0.2.1/llama_server.egg-info/PKG-INFO` & `llama-server-0.2.2/llama_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-server
-Version: 0.2.1
+Version: 0.2.2
 Summary: LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.
 Home-page: https://github.com/nuance1979/llama-server
 Author: Yi Su
 Author-email: nuance@gmail.com
 License: MIT
 Keywords: llama llama.cpp chatbot-ui chatbot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `llama-server-0.2.1/setup.py` & `llama-server-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     req = {
         "dev": [
             "httpx",
             "pre-commit",
             "pytest",
             "pytest-cov",
             "pytest-xdist",
+            "numpy",
         ],
     }
     return req
 
 
 setup(
     name="llama-server",
```

