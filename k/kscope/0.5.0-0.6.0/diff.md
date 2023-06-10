# Comparing `tmp/kscope-0.5.0.tar.gz` & `tmp/kscope-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kscope-0.5.0.tar", last modified: Tue Apr 18 20:33:18 2023, max compression
+gzip compressed data, was "kscope-0.6.0.tar", last modified: Sat Jun 10 13:08:52 2023, max compression
```

## Comparing `kscope-0.5.0.tar` & `kscope-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-04-18 20:33:18.631625 kscope-0.5.0/
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1073 2023-04-18 20:33:06.000000 kscope-0.5.0/LICENSE
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5225 2023-04-18 20:33:18.631625 kscope-0.5.0/PKG-INFO
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     4276 2023-04-18 20:33:06.000000 kscope-0.5.0/README.md
-drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-04-18 20:33:18.631625 kscope-0.5.0/kscope/
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      181 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/__init__.py
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      513 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/hooks.py
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     8971 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/kaleidoscope_sdk.py
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1526 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/utils.py
-drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-04-18 20:33:18.631625 kscope-0.5.0/kscope.egg-info/
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5225 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/PKG-INFO
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      253 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/SOURCES.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        1 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/dependency_links.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      134 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/requires.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        7 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/top_level.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)       38 2023-04-18 20:33:18.631625 kscope-0.5.0/setup.cfg
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1427 2023-04-18 20:33:06.000000 kscope-0.5.0/setup.py
+drwxr-xr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-06-10 13:08:52.644707 kscope-0.6.0/
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     1073 2023-06-10 00:19:17.000000 kscope-0.6.0/LICENSE
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     5904 2023-06-10 13:08:52.644707 kscope-0.6.0/PKG-INFO
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     4955 2023-06-10 00:19:17.000000 kscope-0.6.0/README.md
+drwxr-xr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-06-10 13:08:52.644707 kscope-0.6.0/kscope/
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      226 2023-06-10 13:08:44.000000 kscope-0.6.0/kscope/__init__.py
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      513 2023-06-10 00:19:18.000000 kscope-0.6.0/kscope/hooks.py
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)    10720 2023-06-10 00:19:18.000000 kscope-0.6.0/kscope/kaleidoscope_sdk.py
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     1643 2023-06-10 00:19:18.000000 kscope-0.6.0/kscope/utils.py
+drwxr-xr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-06-10 13:08:52.644707 kscope-0.6.0/kscope.egg-info/
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     5904 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/PKG-INFO
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      253 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/SOURCES.txt
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)        1 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/dependency_links.txt
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      134 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/requires.txt
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)        7 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/top_level.txt
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)       38 2023-06-10 13:08:52.644707 kscope-0.6.0/setup.cfg
+-rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     1427 2023-06-10 13:08:44.000000 kscope-0.6.0/setup.py
```

### Comparing `kscope-0.5.0/LICENSE` & `kscope-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kscope-0.5.0/PKG-INFO` & `kscope-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.5.0
+Version: 0.6.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
@@ -109,14 +109,34 @@
 # First, show a list of modules in the neural network
 print(opt_model.module_names)
 
 # Setup a request for module acivations for a certain module layer
 requested_activations = ['decoder.layers.0']
 activations = opt_model.get_activations("What are activations?", requested_activations)
 print(activations)
+
+# Next, let's manipulate the activations in the model. First, we need to import a few more modules.
+import cloudpickle
+import codecs
+import torch
+from torch import Tensor
+from typing import Callable, Dict
+
+# Define a function to manipulate the activations
+def replace_with_ones(act: Tensor) -> Tensor:
+    """Replace an activation with an activation filled with ones."""
+    out = torch.ones_like(act, dtype=act.dtype).cuda()
+    return out
+
+# Now send the edit request
+editing_fns: Dict[str, Callable] = {}
+editing_fns['decoder.layers.0'] = replace_with_ones
+edited_activations = opt_model.edit_activations("Testing activation editing", editing_fns)
+print(edited_activations)
+
 ```
 
 ## Documentation
 Full documentation and API reference are available at: http://kaleidoscope-sdk.readthedocs.io.
 
 
 ## Contributing
```

### Comparing `kscope-0.5.0/README.md` & `kscope-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,34 @@
 # First, show a list of modules in the neural network
 print(opt_model.module_names)
 
 # Setup a request for module acivations for a certain module layer
 requested_activations = ['decoder.layers.0']
 activations = opt_model.get_activations("What are activations?", requested_activations)
 print(activations)
+
+# Next, let's manipulate the activations in the model. First, we need to import a few more modules.
+import cloudpickle
+import codecs
+import torch
+from torch import Tensor
+from typing import Callable, Dict
+
+# Define a function to manipulate the activations
+def replace_with_ones(act: Tensor) -> Tensor:
+    """Replace an activation with an activation filled with ones."""
+    out = torch.ones_like(act, dtype=act.dtype).cuda()
+    return out
+
+# Now send the edit request
+editing_fns: Dict[str, Callable] = {}
+editing_fns['decoder.layers.0'] = replace_with_ones
+edited_activations = opt_model.edit_activations("Testing activation editing", editing_fns)
+print(edited_activations)
+
 ```
 
 ## Documentation
 Full documentation and API reference are available at: http://kaleidoscope-sdk.readthedocs.io.
 
 
 ## Contributing
```

### Comparing `kscope-0.5.0/kscope/hooks.py` & `kscope-0.6.0/kscope/hooks.py`

 * *Files identical despite different names*

### Comparing `kscope-0.5.0/kscope/kaleidoscope_sdk.py` & `kscope-0.6.0/kscope/kaleidoscope_sdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from functools import cached_property, partial
 from getpass import getpass
 import json
 import requests
 from pathlib import Path
 import sys
 import time
-from typing import Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional, Union
 from urllib.parse import urljoin
 
 from .hooks import TestForwardHook
-from .utils import get, post, decode_str
+from .utils import get, post, decode_str, encode_obj
 
 JWT_TOKEN_FILE = Path(Path.home() / ".kaleidoscope.jwt")
 
 
 class Client:
     def __init__(
         self,
@@ -191,14 +191,36 @@
             "generation_config": generation_config,
         }
 
         response = post(url, body, auth_key=self.auth_key)
 
         return response
 
+    def edit_activations(
+        self,
+        model_instance_id: str,
+        prompts: List[str],
+        modules: Dict[str, Optional[Callable]],
+        generation_config: Dict,
+    ):
+        """Gets activations from the model instance"""
+
+        url = self.create_addr(
+            f"models/instances/{model_instance_id}/edit_activations"
+        )
+        body = {
+            "prompts": prompts,
+            "modules": modules,
+            "generation_config": generation_config,
+        }
+
+        response = post(url, body, auth_key=self.auth_key)
+
+        return response
+
 
 class Model:
     def __init__(
         self, model_instance_id: str, model_name: str, session: GatewaySession
     ):
         """Initializes a model instance
 
@@ -223,15 +245,15 @@
     def is_active(self):
         """Checks if the model instance is active"""
         return self.state == "ACTIVE"
 
     def generate(self, prompts: Union[str, List[str]], generation_config: Dict = {}):
         """Generates text from the model instance
 
-        :param prompts: (str or List[str]) Single prompt or list of prompts to generate from. 
+        :param prompts: (str or List[str]) Single prompt or list of prompts to generate from.
         Supports upto 8 prompts in a single request.
         :param kwargs: (dict) Additional arguments to pass to the model
         """
         if isinstance(prompts, str):
             prompts = [prompts]
         generation_response = self._session.generate(
             self.id, prompts, generation_config
@@ -258,9 +280,34 @@
         )
         for idx in range(len(activations_response["activations"])):
             for elm in activations_response["activations"][idx]:
                 activations_response["activations"][idx][elm] = decode_str(
                     activations_response["activations"][idx][elm]
                 )
 
+        Activations = namedtuple("Activations", activations_response.keys())
+        return Activations(**activations_response)
+
+    def edit_activations(
+        self,
+        prompts: Union[str, List[str]],
+        modules: Dict[str, Optional[Callable]],
+        generation_config: Dict = {},
+    ):
+        """Edits activations for the model instance
+        :param prompts: (str or List[str]) Single prompt or list of prompts to generate from
+        :param modules: (Dict[str, Optional[Callable]]) The layer names and manipulation functions to apply to them
+        """
+        if isinstance(prompts, str):
+            prompts = [prompts]
+        encoded_activation_payload = encode_obj(modules)
+        activations_response = self._session.edit_activations(
+            self.id, prompts, encoded_activation_payload, generation_config
+        )
+        for idx in range(len(activations_response["activations"])):
+            for elm in activations_response["activations"][idx]:
+                activations_response["activations"][idx][elm] = decode_str(
+                    activations_response["activations"][idx][elm]
+                )
+
         Activations = namedtuple("Activations", activations_response.keys())
         return Activations(**activations_response)
```

### Comparing `kscope-0.5.0/kscope/utils.py` & `kscope-0.6.0/kscope/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """
 TODOS:
     1. eventually we need to seperate this out to client and server utils
 """
+import cloudpickle
 import logging
 import json
 import requests
 import pickle
 import codecs
 
 logger = logging.getLogger(__name__)
 
 
 def decode_str(obj_in_str):
     return pickle.loads(codecs.decode(obj_in_str.encode("utf-8"), "base64"))
 
 
+def encode_obj(obj):
+    return codecs.encode(cloudpickle.dumps(obj), "base64").decode("utf-8")
+
+
 def check_response(resp):
     if not resp.ok:
         if resp.status_code == 422:
             raise ValueError(
                 "Request to {} not sucessful, Error Code: {}, please check your auth key".format(
                     resp.url, resp.status_code
                 )
```

### Comparing `kscope-0.5.0/kscope.egg-info/PKG-INFO` & `kscope-0.6.0/kscope.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.5.0
+Version: 0.6.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
@@ -109,14 +109,34 @@
 # First, show a list of modules in the neural network
 print(opt_model.module_names)
 
 # Setup a request for module acivations for a certain module layer
 requested_activations = ['decoder.layers.0']
 activations = opt_model.get_activations("What are activations?", requested_activations)
 print(activations)
+
+# Next, let's manipulate the activations in the model. First, we need to import a few more modules.
+import cloudpickle
+import codecs
+import torch
+from torch import Tensor
+from typing import Callable, Dict
+
+# Define a function to manipulate the activations
+def replace_with_ones(act: Tensor) -> Tensor:
+    """Replace an activation with an activation filled with ones."""
+    out = torch.ones_like(act, dtype=act.dtype).cuda()
+    return out
+
+# Now send the edit request
+editing_fns: Dict[str, Callable] = {}
+editing_fns['decoder.layers.0'] = replace_with_ones
+edited_activations = opt_model.edit_activations("Testing activation editing", editing_fns)
+print(edited_activations)
+
 ```
 
 ## Documentation
 Full documentation and API reference are available at: http://kaleidoscope-sdk.readthedocs.io.
 
 
 ## Contributing
```

### Comparing `kscope-0.5.0/setup.py` & `kscope-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="kscope",
-    version="0.5.0",
+    version="0.6.0",
     description="A user toolkit for analyzing and interfacing with Large Language Models (LLMs)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm",
     requires_python=">=3.7",
     url="https://github.com/VectorInstitute/kaleidoscope-sdk",
     author=["Vector AI Engineering"],
```

