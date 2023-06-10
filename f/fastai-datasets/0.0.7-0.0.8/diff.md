# Comparing `tmp/fastai-datasets-0.0.7.tar.gz` & `tmp/fastai-datasets-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-datasets-0.0.7.tar", last modified: Fri Jun  2 13:39:58 2023, max compression
+gzip compressed data, was "fastai-datasets-0.0.8.tar", last modified: Sat Jun 10 10:06:12 2023, max compression
```

## Comparing `fastai-datasets-0.0.7.tar` & `fastai-datasets-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:39:58.189643 fastai-datasets-0.0.7/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.7/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.7/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4738 2023-06-02 13:39:58.185643 fastai-datasets-0.0.7/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3284 2023-05-20 11:36:01.000000 fastai-datasets-0.0.7/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:39:58.177643 fastai-datasets-0.0.7/fastai_datasets/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    13272 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.7/fastai_datasets/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/cifar10.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      947 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/imagenette.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/lfw.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      882 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/mnist.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3800 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/pairs.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     6947 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/patches.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/pfr.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:39:58.185643 fastai-datasets-0.0.7/fastai_datasets.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4738 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-06-02 13:39:58.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-06-02 13:38:51.000000 fastai-datasets-0.0.7/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-06-02 13:39:58.189643 fastai-datasets-0.0.7/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.7/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:06:12.470435 fastai-datasets-0.0.8/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-06-09 06:54:21.000000 fastai-datasets-0.0.8/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-06-09 06:54:21.000000 fastai-datasets-0.0.8/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4738 2023-06-10 10:06:12.470435 fastai-datasets-0.0.8/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3284 2023-06-09 06:54:21.000000 fastai-datasets-0.0.8/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:06:12.470435 fastai-datasets-0.0.8/fastai_datasets/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    13526 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      170 2023-06-09 06:54:21.000000 fastai-datasets-0.0.8/fastai_datasets/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      752 2023-06-10 10:03:43.000000 fastai-datasets-0.0.8/fastai_datasets/cifar.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      947 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/imagenette.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4698 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/lfw.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      882 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/mnist.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3800 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/pairs.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     6947 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/patches.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      838 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/pfr.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-06-10 10:03:44.000000 fastai-datasets-0.0.8/fastai_datasets/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:06:12.470435 fastai-datasets-0.0.8/fastai_datasets.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4738 2023-06-10 10:06:12.000000 fastai-datasets-0.0.8/fastai_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      606 2023-06-10 10:06:12.000000 fastai-datasets-0.0.8/fastai_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-10 10:06:12.000000 fastai-datasets-0.0.8/fastai_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-06-10 10:06:12.000000 fastai-datasets-0.0.8/fastai_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-09 06:56:34.000000 fastai-datasets-0.0.8/fastai_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       36 2023-06-10 10:06:12.000000 fastai-datasets-0.0.8/fastai_datasets.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-06-10 10:06:12.000000 fastai-datasets-0.0.8/fastai_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      994 2023-06-10 10:03:07.000000 fastai-datasets-0.0.8/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-06-10 10:06:12.470435 fastai-datasets-0.0.8/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-06-09 06:54:21.000000 fastai-datasets-0.0.8/setup.py
```

### Comparing `fastai-datasets-0.0.7/LICENSE` & `fastai-datasets-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.7/PKG-INFO` & `fastai-datasets-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.7
+Version: 0.0.8
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
```

### Comparing `fastai-datasets-0.0.7/README.md` & `fastai-datasets-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.7/fastai_datasets/_modidx.py` & `fastai-datasets-0.0.8/fastai_datasets/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/fastai-datasets',
                 'doc_host': 'https://Irad-Zehavi.github.io',
                 'git_url': 'https://github.com/Irad-Zehavi/fastai-datasets',
                 'lib_path': 'fastai_datasets'},
   'syms': { 'fastai_datasets.all': {},
-            'fastai_datasets.cifar10': {'fastai_datasets.cifar10.CIFAR10': ('cifar10.html#cifar10', 'fastai_datasets/cifar10.py')},
+            'fastai_datasets.cifar': { 'fastai_datasets.cifar.CIFAR10': ('cifar.html#cifar10', 'fastai_datasets/cifar.py'),
+                                       'fastai_datasets.cifar.CIFAR100': ('cifar.html#cifar100', 'fastai_datasets/cifar.py')},
             'fastai_datasets.imagenette': { 'fastai_datasets.imagenette.Imagenette': ( 'imagenette.html#imagenette',
                                                                                        'fastai_datasets/imagenette.py')},
             'fastai_datasets.lfw': { 'fastai_datasets.lfw.LFW': ('Facial Recognition/lfw.html#lfw', 'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFW.__init__': ( 'Facial Recognition/lfw.html#lfw.__init__',
                                                                            'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFW._fetch_file': ( 'Facial Recognition/lfw.html#lfw._fetch_file',
                                                                               'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFW._get_path': ( 'Facial Recognition/lfw.html#lfw._get_path',
                                                                             'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFW._load': ('Facial Recognition/lfw.html#lfw._load', 'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFW._parse_items': ( 'Facial Recognition/lfw.html#lfw._parse_items',
                                                                                'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFW._url': ('Facial Recognition/lfw.html#lfw._url', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW.all': ('Facial Recognition/lfw.html#lfw.all', 'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFW.test': ('Facial Recognition/lfw.html#lfw.test', 'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFWDevMixin': ( 'Facial Recognition/lfw.html#lfwdevmixin',
                                                                           'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFWDevMixin.dev': ( 'Facial Recognition/lfw.html#lfwdevmixin.dev',
                                                                               'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFWPairs': ('Facial Recognition/lfw.html#lfwpairs', 'fastai_datasets/lfw.py'),
                                      'fastai_datasets.lfw.LFWPairsMixin': ( 'Facial Recognition/lfw.html#lfwpairsmixin',
```

### Comparing `fastai-datasets-0.0.7/fastai_datasets/imagenette.py` & `fastai-datasets-0.0.8/fastai_datasets/imagenette.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.7/fastai_datasets/lfw.py` & `fastai-datasets-0.0.8/fastai_datasets/lfw.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,27 +23,31 @@
             self.root = mtcnn_aligned(self.root)
 
 
     @classmethod
     def _url(cls, fname):
         return f'{cls.BASE_URL}/{fname}'
 
+    def all(self):
+        return self._load(items=self._parse_items(self.TEST_ITEMS_FILE_NAME))
+
     def test(self):
         items = self._parse_items(self.TEST_ITEMS_FILE_NAME)
         splits = KFold(n_splits=10, shuffle=False).split(range_of(items))
         return [self._load(items=items, splits=s) for s in splits]
 
     def _fetch_file(self, fname):
         return fetch_file(self._url(fname))
 
     @abstractmethod
     def _parse_items(self, fname):
         pass
 
     @abstractmethod
+    @delegates(Datasets)
     def _load(self, **kwargs):
         pass
 
     def _get_path(self, name, num) -> Path:
         return self.root / name / f'{name}_{num:04d}.jpg'
```

### Comparing `fastai-datasets-0.0.7/fastai_datasets/mnist.py` & `fastai-datasets-0.0.8/fastai_datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.7/fastai_datasets/pairs.py` & `fastai-datasets-0.0.8/fastai_datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.7/fastai_datasets/patches.py` & `fastai-datasets-0.0.8/fastai_datasets/patches.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.7/fastai_datasets/pfr.py` & `fastai-datasets-0.0.8/fastai_datasets/pfr.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 import fastai_datasets.patches
 from .utils import *
 
 # %% ../nbs/Facial Recognition/pfr.ipynb 5
 ROOT = data_path()/'105_classes_pins_dataset'
 
-def PinterestFaces(mtcnn=True):
+def PinterestFaces(mtcnn=True, splitter=None):
     """Requires the user to download the file manually"""
     assert ROOT.exists(), f'Please manually download the dataset to {ROOT}'
     dblock = DataBlock(
         blocks=(ImageBlock, CategoryBlock),
         get_items=get_image_files,
-        get_y=lambda p: parent_label(p).replace('pins_', '').replace('_', ' ').title()
+        get_y=lambda p: parent_label(p).replace('pins_', '').replace('_', ' ').title(),
+        splitter=splitter
     )
 
     return dblock.datasets(mtcnn_aligned(ROOT, batched=False) if mtcnn else ROOT)
```

### Comparing `fastai-datasets-0.0.7/fastai_datasets/utils.py` & `fastai-datasets-0.0.8/fastai_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.7/fastai_datasets.egg-info/PKG-INFO` & `fastai-datasets-0.0.8/fastai_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.7
+Version: 0.0.8
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
```

### Comparing `fastai-datasets-0.0.7/fastai_datasets.egg-info/SOURCES.txt` & `fastai-datasets-0.0.8/fastai_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 fastai_datasets/__init__.py
 fastai_datasets/_modidx.py
 fastai_datasets/all.py
-fastai_datasets/cifar10.py
+fastai_datasets/cifar.py
 fastai_datasets/imagenette.py
 fastai_datasets/lfw.py
 fastai_datasets/mnist.py
 fastai_datasets/pairs.py
 fastai_datasets/patches.py
 fastai_datasets/pfr.py
 fastai_datasets/utils.py
```

### Comparing `fastai-datasets-0.0.7/settings.ini` & `fastai-datasets-0.0.8/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastai-datasets
 lib_name = %(repo)s
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastai_datasets
@@ -35,9 +35,9 @@
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Irad-Zehavi
 
 ### Optional ###
 requirements = fastai facenet_pytorch
-# dev_requirements = 
+dev_requirements = nbdev
 # console_scripts =
```

### Comparing `fastai-datasets-0.0.7/setup.py` & `fastai-datasets-0.0.8/setup.py`

 * *Files identical despite different names*

