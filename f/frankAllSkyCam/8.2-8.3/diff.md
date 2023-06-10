# Comparing `tmp/frankAllSkyCam-8.2.tar.gz` & `tmp/frankAllSkyCam-8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-8.2.tar", last modified: Wed Jun  7 21:14:45 2023, max compression
+gzip compressed data, was "frankAllSkyCam-8.3.tar", last modified: Sat Jun 10 17:01:06 2023, max compression
```

## Comparing `frankAllSkyCam-8.2.tar` & `frankAllSkyCam-8.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/
--rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/PKG-INFO
--rwxr--r--   0 pi        (1000) pi        (1000)     3200 2023-06-07 19:09:34.000000 frankAllSkyCam-8.2/README.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-07 21:14:12.000000 frankAllSkyCam-8.2/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     6068 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3877 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/drawtext.py
--rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/exposurecalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/fileManager.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/getextdata.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/index.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1295 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/logos.py
--rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/sqmexp.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/sqmreader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.000000 frankAllSkyCam-8.2/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/watchDog.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      746 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       18 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/top_level.txt
--rwxrw-rw-   0 pi        (1000) pi        (1000)       79 2023-06-07 21:14:45.646027 frankAllSkyCam-8.2/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-07 21:14:28.000000 frankAllSkyCam-8.2/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:01:06.510128 frankAllSkyCam-8.3/
+-rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-10 17:01:06.510128 frankAllSkyCam-8.3/PKG-INFO
+-rwxr--r--   0 pi        (1000) pi        (1000)     3200 2023-06-07 19:09:34.000000 frankAllSkyCam-8.3/README.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:01:06.506128 frankAllSkyCam-8.3/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-10 17:00:34.000000 frankAllSkyCam-8.3/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     6068 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3999 2023-06-10 16:58:25.000000 frankAllSkyCam-8.3/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/drawtext.py
+-rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/exposurecalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/fileManager.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      927 2023-06-10 16:58:11.000000 frankAllSkyCam-8.3/frankAllSkyCam/getextdata.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/index.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1295 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/logos.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/sqmexp.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/sqmreader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.000000 frankAllSkyCam-8.3/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 21:13:55.000000 frankAllSkyCam-8.3/frankAllSkyCam/watchDog.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:01:06.510128 frankAllSkyCam-8.3/frankAllSkyCam.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-10 17:01:06.000000 frankAllSkyCam-8.3/frankAllSkyCam.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      746 2023-06-10 17:01:06.000000 frankAllSkyCam-8.3/frankAllSkyCam.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-10 17:01:06.000000 frankAllSkyCam-8.3/frankAllSkyCam.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       18 2023-06-10 17:01:06.000000 frankAllSkyCam-8.3/frankAllSkyCam.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-10 17:01:06.000000 frankAllSkyCam-8.3/frankAllSkyCam.egg-info/top_level.txt
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       79 2023-06-10 17:01:06.510128 frankAllSkyCam-8.3/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-10 17:00:25.000000 frankAllSkyCam-8.3/setup.py
```

### Comparing `frankAllSkyCam-8.2/PKG-INFO` & `frankAllSkyCam-8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: frankAllSkyCam
-Version: 8.2
+Version: 8.3
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.2.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.3.tar.gz
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
 Keywords: AllSkyCamera,Astronomy,AllSky
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `frankAllSkyCam-8.2/README.txt` & `frankAllSkyCam-8.3/README.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/__main__.py` & `frankAllSkyCam-8.3/frankAllSkyCam/__main__.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-8.3/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/config.py` & `frankAllSkyCam-8.3/frankAllSkyCam/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,18 @@
 
   #top, center (your name)
 top_center_x = 300
 top_center_y = 0
 
 
 [extra_text]
+# et_use = y if you want to add
 et_use= n
+# absolute path to your txt file
+et_data_file = /home/pi/frankAllSkyCam/extra_text.txt
 et_font_size = 18
 et_font_colorR = 0
 et_font_colorG = 255
 et_font_colorB = 255
 et_x_pos = 5
 et_y_pos = 80
```

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/crontab.py` & `frankAllSkyCam-8.3/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-8.3/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/exposurecalc.py` & `frankAllSkyCam-8.3/frankAllSkyCam/exposurecalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-8.3/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-8.3/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/logos.py` & `frankAllSkyCam-8.3/frankAllSkyCam/logos.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/sqmreader.py` & `frankAllSkyCam-8.3/frankAllSkyCam/sqmreader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/startrail.py` & `frankAllSkyCam-8.3/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-8.3/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-8.3/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-8.3/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-8.3/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam.egg-info/PKG-INFO` & `frankAllSkyCam-8.3/frankAllSkyCam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: frankAllSkyCam
-Version: 8.2
+Version: 8.3
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.2.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.3.tar.gz
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
 Keywords: AllSkyCamera,Astronomy,AllSky
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `frankAllSkyCam-8.2/frankAllSkyCam.egg-info/SOURCES.txt` & `frankAllSkyCam-8.3/frankAllSkyCam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.2/setup.py` & `frankAllSkyCam-8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'frankAllSkyCam',
   packages = ['frankAllSkyCam'],
-  version = '8.2',
+  version = '8.3',
   license='MIT',
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',
   author = 'Francesco Sferlazza',
   author_email = 'sferlazza@gmail.com',
   url = 'https://github.com/sferlix/frankAllSkyCam',
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.2.tar.gz',
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.3.tar.gz',
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],
   install_requires=[
           'pytz',
           'numpy',
           'pandas',
       ],
   classifiers=[
```

