# Comparing `tmp/pynball-1.5.6.tar.gz` & `tmp/pynball-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynball-1.5.6.tar", last modified: Sun May 28 12:44:49 2023, max compression
+gzip compressed data, was "pynball-1.5.7.tar", last modified: Sat Jun 10 19:37:39 2023, max compression
```

## Comparing `pynball-1.5.6.tar` & `pynball-1.5.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.126065 pynball-1.5.6/
--rw-rw-rw-   0        0        0      140 2023-04-19 21:02:11.000000 pynball-1.5.6/AUTHORS.md
--rw-rw-rw-   0        0        0     7598 2023-05-28 12:44:37.000000 pynball-1.5.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-04-09 16:05:23.000000 pynball-1.5.6/LICENSE
--rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0    12613 2023-05-28 12:44:49.126065 pynball-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0    11282 2023-04-19 21:46:58.000000 pynball-1.5.6/README.md
--rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.6/pyproject.toml
--rw-rw-rw-   0        0        0     1571 2023-05-28 12:44:49.126065 pynball-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:30:25.000000 pynball-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.016680 pynball-1.5.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.047935 pynball-1.5.6/src/pynball/
--rw-rw-rw-   0        0        0      293 2023-05-28 12:44:38.000000 pynball-1.5.6/src/pynball/__init__.py
--rw-rw-rw-   0        0        0    31371 2023-05-28 11:13:49.000000 pynball-1.5.6/src/pynball/pynball.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.063553 pynball-1.5.6/src/pynball.egg-info/
--rw-rw-rw-   0        0        0    12613 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-05-28 12:44:49.000000 pynball-1.5.6/src/pynball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.110432 pynball-1.5.6/tests/
--rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.6/tests/test__check_pyenv.py
--rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.6/tests/test__check_virtual_env.py
--rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.6/tests/test__execute.py
--rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.6/tests/test__get_pynball.py
--rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.6/tests/test__message.py
--rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.6/tests/test__set_get_del_env.py
--rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.6/tests/test__set_pynball.py
--rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.6/tests/test_add.py
--rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.6/tests/test_delete.py
--rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.6/tests/test_lsproject.py
--rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.6/tests/test_mkproject.py
--rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.6/tests/test_rmproject.py
--rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.6/tests/test_version.py
--rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.6/tests/test_versions.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:37:39.467525 pynball-1.5.7/
+-rw-rw-rw-   0        0        0      140 2023-04-19 21:02:11.000000 pynball-1.5.7/AUTHORS.md
+-rw-rw-rw-   0        0        0     7911 2023-06-10 19:37:26.000000 pynball-1.5.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-04-09 16:05:23.000000 pynball-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    13171 2023-06-10 19:37:39.468527 pynball-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11315 2023-06-10 19:12:02.000000 pynball-1.5.7/README.md
+-rw-rw-rw-   0        0        0     2159 2023-06-10 18:44:20.000000 pynball-1.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0     2096 2023-06-10 19:37:39.473527 pynball-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:30:25.000000 pynball-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:37:39.351532 pynball-1.5.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 19:37:39.389540 pynball-1.5.7/src/pynball/
+-rw-rw-rw-   0        0        0      293 2023-06-10 19:37:26.000000 pynball-1.5.7/src/pynball/__init__.py
+-rw-rw-rw-   0        0        0    31371 2023-05-28 11:13:49.000000 pynball-1.5.7/src/pynball/pynball.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:37:39.408532 pynball-1.5.7/src/pynball.egg-info/
+-rw-rw-rw-   0        0        0    13171 2023-06-10 19:37:39.000000 pynball-1.5.7/src/pynball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-06-10 19:37:39.000000 pynball-1.5.7/src/pynball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 19:37:39.000000 pynball-1.5.7/src/pynball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-10 19:37:39.000000 pynball-1.5.7/src/pynball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-06-10 19:37:39.000000 pynball-1.5.7/src/pynball.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 19:37:39.000000 pynball-1.5.7/src/pynball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 19:37:39.465531 pynball-1.5.7/tests/
+-rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.7/tests/test__check_pyenv.py
+-rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.7/tests/test__check_virtual_env.py
+-rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.7/tests/test__execute.py
+-rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.7/tests/test__get_pynball.py
+-rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.7/tests/test__message.py
+-rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.7/tests/test__set_get_del_env.py
+-rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.7/tests/test__set_pynball.py
+-rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.7/tests/test_add.py
+-rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.7/tests/test_delete.py
+-rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.7/tests/test_lsproject.py
+-rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.7/tests/test_mkproject.py
+-rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.7/tests/test_rmproject.py
+-rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.7/tests/test_version.py
+-rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.7/tests/test_versions.py
```

### Comparing `pynball-1.5.6/CHANGELOG.md` & `pynball-1.5.7/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.7 (2023-06-10)
+### Fix
+* Tasks invoke script ([`433d68b`](https://github.com/Stephen-RA-King/pynball/commit/433d68b060afd8f492b54e65328bd5ed83375a8b))
+
+### Documentation
+* Add citation badge ([`de25c9d`](https://github.com/Stephen-RA-King/pynball/commit/de25c9dcba347dce13c98c7ea6fdcdb1ff1ec7c2))
+
 ## v1.5.6 (2023-05-28)
 
 
 ## v1.5.5 (2023-04-21)
 ### Fix
 * Shebang for version 3 env ([`57d4c92`](https://github.com/Stephen-RA-King/pynball/commit/57d4c927521b73c715f5f574fe208b2f9966f878))
```

### Comparing `pynball-1.5.6/LICENSE` & `pynball-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/PKG-INFO` & `pynball-1.5.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.6
-Summary: Utility command line tool to manage python versions
+Version: 1.5.7
+Summary: Utility command line tool to manage python versions and virtual environments
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
-Keywords: utility
+Project-URL: documentation, https://pynamer.readthedocs.io/en/latest/
+Project-URL: Release Notes, https://github.com/Stephen-RA-King/pynamer/releases
+Project-URL: Source Code, https://github.com/Stephen-RA-King/pynamer/
+Project-URL: Issue Tracker, https://github.com/Stephen-RA-King/pynamer/issues
+Keywords: python-version-management,python-version-manager,virtualenv-manager,python-version-selector,python-versions,python-environment
 Platform: windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.md
 
 # Pynball
 
 _**Centralized management and utilization of all your Python versions, installations and virtual environments.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
@@ -59,18 +64,18 @@
 Or you may have a mixture of installations including pyenv, custom installations,
 system installations etc. Pynball can make leveraging such environments a lot easier.
 
 ## Features
 
 ---
 
-- Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
-- Easily create Virtual Environments using any Python version.
-- Track which virtual environments have which Python versions and tox versions.
-- Quickly change the System interpreter
+-   Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
+-   Easily create Virtual Environments using any Python version.
+-   Track which virtual environments have which Python versions and tox versions.
+-   Quickly change the System interpreter
 
 ## Pre Installation Requirements
 
 ---
 
 #### Minimum Requirements
 
@@ -244,18 +249,17 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
-- [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
-- [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
-- [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
-- [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
+-   [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**][wiki]
 
 ## Meta
 
 ---
 
@@ -267,14 +271,16 @@
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
+[![DOI](https://zenodo.org/badge/464560536.svg)](https://zenodo.org/badge/latestdoi/464560536)
+
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
```

### Comparing `pynball-1.5.6/README.md` & `pynball-1.5.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 Or you may have a mixture of installations including pyenv, custom installations,
 system installations etc. Pynball can make leveraging such environments a lot easier.
 
 ## Features
 
 ---
 
-- Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
-- Easily create Virtual Environments using any Python version.
-- Track which virtual environments have which Python versions and tox versions.
-- Quickly change the System interpreter
+-   Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
+-   Easily create Virtual Environments using any Python version.
+-   Track which virtual environments have which Python versions and tox versions.
+-   Quickly change the System interpreter
 
 ## Pre Installation Requirements
 
 ---
 
 #### Minimum Requirements
 
@@ -215,18 +215,17 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
-- [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
-- [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
-- [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
-- [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
+-   [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**][wiki]
 
 ## Meta
 
 ---
 
@@ -238,14 +237,16 @@
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
+[![DOI](https://zenodo.org/badge/464560536.svg)](https://zenodo.org/badge/latestdoi/464560536)
+
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
```

### Comparing `pynball-1.5.6/pyproject.toml` & `pynball-1.5.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool]
 [tool.black]
 line-length = 88
 
-[tool.pytest.ini_options]
-# https://docs.pytest.org/en/6.2.x/reference.html?highlight=minversion#configuration-options
-minversion = "6.0"
-testpaths = [
-    "tests",
-]
+
 
 [tool.isort]
 import_heading_stdlib = "Core Library modules"
 import_heading_thirdparty = "Third party modules"
 import_heading_firstparty = "First party modules"
 import_heading_localfolder = "Local modules"
 include_trailing_comma = true
@@ -48,16 +43,22 @@
 warn_unused_ignores = true
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_configs = true
 disallow_untyped_calls = false
 disallow_incomplete_defs = true
 follow_imports = "skip"
-html_report = "mypy-report"
+html_report = "reports/mypy"
+cache_dir = 'cache/.mypy_cache'
 mypy_path = "typeshed/pyi:typeshed/imports"
+exclude = [
+    '^tests/[\w]*.py$',
+    '^tools/[\w]*.py$',
+    '^tasks.py$'
+]
 
 [tool.semantic_release]
 version_variable = [
     "src/pynball/__init__.py:__version__",
     "docs/conf.py:version",
 ]
 branch = "main"
```

### Comparing `pynball-1.5.6/setup.cfg` & `pynball-1.5.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -10,90 +10,122 @@
 00000090: 5374 6570 6865 6e20 5220 4120 4b69 6e67  Stephen R A King
 000000a0: 0d0a 6d61 696e 7461 696e 6572 5f65 6d61  ..maintainer_ema
 000000b0: 696c 203d 2073 6b69 6e67 2e67 6974 6875  il = sking.githu
 000000c0: 6240 676d 6169 6c2e 636f 6d0d 0a64 6573  b@gmail.com..des
 000000d0: 6372 6970 7469 6f6e 203d 2055 7469 6c69  cription = Utili
 000000e0: 7479 2063 6f6d 6d61 6e64 206c 696e 6520  ty command line 
 000000f0: 746f 6f6c 2074 6f20 6d61 6e61 6765 2070  tool to manage p
-00000100: 7974 686f 6e20 7665 7273 696f 6e73 0d0a  ython versions..
-00000110: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000120: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000130: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-00000140: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000150: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000160: 6e0d 0a6b 6579 776f 7264 7320 3d20 7574  n..keywords = ut
-00000170: 696c 6974 792c 0d0a 706c 6174 666f 726d  ility,..platform
-00000180: 7320 3d20 7769 6e64 6f77 730d 0a75 726c  s = windows..url
-00000190: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-000001a0: 622e 636f 6d2f 7374 6570 6865 6e2d 7261  b.com/stephen-ra
-000001b0: 2d6b 696e 672f 7079 6e62 616c 6c0d 0a64  -king/pynball..d
-000001c0: 6f77 6e6c 6f61 645f 7572 6c20 3d20 0d0a  ownload_url = ..
-000001d0: 6c69 6365 6e73 6520 3d20 4d49 540d 0a63  license = MIT..c
-000001e0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-000001f0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000200: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
-00000210: 7469 6f6e 2f53 7461 626c 650d 0a09 456e  tion/Stable...En
-00000220: 7669 726f 6e6d 656e 7420 3a3a 2043 6f6e  vironment :: Con
-00000230: 736f 6c65 0d0a 0949 6e74 656e 6465 6420  sole...Intended 
-00000240: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000250: 6c6f 7065 7273 0d0a 094f 7065 7261 7469  lopers...Operati
-00000260: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
-00000270: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
-00000280: 730d 0a09 546f 7069 6320 3a3a 2053 7973  s...Topic :: Sys
-00000290: 7465 6d20 3a3a 2049 6e73 7461 6c6c 6174  tem :: Installat
-000002a0: 696f 6e2f 5365 7475 700d 0a09 4e61 7475  ion/Setup...Natu
-000002b0: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
-000002c0: 456e 676c 6973 680d 0a09 5072 6f67 7261  English...Progra
-000002d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002e0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-000002f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000300: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000310: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
-00000320: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000330: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000340: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
-00000350: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000360: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
-00000370: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000380: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000390: 332e 3130 0d0a 0d0a 5b6f 7074 696f 6e73  3.10....[options
-000003a0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-000003b0: 200d 0a09 3d73 7263 0d0a 7061 636b 6167   ...=src..packag
-000003c0: 6573 203d 2066 696e 643a 0d0a 696e 636c  es = find:..incl
-000003d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-000003e0: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
-000003f0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
-00000400: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000410: 6573 203d 200d 0a09 636c 6963 6b3e 3d38  es = ...click>=8
-00000420: 2e31 2e33 2c3c 382e 322e 300d 0a09 7079  .1.3,<8.2.0...py
-00000430: 7468 6f6e 2d6d 6167 6963 2d62 696e 3d3d  thon-magic-bin==
-00000440: 302e 342e 3134 3b70 6c61 7466 6f72 6d5f  0.4.14;platform_
-00000450: 7379 7374 656d 3d3d 2757 696e 646f 7773  system=='Windows
-00000460: 270d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  '....[options.pa
-00000470: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000480: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
-00000490: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-000004a0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-000004b0: 6970 7473 203d 200d 0a09 7079 6e62 616c  ipts = ...pynbal
-000004c0: 6c20 3d20 7079 6e62 616c 6c2e 7079 6e62  l = pynball.pynb
-000004d0: 616c 6c3a 636c 690d 0a0d 0a5b 666c 616b  all:cli....[flak
-000004e0: 6538 5d0d 0a64 6f63 7374 7269 6e67 2d63  e8]..docstring-c
-000004f0: 6f6e 7665 6e74 696f 6e20 3d20 6e75 6d70  onvention = nump
-00000500: 790d 0a6d 6178 2d63 6f6d 706c 6578 6974  y..max-complexit
-00000510: 7920 3d20 3138 0d0a 6d61 782d 6c69 6e65  y = 18..max-line
-00000520: 2d6c 656e 6774 6820 3d20 3838 0d0a 7365  -length = 88..se
-00000530: 6c65 6374 203d 2042 2c20 4239 2c20 432c  lect = B, B9, C,
-00000540: 2044 2c20 452c 2046 2c20 4e2c 2057 0d0a   D, E, F, N, W..
-00000550: 6578 636c 7564 6520 3d20 7465 7374 732f  exclude = tests/
-00000560: 2a2c 2e74 6f78 2f2a 2c2e 6e6f 782f 2a2c  *,.tox/*,.nox/*,
-00000570: 646f 6373 2f2a 2c2e 6769 742f 2a2c 2e67  docs/*,.git/*,.g
-00000580: 6974 6875 622f 2a0d 0a69 676e 6f72 6520  ithub/*..ignore 
-00000590: 3d20 0d0a 0945 3230 332c 0d0a 0957 3530  = ...E203,...W50
-000005a0: 332c 0d0a 7065 722d 6669 6c65 2d69 676e  3,..per-file-ign
-000005b0: 6f72 6573 203d 200d 0a09 5f5f 696e 6974  ores = ...__init
-000005c0: 5f5f 2e70 793a 4634 3031 0d0a 0970 6174  __.py:F401...pat
-000005d0: 686d 6167 6963 2e70 793a 4634 3031 0d0a  hmagic.py:F401..
-000005e0: 0974 6573 745f 7079 6e62 616c 6c2e 7079  .test_pynball.py
-000005f0: 3a46 3430 310d 0a0d 0a5b 6567 675f 696e  :F401....[egg_in
-00000600: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000610: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000620: 0a0d 0a                                  ...
+00000100: 7974 686f 6e20 7665 7273 696f 6e73 2061  ython versions a
+00000110: 6e64 2076 6972 7475 616c 2065 6e76 6972  nd virtual envir
+00000120: 6f6e 6d65 6e74 730d 0a6c 6f6e 675f 6465  onments..long_de
+00000130: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000140: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+00000150: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+00000160: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000170: 742f 6d61 726b 646f 776e 0d0a 6b65 7977  t/markdown..keyw
+00000180: 6f72 6473 203d 2070 7974 686f 6e2d 7665  ords = python-ve
+00000190: 7273 696f 6e2d 6d61 6e61 6765 6d65 6e74  rsion-management
+000001a0: 2c70 7974 686f 6e2d 7665 7273 696f 6e2d  ,python-version-
+000001b0: 6d61 6e61 6765 722c 7669 7274 7561 6c65  manager,virtuale
+000001c0: 6e76 2d6d 616e 6167 6572 2c70 7974 686f  nv-manager,pytho
+000001d0: 6e2d 7665 7273 696f 6e2d 7365 6c65 6374  n-version-select
+000001e0: 6f72 2c70 7974 686f 6e2d 7665 7273 696f  or,python-versio
+000001f0: 6e73 2c70 7974 686f 6e2d 656e 7669 726f  ns,python-enviro
+00000200: 6e6d 656e 740d 0a70 6c61 7466 6f72 6d73  nment..platforms
+00000210: 203d 2077 696e 646f 7773 0d0a 7572 6c20   = windows..url 
+00000220: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000230: 2e63 6f6d 2f73 7465 7068 656e 2d72 612d  .com/stephen-ra-
+00000240: 6b69 6e67 2f70 796e 6261 6c6c 0d0a 646f  king/pynball..do
+00000250: 776e 6c6f 6164 5f75 726c 203d 200d 0a6c  wnload_url = ..l
+00000260: 6963 656e 7365 203d 204d 4954 0d0a 6c69  icense = MIT..li
+00000270: 6365 6e73 655f 6669 6c65 7320 3d20 4c49  cense_files = LI
+00000280: 4345 4e53 450d 0a70 726f 6a65 6374 5f75  CENSE..project_u
+00000290: 726c 7320 3d20 0d0a 0964 6f63 756d 656e  rls = ...documen
+000002a0: 7461 7469 6f6e 203d 2068 7474 7073 3a2f  tation = https:/
+000002b0: 2f70 796e 616d 6572 2e72 6561 6474 6865  /pynamer.readthe
+000002c0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+000002d0: 742f 0d0a 0952 656c 6561 7365 204e 6f74  t/...Release Not
+000002e0: 6573 203d 2068 7474 7073 3a2f 2f67 6974  es = https://git
+000002f0: 6875 622e 636f 6d2f 5374 6570 6865 6e2d  hub.com/Stephen-
+00000300: 5241 2d4b 696e 672f 7079 6e61 6d65 722f  RA-King/pynamer/
+00000310: 7265 6c65 6173 6573 0d0a 0953 6f75 7263  releases...Sourc
+00000320: 6520 436f 6465 203d 2068 7474 7073 3a2f  e Code = https:/
+00000330: 2f67 6974 6875 622e 636f 6d2f 5374 6570  /github.com/Step
+00000340: 6865 6e2d 5241 2d4b 696e 672f 7079 6e61  hen-RA-King/pyna
+00000350: 6d65 722f 0d0a 0949 7373 7565 2054 7261  mer/...Issue Tra
+00000360: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+00000370: 6974 6875 622e 636f 6d2f 5374 6570 6865  ithub.com/Stephe
+00000380: 6e2d 5241 2d4b 696e 672f 7079 6e61 6d65  n-RA-King/pyname
+00000390: 722f 6973 7375 6573 0d0a 636c 6173 7369  r/issues..classi
+000003a0: 6669 6572 7320 3d20 0d0a 0944 6576 656c  fiers = ...Devel
+000003b0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+000003c0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+000003d0: 5374 6162 6c65 0d0a 0945 6e76 6972 6f6e  Stable...Environ
+000003e0: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650d  ment :: Console.
+000003f0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+00000400: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000410: 730d 0a09 4c69 6365 6e73 6520 3a3a 204f  s...License :: O
+00000420: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000430: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+00000440: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000450: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
+00000460: 6e64 6f77 730d 0a09 546f 7069 6320 3a3a  ndows...Topic ::
+00000470: 2053 7973 7465 6d20 3a3a 2049 6e73 7461   System :: Insta
+00000480: 6c6c 6174 696f 6e2f 5365 7475 700d 0a09  llation/Setup...
+00000490: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
+000004a0: 203a 3a20 456e 676c 6973 680d 0a09 5072   :: English...Pr
+000004b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000004c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000004d0: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
+000004e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000004f0: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
+00000500: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000510: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000520: 203a 3a20 332e 380d 0a09 5072 6f67 7261   :: 3.8...Progra
+00000530: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000540: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000550: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000560: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000570: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
+00000580: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000590: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000005a0: 310d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  1....[options]..
+000005b0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+000005c0: 093d 7372 630d 0a70 6163 6b61 6765 7320  .=src..packages 
+000005d0: 3d20 6669 6e64 3a0d 0a69 6e63 6c75 6465  = find:..include
+000005e0: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
+000005f0: 5472 7565 0d0a 7079 7468 6f6e 5f72 6571  True..python_req
+00000600: 7569 7265 7320 3d20 3e3d 332e 380d 0a69  uires = >=3.8..i
+00000610: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000620: 3d20 0d0a 0963 6c69 636b 3e3d 382e 312e  = ...click>=8.1.
+00000630: 332c 3c38 2e32 2e30 0d0a 0970 7974 686f  3,<8.2.0...pytho
+00000640: 6e2d 6d61 6769 632d 6269 6e3d 3d30 2e34  n-magic-bin==0.4
+00000650: 2e31 343b 706c 6174 666f 726d 5f73 7973  .14;platform_sys
+00000660: 7465 6d3d 3d27 5769 6e64 6f77 7327 0d0a  tem=='Windows'..
+00000670: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000680: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+00000690: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
+000006a0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
+000006b0: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
+000006c0: 7320 3d20 0d0a 0970 796e 6261 6c6c 203d  s = ...pynball =
+000006d0: 2070 796e 6261 6c6c 2e70 796e 6261 6c6c   pynball.pynball
+000006e0: 3a63 6c69 0d0a 0d0a 5b66 6c61 6b65 385d  :cli....[flake8]
+000006f0: 0d0a 646f 6373 7472 696e 672d 636f 6e76  ..docstring-conv
+00000700: 656e 7469 6f6e 203d 206e 756d 7079 0d0a  ention = numpy..
+00000710: 6d61 782d 636f 6d70 6c65 7869 7479 203d  max-complexity =
+00000720: 2031 380d 0a6d 6178 2d6c 696e 652d 6c65   18..max-line-le
+00000730: 6e67 7468 203d 2038 380d 0a73 656c 6563  ngth = 88..selec
+00000740: 7420 3d20 422c 2042 392c 2043 2c20 442c  t = B, B9, C, D,
+00000750: 2045 2c20 462c 204e 2c20 570d 0a65 7863   E, F, N, W..exc
+00000760: 6c75 6465 203d 2074 6573 7473 2f2a 2c2e  lude = tests/*,.
+00000770: 746f 782f 2a2c 2e6e 6f78 2f2a 2c64 6f63  tox/*,.nox/*,doc
+00000780: 732f 2a2c 2e67 6974 2f2a 2c2e 6769 7468  s/*,.git/*,.gith
+00000790: 7562 2f2a 0d0a 6967 6e6f 7265 203d 200d  ub/*..ignore = .
+000007a0: 0a09 4532 3033 2c0d 0a09 5735 3033 2c0d  ..E203,...W503,.
+000007b0: 0a70 6572 2d66 696c 652d 6967 6e6f 7265  .per-file-ignore
+000007c0: 7320 3d20 0d0a 095f 5f69 6e69 745f 5f2e  s = ...__init__.
+000007d0: 7079 3a46 3430 310d 0a09 7061 7468 6d61  py:F401...pathma
+000007e0: 6769 632e 7079 3a46 3430 310d 0a09 7465  gic.py:F401...te
+000007f0: 7374 5f70 796e 6261 6c6c 2e70 793a 4634  st_pynball.py:F4
+00000800: 3031 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  01....[egg_info]
+00000810: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000820: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `pynball-1.5.6/src/pynball/pynball.py` & `pynball-1.5.7/src/pynball/pynball.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/src/pynball.egg-info/PKG-INFO` & `pynball-1.5.7/src/pynball.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.6
-Summary: Utility command line tool to manage python versions
+Version: 1.5.7
+Summary: Utility command line tool to manage python versions and virtual environments
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
-Keywords: utility
+Project-URL: documentation, https://pynamer.readthedocs.io/en/latest/
+Project-URL: Release Notes, https://github.com/Stephen-RA-King/pynamer/releases
+Project-URL: Source Code, https://github.com/Stephen-RA-King/pynamer/
+Project-URL: Issue Tracker, https://github.com/Stephen-RA-King/pynamer/issues
+Keywords: python-version-management,python-version-manager,virtualenv-manager,python-version-selector,python-versions,python-environment
 Platform: windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.md
 
 # Pynball
 
 _**Centralized management and utilization of all your Python versions, installations and virtual environments.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
@@ -59,18 +64,18 @@
 Or you may have a mixture of installations including pyenv, custom installations,
 system installations etc. Pynball can make leveraging such environments a lot easier.
 
 ## Features
 
 ---
 
-- Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
-- Easily create Virtual Environments using any Python version.
-- Track which virtual environments have which Python versions and tox versions.
-- Quickly change the System interpreter
+-   Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
+-   Easily create Virtual Environments using any Python version.
+-   Track which virtual environments have which Python versions and tox versions.
+-   Quickly change the System interpreter
 
 ## Pre Installation Requirements
 
 ---
 
 #### Minimum Requirements
 
@@ -244,18 +249,17 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
-- [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
-- [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
-- [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
-- [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
+-   [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**][wiki]
 
 ## Meta
 
 ---
 
@@ -267,14 +271,16 @@
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
+[![DOI](https://zenodo.org/badge/464560536.svg)](https://zenodo.org/badge/latestdoi/464560536)
+
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
```

### Comparing `pynball-1.5.6/src/pynball.egg-info/SOURCES.txt` & `pynball-1.5.7/src/pynball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test__check_pyenv.py` & `pynball-1.5.7/tests/test__check_pyenv.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test__check_virtual_env.py` & `pynball-1.5.7/tests/test__check_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test__get_pynball.py` & `pynball-1.5.7/tests/test__get_pynball.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test__message.py` & `pynball-1.5.7/tests/test__message.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test__set_get_del_env.py` & `pynball-1.5.7/tests/test__set_get_del_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test_add.py` & `pynball-1.5.7/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test_delete.py` & `pynball-1.5.7/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test_lsproject.py` & `pynball-1.5.7/tests/test_lsproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test_mkproject.py` & `pynball-1.5.7/tests/test_mkproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test_rmproject.py` & `pynball-1.5.7/tests/test_rmproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.6/tests/test_versions.py` & `pynball-1.5.7/tests/test_versions.py`

 * *Files identical despite different names*

