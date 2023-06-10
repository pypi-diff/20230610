# Comparing `tmp/nonebot_plugin_wol-1.0.1.tar.gz` & `tmp/nonebot_plugin_wol-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wol-1.0.1.tar", last modified: Sat Jun 10 01:29:55 2023, max compression
+gzip compressed data, was "nonebot_plugin_wol-1.0.3.tar", last modified: Sat Jun 10 01:42:13 2023, max compression
```

## Comparing `nonebot_plugin_wol-1.0.1.tar` & `nonebot_plugin_wol-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 01:29:55.188748 nonebot_plugin_wol-1.0.1/
--rw-rw-rw-   0        0        0    18429 2023-06-10 01:16:24.000000 nonebot_plugin_wol-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      675 2023-06-10 01:29:55.188748 nonebot_plugin_wol-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      114 2023-06-10 01:14:55.000000 nonebot_plugin_wol-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 01:29:55.182778 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/
--rw-rw-rw-   0        0        0     5675 2023-06-10 00:13:14.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/__init__.py
--rw-rw-rw-   0        0        0      175 2023-06-10 00:12:40.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/config.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:29:55.187310 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/img/
--rw-rw-rw-   0        0        0    21704 2023-06-10 00:15:22.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/img/help.png
--rw-rw-rw-   0        0        0      454 2023-06-10 00:45:27.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/pyproject.toml
--rw-rw-rw-   0        0        0     1126 2023-06-10 01:09:11.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:29:55.186308 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol.egg-info/
--rw-rw-rw-   0        0        0      675 2023-06-10 01:29:55.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-06-10 01:29:55.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 01:29:55.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-06-10 01:29:55.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-10 01:29:55.000000 nonebot_plugin_wol-1.0.1/nonebot_plugin_wol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      556 2023-06-10 01:28:32.000000 nonebot_plugin_wol-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 01:29:55.188748 nonebot_plugin_wol-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1125 2023-06-10 01:28:32.000000 nonebot_plugin_wol-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.682581 nonebot_plugin_wol-1.0.3/
+-rw-rw-rw-   0        0        0    18429 2023-06-10 01:16:24.000000 nonebot_plugin_wol-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-06-10 01:42:13.682581 nonebot_plugin_wol-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-06-10 01:14:55.000000 nonebot_plugin_wol-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.676119 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/
+-rw-rw-rw-   0        0        0     5675 2023-06-10 00:13:14.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-06-10 00:12:40.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/config.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.681528 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/img/
+-rw-rw-rw-   0        0        0    21704 2023-06-10 00:15:22.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/img/help.png
+drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.681528 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/tools/
+-rw-rw-rw-   0        0        0     2082 2023-06-10 00:12:40.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/tools/wol.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.680427 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2023-06-10 01:42:02.000000 nonebot_plugin_wol-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 01:42:13.682581 nonebot_plugin_wol-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-06-10 01:41:18.000000 nonebot_plugin_wol-1.0.3/setup.py
```

### Comparing `nonebot_plugin_wol-1.0.1/LICENSE` & `nonebot_plugin_wol-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wol-1.0.1/PKG-INFO` & `nonebot_plugin_wol-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_wol
-Version: 1.0.1
+Version: 1.0.3
 Summary: A WOL Nonebot plugin
 Home-page: https://github.com/twoonefour/nonebot_plugin_wol.git
 Author: TwoOnefour
 Author-email: TwoOnefour <lys214412@gmail.com>
 License: LICENSE
 Project-URL: Homepage, https://github.com/twoonefour/nonebot_plugin_wol
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/__init__.py` & `nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/img/help.png` & `nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/img/help.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wol-1.0.1/nonebot_plugin_wol/setup.py` & `nonebot_plugin_wol-1.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 MAJOR =1
 MINOR =0
-PATCH =0
+PATCH =3
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 fp = open('README.md',encoding="utf-8")
 setup(
     name="nonebot_plugin_wol",
     version=VERSION,
     author="TwoOnefour",
     author_email="lys214412@gmail.com",
     long_description_content_type="text/markdown",
     url='https://github.com/twoonefour/nonebot_plugin_wol.git',
     long_description=fp.read(),
     python_requires=">=3.6",
     install_requires=['ping3>=4.0.4', "nonebot2>=2.0.0rc2", "nb-cli>=0.6.8", "nonebot-plugin-apscheduler>=0.2.0"],
-    packages=["tools"],
-    license='Apache',
+    packages=find_packages(),
+    license='LICENSE',
     classifiers=[
-       'License :: OSI Approved :: Apache Software License',
+       'License :: GNU General Public License v2.0',
        'Natural Language :: English',
        'Operating System :: OS Independent',
        'Programming Language :: Python',
        'Programming Language :: Python :: 3.6',
        'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    package_data={'': ['pyproject.toml', "img/*.png"]},
+    package_data={'': ['pyproject.toml', "img/*.png", "tools/*.py"]},
     include_package_data=True
 
 )
 fp.close()
```

### Comparing `nonebot_plugin_wol-1.0.1/nonebot_plugin_wol.egg-info/PKG-INFO` & `nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-wol
-Version: 1.0.1
+Version: 1.0.3
 Summary: A WOL Nonebot plugin
 Home-page: https://github.com/twoonefour/nonebot_plugin_wol.git
 Author: TwoOnefour
 Author-email: TwoOnefour <lys214412@gmail.com>
 License: LICENSE
 Project-URL: Homepage, https://github.com/twoonefour/nonebot_plugin_wol
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot_plugin_wol-1.0.1/pyproject.toml` & `nonebot_plugin_wol-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "nonebot_plugin_wol"
-version = "1.0.1"
+version = "1.0.3"
 authors = [
-  { name="TwoOnefour", email="lys214412@gmail.com" },
+  { name="TwoOnefour", email="lys214412@gmail.com"},
 ]
 description = "A WOL Nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

