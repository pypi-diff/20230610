# Comparing `tmp/similarity-learning-0.0.3.tar.gz` & `tmp/similarity-learning-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity-learning-0.0.3.tar", last modified: Fri Jun  2 13:42:28 2023, max compression
+gzip compressed data, was "similarity-learning-0.0.4.tar", last modified: Sat Jun 10 10:07:00 2023, max compression
```

## Comparing `similarity-learning-0.0.3.tar` & `similarity-learning-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-18 07:33:16.000000 similarity-learning-0.0.3/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-01-20 02:50:04.000000 similarity-learning-0.0.3/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3444 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1898 2023-05-20 12:47:49.000000 similarity-learning-0.0.3/README.md
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1026 2023-06-02 13:41:48.000000 similarity-learning-0.0.3/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-01-20 02:50:04.000000 similarity-learning-0.0.3/setup.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/similarity_learning/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    11103 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      133 2023-05-23 07:24:39.000000 similarity-learning-0.0.3/similarity_learning/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1064 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/facenet.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1255 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/feature_space_plotting.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1505 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/pair_matching.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2594 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/siamese.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5486 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/similarity_learning.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3444 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      617 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       81 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-18 07:42:39.000000 similarity-learning-0.0.3/similarity_learning.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       64 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       20 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/top_level.txt
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:07:00.078690 similarity-learning-0.0.4/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-06-09 06:54:59.000000 similarity-learning-0.0.4/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-06-09 06:54:59.000000 similarity-learning-0.0.4/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3393 2023-06-10 10:07:00.078690 similarity-learning-0.0.4/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1863 2023-06-09 06:54:59.000000 similarity-learning-0.0.4/README.md
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1025 2023-06-10 10:06:35.000000 similarity-learning-0.0.4/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-06-10 10:07:00.078690 similarity-learning-0.0.4/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-06-09 06:54:59.000000 similarity-learning-0.0.4/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:07:00.078690 similarity-learning-0.0.4/similarity_learning/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-06-10 10:06:42.000000 similarity-learning-0.0.4/similarity_learning/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    11103 2023-06-10 10:06:42.000000 similarity-learning-0.0.4/similarity_learning/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      168 2023-06-09 06:54:59.000000 similarity-learning-0.0.4/similarity_learning/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1064 2023-06-10 10:06:42.000000 similarity-learning-0.0.4/similarity_learning/facenet.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1255 2023-06-10 10:06:42.000000 similarity-learning-0.0.4/similarity_learning/feature_space_plotting.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1505 2023-06-10 10:06:42.000000 similarity-learning-0.0.4/similarity_learning/pair_matching.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2594 2023-06-10 10:06:42.000000 similarity-learning-0.0.4/similarity_learning/siamese.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5486 2023-06-10 10:06:42.000000 similarity-learning-0.0.4/similarity_learning/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:07:00.078690 similarity-learning-0.0.4/similarity_learning.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3393 2023-06-10 10:06:59.000000 similarity-learning-0.0.4/similarity_learning.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      617 2023-06-10 10:06:59.000000 similarity-learning-0.0.4/similarity_learning.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-10 10:06:59.000000 similarity-learning-0.0.4/similarity_learning.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       81 2023-06-10 10:06:59.000000 similarity-learning-0.0.4/similarity_learning.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-09 06:56:43.000000 similarity-learning-0.0.4/similarity_learning.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       63 2023-06-10 10:06:59.000000 similarity-learning-0.0.4/similarity_learning.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       20 2023-06-10 10:06:59.000000 similarity-learning-0.0.4/similarity_learning.egg-info/top_level.txt
```

### Comparing `similarity-learning-0.0.3/LICENSE` & `similarity-learning-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/PKG-INFO` & `similarity-learning-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-learning
-Version: 0.0.3
+Version: 0.0.4
 Summary: A fastai based framework for similarity learning
 Home-page: https://github.com/Irad-Zehavi/similarity-learning
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: similarity-learning
         ================
@@ -31,16 +31,14 @@
         ```
         
         Now we can train a pair-matcher. First let’s construct dataloaders of
         pairs:
         
         ``` python
         from fastai.vision.all import *
-        
-        from fastai_datasets.all import *
         ```
         
         ``` python
         pairs = Pairs(Imagenette(160), .1)
         dls = pairs.dls(after_item=Resize(128),
                         after_batch=Normalize.from_stats(*imagenet_stats))
         ```
@@ -50,39 +48,39 @@
         
         ``` python
         classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
         siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
         siamese.fit_threshold(dls.train)
         ```
         
-            (1.0399999618530273, 0.8839285969734192)
+            (1.0099999904632568, 0.8962054252624512)
         
         Let’s see how good it is:
         
         ``` python
         learn = Learner(dls, siamese, metrics=accuracy)
         learn.validate()
         ```
         
-            (#2) [0.5608958601951599,0.8239796161651611]
+            (#2) [0.5453092455863953,0.8877550959587097]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         Not bad, but we can do better with finetuning:
         
         ``` python
         learn.fit(5, 1e-4)
         learn.validate()
         ```
         
-            (#2) [0.2924809157848358,0.9387755393981934]
+            (#2) [0.26150667667388916,0.954081654548645]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-9-output-2.png)
```

### Comparing `similarity-learning-0.0.3/README.md` & `similarity-learning-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 ```
 
 Now we can train a pair-matcher. First let’s construct dataloaders of
 pairs:
 
 ``` python
 from fastai.vision.all import *
-
-from fastai_datasets.all import *
 ```
 
 ``` python
 pairs = Pairs(Imagenette(160), .1)
 dls = pairs.dls(after_item=Resize(128),
                 after_batch=Normalize.from_stats(*imagenet_stats))
 ```
@@ -42,39 +40,39 @@
 
 ``` python
 classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
 siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
 siamese.fit_threshold(dls.train)
 ```
 
-    (1.0399999618530273, 0.8839285969734192)
+    (1.0099999904632568, 0.8962054252624512)
 
 Let’s see how good it is:
 
 ``` python
 learn = Learner(dls, siamese, metrics=accuracy)
 learn.validate()
 ```
 
-    (#2) [0.5608958601951599,0.8239796161651611]
+    (#2) [0.5453092455863953,0.8877550959587097]
 
 ``` python
 learn.show_results()
 ```
 
 ![](index_files/figure-commonmark/cell-7-output-2.png)
 
 Not bad, but we can do better with finetuning:
 
 ``` python
 learn.fit(5, 1e-4)
 learn.validate()
 ```
 
-    (#2) [0.2924809157848358,0.9387755393981934]
+    (#2) [0.26150667667388916,0.954081654548645]
 
 ``` python
 learn.show_results()
 ```
 
 ![](index_files/figure-commonmark/cell-9-output-2.png)
```

### Comparing `similarity-learning-0.0.3/settings.ini` & `similarity-learning-0.0.4/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = similarity-learning
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = similarity_learning
@@ -35,9 +35,9 @@
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Irad-Zehavi
 
 ### Optional ###
 requirements = fastai fastai_datasets matplotlib facenet_pytorch
-dev_requirements = ipympl
+dev_requirements = nbdev
 # console_scripts =
```

### Comparing `similarity-learning-0.0.3/setup.py` & `similarity-learning-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/similarity_learning/_modidx.py` & `similarity-learning-0.0.4/similarity_learning/_modidx.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/similarity_learning/facenet.py` & `similarity-learning-0.0.4/similarity_learning/facenet.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/similarity_learning/feature_space_plotting.py` & `similarity-learning-0.0.4/similarity_learning/feature_space_plotting.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/similarity_learning/pair_matching.py` & `similarity-learning-0.0.4/similarity_learning/pair_matching.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/similarity_learning/siamese.py` & `similarity-learning-0.0.4/similarity_learning/siamese.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/similarity_learning/utils.py` & `similarity-learning-0.0.4/similarity_learning/utils.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.3/similarity_learning.egg-info/PKG-INFO` & `similarity-learning-0.0.4/similarity_learning.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-learning
-Version: 0.0.3
+Version: 0.0.4
 Summary: A fastai based framework for similarity learning
 Home-page: https://github.com/Irad-Zehavi/similarity-learning
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: similarity-learning
         ================
@@ -31,16 +31,14 @@
         ```
         
         Now we can train a pair-matcher. First let’s construct dataloaders of
         pairs:
         
         ``` python
         from fastai.vision.all import *
-        
-        from fastai_datasets.all import *
         ```
         
         ``` python
         pairs = Pairs(Imagenette(160), .1)
         dls = pairs.dls(after_item=Resize(128),
                         after_batch=Normalize.from_stats(*imagenet_stats))
         ```
@@ -50,39 +48,39 @@
         
         ``` python
         classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
         siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
         siamese.fit_threshold(dls.train)
         ```
         
-            (1.0399999618530273, 0.8839285969734192)
+            (1.0099999904632568, 0.8962054252624512)
         
         Let’s see how good it is:
         
         ``` python
         learn = Learner(dls, siamese, metrics=accuracy)
         learn.validate()
         ```
         
-            (#2) [0.5608958601951599,0.8239796161651611]
+            (#2) [0.5453092455863953,0.8877550959587097]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         Not bad, but we can do better with finetuning:
         
         ``` python
         learn.fit(5, 1e-4)
         learn.validate()
         ```
         
-            (#2) [0.2924809157848358,0.9387755393981934]
+            (#2) [0.26150667667388916,0.954081654548645]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-9-output-2.png)
```

### Comparing `similarity-learning-0.0.3/similarity_learning.egg-info/SOURCES.txt` & `similarity-learning-0.0.4/similarity_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

