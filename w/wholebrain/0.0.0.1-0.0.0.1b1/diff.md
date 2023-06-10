# Comparing `tmp/wholebrain-0.0.0.1.tar.gz` & `tmp/wholebrain-0.0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wholebrain-0.0.0.1.tar", last modified: Sat Jun 10 05:42:37 2023, max compression
+gzip compressed data, was "wholebrain-0.0.0.1b1.tar", last modified: Sat Jun 10 05:50:59 2023, max compression
```

## Comparing `wholebrain-0.0.0.1.tar` & `wholebrain-0.0.0.1b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwx---   0 benju     (1000) jlab_mounts  (1001)        0 2023-06-10 05:42:37.896510 wholebrain-0.0.0.1/
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)    32814 2023-01-28 14:47:21.000000 wholebrain-0.0.0.1/LICENSE.md
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      247 2023-06-10 05:42:37.889194 wholebrain-0.0.0.1/PKG-INFO
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2289 2023-01-25 16:04:56.000000 wholebrain-0.0.0.1/README.md
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)       38 2023-06-10 05:42:37.920022 wholebrain-0.0.0.1/setup.cfg
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      649 2023-01-24 16:51:58.000000 wholebrain-0.0.0.1/setup.py
-drwxrwx---   0 benju     (1000) jlab_mounts  (1001)        0 2023-06-10 05:42:37.559260 wholebrain-0.0.0.1/wholebrain/
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      121 2023-02-17 08:07:25.000000 wholebrain-0.0.0.1/wholebrain/__init__.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2973 2023-02-20 09:10:54.000000 wholebrain-0.0.0.1/wholebrain/cluster.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     1179 2023-01-19 22:27:48.000000 wholebrain-0.0.0.1/wholebrain/decompose.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)    19196 2023-04-03 12:30:40.000000 wholebrain-0.0.0.1/wholebrain/legacy.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)    16021 2023-02-17 07:52:47.000000 wholebrain-0.0.0.1/wholebrain/regression.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2933 2023-04-03 12:30:40.000000 wholebrain-0.0.0.1/wholebrain/spatial.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     1698 2023-02-17 07:52:47.000000 wholebrain-0.0.0.1/wholebrain/stats.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     8741 2023-04-03 12:30:40.000000 wholebrain-0.0.0.1/wholebrain/traces.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     4945 2023-04-03 12:29:57.000000 wholebrain-0.0.0.1/wholebrain/visualize.py
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     3069 2023-02-17 07:52:47.000000 wholebrain-0.0.0.1/wholebrain/xpu.py
-drwxrwx---   0 benju     (1000) jlab_mounts  (1001)        0 2023-06-10 05:42:37.830845 wholebrain-0.0.0.1/wholebrain.egg-info/
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      247 2023-06-10 05:42:36.000000 wholebrain-0.0.0.1/wholebrain.egg-info/PKG-INFO
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      418 2023-06-10 05:42:36.000000 wholebrain-0.0.0.1/wholebrain.egg-info/SOURCES.txt
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)        1 2023-06-10 05:42:36.000000 wholebrain-0.0.0.1/wholebrain.egg-info/dependency_links.txt
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)       39 2023-06-10 05:42:36.000000 wholebrain-0.0.0.1/wholebrain.egg-info/requires.txt
--rwxrwx---   0 benju     (1000) jlab_mounts  (1001)       11 2023-06-10 05:42:36.000000 wholebrain-0.0.0.1/wholebrain.egg-info/top_level.txt
+drwxrwx---   0 benju     (1000) jlab_mounts  (1001)        0 2023-06-10 05:50:59.424173 wholebrain-0.0.0.1b1/
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)    32814 2023-01-28 14:47:21.000000 wholebrain-0.0.0.1b1/LICENSE.md
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2579 2023-06-10 05:50:59.412667 wholebrain-0.0.0.1b1/PKG-INFO
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2289 2023-01-25 16:04:56.000000 wholebrain-0.0.0.1b1/README.md
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)       38 2023-06-10 05:50:59.458913 wholebrain-0.0.0.1b1/setup.cfg
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      754 2023-06-10 05:50:55.000000 wholebrain-0.0.0.1b1/setup.py
+drwxrwx---   0 benju     (1000) jlab_mounts  (1001)        0 2023-06-10 05:50:59.048907 wholebrain-0.0.0.1b1/wholebrain/
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      121 2023-02-17 08:07:25.000000 wholebrain-0.0.0.1b1/wholebrain/__init__.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2973 2023-02-20 09:10:54.000000 wholebrain-0.0.0.1b1/wholebrain/cluster.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     1179 2023-01-19 22:27:48.000000 wholebrain-0.0.0.1b1/wholebrain/decompose.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)    19196 2023-04-03 12:30:40.000000 wholebrain-0.0.0.1b1/wholebrain/legacy.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)    16021 2023-02-17 07:52:47.000000 wholebrain-0.0.0.1b1/wholebrain/regression.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2933 2023-04-03 12:30:40.000000 wholebrain-0.0.0.1b1/wholebrain/spatial.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     1698 2023-02-17 07:52:47.000000 wholebrain-0.0.0.1b1/wholebrain/stats.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     8741 2023-04-03 12:30:40.000000 wholebrain-0.0.0.1b1/wholebrain/traces.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     4945 2023-04-03 12:29:57.000000 wholebrain-0.0.0.1b1/wholebrain/visualize.py
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     3069 2023-02-17 07:52:47.000000 wholebrain-0.0.0.1b1/wholebrain/xpu.py
+drwxrwx---   0 benju     (1000) jlab_mounts  (1001)        0 2023-06-10 05:50:59.341192 wholebrain-0.0.0.1b1/wholebrain.egg-info/
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)     2579 2023-06-10 05:50:58.000000 wholebrain-0.0.0.1b1/wholebrain.egg-info/PKG-INFO
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)      418 2023-06-10 05:50:58.000000 wholebrain-0.0.0.1b1/wholebrain.egg-info/SOURCES.txt
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)        1 2023-06-10 05:50:58.000000 wholebrain-0.0.0.1b1/wholebrain.egg-info/dependency_links.txt
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)       39 2023-06-10 05:50:58.000000 wholebrain-0.0.0.1b1/wholebrain.egg-info/requires.txt
+-rwxrwx---   0 benju     (1000) jlab_mounts  (1001)       11 2023-06-10 05:50:58.000000 wholebrain-0.0.0.1b1/wholebrain.egg-info/top_level.txt
```

### Comparing `wholebrain-0.0.0.1/LICENSE.md` & `wholebrain-0.0.0.1b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/README.md` & `wholebrain-0.0.0.1b1/README.md`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/setup.py` & `wholebrain-0.0.0.1b1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 # python setup.py sdist bdist_wheel
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='wholebrain',
-    version='0.0.0.1',
+    version='0.0.0.1b1',
     description='Population activity analysis',
+    long_description=open("README.md", 'r').read(),
+    long_description_content_type='text/markdown',
     author='jlab.berlin',
     url='https://github.com/danionella/wholebrain',
     packages=[
         'wholebrain',
     ],  #find_packages(include=['exampleproject', 'exampleproject.*']),
     license='mit',
     python_requires='>=3.8',
```

### Comparing `wholebrain-0.0.0.1/wholebrain/cluster.py` & `wholebrain-0.0.0.1b1/wholebrain/cluster.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/decompose.py` & `wholebrain-0.0.0.1b1/wholebrain/decompose.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/legacy.py` & `wholebrain-0.0.0.1b1/wholebrain/legacy.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/regression.py` & `wholebrain-0.0.0.1b1/wholebrain/regression.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/spatial.py` & `wholebrain-0.0.0.1b1/wholebrain/spatial.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/stats.py` & `wholebrain-0.0.0.1b1/wholebrain/stats.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/traces.py` & `wholebrain-0.0.0.1b1/wholebrain/traces.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/visualize.py` & `wholebrain-0.0.0.1b1/wholebrain/visualize.py`

 * *Files identical despite different names*

### Comparing `wholebrain-0.0.0.1/wholebrain/xpu.py` & `wholebrain-0.0.0.1b1/wholebrain/xpu.py`

 * *Files identical despite different names*

