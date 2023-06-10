# Comparing `tmp/convert_labse_tf_pt-2.4.2.tar.gz` & `tmp/convert_labse_tf_pt-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_labse_tf_pt-2.4.2.tar", max compression
+gzip compressed data, was "convert_labse_tf_pt-3.0.0.tar", max compression
```

## Comparing `convert_labse_tf_pt-2.4.2.tar` & `convert_labse_tf_pt-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-22 07:55:36.197878 convert_labse_tf_pt-2.4.2/LICENSE
--rw-r--r--   0        0        0     1384 2023-05-22 07:55:36.197878 convert_labse_tf_pt-2.4.2/README.md
--rw-r--r--   0        0        0     1230 2023-05-22 07:55:36.197878 convert_labse_tf_pt-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      314 2023-05-22 07:55:36.197878 convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-22 07:55:36.197878 convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/configurations.py
--rw-r--r--   0        0        0    18562 2023-05-22 07:55:36.197878 convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/convert.py
--rw-r--r--   0        0        0  5220781 2023-05-22 07:55:36.249881 convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt
--rw-r--r--   0        0        0  1469057 2023-05-22 07:55:36.261882 convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt
--rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 convert_labse_tf_pt-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-10 08:09:16.190973 convert_labse_tf_pt-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2559 2023-06-10 08:09:16.190973 convert_labse_tf_pt-3.0.0/README.md
+-rw-r--r--   0        0        0     1265 2023-06-10 08:09:16.194973 convert_labse_tf_pt-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      314 2023-06-10 08:09:16.194973 convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/__init__.py
+-rw-r--r--   0        0        0     2080 2023-06-10 08:09:16.194973 convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/configurations.py
+-rw-r--r--   0        0        0    18744 2023-06-10 08:09:16.194973 convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/convert.py
+-rw-r--r--   0        0        0  5220781 2023-06-10 08:09:16.234973 convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt
+-rw-r--r--   0        0        0  1469057 2023-06-10 08:09:16.242973 convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt
+-rw-r--r--   0        0        0     3540 1970-01-01 00:00:00.000000 convert_labse_tf_pt-3.0.0/PKG-INFO
```

### Comparing `convert_labse_tf_pt-2.4.2/LICENSE` & `convert_labse_tf_pt-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.2/README.md` & `convert_labse_tf_pt-3.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # LaBSE
 
 ## Project
 
-This project is an implementation to convert Google's [LaBSE](https://tfhub.dev/google/LaBSE/2) model from TensorFlow to PyTorch. It also offers extensions to convert the [smaller-LaBSE model](https://tfhub.dev/jeongukjae/smaller_LaBSE_15lang/1) from TensorFlow to PyTorch.
+This project is an implementation to convert Google's [LaBSE](https://tfhub.dev/google/LaBSE/2) model from TensorFlow to PyTorch. It also offers extensions to convert the [smaller-LaBSE model](https://tfhub.dev/jeongukjae/smaller_LaBSE_15lang/1) from TensorFlow to PyTorch, and the [LEALLA family](https://tfhub.dev/google/collections/LEALLA/1) of models.
 
-The models are uploaded to the [HuggingFace Model Hub](https://huggingface.co/setu4993/) in the PyTorch, HF-compatible TensorFlow and Flax formats, alongwith a compatible tokenizer.
+The models are uploaded to the [HuggingFace Model Hub](https://huggingface.co/setu4993/) in the PyTorch HF-compatible (original and `safetensors`), TensorFlow and Flax formats, alongwith a compatible tokenizer.
 
 - [LaBSE](https://huggingface.co/setu4993/LaBSE)
 - [smaller-LaBSE](https://huggingface.co/setu4993/smaller-LaBSE)
+- [LEALLA-base](https://huggingface.co/setu4993/LEALLA-base)
+- [LEALLA-small](https://huggingface.co/setu4993/LEALLA-small)
+- [LEALLA-large](https://huggingface.co/setu4993/LEALLA-large)
 
 ## Export
 
 To convert and export the models:
 
 ```shell
 poetry install
@@ -24,17 +27,25 @@
 # Clone the already uploaded models.
 cd /path/to/model
 git clone https://huggingface.co/setu4993/LaBSE.git
 
 # Export models anew and update.
 cd /path/to/repo
 poetry install
-poetry run convert_labse --output_path /path/to/model/LaBSE --huggingface_path
+poetry run convert_labse --output_path /path/to/models/LaBSE --huggingface_path
 ```
 
+### Export Commands by Model
+
+1. [LaBSE](https://huggingface.co/setu4993/LaBSE): `poetry run convert_labse --output_path /path/to/models/setu4993/LaBSE --huggingface_path`
+2. [smaller-LaBSE](https://huggingface.co/setu4993/smaller-LaBSE): `poetry run convert_labse --output_path /path/to/models/setu4993/smaller-LaBSE --smaller --huggingface_path`
+3. [LEALLA-base](https://huggingface.co/setu4993/LEALLA-base): `poetry run convert_lealla --size base --output_path /path/to/models/setu4993/LEALLA-base --huggingface_path`
+4. [LEALLA-small](https://huggingface.co/setu4993/LEALLA-small): `poetry run convert_lealla --size small --output_path /path/to/models/setu4993/LEALLA-small --huggingface_path`
+5. [LEALLA-large](https://huggingface.co/setu4993/LEALLA-large): `poetry run convert_lealla --size large --output_path /path/to/models/setu4993/LEALLA-large --huggingface_path`
+
 ## Model Cards
 
 See the [`model-cards` directory](https://github.com/setu4993/convert-labse-tf-pt/tree/main/model-cards) for a copy of the model cards.
 
 ## License
 
 This repository and the conversion code is licensed under the MIT license, but the **model** is distributed with an Apache-2.0 license.
```

### Comparing `convert_labse_tf_pt-2.4.2/pyproject.toml` & `convert_labse_tf_pt-3.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "convert-labse-tf-pt"
-version = "2.4.2"
+version = "3.0.0"
 description = "Convert LaBSE model from TensorFlow to PyTorch."
 license = "MIT"
 authors = ["Setu Shah <setu+labse@setu.me>"]
 readme = "README.md"
 homepage = "https://github.com/setu4993/convert-labse-tf-pt"
 repository = "https://github.com/setu4993/convert-labse-tf-pt"
 keywords = ["transformers", "bert", "labse", "pytorch", "tensorflow"]
 packages = [{ include = "convert_labse_tf_pt", from = "src" }]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
-transformers = { extras = ["flax", "sentencepiece", "torch", "tf"], version = "^4.29.0" }
+transformers = { extras = ["flax", "sentencepiece", "torch", "tf"], version = "^4.29.2,<4.30.0" }
 tensorflow-hub = "^0.12.0"
 ipywidgets = "^7.6.3"
 loguru = "^0.6.0"
+tensorflow-text = "<2.9.0"
 safetensors = "^0.3.1"
 
 [tool.poetry.scripts]
 convert_labse = "convert_labse_tf_pt.convert:convert_labse"
 convert_lealla = "convert_labse_tf_pt.convert:convert_lealla"
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/configurations.py` & `convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/configurations.py`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/convert.py` & `convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 """
 from argparse import ArgumentParser
 from pathlib import Path
 from re import match
 from typing import List, Tuple, Union
 
 import tensorflow_text  # noqa: F401
-import torch.nn.functional as F
 from loguru import logger
+from numpy import ndarray
+from numpy.linalg import norm
 from tensorflow_hub import load
 from torch import from_numpy, matmul, no_grad
+from torch.nn.functional import normalize
 from transformers import (
     BertConfig,
     BertModel,
     BertTokenizerFast,
     FlaxBertModel,
     PretrainedConfig,
     TFBertModel,
@@ -390,17 +392,21 @@
 
     tokenized = tokenizer(sentences, return_tensors="pt", padding="max_length", truncation=True)
     with no_grad():
         output = model(**tokenized)
     return output
 
 
+def l2_normalize_numpy_array(array: ndarray) -> ndarray:
+    return array / norm(array, ord=2, axis=1).reshape(-1, 1)
+
+
 def similarity(embeddings_1, embeddings_2):
-    normalized_embeddings_1 = F.normalize(embeddings_1, p=2)
-    normalized_embeddings_2 = F.normalize(embeddings_2, p=2)
+    normalized_embeddings_1 = normalize(embeddings_1, p=2)
+    normalized_embeddings_2 = normalize(embeddings_2, p=2)
     return matmul(normalized_embeddings_1, normalized_embeddings_2.transpose(0, 1))
 
 
 def get_base_arg_parser() -> ArgumentParser:
     parser = ArgumentParser()
     parser.add_argument(
         "--tf_saved_model",
```

### Comparing `convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt` & `convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.2/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt` & `convert_labse_tf_pt-3.0.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.2/PKG-INFO` & `convert_labse_tf_pt-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-labse-tf-pt
-Version: 2.4.2
+Version: 3.0.0
 Summary: Convert LaBSE model from TensorFlow to PyTorch.
 Home-page: https://github.com/setu4993/convert-labse-tf-pt
 License: MIT
 Keywords: transformers,bert,labse,pytorch,tensorflow
 Author: Setu Shah
 Author-email: setu+labse@setu.me
 Requires-Python: >=3.8,<3.11
@@ -13,28 +13,32 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ipywidgets (>=7.6.3,<8.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: safetensors (>=0.3.1,<0.4.0)
 Requires-Dist: tensorflow-hub (>=0.12.0,<0.13.0)
-Requires-Dist: transformers[flax,sentencepiece,tf,torch] (>=4.29.0,<5.0.0)
+Requires-Dist: tensorflow-text (<2.9.0)
+Requires-Dist: transformers[flax,sentencepiece,tf,torch] (>=4.29.2,<4.30.0)
 Project-URL: Repository, https://github.com/setu4993/convert-labse-tf-pt
 Description-Content-Type: text/markdown
 
 # LaBSE
 
 ## Project
 
-This project is an implementation to convert Google's [LaBSE](https://tfhub.dev/google/LaBSE/2) model from TensorFlow to PyTorch. It also offers extensions to convert the [smaller-LaBSE model](https://tfhub.dev/jeongukjae/smaller_LaBSE_15lang/1) from TensorFlow to PyTorch.
+This project is an implementation to convert Google's [LaBSE](https://tfhub.dev/google/LaBSE/2) model from TensorFlow to PyTorch. It also offers extensions to convert the [smaller-LaBSE model](https://tfhub.dev/jeongukjae/smaller_LaBSE_15lang/1) from TensorFlow to PyTorch, and the [LEALLA family](https://tfhub.dev/google/collections/LEALLA/1) of models.
 
-The models are uploaded to the [HuggingFace Model Hub](https://huggingface.co/setu4993/) in the PyTorch, HF-compatible TensorFlow and Flax formats, alongwith a compatible tokenizer.
+The models are uploaded to the [HuggingFace Model Hub](https://huggingface.co/setu4993/) in the PyTorch HF-compatible (original and `safetensors`), TensorFlow and Flax formats, alongwith a compatible tokenizer.
 
 - [LaBSE](https://huggingface.co/setu4993/LaBSE)
 - [smaller-LaBSE](https://huggingface.co/setu4993/smaller-LaBSE)
+- [LEALLA-base](https://huggingface.co/setu4993/LEALLA-base)
+- [LEALLA-small](https://huggingface.co/setu4993/LEALLA-small)
+- [LEALLA-large](https://huggingface.co/setu4993/LEALLA-large)
 
 ## Export
 
 To convert and export the models:
 
 ```shell
 poetry install
@@ -47,17 +51,25 @@
 # Clone the already uploaded models.
 cd /path/to/model
 git clone https://huggingface.co/setu4993/LaBSE.git
 
 # Export models anew and update.
 cd /path/to/repo
 poetry install
-poetry run convert_labse --output_path /path/to/model/LaBSE --huggingface_path
+poetry run convert_labse --output_path /path/to/models/LaBSE --huggingface_path
 ```
 
+### Export Commands by Model
+
+1. [LaBSE](https://huggingface.co/setu4993/LaBSE): `poetry run convert_labse --output_path /path/to/models/setu4993/LaBSE --huggingface_path`
+2. [smaller-LaBSE](https://huggingface.co/setu4993/smaller-LaBSE): `poetry run convert_labse --output_path /path/to/models/setu4993/smaller-LaBSE --smaller --huggingface_path`
+3. [LEALLA-base](https://huggingface.co/setu4993/LEALLA-base): `poetry run convert_lealla --size base --output_path /path/to/models/setu4993/LEALLA-base --huggingface_path`
+4. [LEALLA-small](https://huggingface.co/setu4993/LEALLA-small): `poetry run convert_lealla --size small --output_path /path/to/models/setu4993/LEALLA-small --huggingface_path`
+5. [LEALLA-large](https://huggingface.co/setu4993/LEALLA-large): `poetry run convert_lealla --size large --output_path /path/to/models/setu4993/LEALLA-large --huggingface_path`
+
 ## Model Cards
 
 See the [`model-cards` directory](https://github.com/setu4993/convert-labse-tf-pt/tree/main/model-cards) for a copy of the model cards.
 
 ## License
 
 This repository and the conversion code is licensed under the MIT license, but the **model** is distributed with an Apache-2.0 license.
```

