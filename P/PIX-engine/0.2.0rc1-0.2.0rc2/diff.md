# Comparing `tmp/pix_engine-0.2.0rc1.tar.gz` & `tmp/PIX-engine-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "PIX-engine-0.2.0rc2.tar", last modified: Sat Jun 10 16:16:09 2023, max compression
```

## Comparing `pix_engine-0.2.0rc1.tar` & `PIX-engine-0.2.0rc2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/requirements.txt
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.github/workflows/pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/pix/__init__.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/pix/engine.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:16:09.424852 PIX-engine-0.2.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-10 16:15:58.000000 PIX-engine-0.2.0rc2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:16:09.424852 PIX-engine-0.2.0rc2/PIX_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-10 16:16:09.000000 PIX-engine-0.2.0rc2/PIX_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-10 16:16:09.000000 PIX-engine-0.2.0rc2/PIX_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:16:09.000000 PIX-engine-0.2.0rc2/PIX_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 16:16:09.000000 PIX-engine-0.2.0rc2/PIX_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-10 16:16:09.000000 PIX-engine-0.2.0rc2/PIX_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-10 16:16:09.424852 PIX-engine-0.2.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-10 16:15:58.000000 PIX-engine-0.2.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 16:15:58.000000 PIX-engine-0.2.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:16:09.424852 PIX-engine-0.2.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-10 16:15:58.000000 PIX-engine-0.2.0rc2/setup.py
```

### Comparing `pix_engine-0.2.0rc1/LICENSE` & `PIX-engine-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_engine-0.2.0rc1/PKG-INFO` & `PIX-engine-0.2.0rc2/PIX_engine.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: PIX-engine
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Terminal game engine that is community supported and open source
-Project-URL: Homepage, https://github.com/Retaki/PIX
-Project-URL: Bug Tracker, https://github.com/Retaki/PIX/issues
-Project-URL: Documentation, https://pix-five.vercel.app/
-Author-email: TVRework <boxeigit@gmail.com>
-License-File: LICENSE
+Home-page: https://github.com/Retaki/PIX
+Author: Retaki
+Author-email: boxeigit@gmail.com
+License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # PIX
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/TVRework/PIX?quickstart=1)
 
 PIX is a **python terminal game engine** that is community supported and open source. Develop **games 🎮** _(and applications)_ with **ease.**
 
 ## Installation
 
 We offer two different versions. **Production Release** is the currently supported version while **Canary** is all RCs, alphas, and betas.
 
-### Production Release
+### Release
 
 ```shell
-pip install PIX-engine==0.1.0
+pip install PIX-engine
 ```
 
 ### Canary
+
 Warning! This version may be unstable, not working as intented, and more. Please leave any feedback you have on our issues board.
 
 ```shell
-pip install PIX-engine==0.1.0
+pip install PIX-engine==0.2.0rc1
 ```
 
 **Or,** clone this repoisitory to edit and contribute towards PIX's development and open source.
```

