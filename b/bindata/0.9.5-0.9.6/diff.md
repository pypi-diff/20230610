# Comparing `tmp/bindata-0.9.5.tar.gz` & `tmp/bindata-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bindata-0.9.5.tar", last modified: Fri Jun  9 23:13:12 2023, max compression
+gzip compressed data, was "bindata-0.9.6.tar", last modified: Sat Jun 10 00:06:44 2023, max compression
```

## Comparing `bindata-0.9.5.tar` & `bindata-0.9.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 23:13:12.956578 bindata-0.9.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-05-12 08:59:34.000000 bindata-0.9.5/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3820 2023-06-09 23:13:12.956578 bindata-0.9.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3347 2023-06-09 23:11:48.000000 bindata-0.9.5/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 23:13:12.952578 bindata-0.9.5/bindata/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      342 2023-06-09 23:11:55.000000 bindata-0.9.5/bindata/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/_generate_simulvals.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2281 2023-06-09 23:11:14.000000 bindata-0.9.5/bindata/_simuvals_class.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4678 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/bindata.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3766 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/check_commonprob.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 23:13:12.956578 bindata-0.9.5/bindata/res/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26897 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/res/binary.png
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   180290 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/res/simulvals.pickle
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3619 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/simul_commonprob.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 23:13:12.956578 bindata-0.9.5/bindata/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      101 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6245 2023-05-12 08:59:34.000000 bindata-0.9.5/bindata/tests/test_all.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 23:13:12.952578 bindata-0.9.5/bindata.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3820 2023-06-09 23:13:12.000000 bindata-0.9.5/bindata.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      441 2023-06-09 23:13:12.000000 bindata-0.9.5/bindata.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-09 23:13:12.000000 bindata-0.9.5/bindata.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-06-09 23:13:12.000000 bindata-0.9.5/bindata.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-06-09 23:13:12.000000 bindata-0.9.5/bindata.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-09 23:13:12.956578 bindata-0.9.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      939 2023-06-09 20:58:22.000000 bindata-0.9.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-10 00:06:44.564581 bindata-0.9.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-05-12 08:59:34.000000 bindata-0.9.6/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3820 2023-06-10 00:06:44.564581 bindata-0.9.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3347 2023-06-10 00:05:27.000000 bindata-0.9.6/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-10 00:06:44.560581 bindata-0.9.6/bindata/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      342 2023-06-10 00:05:23.000000 bindata-0.9.6/bindata/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/_generate_simulvals.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2313 2023-06-10 00:05:43.000000 bindata-0.9.6/bindata/_simuvals_class.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4678 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/bindata.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3766 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/check_commonprob.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-10 00:06:44.564581 bindata-0.9.6/bindata/res/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26897 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/res/binary.png
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   180290 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/res/simulvals.pickle
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3619 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/simul_commonprob.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-10 00:06:44.564581 bindata-0.9.6/bindata/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      101 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6245 2023-05-12 08:59:34.000000 bindata-0.9.6/bindata/tests/test_all.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-10 00:06:44.560581 bindata-0.9.6/bindata.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3820 2023-06-10 00:06:44.000000 bindata-0.9.6/bindata.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      441 2023-06-10 00:06:44.000000 bindata-0.9.6/bindata.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-10 00:06:44.000000 bindata-0.9.6/bindata.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-06-10 00:06:44.000000 bindata-0.9.6/bindata.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-06-10 00:06:44.000000 bindata-0.9.6/bindata.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-10 00:06:44.564581 bindata-0.9.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      939 2023-06-09 20:58:22.000000 bindata-0.9.6/setup.py
```

### Comparing `bindata-0.9.5/LICENSE.txt` & `bindata-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bindata-0.9.5/PKG-INFO` & `bindata-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bindata
-Version: 0.9.5
+Version: 0.9.6
 Summary: A library for sampling correlated binary variates.
 Home-page: https://github.com/LucaMingarelli/bindata
 Author: Luca Mingarelli
 Author-email: lucamingarelli@me.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # bindata <img src="https://raw.githubusercontent.com/LucaMingarelli/bindata/master/bindata/res/binary.png"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/bindata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/bindata)
-[![version](https://img.shields.io/badge/version-0.9.5-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.9.6-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/bindata.svg)](https://pypi.org/project/bindata/)
 [![License](https://img.shields.io/pypi/l/bindata.svg)](https://github.com/LucaMingarelli/bindata/blob/master/LICENSE.txt)
 
 [//]: # ([![Downloads]&#40;https://static.pepy.tech/personalized-badge/bindata?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads&#41;]&#40;https://pepy.tech/project/bindata&#41;)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: bindata Version: 0.9.5 Summary: A library for
+Metadata-Version: 2.1 Name: bindata Version: 0.9.6 Summary: A library for
 sampling correlated binary variates. Home-page: https://github.com/
 LucaMingarelli/bindata Author: Luca Mingarelli Author-email:
 lucamingarelli@me.com License: MIT Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE.txt # bindata [https://
 raw.githubusercontent.com/LucaMingarelli/bindata/master/bindata/res/binary.png]
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/
 bindata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)]
 (https://app.circleci.com/pipelines/github/LucaMingarelli/bindata) [![version]
-(https://img.shields.io/badge/version-0.9.5-success.svg)](#) [![PyPI Latest
+(https://img.shields.io/badge/version-0.9.6-success.svg)](#) [![PyPI Latest
 Release](https://img.shields.io/pypi/v/bindata.svg)](https://pypi.org/project/
 bindata/) [![License](https://img.shields.io/pypi/l/bindata.svg)](https://
 github.com/LucaMingarelli/bindata/blob/master/LICENSE.txt) [//]: # ([!
 [Downloads](https://static.pepy.tech/personalized-badge/
 bindata?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)]
 (https://pepy.tech/project/bindata)) A python replication of the omonymous R
 library [`bindata`](https://cran.r-project.org/web/packages/bindata/
```

### Comparing `bindata-0.9.5/README.md` & `bindata-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # bindata <img src="https://raw.githubusercontent.com/LucaMingarelli/bindata/master/bindata/res/binary.png"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/bindata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/bindata)
-[![version](https://img.shields.io/badge/version-0.9.5-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.9.6-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/bindata.svg)](https://pypi.org/project/bindata/)
 [![License](https://img.shields.io/pypi/l/bindata.svg)](https://github.com/LucaMingarelli/bindata/blob/master/LICENSE.txt)
 
 [//]: # ([![Downloads]&#40;https://static.pepy.tech/personalized-badge/bindata?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads&#41;]&#40;https://pepy.tech/project/bindata&#41;)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # bindata [https://raw.githubusercontent.com/LucaMingarelli/bindata/master/
 bindata/res/binary.png] [![CircleCI](https://circleci.com/gh/LucaMingarelli/
 bindata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)]
 (https://app.circleci.com/pipelines/github/LucaMingarelli/bindata) [![version]
-(https://img.shields.io/badge/version-0.9.5-success.svg)](#) [![PyPI Latest
+(https://img.shields.io/badge/version-0.9.6-success.svg)](#) [![PyPI Latest
 Release](https://img.shields.io/pypi/v/bindata.svg)](https://pypi.org/project/
 bindata/) [![License](https://img.shields.io/pypi/l/bindata.svg)](https://
 github.com/LucaMingarelli/bindata/blob/master/LICENSE.txt) [//]: # ([!
 [Downloads](https://static.pepy.tech/personalized-badge/
 bindata?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)]
 (https://pepy.tech/project/bindata)) A python replication of the omonymous R
 library [`bindata`](https://cran.r-project.org/web/packages/bindata/
```

### Comparing `bindata-0.9.5/bindata/_simuvals_class.py` & `bindata-0.9.6/bindata/_simuvals_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """  Created on 13/03/2023::
 ------------- _simuvals_class.py -------------
 
 **Authors**: L. Mingarelli
 """
 import pickle
 import numpy as np
+import os
 
 try:
-    with open(f"{'/'.join(__file__.split('/')[:-1])}/res/simulvals.pickle", 'rb') as f:
+    root = os.path.dirname(__file__)
+    with open(os.path.join(root, 'res', 'simulvals.pickle'), 'rb') as f:
         _SimulVals = pickle.load(f)
 except:
     with open("./bindata/res/simulvals.pickle", 'rb') as f:
         _SimulVals = pickle.load(f)
```

### Comparing `bindata-0.9.5/bindata/bindata.py` & `bindata-0.9.6/bindata/bindata.py`

 * *Files identical despite different names*

### Comparing `bindata-0.9.5/bindata/check_commonprob.py` & `bindata-0.9.6/bindata/check_commonprob.py`

 * *Files identical despite different names*

### Comparing `bindata-0.9.5/bindata/res/binary.png` & `bindata-0.9.6/bindata/res/binary.png`

 * *Files identical despite different names*

### Comparing `bindata-0.9.5/bindata/res/simulvals.pickle` & `bindata-0.9.6/bindata/res/simulvals.pickle`

 * *Files identical despite different names*

### Comparing `bindata-0.9.5/bindata/simul_commonprob.py` & `bindata-0.9.6/bindata/simul_commonprob.py`

 * *Files identical despite different names*

### Comparing `bindata-0.9.5/bindata/tests/test_all.py` & `bindata-0.9.6/bindata/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `bindata-0.9.5/bindata.egg-info/PKG-INFO` & `bindata-0.9.6/bindata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bindata
-Version: 0.9.5
+Version: 0.9.6
 Summary: A library for sampling correlated binary variates.
 Home-page: https://github.com/LucaMingarelli/bindata
 Author: Luca Mingarelli
 Author-email: lucamingarelli@me.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # bindata <img src="https://raw.githubusercontent.com/LucaMingarelli/bindata/master/bindata/res/binary.png"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/bindata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/bindata)
-[![version](https://img.shields.io/badge/version-0.9.5-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.9.6-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/bindata.svg)](https://pypi.org/project/bindata/)
 [![License](https://img.shields.io/pypi/l/bindata.svg)](https://github.com/LucaMingarelli/bindata/blob/master/LICENSE.txt)
 
 [//]: # ([![Downloads]&#40;https://static.pepy.tech/personalized-badge/bindata?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads&#41;]&#40;https://pepy.tech/project/bindata&#41;)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: bindata Version: 0.9.5 Summary: A library for
+Metadata-Version: 2.1 Name: bindata Version: 0.9.6 Summary: A library for
 sampling correlated binary variates. Home-page: https://github.com/
 LucaMingarelli/bindata Author: Luca Mingarelli Author-email:
 lucamingarelli@me.com License: MIT Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE.txt # bindata [https://
 raw.githubusercontent.com/LucaMingarelli/bindata/master/bindata/res/binary.png]
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/
 bindata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)]
 (https://app.circleci.com/pipelines/github/LucaMingarelli/bindata) [![version]
-(https://img.shields.io/badge/version-0.9.5-success.svg)](#) [![PyPI Latest
+(https://img.shields.io/badge/version-0.9.6-success.svg)](#) [![PyPI Latest
 Release](https://img.shields.io/pypi/v/bindata.svg)](https://pypi.org/project/
 bindata/) [![License](https://img.shields.io/pypi/l/bindata.svg)](https://
 github.com/LucaMingarelli/bindata/blob/master/LICENSE.txt) [//]: # ([!
 [Downloads](https://static.pepy.tech/personalized-badge/
 bindata?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)]
 (https://pepy.tech/project/bindata)) A python replication of the omonymous R
 library [`bindata`](https://cran.r-project.org/web/packages/bindata/
```

### Comparing `bindata-0.9.5/setup.py` & `bindata-0.9.6/setup.py`

 * *Files identical despite different names*

