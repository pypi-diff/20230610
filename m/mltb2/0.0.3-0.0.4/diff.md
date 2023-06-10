# Comparing `tmp/mltb2-0.0.3.tar.gz` & `tmp/mltb2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.0.3.tar", last modified: Tue Jun  6 09:57:04 2023, max compression
+gzip compressed data, was "dist/mltb2-0.0.4.tar", last modified: Sat Jun 10 12:39:25 2023, max compression
```

## Comparing `mltb2-0.0.3.tar` & `mltb2-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-06 09:56:55.000000 mltb2-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 09:56:55.000000 mltb2-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 09:57:04.926392 mltb2-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-06 09:56:55.000000 mltb2-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-06 09:56:55.000000 mltb2-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-06 09:57:04.926392 mltb2-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-06 09:56:55.000000 mltb2-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-10 12:39:14.000000 mltb2-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-10 12:39:14.000000 mltb2-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-10 12:39:25.000000 mltb2-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-10 12:39:14.000000 mltb2-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-10 12:39:14.000000 mltb2-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-10 12:39:25.000000 mltb2-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-10 12:39:14.000000 mltb2-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_transformers.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mltb2-0.0.3/LICENSE` & `mltb2-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.3/PKG-INFO` & `mltb2-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
 Project-URL: Source Code, https://github.com/telekom/mltb2
 Keywords: optuna deep-learning ml ai machine-learning hyperparameter-optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: checking
 Provides-Extra: optional
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `mltb2-0.0.3/README.md` & `mltb2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.3/mltb2/optuna.py` & `mltb2-0.0.4/mltb2/optuna.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Copyright (c) 2021 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""Optuna only functionality."""
+"""Optuna specific functionality.
+
+This module is based on `Optuna <https://optuna.readthedocs.io/en/stable/>`_.
+"""
+
 
 import logging
 
 import numpy as np
 import optuna
 from optuna.pruners import BasePruner
 from optuna.study import StudyDirection
```

### Comparing `mltb2-0.0.3/mltb2/plot.py` & `mltb2-0.0.4/mltb2/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Copyright (c) 2018 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""A collection of plot tools."""
+"""A collection of plot tools.
+
+This module is based on `Matplotlib <https://matplotlib.org/>`_.
+"""
 
 from typing import Optional
 
 import matplotlib.pyplot as plt
 
 
 # see https://matplotlib.org/api/_as_gen/matplotlib.axes.Axes.twinx.html
```

### Comparing `mltb2-0.0.3/mltb2/somajo.py` & `mltb2-0.0.4/mltb2/somajo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""SoMaJo tools."""
+"""SoMaJo specific functionality.
+
+This module is based on `SoMaJo <https://github.com/tsproisl/SoMaJo>`_.
+"""
 
 
 from dataclasses import dataclass, field
 from typing import List, Set
 
 from somajo import SoMaJo
-from tqdm.auto import tqdm
+from tqdm import tqdm
 
 
 @dataclass
 class SoMaJoSentenceSplitter:
     """Use SoMaJo to split text into sentences.
 
     Args:
         language: The language. ``de_CMC`` for German or ``en_PTB`` for English.
         show_progress_bar: Show a progressbar during processing.
     """
 
     language: str
     somajo: SoMaJo = field(init=False, repr=False)
-    show_progress_bar: bool = True
+    show_progress_bar: bool = False
 
     def __post_init__(self):
         """Do post init."""
         self.somajo = SoMaJo(self.language)
 
     # see https://github.com/tsproisl/SoMaJo/issues/17
     @staticmethod
```

### Comparing `mltb2-0.0.3/mltb2/somajo_transformers.py` & `mltb2-0.0.4/mltb2/somajo_transformers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # Copyright (c) 2023 Philip May
 # Copyright (c) 2023 Philip May, Deutsche Telekom AG
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""SoMaJo and Transformers tools."""
+"""Hugging Face Transformers and SoMaJo specific functionality.
+
+This module is based on
+`Hugging Face Transformers <https://huggingface.co/docs/transformers/index>`_ and
+`SoMaJo <https://github.com/tsproisl/SoMaJo>`_.
+"""
 
 
 from dataclasses import dataclass
 from typing import List
 
-from tqdm.auto import tqdm
+from tqdm import tqdm
 
 from mltb2.somajo import SoMaJoSentenceSplitter
 from mltb2.transformers import TransformersTokenCounter
 
 
 @dataclass
 class TextSplitter:
@@ -24,21 +29,21 @@
     Args:
         max_token: Maximum number of tokens per text section.
         somajo_sentence_splitter: The sentence splitter to be used.
         transformers_token_counter: The token counter to be used.
         show_progress_bar: Show a progressbar during processing.
         ignore_overly_long_sentences: If this is ``False`` an ``ValueError`` exception is
             raised if a sentence is longer than ``max_token``.
-            If it is true, then the sentence is simply ignored.
+            If it is ``True``, then the sentence is simply ignored.
     """
 
     max_token: int
     somajo_sentence_splitter: SoMaJoSentenceSplitter
     transformers_token_counter: TransformersTokenCounter
-    show_progress_bar: bool = True
+    show_progress_bar: bool = False
     ignore_overly_long_sentences: bool = False
 
     def __call__(self, text: str) -> List[str]:
         """Split the text into sections.
 
         Args:
             text: The text to be split.
```

### Comparing `mltb2-0.0.3/mltb2/transformers.py` & `mltb2-0.0.4/mltb2/transformers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""Transformers tools."""
+"""Hugging Face Transformers specific functionality.
+
+This module is based on
+`Hugging Face Transformers <https://huggingface.co/docs/transformers/index>`_.
+"""
 
 import os
 from dataclasses import dataclass, field
 from typing import Iterable, List, Union
 
 import sklearn
 import torch
-from tqdm.auto import tqdm
+from tqdm import tqdm
 from transformers import AutoTokenizer
 from transformers.tokenization_utils import PreTrainedTokenizerBase
 
 
 @dataclass
 class TransformersTokenCounter:
     """Count Transformers tokenizer tokens.
@@ -24,15 +28,15 @@
             The *model id* of a tokenizer hosted inside a model repo on huggingface.co or
             a path to a *directory* containing a tokenizer.
         show_progress_bar: Show a progressbar during processing.
     """
 
     pretrained_model_name_or_path: Union[str, os.PathLike]
     tokenizer: PreTrainedTokenizerBase = field(init=False, repr=False)
-    show_progress_bar: bool = True
+    show_progress_bar: bool = False
 
     def __post_init__(self):
         """Do post init."""
         self.tokenizer = AutoTokenizer.from_pretrained(self.pretrained_model_name_or_path)
 
     def __call__(self, text: Union[str, Iterable]) -> Union[int, List[int]]:
         """Count tokens for text.
```

### Comparing `mltb2-0.0.3/mltb2.egg-info/PKG-INFO` & `mltb2-0.0.4/mltb2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
 Project-URL: Source Code, https://github.com/telekom/mltb2
 Keywords: optuna deep-learning ml ai machine-learning hyperparameter-optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: checking
 Provides-Extra: optional
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `mltb2-0.0.3/pyproject.toml` & `mltb2-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 line-length = 99
-target-version = ["py38"]
+target-version = ["py37"]
 
 [tool.isort]
 profile = "black"
 lines_after_imports = 2
 line_length = 99
 
 [tool.pylint."MASTER"]
```

### Comparing `mltb2-0.0.3/setup.py` & `mltb2-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,24 @@
         "isort",
         "mdformat",
         "pydocstyle",
         "mypy",
         "pylint",
         "pylintfileheader",
     ],
-    "optional": ["optuna", "SoMaJo", "transformers", "torch", "scikit-learn", "matplotlib"],
+    "optional": [
+        "optuna",
+        "SoMaJo",
+        "transformers",
+        "torch",
+        "scikit-learn",
+        "matplotlib",
+        "platformdirs",
+        "fasttext-wheel",
+    ],
     "testing": ["pytest", "packaging"],
     "doc": ["sphinx", "sphinx_rtd_theme", "myst_parser", "sphinx_copybutton"],
 }
 
 # add "all"
 all_extra_packages = list(
     {package_name for value in extras_require.values() for package_name in value}
@@ -63,31 +72,32 @@
         "Bug Tracker": source_code + "/issues",
         "Documentation": "https://telekom.github.io/mltb2/",
         "Source Code": source_code,
         # "Contributing": source_code + "/blob/main/CONTRIBUTING.md",
         # "Code of Conduct": source_code + "/blob/main/CODE_OF_CONDUCT.md",
     },
     packages=setuptools.find_packages(),
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     install_requires=install_requires,
     extras_require=extras_require,
     keywords=keywords,
     classifiers=[
         "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
         # "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         # "Intended Audience :: Education",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        # "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `mltb2-0.0.3/tests/test_optuna.py` & `mltb2-0.0.4/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.3/tests/test_somajo.py` & `mltb2-0.0.4/tests/test_somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.3/tests/test_somajo_transformers.py` & `mltb2-0.0.4/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.3/tests/test_transformers.py` & `mltb2-0.0.4/tests/test_transformers.py`

 * *Files identical despite different names*

