# Comparing `tmp/langdash-1.1.1a1.tar.gz` & `tmp/langdash-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.1.1a1.tar", last modified: Fri Jun  9 18:58:59 2023, max compression
+gzip compressed data, was "langdash-1.2.0a1.tar", last modified: Sat Jun 10 03:27:02 2023, max compression
```

## Comparing `langdash-1.1.1a1.tar` & `langdash-1.2.0a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 18:58:59.186443 langdash-1.1.1a1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.1.1a1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.1.1a1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-09 18:58:59.186443 langdash-1.1.1a1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1804 2023-06-08 05:12:48.000000 langdash-1.1.1a1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 18:58:59.182442 langdash-1.1.1a1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       64 2023-06-09 18:58:51.000000 langdash-1.1.1a1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    22213 2023-06-09 18:58:51.000000 langdash-1.1.1a1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 18:58:59.178442 langdash-1.1.1a1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.1.1a1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.1.1a1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.1.1a1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      793 2023-06-09 06:56:17.000000 langdash-1.1.1a1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.1.1a1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7006 2023-06-07 02:26:23.000000 langdash-1.1.1a1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 18:58:59.182442 langdash-1.1.1a1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.1.1a1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.1.1a1/langdash/models/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     6902 2023-06-09 18:58:51.000000 langdash-1.1.1a1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.1.1a1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7973 2023-06-07 02:26:23.000000 langdash-1.1.1a1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.1.1a1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     7460 2023-06-09 06:56:17.000000 langdash-1.1.1a1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.1.1a1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2759 2023-06-09 06:56:17.000000 langdash-1.1.1a1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 18:58:59.182442 langdash-1.1.1a1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.1.1a1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1093 2023-06-09 18:58:51.000000 langdash-1.1.1a1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.1.1a1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.1.1a1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 18:58:59.182442 langdash-1.1.1a1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-09 18:58:59.000000 langdash-1.1.1a1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-09 18:58:59.000000 langdash-1.1.1a1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-09 18:58:59.000000 langdash-1.1.1a1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-09 18:58:59.000000 langdash-1.1.1a1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-09 18:58:59.000000 langdash-1.1.1a1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-09 18:58:59.186443 langdash-1.1.1a1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.1.1a1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.2.0a1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.2.0a1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     2854 2023-06-10 03:27:02.566714 langdash-1.2.0a1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1945 2023-06-10 03:20:18.000000 langdash-1.2.0a1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       64 2023-06-10 03:26:41.000000 langdash-1.2.0a1/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22279 2023-06-10 03:17:16.000000 langdash-1.2.0a1/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.562714 langdash-1.2.0a1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.2.0a1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.2.0a1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      793 2023-06-09 06:56:17.000000 langdash-1.2.0a1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.2.0a1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.2.0a1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/models/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7092 2023-06-10 00:53:03.000000 langdash-1.2.0a1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9657 2023-06-10 03:09:39.000000 langdash-1.2.0a1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.2.0a1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7536 2023-06-10 00:53:03.000000 langdash-1.2.0a1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2741 2023-06-10 03:12:00.000000 langdash-1.2.0a1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.562714 langdash-1.2.0a1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.2.0a1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1093 2023-06-09 18:58:51.000000 langdash-1.2.0a1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.2.0a1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.2.0a1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2854 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-10 03:27:02.566714 langdash-1.2.0a1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.2.0a1/setup.py
```

### Comparing `langdash-1.1.1a1/LICENSE.txt` & `langdash-1.2.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/PKG-INFO` & `langdash-1.2.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.1.1a1
+Version: 1.2.0a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -26,22 +26,24 @@
 
 [**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
 
 A simple library for interfacing with language models.
 
 **Currently in alpha!**
 
-Features:
+**Features:**
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends.
 
-Documentation: [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
+**Documentation:** [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
+
+**Repository:** [main](https://git.mysymphony.jp.net/nana/langdash/) / [Gitlab mirror](https://gitlab.com/nanamochizuki77/langdash)
 
 ## Installation
 
 Use [pip](https://pip.pypa.io/en/stable/) to install. By default, langdash does not come preinstalled with any additional modules. You will have to specify what you need like in the following command:
 
 ```
 pip install --user langdash[embeddings,sentence_transformers]
```

### Comparing `langdash-1.1.1a1/README.md` & `langdash-1.2.0a1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 [**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
 
 A simple library for interfacing with language models.
 
 **Currently in alpha!**
 
-Features:
+**Features:**
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends.
 
-Documentation: [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
+**Documentation:** [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
+
+**Repository:** [main](https://git.mysymphony.jp.net/nana/langdash/) / [Gitlab mirror](https://gitlab.com/nanamochizuki77/langdash)
 
 ## Installation
 
 Use [pip](https://pip.pypa.io/en/stable/) to install. By default, langdash does not come preinstalled with any additional modules. You will have to specify what you need like in the following command:
 
 ```
 pip install --user langdash[embeddings,sentence_transformers]
```

### Comparing `langdash-1.1.1a1/langdash/chains.py` & `langdash-1.2.0a1/langdash/chains.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from dataclasses import dataclass
 from collections import OrderedDict
 from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, TYPE_CHECKING, cast
 import re
 import random
 import copy
 import warnings
+from weakref import WeakKeyDictionary
+from math import inf
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
 from langdash.infer import InferArgs
 
 if TYPE_CHECKING:
   from langdash.core import Langdash
   from langdash.llm_session import LLMGenerationSession, LLMState
@@ -179,23 +181,52 @@
     self,
     session: "LLMGenerationSession",
     args: LDNodeArgs = {},
     return_session: bool = False,
     set_global_args: bool = False,
   ) -> Union["LDResult", Tuple["LDResult", "LLMGenerationSession"]]:
     result = LDResult()
+
     for node in self._node_pass(session, args):
       generator = node(session, args)
-      if isinstance(node, (LDReturns, LDChoice)):
-        returns = node._returns
-        result.update_results(returns, self._returns[returns], generator)
+
+      if isinstance(node, LDReturns):
+        text = ""
+        for resp in generator:
+          assert isinstance(resp, RespInfer)
+          text = resp.running_infer
+        result.returns[node._returns] = text
+
+      elif isinstance(node, LDChoice):
+        resp = next(generator)
+        assert isinstance(resp, RespInfer)
+        result.returns[node._returns] = resp.running_infer
+
+        resp = next(generator)
+        assert isinstance(resp, RespInject)
+        result.completion_tokens += resp.tokens_counter
+
       elif isinstance(node, LDRepeat):
-        result.update_results_array(returns, generator)
+        text = ""
+        for resp in generator:
+          assert isinstance(resp, RespInfer)
+          text = resp.running_infer
+          if resp.tokid != -1:
+            result.completion_tokens += 1
+          else:
+            result.returns[key].append(text)
+            text = ""
+
       else:
-        result.update_stats(generator)
+        for resp in generator:
+          if isinstance(resp, RespInject):
+            result.prompt_tokens += resp.tokens_counter
+          else:
+            raise NotImplementedError(resp.__class__.__name__)
+
     if return_session:
       if set_global_args:
         session.global_args = args
       return result, session
     return result
 
   def call(self, ctx: Union[str, "LLMGenerationSession"], **kwargs):
@@ -215,26 +246,26 @@
     Returns:
       (LDResult) The result, or a tuple with (result, session).
     """
     return self._call(session=self._load_session(ctx), **kwargs)
 
 
 @dataclass
-class LDChainCacheState:
+class _LDChainCacheState:
   state: "LLMState"
   skip_nodes: int
 
 
-LDChainCacheStoreDict = OrderedDict[FrozenSet[Tuple[str, Any]],
-                                    LDChainCacheState]
+_LDChainCacheStoreDict = OrderedDict[FrozenSet[Tuple[str, Any]],
+                                     _LDChainCacheState]
 
 
 @dataclass(frozen=True)
 class LDChainCacheStore:
-  _dict: LDChainCacheStoreDict
+  _dict: _LDChainCacheStoreDict
   _model: str
   _model_kwargs: dict
 
 
 class LDChainCached(LDChain):
 
   def __init__(self, model: str, model_kwargs: dict, **kwargs):
@@ -261,15 +292,15 @@
         _arg_first_used_at[k] = self._any_arg_first_use
 
     self._arg_first_used_at: Dict[str, int] = _arg_first_used_at
     self._arg_first_used_at_ordered: List[str] = list(_arg_first_used_at.keys())
     self._arg_first_used_at_ordered.sort(key=lambda k: _arg_first_used_at[k])
 
     # cache session per argument use
-    self._state_cache: LDChainCacheStoreDict = OrderedDict()
+    self._state_cache: _LDChainCacheStoreDict = OrderedDict()
     if len(self._args) == 0:
       self.max_states_to_cache = 1
     else:
       self.max_states_to_cache = min(len(self._args) + 2, 8)
     self._skip_nodes = 0
 
   # State cache functions
@@ -296,41 +327,41 @@
     return LDChainCacheStore(
       _dict=copy.deepcopy(self._state_cache),
       _model=self._model,
       _model_kwargs=copy.deepcopy(self._model_kwargs)
     )
 
   def _set_state_cache(
-    self, key: FrozenSet[Tuple[str, Any]], value: LDChainCacheState
+    self, key: FrozenSet[Tuple[str, Any]], value: _LDChainCacheState
   ):
     self._state_cache[key] = value
     self._update_state_cache(key)
     if len(self._state_cache) > self.max_states_to_cache:
       self._state_cache.popitem(last=True)
 
   def _update_state_cache(self, key: FrozenSet[Tuple[str, Any]]):
     self._state_cache.move_to_end(key, last=False)
 
   def _get_state_cache(
     self, key: FrozenSet[Tuple[str, Any]]
-  ) -> LDChainCacheState:
+  ) -> _LDChainCacheState:
     self._update_state_cache(key)
     return self._state_cache[key]
 
   def _arg_subset_sorted_by_idx(self, args: LDNodeArgs):
     current_subset: LDNodeArgs = {}
     yield current_subset
     for arg in self._arg_first_used_at_ordered:
       current_subset[arg] = args[arg]
       yield current_subset
 
   # Inference functions
 
   def _node_pass(self, session: "LLMGenerationSession", args: LDNodeArgs):
-    last_state_key: Optional[LDChainCacheState] = None
+    last_state_key: Optional[_LDChainCacheState] = None
     for i in range(self._skip_nodes, len(self._nodes)):
       node = self._nodes[i]
       session.tokens_counter = 0
       yield node
       if isinstance(node, LDText) and last_state_key is not None:
         last_state_key.state = session.clone_state()
         last_state_key.skip_nodes = (i + 1)
@@ -345,15 +376,15 @@
           (k, v)
           for k, v in args.items()
           if self._arg_first_used_at[k] <= cached_idx
         )
         if current_keys not in self._state_cache:
           self._set_state_cache(
             current_keys,
-            LDChainCacheState(
+            _LDChainCacheState(
               state=session.clone_state(), skip_nodes=(cached_idx + 1)
             )
           )
         else:
           self._update_state_cache(current_keys)
         last_state_key = self._state_cache[current_keys]
       else:
@@ -376,15 +407,15 @@
     if frozenset() not in self._state_cache:
       text_node = self._nodes[0]
 
       if isinstance(text_node, LDText):
         session.inject(text_node._text)
         self._set_state_cache(
           frozenset(),
-          LDChainCacheState(state=session.clone_state(), skip_nodes=1)
+          _LDChainCacheState(state=session.clone_state(), skip_nodes=1)
         )
         self._skip_nodes = 1
 
       return session
 
     if args is None:
       old_state_cache = self._get_state_cache(frozenset())
@@ -429,66 +460,14 @@
   completion_tokens: int
 
   def __init__(self):
     self.returns = {}
     self.prompt_tokens = 0
     self.completion_tokens = 0
 
-  def update_results(self, key: str, cast_function, generator: LDNodeGenerator):
-    """
-    Update the results with the given key.
-    
-    Args:
-      key (str): The key of the language model.
-      cast_function: The function to cast the results.
-      generator (LDNodeGenerator): Node generator that runs to get the results.
-    """
-    text = ""
-    for resp in generator:
-      if isinstance(resp, RespInfer):
-        text = resp.running_infer
-        if resp.tokid != -1:
-          self.completion_tokens += 1
-      else:
-        raise NotImplementedError(resp.__class__.__name__)
-    self.returns[key] = cast_function(text)
-
-  def update_results_array(self, key: str, generator: LDNodeGenerator):
-    """
-    Appends array in generator to result.
-    
-    Args:
-      key (str): The key of the language model.
-      generator (LDNodeGenerator): Node generator that runs to get the results.
-    """
-    text = ""
-    for resp in generator:
-      if isinstance(resp, RespInfer):
-        text = resp.running_infer
-        if resp.tokid != -1:
-          self.completion_tokens += 1
-        else:
-          self.returns[key].append(text)
-          text = ""
-      else:
-        raise NotImplementedError(resp.__class__.__name__)
-
-  def update_stats(self, generator: LDNodeGenerator):
-    """
-    Update the stats of the result, given a node generator.
-    
-    Args:
-      generator (LDNodeGenerator): Node generator to get the results.
-    """
-    for resp in generator:
-      if isinstance(resp, RespInject):
-        self.prompt_tokens += resp.tokens_counter
-      else:
-        continue
-
 
 class LDNode:
   """ Base class for langdash nodes. """
 
   def __init__(self, ld: "Langdash"):
     self._ld = ld
 
@@ -598,14 +577,20 @@
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       elif respinfer.tokid == -1:  # end
         if self._padleft and respinfer.running_infer.startswith(self._padleft):
           respinfer.running_infer = respinfer.running_infer[len(self._padleft):]
       yield respinfer
 
 
+@dataclass(frozen=True)
+class _LDChoiceTokensCache:
+  choices_tokens: List[List[int]]
+  heal_prefix: str
+
+
 class LDChoice(LDNode):
   """ Choice node """
 
   def __init__(
     self,
     ld: "Langdash",
     returns: str,
@@ -616,72 +601,95 @@
   ):
     super().__init__(ld)
     self._returns = returns
     self._choices = choices
     self._padleft = padleft
     self._padright = padright
     self._argmax = argmax
+
     self._choices_preprocessed = [
       f"{self._padleft}{choice}{self._padright}" for choice in self._choices
     ]
+    self._token_cache: WeakKeyDictionary[
+      str, _LDChoiceTokensCache] = WeakKeyDictionary()
 
   def __repr__(self):
     return f"<Choices {self._returns}>"
 
+  def _get_token_cache(
+    self, session: "LLMGenerationSession", heal_prefix: str
+  ) -> _LDChoiceTokensCache:
+    try:
+      cache = self._token_cache[session]
+      if cache.heal_prefix == heal_prefix:
+        return cache
+    except KeyError:
+      pass
+    cache = _LDChoiceTokensCache(
+      choices_tokens=[
+        session.tokenize(heal_prefix + text)
+        for text in self._choices_preprocessed
+      ],
+      heal_prefix=heal_prefix
+    )
+    self._token_cache[session] = cache
+    return cache
+
   def __call__(
     self, session: "LLMGenerationSession", args: LDNodeArgs
   ) -> LDNodeGenerator:
     from langdash.llm_session import LLMGenerationSessionForRawText
 
-    tokids = [-1] * len(self._choices_preprocessed)
-    has_multiple_tokens = False
-
-    heal_padleft: Optional[str] = None
+    heal_prefix: str = ""
     if session.token_healing and \
       isinstance(session, LLMGenerationSessionForRawText) and \
       session._next_token is not None:
-      heal_padleft = session._next_token[1]
+      heal_prefix = session._next_token[1]
       session._next_token = None
 
-    for i, text in enumerate(self._choices_preprocessed):
-      if heal_padleft is not None:
-        text_tokids = session.tokenize(heal_padleft + text)
-      else:
-        text_tokids = session.tokenize(text)
-      if len(text_tokids) > 1:
-        has_multiple_tokens = True
-        break
-      tokids[i] = text_tokids[0]
-
-    if has_multiple_tokens:
-      # TODO: handle multiple tokens
-      raise NotImplementedError("handle multiple tokens not implemented")
-    else:
+    cache = self._get_token_cache(session, heal_prefix)
+    choices_tokens: List[Tuple[int, List[int]]] = [
+      (i, list(reversed(tokens)))
+      for i, tokens in enumerate(cache.choices_tokens)
+    ]
+
+    while len(choices_tokens) > 1:
       probs = session.next_token_probs()
-      weights = [probs[tokid] for tokid in tokids]
+
       if self._argmax:
-        inject_idx = self._choices.index(max(self._choices))
+        tokid = -1
+        tokid_prob = -inf
+        for _, tokens in choices_tokens:
+          cur_tokid = tokens[-1]
+          if probs[cur_tokid] > tokid_prob:
+            tokid = cur_tokid
+            tokid_prob = probs[cur_tokid]
       else:
-        inject_idx = random.choices(
-          range(len(self._choices)), weights=weights
-        )[0]
-      tokid_inject = tokids[inject_idx]
-      session.inject(tokid_inject)
-      tokstr = self._choices[inject_idx]
-      yield RespInfer(
-        tokid=tokid_inject,
-        tokstr=tokstr,
-        running_infer=tokstr,
-      )
-      # for parity with RespInfer
-      yield RespInfer(
-        tokid=-1,
-        tokstr="",
-        running_infer=tokstr,
-      )
+        cur_choice_tokens = []
+        cur_choice_weights = []
+        for _, tokens in choices_tokens:
+          tokid = tokens[-1]
+          cur_choice_tokens.append(tokid)
+          cur_choice_weights.append(probs[tokid])
+        tokid = random.choices(cur_choice_tokens, weights=cur_choice_weights)[0]
+
+      session.inject(tokid)
+
+      old_choices_tokens = choices_tokens
+      choices_tokens = []
+      for i, tokens in old_choices_tokens:
+        if tokens[-1] == tokid:
+          tokens.pop()
+          choices_tokens.append((i, tokens))
+
+    choice, remaining = choices_tokens.pop()
+    for tokid in reversed(remaining):
+      session.inject(tokid)
+    yield RespInfer(-1, "", self._choices[choice])
+    yield RespInject(tokens_counter=len(cache.choices_tokens[choice]))
 
 
 class LDRepeat(LDNode):
   """ Repeat node """
 
   def __init__(
     self,
```

### Comparing `langdash-1.1.1a1/langdash/classify/token_qa.py` & `langdash-1.2.0a1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/core.py` & `langdash-1.2.0a1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/infer.py` & `langdash-1.2.0a1/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/llm.py` & `langdash-1.2.0a1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/llm_session.py` & `langdash-1.2.0a1/langdash/llm_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,20 @@
       (List[int]) The list of tokens.
     """
     raise NotImplementedError("tokenize")
 
   def decode(self, tokids: List[int]) -> str:
     raise NotImplementedError("decode")
 
+  def next_token_logits(self) -> List[float]:
+    """
+    Returns the logits for next token.
+    """
+    raise NotImplementedError("next_token_logits")
+
   def next_token_probs(self) -> List[float]:
     """
     Returns the probabilities for next token.
     """
     raise NotImplementedError("next_token_probs")
 
   def flush_token(self):
@@ -129,22 +135,22 @@
 
   def infer(
     self,
     end: Optional[Union[str, int]],
     args: Optional[InferArgs] = None
   ) -> Generator[RespInfer, None, None]:
     """
-    Infer the next token from the input sequence.
+    Infer the next tokens from the input sequence.
 
     Args:
       end (Optional[Union[str, int]]):
         The end of the output sequence.
         If set to None, the output sequence will be generated until the maximum number of tokens is reached.
       args (Optional[InferArgs]):
-        Optionak inference parameters.
+        Optional inference parameters.
         
     Returns:
       Inference response
     """
     if not args:
       args = self.default_infer_args
     yield from self._infer(end, args)
```

### Comparing `langdash-1.1.1a1/langdash/models/_bpe.py` & `langdash-1.2.0a1/langdash/models/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/models/llama_cpp.py` & `langdash-1.2.0a1/langdash/models/llama_cpp.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,23 +86,29 @@
 
   def _eval(self, token: int):
     return self._llama.eval([token])
 
   def _eval_mult(self, tokens: List[int]):
     return self._llama.eval(tokens)
 
-  def next_token_probs(self):
+  def _next_token_logits_raw(self):
     self._llama.enter_session(self)
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       logits = self._eval(self._next_token[0])
-    return sampling.logits_to_probs(logits).tolist()
+    return logits
+
+  def next_token_logits(self) -> List[float]:
+    return self._next_token_logits_raw().tolist()
+
+  def next_token_probs(self) -> List[float]:
+    return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def set_state(self, state: Optional[LlamaState]):
     self._llama.set_state(self, state)
     if state == None:
       self._logits = None
     else:
       self._logits = self._llama.load_logits_from_llama()
```

### Comparing `langdash-1.1.1a1/langdash/models/mock.py` & `langdash-1.2.0a1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/models/rwkv_cpp.py` & `langdash-1.2.0a1/langdash/models/rwkv_cpp.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,90 +9,121 @@
 from langdash.infer import InferArgs
 import langdash.sampling as sampling
 import langdash.models._bpe as bpe
 
 import os
 import sys
 import torch
-import pathlib
+import tokenizers
 
 _rwkv_lib: Optional[str] = None
+_rwkv_cpp_folder: Optional[str] = None
 
-RWKV_CPP_COMMIT = "9e2a0de8436a956c5ef80fbd5f4184311a7a568d"
+RWKV_CPP_COMMIT_DEFAULT = "82c4ac78f4d10ef1af87104fc051ea2119eaaddf"
+RWKV_CPP_COMMIT = os.environ.get(
+  "LANGDASH_RWKV_CPP_COMMIT", RWKV_CPP_COMMIT_DEFAULT
+)
+RWKV_CPP_FORCE_RECOMPILE = os.environ.get(
+  "LANGDASH_RWKV_FORCE_RECOMPILE", ""
+) == "1"
 
 
 def _load_rwkv_import():
-  global _rwkv_lib
+  global _rwkv_lib, _rwkv_cpp_folder
 
   import subprocess
   import shutil
 
   import langdash
-  rwkv_cpp_folder = os.path.join(
+  _rwkv_cpp_folder = os.path.join(
     os.path.dirname(langdash.__file__), "extern/rwkv.cpp"
   )
 
-  if not os.path.isdir(rwkv_cpp_folder):
+  force_recompile = RWKV_CPP_FORCE_RECOMPILE
+
+  git = shutil.which("git")
+
+  if not os.path.isdir(_rwkv_cpp_folder):
     print("rwkv.cpp isn't installed, clone and install? (requires git, cmake)")
     do_install = input("Type 'y' (without quotes) to install: ") == "y"
     if not do_install:
       raise ImportError("rwkv.cpp is not installed")
-
-    os.makedirs(rwkv_cpp_folder, exist_ok=True)
-    git = shutil.which("git")
     if git is None:
       raise ImportError("git is needed for compiling rwkv.cpp")
+
+    os.makedirs(_rwkv_cpp_folder, exist_ok=True)
+
     subprocess.check_call(
       [
         git, "clone", "--recursive", "https://github.com/saharNooby/rwkv.cpp",
-        rwkv_cpp_folder
+        _rwkv_cpp_folder
       ]
     )
     subprocess.check_call(
-      [git, "checkout", RWKV_CPP_COMMIT], cwd=rwkv_cpp_folder
+      [git, "checkout", RWKV_CPP_COMMIT], cwd=_rwkv_cpp_folder
     )
-    subprocess.check_call([git, "submodule", "update"], cwd=rwkv_cpp_folder)
+    subprocess.check_call([git, "submodule", "update"], cwd=_rwkv_cpp_folder)
+
+  elif git is not None:
+    current_commit = subprocess.check_output(
+      [git, "rev-parse", "HEAD"], cwd=_rwkv_cpp_folder, encoding="utf-8"
+    ).strip()
+    if current_commit != RWKV_CPP_COMMIT:
+      subprocess.check_call(
+        [git, "pull", "origin", "master"], cwd=_rwkv_cpp_folder
+      )
+      subprocess.check_call(
+        [git, "checkout", RWKV_CPP_COMMIT], cwd=_rwkv_cpp_folder
+      )
+      subprocess.check_call([git, "submodule", "update"], cwd=_rwkv_cpp_folder)
+      force_recompile = True
+
+  if force_recompile:
+    os.unlink(os.path.join(_rwkv_cpp_folder, "CMakeCache.txt"))
 
   if "win32" in sys.platform or "cygwin" in sys.platform:
     file_name = "rwkv.dll"
   elif "darwin" in sys.platform:
     file_name = "librwkv.dylib"
   else:
     file_name = "librwkv.so"
 
-  _rwkv_lib = os.path.join(rwkv_cpp_folder, file_name)
+  _rwkv_lib = os.path.join(_rwkv_cpp_folder, file_name)
 
-  if not os.path.isfile(_rwkv_lib):
+  if force_recompile or not os.path.isfile(_rwkv_lib):
     cmake = shutil.which("cmake")
     if cmake is None:
       raise ImportError("cmake is needed for compiling rwkv.cpp")
-    subprocess.check_call([cmake, "."], cwd=rwkv_cpp_folder)
+    subprocess.check_call([cmake, "."], cwd=_rwkv_cpp_folder)
     subprocess.check_call(
-      [cmake, "--build", ".", "--config", "Release"], cwd=rwkv_cpp_folder
+      [cmake, "--build", ".", "--config", "Release"], cwd=_rwkv_cpp_folder
     )
-  sys.path.append(os.path.join(rwkv_cpp_folder, "rwkv"))
+
+  sys.path.insert(0, os.path.join(_rwkv_cpp_folder, "rwkv"))
 
 
 _load_rwkv_import()
 
-import tokenizers  # type: ignore
 import rwkv_cpp_model  # type: ignore
 import rwkv_cpp_shared_library  # type: ignore
+import rwkv_tokenizer  # type: ignore
+
+sys.path.pop(0)
 
 
 @dataclass
 class RwkvCppState(LLMState):
   _logits: Optional[torch.Tensor] = None
   _state: Optional[torch.Tensor] = None
   _next_token: Optional[Tuple[int, str]] = None
 
 
 @dataclass
 class RwkvCppExtras:
-  tokenizer: tokenizers.Tokenizer
+  tokenizer: Union[tokenizers.Tokenizer, rwkv_tokenizer.TRIE_TOKENIZER]
   vocab: Dict[str, int]
 
 
 class RwkvCppSession(
   LLMGenerationSessionForRawText["RwkvCppModel", RwkvCppState, torch.Tensor]
 ):
   """
@@ -106,15 +137,20 @@
     super().__init__(*args, **kwargs)
 
     def load_model(llm: RwkvCppModel):
       assert _rwkv_lib is not None
       model = rwkv_cpp_model.RWKVModel(
         rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path
       )
-      tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
+      if llm._tokenizer_type == "20B":
+        tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
+      elif llm._tokenizer_type == "world":
+        tokenizer = rwkv_tokenizer.TRIE_TOKENIZER(llm._tokenizer_path)
+      else:
+        raise ValueError(f"unknown tokenizer type {llm._tokenizer_type}")
       extras = RwkvCppExtras(
         tokenizer=tokenizer,
         vocab={
           bpe.decode(logits_tokstr): logits_tokid
           for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
         }
       )
@@ -150,22 +186,28 @@
     return self._extras.tokenizer.encode(
       text, add_special_tokens=add_special_tokens
     ).ids
 
   def decode(self, tokids: List[int]) -> str:
     return self._extras.tokenizer.decode(tokids)
 
-  def next_token_probs(self) -> List[float]:
+  def _next_token_logits_raw(self):
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       logits, _ = self._rwkv.eval(self._next_token[0], self._state)
-    return sampling.logits_to_probs(logits).tolist()
+    return logits
+
+  def next_token_logits(self) -> List[float]:
+    return self._next_token_logits_raw().tolist()
+
+  def next_token_probs(self) -> List[float]:
+    return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def _infer(self, end: Optional[Union[str, int]],
              args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
 
@@ -244,24 +286,38 @@
 class RwkvCppModel(LLM[RwkvCppSession]):
   """
   rwkv.cpp model
   """
 
   Session = RwkvCppSession
 
-  def __init__(self, model_path: str, tokenizer_path: Optional[str] = None):
+  def __init__(
+    self,
+    model_path: str,
+    tokenizer_path: Optional[str] = None,
+    tokenizer_type: str = "20B"
+  ):
     """
     Creates a template for the RWKV language model (using the rwkv.cpp library).
     
     Args:
       model_path (str): Path to the model file.
       tokenizer_path (Optional[str]):
         Path to the tokenizer file.
-        If None is given, the tokenizer is assumed to be the model_path / '20B_tokenizer.json'.
+        If None is given, the built-in tokenizer will be used.
+      tokenizer_type (str):
+        Either `"world"` or `"20B"`.
     """
     self._model_path = model_path
+    self._tokenizer_type = tokenizer_type
     if tokenizer_path is None:
+      builtin_tokenizer_paths = {
+        "world": "rwkv/rwkv_vocab_v20230424.txt",
+        "20B": "rwkv/20B_tokenizer.json",
+      }
       self._tokenizer_path = str(
-        pathlib.Path(os.path.abspath(model_path)).parent / "20B_tokenizer.json"
+        os.path.join(
+          _rwkv_cpp_folder, builtin_tokenizer_paths[self._tokenizer_type]
+        )
       )
     else:
       self._tokenizer_path = tokenizer_path
```

### Comparing `langdash-1.1.1a1/langdash/models/sentence_transformers.py` & `langdash-1.2.0a1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/models/transformers.py` & `langdash-1.2.0a1/langdash/models/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,14 @@
     self._model, self._extras = self._ld._get_model_internal(
       self._llm, load_model
     )
     self._logits = None
     self._state = None
     self._next_token = None
 
-  def _heal_token(self, tok_a: int, tok_b: int) -> str:
-    return self._extras.tokenizer.decode([tok_a, tok_b])
-
   def set_state(self, state: Optional[TransformersState]):
     if state is None:
       self._logits = None
       self._state = None
       self._next_token = None
     else:
       self._logits = copy.deepcopy(state._logits)
@@ -127,15 +124,15 @@
     return self._extras.tokenizer.decode(tokids)
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     return self._extras.tokenizer.encode(
       text, add_special_tokens=add_special_tokens
     ).tolist()
 
-  def next_token_probs(self):
+  def _next_token_logits_raw(self):
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       if model_is_rwkv(self._model):
         logits = self._model.forward(
@@ -145,15 +142,21 @@
         )._logits[-1]
       else:
         logits = self._model.forward(
           torch.IntTensor([self._next_token[0]]),
           past_key_values=self._state,
           use_cache=True
         )._logits[-1]
-    return sampling.logits_to_probs(logits).tolist()
+    return logits
+
+  def next_token_logits(self) -> List[float]:
+    return self._next_token_logits_raw().tolist()
+
+  def next_token_probs(self) -> List[float]:
+    return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def _infer(self, end: Optional[Union[str, int]],
              args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
     stops_at_eot = (
```

### Comparing `langdash-1.1.1a1/langdash/response.py` & `langdash-1.2.0a1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/sampling.py` & `langdash-1.2.0a1/langdash/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,8 +83,8 @@
   """
   probs = _output_probs(*args, **kwargs)
   return int(torch.multinomial(probs, num_samples=1)[0])
 
 
 def logits_to_probs(logits: torch.Tensor):
   """ Converts logit tensor to probability tensor using softmax. """
-  return torch.nn.functional.softmax(logits, dim=-1)
+  return F.softmax(logits, dim=-1)
```

### Comparing `langdash-1.1.1a1/langdash/search/embedding_search.py` & `langdash-1.2.0a1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/search/engine.py` & `langdash-1.2.0a1/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash/search/multichoice_search.py` & `langdash-1.2.0a1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/langdash.egg-info/PKG-INFO` & `langdash-1.2.0a1/langdash.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.1.1a1
+Version: 1.2.0a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -26,22 +26,24 @@
 
 [**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
 
 A simple library for interfacing with language models.
 
 **Currently in alpha!**
 
-Features:
+**Features:**
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends.
 
-Documentation: [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
+**Documentation:** [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
+
+**Repository:** [main](https://git.mysymphony.jp.net/nana/langdash/) / [Gitlab mirror](https://gitlab.com/nanamochizuki77/langdash)
 
 ## Installation
 
 Use [pip](https://pip.pypa.io/en/stable/) to install. By default, langdash does not come preinstalled with any additional modules. You will have to specify what you need like in the following command:
 
 ```
 pip install --user langdash[embeddings,sentence_transformers]
```

### Comparing `langdash-1.1.1a1/langdash.egg-info/SOURCES.txt` & `langdash-1.2.0a1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.1.1a1/setup.py` & `langdash-1.2.0a1/setup.py`

 * *Files identical despite different names*

