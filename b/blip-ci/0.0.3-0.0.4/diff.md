# Comparing `tmp/blip-ci-0.0.3.tar.gz` & `tmp/blip-ci-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blip-ci-0.0.3.tar", last modified: Thu Feb 23 15:09:22 2023, max compression
+gzip compressed data, was "blip-ci-0.0.4.tar", last modified: Sat Jun 10 16:07:37 2023, max compression
```

## Comparing `blip-ci-0.0.3.tar` & `blip-ci-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-23 15:09:22.025479 blip-ci-0.0.3/
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     1482 2023-02-11 21:25:03.000000 blip-ci-0.0.3/LICENSE.txt
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)       96 2023-02-11 21:53:07.000000 blip-ci-0.0.3/MANIFEST.in
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    10072 2023-02-23 15:09:22.025479 blip-ci-0.0.3/PKG-INFO
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     9544 2023-02-11 21:25:03.000000 blip-ci-0.0.3/README.md
-drwxrwxr-x   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-23 15:09:22.025479 blip-ci-0.0.3/blip/
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/__init__.py
-drwxrwxr-x   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-23 15:09:22.025479 blip-ci-0.0.3/blip/configs/
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      485 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/bert_config.json
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      651 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/caption_coco.yaml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      485 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/med_config.json
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      441 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/nlvr.yaml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      352 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/nocaps.yaml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      479 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/pretrain.yaml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      655 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/retrieval_coco.yaml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      658 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/retrieval_flickr.yaml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      354 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/retrieval_msrvtt.yaml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)      639 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/configs/vqa.yaml
-drwxrwxr-x   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-23 15:09:22.025479 blip-ci-0.0.3/blip/data/
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     5189 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/__init__.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     4711 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/coco_karpathy_dataset.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     3346 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/flickr30k_dataset.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     2722 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/nlvr_dataset.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     1139 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/nocaps_dataset.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     1632 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/pretrain_dataset.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     3449 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/utils.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     4005 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/video_dataset.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     3454 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/data/vqa_dataset.py
-drwxrwxr-x   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-23 15:09:22.025479 blip-ci-0.0.3/blip/models/
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/__init__.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    10934 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/blip.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     3148 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/blip_itm.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     4374 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/blip_nlvr.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    16054 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/blip_pretrain.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    13747 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/blip_retrieval.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     8957 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/blip_vqa.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    41786 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/med.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    36738 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/nlvr_encoder.py
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    14240 2023-02-11 21:25:03.000000 blip-ci-0.0.3/blip/models/vit.py
-drwxrwxr-x   0 blackpawn  (1000) blackpawn  (1000)        0 2023-02-23 15:09:22.025479 blip-ci-0.0.3/blip_ci.egg-info/
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)    10072 2023-02-23 15:09:22.000000 blip-ci-0.0.3/blip_ci.egg-info/PKG-INFO
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     1041 2023-02-23 15:09:22.000000 blip-ci-0.0.3/blip_ci.egg-info/SOURCES.txt
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)        1 2023-02-23 15:09:22.000000 blip-ci-0.0.3/blip_ci.egg-info/dependency_links.txt
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)       79 2023-02-23 15:09:22.000000 blip-ci-0.0.3/blip_ci.egg-info/requires.txt
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)        5 2023-02-23 15:09:22.000000 blip-ci-0.0.3/blip_ci.egg-info/top_level.txt
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)       80 2023-02-11 21:33:46.000000 blip-ci-0.0.3/pyproject.toml
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)        6 2023-02-11 21:25:03.000000 blip-ci-0.0.3/requirements-dev.txt
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)       51 2023-02-17 22:44:22.000000 blip-ci-0.0.3/requirements.txt
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)       38 2023-02-23 15:09:22.025479 blip-ci-0.0.3/setup.cfg
--rw-rw-r--   0 blackpawn  (1000) blackpawn  (1000)     1486 2023-02-23 15:08:51.000000 blip-ci-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-10 16:07:28.000000 blip-ci-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-10 16:07:28.000000 blip-ci-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-10 16:07:37.602746 blip-ci-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-10 16:07:28.000000 blip-ci-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.598746 blip-ci-0.0.4/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.598746 blip-ci-0.0.4/blip/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/bert_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/caption_coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/nlvr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/nocaps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/pretrain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/retrieval_coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/retrieval_flickr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/retrieval_msrvtt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/vqa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/blip/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/coco_karpathy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/flickr30k_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/nlvr_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/nocaps_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/pretrain_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/vqa_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/blip/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_nlvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41786 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36738 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/nlvr_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/blip_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 16:07:28.000000 blip-ci-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 16:07:28.000000 blip-ci-0.0.4/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-10 16:07:28.000000 blip-ci-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:07:37.602746 blip-ci-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1486 2023-06-10 16:07:28.000000 blip-ci-0.0.4/setup.py
```

### Comparing `blip-ci-0.0.3/LICENSE.txt` & `blip-ci-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/PKG-INFO` & `blip-ci-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blip-ci
-Version: 0.0.3
+Version: 0.0.4
 Summary: BLIP library for use with CLIP Interrogator
 Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce
 Author-email: 
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blip-ci Version: 0.0.3 Summary: BLIP library for
+Metadata-Version: 2.1 Name: blip-ci Version: 0.0.4 Summary: BLIP library for
 use with CLIP Interrogator Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce Author-email: License: BSD-3 Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 2 - Pre-Alpha Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: all License-File: LICENSE.txt ## BLIP:
 Bootstrapping Language-Image Pre-training for Unified Vision-Language
```

### Comparing `blip-ci-0.0.3/README.md` & `blip-ci-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/configs/caption_coco.yaml` & `blip-ci-0.0.4/blip/configs/caption_coco.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/configs/retrieval_coco.yaml` & `blip-ci-0.0.4/blip/configs/retrieval_coco.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/configs/retrieval_flickr.yaml` & `blip-ci-0.0.4/blip/configs/retrieval_flickr.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/configs/vqa.yaml` & `blip-ci-0.0.4/blip/configs/vqa.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/__init__.py` & `blip-ci-0.0.4/blip/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/coco_karpathy_dataset.py` & `blip-ci-0.0.4/blip/data/coco_karpathy_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/flickr30k_dataset.py` & `blip-ci-0.0.4/blip/data/flickr30k_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/nlvr_dataset.py` & `blip-ci-0.0.4/blip/data/nlvr_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/nocaps_dataset.py` & `blip-ci-0.0.4/blip/data/nocaps_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/pretrain_dataset.py` & `blip-ci-0.0.4/blip/data/pretrain_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/utils.py` & `blip-ci-0.0.4/blip/data/utils.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/video_dataset.py` & `blip-ci-0.0.4/blip/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/data/vqa_dataset.py` & `blip-ci-0.0.4/blip/data/vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/blip.py` & `blip-ci-0.0.4/blip/models/blip.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/blip_itm.py` & `blip-ci-0.0.4/blip/models/blip_itm.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/blip_nlvr.py` & `blip-ci-0.0.4/blip/models/blip_nlvr.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/blip_pretrain.py` & `blip-ci-0.0.4/blip/models/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/blip_retrieval.py` & `blip-ci-0.0.4/blip/models/blip_retrieval.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/blip_vqa.py` & `blip-ci-0.0.4/blip/models/blip_vqa.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/med.py` & `blip-ci-0.0.4/blip/models/med.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/nlvr_encoder.py` & `blip-ci-0.0.4/blip/models/nlvr_encoder.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip/models/vit.py` & `blip-ci-0.0.4/blip/models/vit.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/blip_ci.egg-info/PKG-INFO` & `blip-ci-0.0.4/blip_ci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blip-ci
-Version: 0.0.3
+Version: 0.0.4
 Summary: BLIP library for use with CLIP Interrogator
 Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce
 Author-email: 
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blip-ci Version: 0.0.3 Summary: BLIP library for
+Metadata-Version: 2.1 Name: blip-ci Version: 0.0.4 Summary: BLIP library for
 use with CLIP Interrogator Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce Author-email: License: BSD-3 Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 2 - Pre-Alpha Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: all License-File: LICENSE.txt ## BLIP:
 Bootstrapping Language-Image Pre-training for Unified Vision-Language
```

### Comparing `blip-ci-0.0.3/blip_ci.egg-info/SOURCES.txt` & `blip-ci-0.0.4/blip_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.3/setup.py` & `blip-ci-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         DEVELOPMENT_MODULES = [line.strip()
                                for line in file if "-e" not in line]
     extras = {"dev": DEVELOPMENT_MODULES}
     extras["all"] = [item for group in extras.values() for item in group]
 
     setup(
         name="blip-ci",
-        version="0.0.3",
+        version="0.0.4",
         license="BSD-3",
         author="salesforce",
         author_email="",
         url="https://github.com/pharmapsychotic/BLIP",
         description="BLIP library for use with CLIP Interrogator",
         long_description=open('README.md', encoding="utf8").read(),
         long_description_content_type="text/markdown",
```

