# Comparing `tmp/morsecode_enhanced-1.0.1.tar.gz` & `tmp/morsecode_enhanced-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morsecode_enhanced-1.0.1.tar", last modified: Sat Jun 10 10:52:10 2023, max compression
+gzip compressed data, was "morsecode_enhanced-1.0.2.tar", last modified: Sat Jun 10 11:05:41 2023, max compression
```

## Comparing `morsecode_enhanced-1.0.1.tar` & `morsecode_enhanced-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 10:52:10.241866 morsecode_enhanced-1.0.1/
--rw-rw-rw-   0        0        0     1055 2023-06-10 08:21:58.000000 morsecode_enhanced-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1977 2023-06-10 10:52:10.239870 morsecode_enhanced-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1235 2023-06-10 10:37:47.000000 morsecode_enhanced-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 10:52:10.185868 morsecode_enhanced-1.0.1/morsecode_enhanced/
--rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.1/morsecode_enhanced/__init__.py
--rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.1/morsecode_enhanced/morsecode_enhanced.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:52:10.233885 morsecode_enhanced-1.0.1/morsecode_enhanced.egg-info/
--rw-rw-rw-   0        0        0     1977 2023-06-10 10:52:09.000000 morsecode_enhanced-1.0.1/morsecode_enhanced.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-10 10:52:09.000000 morsecode_enhanced-1.0.1/morsecode_enhanced.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 10:52:09.000000 morsecode_enhanced-1.0.1/morsecode_enhanced.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-10 10:52:09.000000 morsecode_enhanced-1.0.1/morsecode_enhanced.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 10:52:10.242931 morsecode_enhanced-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-06-10 10:45:59.000000 morsecode_enhanced-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 11:05:41.114910 morsecode_enhanced-1.0.2/
+-rw-rw-rw-   0        0        0     1055 2023-06-10 08:21:58.000000 morsecode_enhanced-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1977 2023-06-10 11:05:41.110948 morsecode_enhanced-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1235 2023-06-10 10:37:47.000000 morsecode_enhanced-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 11:05:41.072060 morsecode_enhanced-1.0.2/morsecode_enhanced/
+-rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.2/morsecode_enhanced/__init__.py
+-rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.2/morsecode_enhanced/morsecode_enhanced.py
+drwxrwxrwx   0        0        0        0 2023-06-10 11:05:41.105932 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/
+-rw-rw-rw-   0        0        0     1977 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 11:05:41.114910 morsecode_enhanced-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-06-10 11:05:32.000000 morsecode_enhanced-1.0.2/setup.py
```

### Comparing `morsecode_enhanced-1.0.1/LICENSE.txt` & `morsecode_enhanced-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morsecode_enhanced-1.0.1/PKG-INFO` & `morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: morsecode_enhanced
-Version: 1.0.1
+Name: morsecode-enhanced
+Version: 1.0.2
 Summary: A package for encoding and decoding Morse code.
 Home-page: https://github.com/danysrour/morsecode_enhanced
 Author: Dany Srour
 Author-email: dany.srour@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morsecode_enhanced-1.0.1/README.md` & `morsecode_enhanced-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `morsecode_enhanced-1.0.1/morsecode_enhanced/__init__.py` & `morsecode_enhanced-1.0.2/morsecode_enhanced/__init__.py`

 * *Files identical despite different names*

### Comparing `morsecode_enhanced-1.0.1/morsecode_enhanced/morsecode_enhanced.py` & `morsecode_enhanced-1.0.2/morsecode_enhanced/morsecode_enhanced.py`

 * *Files identical despite different names*

### Comparing `morsecode_enhanced-1.0.1/morsecode_enhanced.egg-info/PKG-INFO` & `morsecode_enhanced-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: morsecode-enhanced
-Version: 1.0.1
+Name: morsecode_enhanced
+Version: 1.0.2
 Summary: A package for encoding and decoding Morse code.
 Home-page: https://github.com/danysrour/morsecode_enhanced
 Author: Dany Srour
 Author-email: dany.srour@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morsecode_enhanced-1.0.1/setup.py` & `morsecode_enhanced-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='morsecode_enhanced',
-    version='1.0.1',
+    version='1.0.2',
     author='Dany Srour',
     author_email='dany.srour@gmail.com',
     description='A package for encoding and decoding Morse code.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/danysrour/morsecode_enhanced',
     packages=['morsecode_enhanced'],
@@ -16,10 +16,13 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
+    install_requires=[
+            'playsound>=1.3.0',
+    ],
     python_requires='>=3.6',
     exclude_package_data={'': ['tests/*']},
 )
```

