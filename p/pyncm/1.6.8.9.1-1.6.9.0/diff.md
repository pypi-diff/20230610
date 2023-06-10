# Comparing `tmp/pyncm-1.6.8.9.1.tar.gz` & `tmp/pyncm-1.6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncm-1.6.8.9.1.tar", last modified: Wed Apr  5 04:43:28 2023, max compression
+gzip compressed data, was "pyncm-1.6.9.0.tar", last modified: Sat Jun 10 00:56:23 2023, max compression
```

## Comparing `pyncm-1.6.8.9.1.tar` & `pyncm-1.6.9.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:43:28.075457 pyncm-1.6.8.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-04-05 04:43:28.075457 pyncm-1.6.8.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:43:28.071457 pyncm-1.6.8.9.1/demos/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/demos/二维码登录.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/demos/云盘上传.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/demos/手机登录.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/demos/获取单曲下载链接.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/demos/足迹伪装.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:43:28.071457 pyncm-1.6.8.9.1/pyncm/
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27061 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:43:28.075457 pyncm-1.6.8.9.1/pyncm/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/album.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/cloudsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:43:28.075457 pyncm-1.6.8.9.1/pyncm/apis/miniprograms/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/miniprograms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/miniprograms/difm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/miniprograms/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/miniprograms/sportsfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/miniprograms/zonefm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/apis/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:43:28.075457 pyncm-1.6.8.9.1/pyncm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/utils/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/utils/lrcparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyncm/utils/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:43:28.075457 pyncm-1.6.8.9.1/pyncm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-04-05 04:43:28.000000 pyncm-1.6.8.9.1/pyncm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-05 04:43:28.000000 pyncm-1.6.8.9.1/pyncm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 04:43:28.000000 pyncm-1.6.8.9.1/pyncm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-05 04:43:28.000000 pyncm-1.6.8.9.1/pyncm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 04:43:28.000000 pyncm-1.6.8.9.1/pyncm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 04:43:28.000000 pyncm-1.6.8.9.1/pyncm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 04:43:28.075457 pyncm-1.6.8.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-05 04:43:17.000000 pyncm-1.6.8.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.950317 pyncm-1.6.9.0/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/二维码登录.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/云盘上传.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/手机登录.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/获取单曲下载链接.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/demos/足迹伪装.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.950317 pyncm-1.6.9.0/pyncm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27061 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/cloudsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm/apis/miniprograms/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/difm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/sportsfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/miniprograms/zonefm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/apis/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/lrcparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyncm/utils/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/pyncm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 00:56:23.000000 pyncm-1.6.9.0/pyncm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:56:23.954317 pyncm-1.6.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-10 00:56:12.000000 pyncm-1.6.9.0/setup.py
```

### Comparing `pyncm-1.6.8.9.1/LICENSE` & `pyncm-1.6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/PKG-INFO` & `pyncm-1.6.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyncm
-Version: 1.6.8.9.1
+Version: 1.6.9.0
 Summary: NeteaseCloudMusic APIs for Python 3.x 适用于 Python 3 的网易云音乐 API
 Home-page: https://github.com/greats3an/pyncm
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Logo](https://github.com/greats3an/pyncm/raw/master/demos/_logo.png)
 
 # PyNCM
-
+**注意** : 异步使用，请移步 [`async` 分支](https://github.com/mos9527/pyncm/tree/async)
 # 安装
     pip install pyncm
 可选 （若不考虑使用CLI则请忽略）
 - `mutagen` : 为下载的音乐打上封面等
 - `tqdm`    : 显示实时下载进度
 - `coloredlogs` : 彩色日志输出
```

### Comparing `pyncm-1.6.8.9.1/README.md` & `pyncm-1.6.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![Logo](https://github.com/greats3an/pyncm/raw/master/demos/_logo.png)
 
 # PyNCM
-
+**注意** : 异步使用，请移步 [`async` 分支](https://github.com/mos9527/pyncm/tree/async)
 # 安装
     pip install pyncm
 可选 （若不考虑使用CLI则请忽略）
 - `mutagen` : 为下载的音乐打上封面等
 - `tqdm`    : 显示实时下载进度
 - `coloredlogs` : 彩色日志输出
```

### Comparing `pyncm-1.6.8.9.1/demos/__init__.py` & `pyncm-1.6.9.0/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/demos/二维码登录.py` & `pyncm-1.6.9.0/demos/二维码登录.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/demos/云盘上传.py` & `pyncm-1.6.9.0/demos/云盘上传.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/demos/手机登录.py` & `pyncm-1.6.9.0/demos/手机登录.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/demos/足迹伪装.py` & `pyncm-1.6.9.0/demos/足迹伪装.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/__init__.py` & `pyncm-1.6.9.0/pyncm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     >>> pyncm.SetNewSession(
             pyncm.LoadSessionFromString(save)
         )
 
 # 注意事项
     - (PR#11) 海外用户可能经历 460 "Cheating" 问题，可通过添加以下 Header 解决: `X-Real-IP = 118.88.88.88`    
 """
-__version__ = "1.6.8.9.1"
+__version__ = "1.6.9.0"
 
 from threading import current_thread
 from typing import Text, Union
 from time import time
 from .utils.crypto import EapiEncrypt, EapiDecrypt, HexCompose
 import requests, logging, json, os
 logger = logging.getLogger("pyncm.api")
```

### Comparing `pyncm-1.6.8.9.1/pyncm/__main__.py` & `pyncm-1.6.9.0/pyncm/__main__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/__init__.py` & `pyncm-1.6.9.0/pyncm/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/album.py` & `pyncm-1.6.9.0/pyncm/apis/album.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/artist.py` & `pyncm-1.6.9.0/pyncm/apis/artist.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/cloud.py` & `pyncm-1.6.9.0/pyncm/apis/cloud.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/cloudsearch.py` & `pyncm-1.6.9.0/pyncm/apis/cloudsearch.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/login.py` & `pyncm-1.6.9.0/pyncm/apis/login.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/miniprograms/difm.py` & `pyncm-1.6.9.0/pyncm/apis/miniprograms/difm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/miniprograms/radio.py` & `pyncm-1.6.9.0/pyncm/apis/miniprograms/radio.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/miniprograms/sportsfm.py` & `pyncm-1.6.9.0/pyncm/apis/miniprograms/sportsfm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/miniprograms/zonefm.py` & `pyncm-1.6.9.0/pyncm/apis/miniprograms/zonefm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/playlist.py` & `pyncm-1.6.9.0/pyncm/apis/playlist.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/track.py` & `pyncm-1.6.9.0/pyncm/apis/track.py`

 * *Files 15% similar despite different names*

```diff
@@ -110,14 +110,35 @@
     return "/weapi/song/lyric", {
         "id": str(song_id),
         "lv": str(lv),
         "tv": str(tv),
         "rv": str(rv),
     }
 
+@EapiCryptoRequest
+def GetTrackLyricsNew(song_id: str):
+    """PC 端 - 获取歌曲歌词 (新 API)
+
+    Args:
+        song_id (str): 歌曲 ID
+
+    Returns:
+        dict
+    """
+    return "/eapi/song/lyric/v1", {
+        "id": str(song_id),
+        "cp": False,
+        "lv": 0,
+        "tv": 0,
+        "rv": 0,
+        "kv": 0,
+        "yv": 0,
+        "ytv": 0,
+        "yrv": 0,
+    }
 
 @WeapiCryptoRequest
 def GetTrackComments(song_id, offset=0, limit=20, beforeTime=0):
     """网页端 - 获取歌曲评论
 
     Args:
         album_id (str): 歌曲ID
```

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/user.py` & `pyncm-1.6.9.0/pyncm/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/apis/video.py` & `pyncm-1.6.9.0/pyncm/apis/video.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/utils/__init__.py` & `pyncm-1.6.9.0/pyncm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/utils/aes.py` & `pyncm-1.6.9.0/pyncm/utils/aes.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/utils/crypto.py` & `pyncm-1.6.9.0/pyncm/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/utils/helper.py` & `pyncm-1.6.9.0/pyncm/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/utils/lrcparser.py` & `pyncm-1.6.9.0/pyncm/utils/lrcparser.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm/utils/security.py` & `pyncm-1.6.9.0/pyncm/utils/security.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/pyncm.egg-info/PKG-INFO` & `pyncm-1.6.9.0/pyncm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyncm
-Version: 1.6.8.9.1
+Version: 1.6.9.0
 Summary: NeteaseCloudMusic APIs for Python 3.x 适用于 Python 3 的网易云音乐 API
 Home-page: https://github.com/greats3an/pyncm
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Logo](https://github.com/greats3an/pyncm/raw/master/demos/_logo.png)
 
 # PyNCM
-
+**注意** : 异步使用，请移步 [`async` 分支](https://github.com/mos9527/pyncm/tree/async)
 # 安装
     pip install pyncm
 可选 （若不考虑使用CLI则请忽略）
 - `mutagen` : 为下载的音乐打上封面等
 - `tqdm`    : 显示实时下载进度
 - `coloredlogs` : 彩色日志输出
```

### Comparing `pyncm-1.6.8.9.1/pyncm.egg-info/SOURCES.txt` & `pyncm-1.6.9.0/pyncm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.8.9.1/setup.py` & `pyncm-1.6.9.0/setup.py`

 * *Files identical despite different names*

