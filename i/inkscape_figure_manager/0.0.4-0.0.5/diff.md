# Comparing `tmp/inkscape_figure_manager-0.0.4.tar.gz` & `tmp/inkscape_figure_manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_figure_manager-0.0.4.tar", last modified: Tue Jun  6 19:30:31 2023, max compression
+gzip compressed data, was "inkscape_figure_manager-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `inkscape_figure_manager-0.0.4.tar` & `inkscape_figure_manager-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.4/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/LICENSE
--rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.4/MANIFEST.in
--rw-r--r--   0        0        0      224 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/Pipfile
--rw-r--r--   0        0        0    28263 2023-04-19 04:06:10.275214 inkscape_figure_manager-0.0.4/Pipfile.lock
--rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.0.4/README.md
--rw-r--r--   0        0        0      709 2023-06-06 19:29:51.936382 inkscape_figure_manager-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/__init__.py
--rw-r--r--   0        0        0     7777 2023-06-06 19:20:41.239737 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/__main__.py
--rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/daemon.py
--rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/picker.py
--rw-r--r--   0        0        0     1989 2023-04-19 20:08:36.387298 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/template.svg
--rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher.py
--rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher_daemon.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/LICENSE
+-rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.5/MANIFEST.in
+-rw-r--r--   0        0        0      241 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/Pipfile
+-rw-r--r--   0        0        0    28498 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/Pipfile.lock
+-rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.0.5/README.md
+-rw-r--r--   0        0        0      709 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/__init__.py
+-rw-r--r--   0        0        0     8802 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/__main__.py
+-rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/daemon.py
+-rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/picker.py
+-rw-r--r--   0        0        0     1989 2023-04-19 20:08:36.387298 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/template.svg
+-rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher.py
+-rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher_daemon.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.0.5/PKG-INFO
```

### Comparing `inkscape_figure_manager-0.0.4/LICENSE` & `inkscape_figure_manager-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.4/Pipfile.lock` & `inkscape_figure_manager-0.0.5/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9657738095238096%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'2258572b51d7140287940b7690ce378854746866bac2ac9b827390880382c7e2'}}",*

 * * "'develop'": "{'astroid': {'hashes': "*

 * *              "['sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324', "*

 * *              "'sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f'], "*

 * *              "'version': '==2.15.5'}, 'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *            […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1b699c9777afa2c4cb203fcee9d933eb66c198762b977a51fa0e7c3be9b4459d"
+            "sha256": "2258572b51d7140287940b7690ce378854746866bac2ac9b827390880382c7e2"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
@@ -85,27 +85,27 @@
             "index": "pypi",
             "version": "==3.0.0"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:44224ad27c54d770233751315fa7f74c46fa3ee0fab7beef1065f99f09897efe",
-                "sha256:f11e74658da0f2a14a8d19776a8647900870a63de71db83713a8e77a6af52662"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.3"
+            "version": "==2.15.5"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
                 "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
                 "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
                 "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
@@ -190,35 +190,35 @@
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20.1"
         },
         "flit": {
             "hashes": [
-                "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
-                "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
+                "sha256:076c3aaba5ac24cf0ad3251f910900d95a08218e6bcb26f21fef1036cc4679ca",
+                "sha256:d75edf5eb324da20d53570a6a6f87f51e606eee8384925cd66a90611140844c7"
             ],
             "index": "pypi",
-            "version": "==3.8.0"
+            "version": "==3.9.0"
         },
         "flit-core": {
             "hashes": [
-                "sha256:64a29ec845164a6abe1136bf4bc5ae012bdfe758ed42fc7571a9059a7c80bd83",
-                "sha256:b305b30c99526df5e63d6022dd2310a0a941a187bd3884f4c8ef0418df6c39f3"
+                "sha256:72ad266176c4a3fcfab5f2930d76896059851240570ce9a98733b658cb786eba",
+                "sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==3.8.0"
+            "version": "==3.9.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -280,35 +280,43 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
-                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.0"
+            "version": "==3.5.1"
         },
         "pylint": {
             "hashes": [
-                "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
-                "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "index": "pypi",
-            "version": "==2.17.2"
+            "version": "==2.17.4"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
+        },
+        "setuptools": {
+            "hashes": [
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+            ],
+            "index": "pypi",
+            "version": "==67.8.0"
         },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
@@ -320,35 +328,35 @@
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c",
-                "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.7"
+            "version": "==0.11.8"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==4.5.0"
+            "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         },
         "wrapt": {
             "hashes": [
                 "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
                 "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
                 "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
                 "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
```

### Comparing `inkscape_figure_manager-0.0.4/README.md` & `inkscape_figure_manager-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.4/pyproject.toml` & `inkscape_figure_manager-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = 'inkscape_figure_manager'
-version = '0.0.4'
+version = '0.0.5'
 authors = [
   { name="Silas Waxter" },
   { name="Gille Castel" },
 ]
 description = "An API for managing inkscape figures."
 readme = "README.md"
 classifiers = [
```

### Comparing `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/__main__.py` & `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import os
 import subprocess
 import sys
 import warnings
 from pathlib import Path
 from shutil import copy
+import re
 
 import click
 from appdirs import user_config_dir
 
 from inkscape_figure_manager import picker
 from inkscape_figure_manager.watcher import EXPORT_EXTENSTION_NO_DOT, Watcher
 from inkscape_figure_manager.watcher_daemon import WatcherDaemon
@@ -18,15 +19,15 @@
 APPLICATION_NAME = "inkscape-figure-manager"
 # os-agnostic path to current user's configuration directory for this
 # application
 APP_USER_CONFIG_DIR = Path(user_config_dir(APPLICATION_NAME, False))
 TEMPLATE_FILE_PATH = APP_USER_CONFIG_DIR / 'template.svg'
 # error codes:
 ERROR_CODE_CREATED_FILE_ALREADY_EXISTS = 1
-ERROR_CODE_EDITED_FILE_PATH_DOES_NOT_EXIST = 2
+ERROR_CODE_EDIT_UNHANDLED_FILETYPE = 2
 ERROR_CODE_GIT_REPO_DNE = 3
 ERROR_CODE_BAD_DIR_TO_WATCH = 4
 
 logging.basicConfig(level=os.environ.get("LOGLEVEL", "INFO"))
 log = logging.getLogger('inkscape-figures')
 
 
@@ -154,37 +155,58 @@
     print(markdown_include_image_text(alternate_text,
                                       relative_figure_exported))
 
 
 @cli.command()
 @click.argument(
     'path',
-    default=os.getcwd(),
+    default="",
     type=click.Path(exists=True, file_okay=True, dir_okay=True),
 )
-def edit(path):
+@click.pass_context
+def edit(ctx, path):
     """
     Edits a figure.
 
-    PATH: The path to either a figure or a directory containing one or more
-    figures. When multiple figures are within the directory, a picker will
-    be used for selection. Default is the current working directory.
+    PATH: The path to a figure file, markdown file, or a directory.
+            Figure File:    Edit the figure passed.
+            Markdown File:  Edit a figure included in the markdown file
+                            (Use the picker if there is more than one)
+            Directory:      Edit a figure within the directory
+                            (use the picker if there is more than one)
     """
     path = Path(path).absolute()
 
-    # ensure path exists
-    if not path.exists():
-        eprint(f"The path does not exsist; received '{path}'.")
-        sys.exit(ERROR_CODE_EDITED_FILE_PATH_DOES_NOT_EXIST)
-
     selected_file = None
-    if path.is_file():
-        selected_file = path
+    while path.is_file():
+        if str(path).endswith('.svg'):
+            selected_file = path
+            break
+        if str(path).endswith('.md'):
+            # PARSE file for figures
+            markdown_file = open(str(path), "r")
+            markdown_content = markdown_file.read()
+            figures = re.findall("!\[.*?\]\((.*?)\.png\)", markdown_content)
+            for i in range(len(figures)):
+                figures[i] = figures[i] + ".svg"
+
+            returncode, index = picker.pick(figures)
+            if returncode != 0:
+                print("Picker returned with non-zero exit status.")
+                return
+            if index is ValueError:
+                print("A value error occurred while choosing with the picker.")
+                return
+            selected_file = str(path.parent) + "/" + figures[index]
+            break
+        eprint("Error: file is neither markdown nor figure.\n"
+            "Try 'python -m inkscape_figure_manager edit --help' for help.")
+        sys.exit(ERROR_CODE_EDIT_UNHANDLED_FILETYPE)
 
-    elif path.is_dir():
+    if path.is_dir():
         # Find svg files and sort them
         files = path.glob('*.svg')
         files = sorted(files, key=lambda f: f.stat().st_mtime, reverse=True)
 
         # if there is only one figure in the directory select it
         if len(files) == 1:
             selected_file = files[0]
@@ -197,15 +219,15 @@
                 print("Picker returned with non-zero exit status.")
                 return
             if index is ValueError:
                 print("A value error occurred while choosing with the picker.")
                 return
             selected_file = files[index]
 
-    WatcherDaemon.ensure_watch(selected_file.parent)
+    WatcherDaemon.ensure_watch(Path(selected_file).parent)
     open_inkscape(selected_file)
 
 
 def ensure_init():
     """
     Ensures the configuration directories and a figure template exist.
     """
```

### Comparing `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/daemon.py` & `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/picker.py` & `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/picker.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/template.svg` & `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/template.svg`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher.py` & `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.4/src/inkscape_figure_manager/watcher_daemon.py` & `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher_daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.4/PKG-INFO` & `inkscape_figure_manager-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_figure_manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: An API for managing inkscape figures.
 Author: Silas Waxter, Gille Castel
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Dist: click
 Requires-Dist: appdirs
```

