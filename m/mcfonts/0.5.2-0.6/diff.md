# Comparing `tmp/mcfonts-0.5.2.tar.gz` & `tmp/mcfonts-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcfonts-0.5.2.tar", last modified: Thu Jan 26 23:43:25 2023, max compression
+gzip compressed data, was "mcfonts-0.6.tar", last modified: Sat Jun 10 20:41:59 2023, max compression
```

## Comparing `mcfonts-0.5.2.tar` & `mcfonts-0.6.tar`

### file list

```diff
@@ -1,48 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:43:25.549713 mcfonts-0.5.2/
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-01-26 23:43:08.000000 mcfonts-0.5.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8120 2023-01-26 23:43:25.549713 mcfonts-0.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6790 2023-01-26 23:43:08.000000 mcfonts-0.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:43:25.537712 mcfonts-0.5.2/mcfonts/
--rw-rw-rw-   0 root         (0) root         (0)    18606 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4760 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     6456 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/compacting.py
--rw-rw-rw-   0 root         (0) root         (0)    21415 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     9441 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/coverage_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9132 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/importing.py
--rw-rw-rw-   0 root         (0) root         (0)    42194 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:43:25.546712 mcfonts-0.5.2/mcfonts/template_hexchar_textures/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/0.png
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/1.png
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/2.png
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/3.png
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/4.png
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/5.png
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/6.png
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/7.png
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/8.png
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/9.png
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/a.png
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/b.png
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/box4.png
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/box6.png
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/c.png
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/d.png
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/e.png
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/template_hexchar_textures/f.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:43:25.549713 mcfonts-0.5.2/mcfonts/utils/
--rw-rw-rw-   0 root         (0) root         (0)     6651 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16795 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/utils/bitmap.py
--rw-rw-rw-   0 root         (0) root         (0)    15693 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/utils/exporting.py
--rw-rw-rw-   0 root         (0) root         (0)     4788 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/utils/legacy_unicode.py
--rw-rw-rw-   0 root         (0) root         (0)     4487 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/utils/rangestring.py
--rw-rw-rw-   0 root         (0) root         (0)     7035 2023-01-26 23:43:08.000000 mcfonts-0.5.2/mcfonts/utils/unicode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:43:25.539712 mcfonts-0.5.2/mcfonts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8120 2023-01-26 23:43:25.000000 mcfonts-0.5.2/mcfonts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1272 2023-01-26 23:43:25.000000 mcfonts-0.5.2/mcfonts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 23:43:25.000000 mcfonts-0.5.2/mcfonts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      145 2023-01-26 23:43:25.000000 mcfonts-0.5.2/mcfonts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-26 23:43:25.000000 mcfonts-0.5.2/mcfonts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-01-26 23:43:08.000000 mcfonts-0.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 23:43:25.550713 mcfonts-0.5.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:41:59.893875 mcfonts-0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-10 20:41:47.000000 mcfonts-0.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     8687 2023-06-10 20:41:59.893875 mcfonts-0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7359 2023-06-10 20:41:47.000000 mcfonts-0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:41:59.885874 mcfonts-0.6/mcfonts/
+-rw-rw-rw-   0 root         (0) root         (0)    30777 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5263 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4759 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/compacting.py
+-rw-rw-rw-   0 root         (0) root         (0)    12577 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10398 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/coverage_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      902 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9030 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16599 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/glyphs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:41:59.888874 mcfonts-0.6/mcfonts/providers/
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    19857 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/bitmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     9036 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/legacy_unicode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4900 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/space.py
+-rw-rw-rw-   0 root         (0) root         (0)     1808 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/ttf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3815 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/unihex.py
+-rw-rw-rw-   0 root         (0) root         (0)     8132 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/providers/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:41:59.891874 mcfonts-0.6/mcfonts/template_hexchar_textures/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/0.png
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/1.png
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/2.png
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/3.png
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/4.png
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/5.png
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/6.png
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/7.png
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/8.png
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/9.png
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/a.png
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/b.png
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/box4.png
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/box6.png
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/c.png
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/d.png
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/e.png
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/template_hexchar_textures/f.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:41:59.892874 mcfonts-0.6/mcfonts/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)    25983 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/utils/exporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     5019 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/utils/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8584 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/utils/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     5598 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/utils/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     4696 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/utils/unicode.py
+-rw-rw-rw-   0 root         (0) root         (0)     5280 2023-06-10 20:41:47.000000 mcfonts-0.6/mcfonts/utils/unihex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:41:59.886874 mcfonts-0.6/mcfonts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8687 2023-06-10 20:41:59.000000 mcfonts-0.6/mcfonts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-10 20:41:59.000000 mcfonts-0.6/mcfonts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 20:41:59.000000 mcfonts-0.6/mcfonts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-10 20:41:59.000000 mcfonts-0.6/mcfonts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-10 20:41:59.000000 mcfonts-0.6/mcfonts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2023-06-10 20:41:47.000000 mcfonts-0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 20:41:59.893875 mcfonts-0.6/setup.cfg
```

### Comparing `mcfonts-0.5.2/LICENSE.txt` & `mcfonts-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mcfonts-0.5.2/PKG-INFO` & `mcfonts-0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcfonts
-Version: 0.5.2
+Version: 0.6
 Summary: A module for exporting, manipulating, and working with Minecraft fonts
 Author: WhoAteMyButter
 License: MIT
 Project-URL: Documentation, https://mcfonts.readthedocs.io
 Project-URL: Source, https://gitlab.com/whoatemybutter/mcfonts
 Project-URL: Changelog, https://gitlab.com/whoatemybutter/mcfonts/-/blob/master/CHANGELOG.md
 Project-URL: Issues, https://gitlab.com/whoatemybutter/mcfonts/-/issues
@@ -19,31 +19,30 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 [![mcfonts](logo.png)](https://gitlab.com/whoatemybutter/mcfonts)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Pylint](https://img.shields.io/badge/pylint-9.98-ffbf48)](https://pylint.pycqa.org/en/latest/)
+[![Pylint](https://img.shields.io/badge/pylint-9.94-ffbf48)](https://pylint.pycqa.org/en/latest/)
 [![License](https://img.shields.io/badge/license-MIT-a51931)](https://spdx.org/licenses/MIT.html)
 [![PyPi](https://img.shields.io/pypi/v/mcfonts)](https://pypi.org/project/mcfonts/)
 [![GitLab Release (latest by SemVer)](https://img.shields.io/gitlab/v/release/38935127?sort=semver)](https://gitlab.com/whoatemybutter/mcfonts/-/releases)
 
 **mcfonts** is a versatile, fast, and extensible package for working with Minecraft fonts.
 <br/>
-mcfonts works with any font JSON and can export every kind of texture & size,
-no matter the amount or complexity.
+mcfonts works with any font JSON and can export every kind of texture & size, no matter the amount or complexity.
 <br/>
 It can be used anywhere in places that deal with Minecraft fonts.
 
 > ⚠️ mcfonts is in beta. API may change at any time, read the changelog carefully.
 
 ---
 
@@ -59,127 +58,146 @@
     - [🚫 Disclaimer](#-disclaimer)
 - [📎 Links](#-links)
 
 ---
 
 ## 📦 Installation
 
-`mcfonts` is available on PyPi.
-It requires a Python version of **at least 3.10.0.**
-
-#### It depends on these packages:
-* [fontTools](https://pypi.org/project/fontTools/): for exporting to OpenType
-* [lxml](https://pypi.org/project/lxml/): for fast XML parsing
-* [Pillow](https://pypi.org/project/Pillow/): for processing font textures
-* [tinyunicodeblock](https://pypi.org/project/tinyunicodeblock/): for font coverage summaries
-* [jsonschema](https://pypi.org/project/jsonschema): for font JSON validation
-
-#### It also has these **optional dependencies**:
-
-`docs`: Generating documentation
-* [sphinx](https://pypi.org/project/sphinx/): for generating documentation
-* [sphinx-autoapi](https://pypi.org/project/sphinx-autoapi/): for generating code documentation
-* [furo](https://pypi.org/project/furo/): for documentation theme
+`mcfonts` is available on PyPI.
+It requires a Python version of **at least 3.11.0.**
 
 To install `mcfonts` with pip, run:
 ```shell
 python -m pip install mcfonts
 ```
 
 If you would like the ability to generate documentation alongside it, run:
 ```shell
 python -m pip install mcfonts[docs]
 ```
 
+### "externally-managed-environment"
+
+This error occurs on some Linux distributions such as Fedora 38 and Ubuntu 23.04.
+It can be solved by either:
+
+1. Using a [virtual environment (venv)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)
+2. Using [pipx](https://github.com/pypa/pipx)
+
+### Dependencies
+
+* [fontTools](https://pypi.org/project/fontTools/): for exporting to OpenType
+* [lxml](https://pypi.org/project/lxml/): for fast XML parsing
+* [Pillow](https://pypi.org/project/Pillow/): for processing font textures
+* [tinyunicodeblock](https://pypi.org/project/tinyunicodeblock/): for font coverage summaries
+* [jsonschema](https://pypi.org/project/jsonschema): for the font JSON validation
+* [unirange](https://pypi.org/project/unirange/): for special unirange shortcuts
+
+#### Optional dependencies
+
+`docs`: Generating documentation
+* [sphinx](https://pypi.org/project/sphinx/): for generating documentation
+* [sphinx-autoapi](https://pypi.org/project/sphinx-autoapi/): for generating code documentation
+* [sphinxext-opengraph](https://pypi.org/project/sphinxext-opengraph/): for meta tags
+* [sphinx-immaterial](https://pypi.org/project/sphinx-immaterial/): for documentation theme
+
 ---
 
 ## 🧮 Features
 
 * Handles these providers:
     * `space`
     * `bitmap`
     * `legacy_unicode`
     * `ttf`
+    * `unihex`
+    * `reference`
 * Warns of invalid data
 * Finds oversights that the Vanilla client does not notice
 * Generates optimized and space-saving glyph paths
 * Works with any font, not just Vanilla
 * Works on fonts with double, triple, or quadruple scales
 * Generates summaries of fonts
 * Allows easy inspection of a font's details
 * Contains glyph utilities and compacting functions
+* Works on new 1.20+ `unihex` and `reference` providers
 
 ---
 
 ## 🛠 Usage
 Using `mcfonts` is simple.
-Most functionality begins by using a function in the `mcfonts.importing` module.
 
 ```python
-import mcfonts.importing
-font = mcfonts.importing.from_java_font_file("path/to/font.json")
+import mcfonts
+
+font = mcfonts.from_java_font_file("path/to/font.json")
 # Do stuff with `font`...
 ```
 
 ### Exporting
 
 To export to OpenType:
 
 ```python
-import mcfonts.importing
-font = mcfonts.importing.from_java_font_file("path/to/font.json")
+import mcfonts
+
+font = mcfonts.from_java_font_file("path/to/font.json")
 font.export("My cool font").save("My cool font.otf")
 ```
 That's it. Your font is at `./My cool font.otf`.
 
 If you have a font with ~200 characters, it generated in ~0.3 seconds.
 <br/>
-If you have a font with ~2,000 characters, it generated in ~4.9 seconds.
+If you have a font with ~2,000 characters, it generated in ~3.2 seconds.
 <br/>
-If you have a font with ~15,000 characters, it generated in ~33.7 seconds.
+If you have a font with ~13,000 characters, it generated in ~9.9 seconds.
 <br/>
 If you have a font with ~60,000 characters, you've made a mistake.
-<small>(your font generated in ~2 minutes, 5 seconds.)</small>
+<small>(your font generated in ~1 minute, 14 seconds.)</small>
 
 > ❗ Note: Only OpenType fonts are supported for exporting.</br>
 > Use other utilities such as [FontForge](https://fontforge.org/en-US/) to convert between formats.
 
 ---
 
 ## ❓ Why?
 ### ⏳ It's fast
 
 In the time it has taken you to read this sentence,
 a font with 1,000 glyphs has already been generated.
 
-A 13,000 glyph font takes ~30 seconds.
+A 13,000 glyph font takes 10 seconds.
 
-A simple 100 glyph font? A fraction of a second; it takes 1/100s.
+A simple 100 glyph font? A fraction of a second; it takes 0.1s.
 
 ### ➿ It's versatile
 
 `mcfonts` works on fonts of any height, ascent, and size.
-It correctly compensates for oversized characters,
+
+It correctly compensates & warns about oversized characters,
 translucent textures, and invalid data.
 
 ### 🧠 It makes sense
 
 Fonts are organized by a class, instead of using individual functions.
+
 Providers, too, have their own classes.
-Exporting and compacting are separated into their own functions,
-which makes debugging & modification easy.
 
-**`mcfonts` does not fix mistakes in fonts.**
+Exporting and compacting are separated into their own functions, which makes debugging & modification easy.
+
+> **`mcfonts` does not fix mistakes in fonts.**
+
 It will extrapolate missing data, but empty/corrupt textures, invalid numbers,
-or extreme cases, result in an error when trying to create a `MinecraftFont` instance.
+or extreme cases will result in an error when trying to create a `MinecraftFont` instance with them.
 
 This gives you the ability to correct these problems, instead of silently making them work
 (sometimes with limited effectiveness) and keeping you in the dark about future issues.
 
 ### 📜 It's documented
+
 `mcfonts` has extensive documentation, both externally and in the source code.
 Functions are carefully written with rST-style docstrings,
 and module variables are given precise descriptions.
 
 ---
 
 ## 📒 Documentation
@@ -187,53 +205,53 @@
 Documentation for `mcfonts` is available at https://mcfonts.readthedocs.io.
 
 ### Building locally
 You can build the documentation yourself by grabbing a copy of the source code:
 
 ```shell
 git clone https://gitlab.com/whoatemybutter/mcfonts.git
+cd mcfonts/docs
 ```
 
 The documenation has a few requirements, install them all with:
 ```shell
-python -m pip install furo Sphinx sphinx-autoapi
+python -m pip install -r requirements.txt
 ```
 
-There should be a `docs` directory; go to it.
 Run `make html` to begin building the documentation.
 It will be at `_build/html/index.html`.
 
 ---
 
 ## 📰 Changelog
 
 The changelog is at [CHANGELOG.md](CHANGELOG.md).
 
 ---
 
 ## 📜 License
 
-`mcfonts` is licensed under
-[MIT](https://spdx.org/licenses/MIT.html).
+`mcfonts` is licensed under the [MIT license](https://spdx.org/licenses/MIT.html).
 <br/>
 Fonts created with this tool are under **no explicit license**; you can license them in any way you want.
 This includes under a paid license.<br/>
 *By default, fonts created by this tool are under the public domain.*
 
 Although credit is embedded in exported fonts, *removing this credit **is** allowed*,
-and the function parameter `MinecraftFont.export(include_credit)` may be set to `False`.
+and the function parameter `mcfonts.MinecraftFont.export(include_credit)` may be set to `False`.
 <br/>
 
-**Keeping it is greatly appreciated and helps make `mcfonts` better.
+**Keeping it in is greatly appreciated and helps make `mcfonts` better.
 There is no disadvantage to leaving the credit in.**
 
 ### 🚫 Disclaimer
 
 > **mcfonts is not affiliated, endorsed, created, supported, or an official product
-> by Mojang Studios or by Microsoft Corporation in any way.**
+> by Mojang Studios or by Microsoft Corporation or by any of their associates in any way.**
 
 ---
 
 ## 📎 Links
 
 * [Minecraft Wiki - Fonts](https://minecraft.fandom.com/wiki/Resource_Pack#Fonts)
 * [OpenType specification](https://docs.microsoft.com/en-us/typography/opentype/spec/)
+* [FontForge](https://fontforge.org/)
```

### Comparing `mcfonts-0.5.2/README.md` & `mcfonts-0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [![mcfonts](logo.png)](https://gitlab.com/whoatemybutter/mcfonts)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Pylint](https://img.shields.io/badge/pylint-9.98-ffbf48)](https://pylint.pycqa.org/en/latest/)
+[![Pylint](https://img.shields.io/badge/pylint-9.94-ffbf48)](https://pylint.pycqa.org/en/latest/)
 [![License](https://img.shields.io/badge/license-MIT-a51931)](https://spdx.org/licenses/MIT.html)
 [![PyPi](https://img.shields.io/pypi/v/mcfonts)](https://pypi.org/project/mcfonts/)
 [![GitLab Release (latest by SemVer)](https://img.shields.io/gitlab/v/release/38935127?sort=semver)](https://gitlab.com/whoatemybutter/mcfonts/-/releases)
 
 **mcfonts** is a versatile, fast, and extensible package for working with Minecraft fonts.
 <br/>
-mcfonts works with any font JSON and can export every kind of texture & size,
-no matter the amount or complexity.
+mcfonts works with any font JSON and can export every kind of texture & size, no matter the amount or complexity.
 <br/>
 It can be used anywhere in places that deal with Minecraft fonts.
 
 > ⚠️ mcfonts is in beta. API may change at any time, read the changelog carefully.
 
 ---
 
@@ -29,127 +28,146 @@
     - [🚫 Disclaimer](#-disclaimer)
 - [📎 Links](#-links)
 
 ---
 
 ## 📦 Installation
 
-`mcfonts` is available on PyPi.
-It requires a Python version of **at least 3.10.0.**
-
-#### It depends on these packages:
-* [fontTools](https://pypi.org/project/fontTools/): for exporting to OpenType
-* [lxml](https://pypi.org/project/lxml/): for fast XML parsing
-* [Pillow](https://pypi.org/project/Pillow/): for processing font textures
-* [tinyunicodeblock](https://pypi.org/project/tinyunicodeblock/): for font coverage summaries
-* [jsonschema](https://pypi.org/project/jsonschema): for font JSON validation
-
-#### It also has these **optional dependencies**:
-
-`docs`: Generating documentation
-* [sphinx](https://pypi.org/project/sphinx/): for generating documentation
-* [sphinx-autoapi](https://pypi.org/project/sphinx-autoapi/): for generating code documentation
-* [furo](https://pypi.org/project/furo/): for documentation theme
+`mcfonts` is available on PyPI.
+It requires a Python version of **at least 3.11.0.**
 
 To install `mcfonts` with pip, run:
 ```shell
 python -m pip install mcfonts
 ```
 
 If you would like the ability to generate documentation alongside it, run:
 ```shell
 python -m pip install mcfonts[docs]
 ```
 
+### "externally-managed-environment"
+
+This error occurs on some Linux distributions such as Fedora 38 and Ubuntu 23.04.
+It can be solved by either:
+
+1. Using a [virtual environment (venv)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)
+2. Using [pipx](https://github.com/pypa/pipx)
+
+### Dependencies
+
+* [fontTools](https://pypi.org/project/fontTools/): for exporting to OpenType
+* [lxml](https://pypi.org/project/lxml/): for fast XML parsing
+* [Pillow](https://pypi.org/project/Pillow/): for processing font textures
+* [tinyunicodeblock](https://pypi.org/project/tinyunicodeblock/): for font coverage summaries
+* [jsonschema](https://pypi.org/project/jsonschema): for the font JSON validation
+* [unirange](https://pypi.org/project/unirange/): for special unirange shortcuts
+
+#### Optional dependencies
+
+`docs`: Generating documentation
+* [sphinx](https://pypi.org/project/sphinx/): for generating documentation
+* [sphinx-autoapi](https://pypi.org/project/sphinx-autoapi/): for generating code documentation
+* [sphinxext-opengraph](https://pypi.org/project/sphinxext-opengraph/): for meta tags
+* [sphinx-immaterial](https://pypi.org/project/sphinx-immaterial/): for documentation theme
+
 ---
 
 ## 🧮 Features
 
 * Handles these providers:
     * `space`
     * `bitmap`
     * `legacy_unicode`
     * `ttf`
+    * `unihex`
+    * `reference`
 * Warns of invalid data
 * Finds oversights that the Vanilla client does not notice
 * Generates optimized and space-saving glyph paths
 * Works with any font, not just Vanilla
 * Works on fonts with double, triple, or quadruple scales
 * Generates summaries of fonts
 * Allows easy inspection of a font's details
 * Contains glyph utilities and compacting functions
+* Works on new 1.20+ `unihex` and `reference` providers
 
 ---
 
 ## 🛠 Usage
 Using `mcfonts` is simple.
-Most functionality begins by using a function in the `mcfonts.importing` module.
 
 ```python
-import mcfonts.importing
-font = mcfonts.importing.from_java_font_file("path/to/font.json")
+import mcfonts
+
+font = mcfonts.from_java_font_file("path/to/font.json")
 # Do stuff with `font`...
 ```
 
 ### Exporting
 
 To export to OpenType:
 
 ```python
-import mcfonts.importing
-font = mcfonts.importing.from_java_font_file("path/to/font.json")
+import mcfonts
+
+font = mcfonts.from_java_font_file("path/to/font.json")
 font.export("My cool font").save("My cool font.otf")
 ```
 That's it. Your font is at `./My cool font.otf`.
 
 If you have a font with ~200 characters, it generated in ~0.3 seconds.
 <br/>
-If you have a font with ~2,000 characters, it generated in ~4.9 seconds.
+If you have a font with ~2,000 characters, it generated in ~3.2 seconds.
 <br/>
-If you have a font with ~15,000 characters, it generated in ~33.7 seconds.
+If you have a font with ~13,000 characters, it generated in ~9.9 seconds.
 <br/>
 If you have a font with ~60,000 characters, you've made a mistake.
-<small>(your font generated in ~2 minutes, 5 seconds.)</small>
+<small>(your font generated in ~1 minute, 14 seconds.)</small>
 
 > ❗ Note: Only OpenType fonts are supported for exporting.</br>
 > Use other utilities such as [FontForge](https://fontforge.org/en-US/) to convert between formats.
 
 ---
 
 ## ❓ Why?
 ### ⏳ It's fast
 
 In the time it has taken you to read this sentence,
 a font with 1,000 glyphs has already been generated.
 
-A 13,000 glyph font takes ~30 seconds.
+A 13,000 glyph font takes 10 seconds.
 
-A simple 100 glyph font? A fraction of a second; it takes 1/100s.
+A simple 100 glyph font? A fraction of a second; it takes 0.1s.
 
 ### ➿ It's versatile
 
 `mcfonts` works on fonts of any height, ascent, and size.
-It correctly compensates for oversized characters,
+
+It correctly compensates & warns about oversized characters,
 translucent textures, and invalid data.
 
 ### 🧠 It makes sense
 
 Fonts are organized by a class, instead of using individual functions.
+
 Providers, too, have their own classes.
-Exporting and compacting are separated into their own functions,
-which makes debugging & modification easy.
 
-**`mcfonts` does not fix mistakes in fonts.**
+Exporting and compacting are separated into their own functions, which makes debugging & modification easy.
+
+> **`mcfonts` does not fix mistakes in fonts.**
+
 It will extrapolate missing data, but empty/corrupt textures, invalid numbers,
-or extreme cases, result in an error when trying to create a `MinecraftFont` instance.
+or extreme cases will result in an error when trying to create a `MinecraftFont` instance with them.
 
 This gives you the ability to correct these problems, instead of silently making them work
 (sometimes with limited effectiveness) and keeping you in the dark about future issues.
 
 ### 📜 It's documented
+
 `mcfonts` has extensive documentation, both externally and in the source code.
 Functions are carefully written with rST-style docstrings,
 and module variables are given precise descriptions.
 
 ---
 
 ## 📒 Documentation
@@ -157,53 +175,53 @@
 Documentation for `mcfonts` is available at https://mcfonts.readthedocs.io.
 
 ### Building locally
 You can build the documentation yourself by grabbing a copy of the source code:
 
 ```shell
 git clone https://gitlab.com/whoatemybutter/mcfonts.git
+cd mcfonts/docs
 ```
 
 The documenation has a few requirements, install them all with:
 ```shell
-python -m pip install furo Sphinx sphinx-autoapi
+python -m pip install -r requirements.txt
 ```
 
-There should be a `docs` directory; go to it.
 Run `make html` to begin building the documentation.
 It will be at `_build/html/index.html`.
 
 ---
 
 ## 📰 Changelog
 
 The changelog is at [CHANGELOG.md](CHANGELOG.md).
 
 ---
 
 ## 📜 License
 
-`mcfonts` is licensed under
-[MIT](https://spdx.org/licenses/MIT.html).
+`mcfonts` is licensed under the [MIT license](https://spdx.org/licenses/MIT.html).
 <br/>
 Fonts created with this tool are under **no explicit license**; you can license them in any way you want.
 This includes under a paid license.<br/>
 *By default, fonts created by this tool are under the public domain.*
 
 Although credit is embedded in exported fonts, *removing this credit **is** allowed*,
-and the function parameter `MinecraftFont.export(include_credit)` may be set to `False`.
+and the function parameter `mcfonts.MinecraftFont.export(include_credit)` may be set to `False`.
 <br/>
 
-**Keeping it is greatly appreciated and helps make `mcfonts` better.
+**Keeping it in is greatly appreciated and helps make `mcfonts` better.
 There is no disadvantage to leaving the credit in.**
 
 ### 🚫 Disclaimer
 
 > **mcfonts is not affiliated, endorsed, created, supported, or an official product
-> by Mojang Studios or by Microsoft Corporation in any way.**
+> by Mojang Studios or by Microsoft Corporation or by any of their associates in any way.**
 
 ---
 
 ## 📎 Links
 
 * [Minecraft Wiki - Fonts](https://minecraft.fandom.com/wiki/Resource_Pack#Fonts)
 * [OpenType specification](https://docs.microsoft.com/en-us/typography/opentype/spec/)
+* [FontForge](https://fontforge.org/)
```

### Comparing `mcfonts-0.5.2/mcfonts/__main__.py` & `mcfonts-0.6/mcfonts/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,159 +1,156 @@
 #!/usr/bin/env python3
 # coding=utf-8
 # SPDX-License-Identifier: MIT
-"""
-CLI front-end for mcfonts.
-"""
+"""Command-line tool front-end for mcfonts."""
+from __future__ import annotations
+
 import argparse
 import sys
 
 import PIL.Image
-import mcfonts.importing
-import mcfonts.utils.bitmap
 
-if __name__ != "__main__":
-    raise NotImplementedError
+import mcfonts.utils.resources
+import mcfonts.compacting
+
+if __name__ == "__main__":
+
+    INPUT_HELP = (
+        "Path to folder, JSON, or ZIP file of font. "
+        "If folder, this folder must be a resource pack. "
+        "If JSON, this file must be a font JSON file. "
+        "If ZIP, this file must be a resource pack archive. "
+        "If -, stdin is used."
+    )
+
+    parser = argparse.ArgumentParser(
+        description="""
+        mcfonts is a versatile, fast, and extensible package for working with Minecraft fonts.
+        
+        The CLI front-end does not expose every possible option.
+        For more in-depth usage, import the mcfonts module in Python.
+        """
+    )
+
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="version",
+        version="mcfonts " + ".".join(str(x) for x in mcfonts.__version__),
+    )
+
+    subparsers = parser.add_subparsers(title="Functions")
+
+    export_parser = subparsers.add_parser("export", help="export a font file to an OpenType font")
+    export_parser.add_argument(
+        "input",
+        type=argparse.FileType(),
+        default=(None if sys.stdin.isatty() else sys.stdin),
+        help=INPUT_HELP,
+    )
+    export_parser.add_argument("outfile", type=argparse.FileType("wb"), default=sys.stdout)
+    export_parser.add_argument(
+        "-c",
+        "--color",
+        default=False,
+        action="store_true",
+        help="To read colors in referenced resources",
+    )
+    export_parser.add_argument("-n", "--font-name", help="What the font name of the output should be")
+    export_parser.set_defaults(export=True)
+
+    info_parser = subparsers.add_parser("info", help="print information about a font file")
+    info_parser.add_argument(
+        "input",
+        type=argparse.FileType(),
+        default=(None if sys.stdin.isatty() else sys.stdin),
+        help=INPUT_HELP,
+    )
+
+    info_parser.add_argument(
+        "-t",
+        "--table-chars",
+        action="store_true",
+        default=False,
+        help="to put characters into a formatter table or put in single list",
+    )
+    info_parser.add_argument(
+        "-s",
+        "--summary-only",
+        action="store_true",
+        default=False,
+        help="to print only a small summary",
+    )
+    info_parser.set_defaults(info=True)
+
+    compact_parser = subparsers.add_parser("compact", help="fit the glyphs in the minimum amount of space needed")
+    compact_parser.add_argument(
+        "input",
+        type=argparse.FileType("rb"),
+        default=(None if sys.stdin.isatty() else sys.stdin),
+        help="Path to PNG file.",
+    )
+    compact_parser.add_argument(
+        "char-counts",
+        nargs=2,
+        type=int,
+        default=(16, 16),
+        help="Two numbers of the characters in each row and column of the input file.",
+    )
+    compact_parser.add_argument(
+        "-c",
+        "--chars-in-row",
+        type=int,
+        default=16,
+        help="The desired number of glyphs to put in one row, set to 0 for square. Default is 16.",
+    )
+    compact_parser.add_argument("outfile", type=argparse.FileType("wb"), default=sys.stdout)
+    compact_parser.set_defaults(compact=True)
+
+    compare_parser = subparsers.add_parser("compare", help="compare two fonts")
+    compare_parser.add_argument(
+        "input1",
+        type=argparse.FileType("rb"),
+        default=(None if sys.stdin.isatty() else sys.stdin),
+        help=INPUT_HELP,
+    )
+    compare_parser.add_argument(
+        "input2",
+        type=argparse.FileType("rb"),
+        default=(None if sys.stdin.isatty() else sys.stdin),
+        help=INPUT_HELP,
+    )
+    compare_parser.add_argument(
+        "-s",
+        "--swap",
+        action="store_true",
+        default=(None if sys.stdin.isatty() else sys.stdin),
+        help="swap the order of fonts compared",
+    )
+    compare_parser.set_defaults(compare=True)
+
+    vargs = vars(parser.parse_args(args=None if sys.argv[1:] else ["--help"]))
 
-INPUT_HELP = (
-    "Path to folder, JSON, or ZIP file of font. "
-    "If folder, this folder must be a resource pack. "
-    "If JSON, this file must be a font JSON file. "
-    "If ZIP, this file must be a resource pack archive. "
-    "If -, stdin is used."
-)
-
-parser = argparse.ArgumentParser(
-    description="""
-    mcfonts is a versatile, fast, and extensible package for working with Minecraft fonts.
-    
-    The CLI front-end does not expose every possible option.
-    For more in-depth usage, import the mcfonts module in Python.
-    """
-)
-
-parser.add_argument(
-    "-v",
-    "--version",
-    action="version",
-    version="mcfonts " + ".".join(str(x) for x in mcfonts.__version__),
-)
-
-subparsers = parser.add_subparsers(title="Functions")
-
-export_parser = subparsers.add_parser("export", help="export a font file to an OpenType font")
-export_parser.add_argument(
-    "input",
-    type=argparse.FileType(),
-    default=(None if sys.stdin.isatty() else sys.stdin),
-    help=INPUT_HELP,
-)
-export_parser.add_argument("outfile", type=argparse.FileType("wb"), default=sys.stdout)
-export_parser.add_argument(
-    "-c",
-    "--color",
-    default=False,
-    action="store_true",
-    help="To read colors in referenced resources",
-)
-export_parser.add_argument("-n", "--font-name", help="What the font name of the output should be")
-export_parser.set_defaults(export=True)
-
-
-info_parser = subparsers.add_parser("info", help="print information about a font file")
-info_parser.add_argument(
-    "input",
-    type=argparse.FileType(),
-    default=(None if sys.stdin.isatty() else sys.stdin),
-    help=INPUT_HELP,
-)
-
-info_parser.add_argument(
-    "-t",
-    "--table-chars",
-    action="store_true",
-    default=False,
-    help="to put characters into a formatter table or put in single list",
-)
-info_parser.add_argument(
-    "-s",
-    "--summary-only",
-    action="store_true",
-    default=False,
-    help="to print only a small summary",
-)
-info_parser.set_defaults(info=True)
-
-compact_parser = subparsers.add_parser("compact", help="fit the glyphs in the minimum amount of space needed")
-compact_parser.add_argument(
-    "input",
-    type=argparse.FileType("rb"),
-    default=(None if sys.stdin.isatty() else sys.stdin),
-    help="Path to PNG file",
-)
-compact_parser.add_argument(
-    "glyphsize",
-    nargs=2,
-    type=int,
-    default=(8, 8),
-    help="Two numbers of the size of 1 glyph in `input`, (width, height)",
-)
-compact_parser.add_argument(
-    "-c",
-    "--chars-in-row",
-    type=int,
-    default=16,
-    help="The desired number of glyphs to put in one row, set to 0 for square.",
-)
-compact_parser.add_argument("outfile", type=argparse.FileType("wb"), default=sys.stdout)
-compact_parser.set_defaults(compact=True)
-
-
-compare_parser = subparsers.add_parser("compare", help="compare two fonts")
-compare_parser.add_argument(
-    "input1",
-    type=argparse.FileType("rb"),
-    default=(None if sys.stdin.isatty() else sys.stdin),
-    help=INPUT_HELP,
-)
-compare_parser.add_argument(
-    "input2",
-    type=argparse.FileType("rb"),
-    default=(None if sys.stdin.isatty() else sys.stdin),
-    help=INPUT_HELP,
-)
-compare_parser.add_argument(
-    "-s",
-    "--swap",
-    action="store_true",
-    default=(None if sys.stdin.isatty() else sys.stdin),
-    help="swap the order of fonts compared",
-)
-compare_parser.set_defaults(compare=True)
-
-vargs = vars(parser.parse_args(args=None if sys.argv[1:] else ["--help"]))
-
-if vargs.get("export", False):
-    mcfonts.importing.from_java_font_file(vargs["input"].name, vargs["color"]).export(vargs["font_name"]).save(
-        vargs["outfile"], False
-    )
-elif vargs.get("info", False):
-    mcfonts.importing.from_java_ambiguous(vargs["input"].name).print_info(
-        vargs.get("table_chars", False), vargs.get("summary_only", False)
-    )
-elif vargs.get("compact"):
-    resource = PIL.Image.open(vargs["input"])
-    cell_size: tuple[int, int] = tuple(vargs["glyphsize"])
-    glyphs = list(mcfonts.utils.bitmap.resource_to_glyphs(resource, cell_size))
-    compacted = mcfonts.compacting.compact_glyphs(
-        glyphs,
-        vargs["chars_in_row"](resource.width // cell_size[0], resource.height // cell_size[1]),
-    )
-    compacted[0].save(vargs["outfile"])
-    print(compacted[1])
-elif vargs.get("compare"):
-    font1 = mcfonts.importing.from_java_ambiguous(vargs["input1"].name)
-    font2 = mcfonts.importing.from_java_ambiguous(vargs["input2"].name)
-    if vargs.get("swap", False):
-        font2.compare(font1)
-    else:
-        font1.compare(font2)
+    if vargs.get("export", False):
+        mcfonts.from_java_font_file(vargs["input"].name, vargs["color"]).export(vargs["font_name"]).save(
+            vargs["outfile"], False
+        )
+    elif vargs.get("info", False):
+        mcfonts.from_java_ambiguous(vargs["input"].name).print_info(
+            vargs.get("table_chars", False), vargs.get("summary_only", False)
+        )
+    elif vargs.get("compact"):
+        resource = PIL.Image.open(vargs["input"])
+        cell_size = tuple(vargs["char_counts"])
+        compacted = mcfonts.compacting.compact_images(
+            list(mcfonts.utils.resources.divide_resource_by_grid(resource, cell_size)),
+            vargs["chars_in_row"](resource.width // cell_size[0], resource.height // cell_size[1]),
+        )
+        compacted[0].save(vargs["outfile"])
+        print(compacted[1])
+    elif vargs.get("compare"):
+        font1 = mcfonts.from_java_ambiguous(vargs["input1"].name)
+        font2 = mcfonts.from_java_ambiguous(vargs["input2"].name)
+        if vargs.get("swap", False):
+            font2.compare(font1)
+        else:
+            font1.compare(font2)
```

### Comparing `mcfonts-0.5.2/mcfonts/utils/exporting.py` & `mcfonts-0.6/mcfonts/glyphs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,387 +1,478 @@
 #!/usr/bin/env python3
 # coding=utf-8
 # SPDX-License-Identifier: MIT
 """
-Functions for exporting various character/provider formats into XML-representable data.
-
-Contains functions for handling various providers and exporting them into font XMLs.
-These providers are handled:
-
-* space
-* bitmap
-* legacy_unicode
-* mcfonts:options
+TODO doc
+- this
+- add basic doc for all getters
 """
-import datetime
+from __future__ import annotations
 
+import abc
+import dataclasses
+import math
+
+import PIL.Image
 import fontTools.pens.t2CharStringPen
 import lxml.etree
-import PIL.Image
+
 import mcfonts.constants
 import mcfonts.exceptions
-import mcfonts.utils.unicode
-
-
-def glyph_to_program(
-    glyph: PIL.Image.Image, ascent: int, pixel_size: float, options: dict | None = None
-) -> list[str | int] | None:
-    """
-    Create a Type 2 charstring program given a glyph sheet.
-    If the glyph is empty or has no white pixels,
-    None will be returned. Otherwise, a list of strings will be.
-
-    These charstrings are **not** optimized or checked for overlaps.
-    In FontForge, use :menuselection:`E&lement --> O&verlap --> &Remove Overlap` manually
-    afterwards.
-
-    :param glyph: A :class:`PIL.Image.Image` of the individual character, **not** the font sheet.
-    :param ascent: The ascent of this glyph, equal to ``(ascent - height) * (glyph_height / height)``.
-    :param pixel_size: How big each pixel should be.
-    :param options:
-        A specialized dictionary that should be derived
-        from an instance of :class:`mcfonts.providers.OptionsProvider`.
-        Should be in the form of {field*: value}. For example, an Options dictionary of
-        ``{"width": {"a": 4}, "spacing": {"a": 2}}``
-        should transform into ``{"width": 4, "spacing": 2}``.
-        Use :meth:`mcfonts.providers.OptionsProvider.get_options_for_char` for this.
-    :returns:
-        A list of strings of the glyph's program,
-        or None if there was no pixel data in ``glyph``.
-    """
-    # Excess is a number of how far away the glyph is from the left edge of the canvas
-    if options is None:
-        options = {}
-    excess = get_glyph_nominals(glyph)
-    # If excess is -1 (special case), there is nothing here but a space.
-    if excess[1] == -1:
-        return None
-    # No components to resolve, so no glyphSet is needed; using {}
-    pen = fontTools.pens.t2CharStringPen.T2CharStringPen(0, {}, 0)
-    modifiers = [0, 0]
-    width = (excess[1] * pixel_size) + 125
-    if options.get("fullwidth", False) is True:
-        width = glyph.width * pixel_size
-    # If shift is [0, 0], ignore it.
-    if options.get("shift", [0, 0]) != [0, 0]:
-        modifiers = options["shift"]
-    if options.get("spacing") is not None:
-        width = (excess[1] + options["spacing"]) * pixel_size
-    if options.get("width") is not None:
-        width = options["width"] * pixel_size
-    if glyph.mode == "RGBA":
-        data = glyph.getdata(3)
-    elif glyph.mode == "LA":
-        data = glyph.getdata(1)
-    else:
-        data = glyph.getdata(0)
-    for index, pixel in enumerate(data):
-        if pixel >= 180:
-            x_position = index % glyph.width
-            y_position = index // glyph.width
-            pen.moveTo(
-                (
-                    (x_position + modifiers[0]) * pixel_size,
-                    (glyph.height - y_position + ascent + modifiers[1]) * pixel_size,
-                )
-            )
-            # Left X, top right
-            pen.lineTo(
-                (
-                    (x_position + 1 + modifiers[0]) * pixel_size,
-                    (glyph.height - y_position + ascent + modifiers[1]) * pixel_size,
-                )
-            )
-            # Down Y, bottom left
-            pen.lineTo(
-                (
-                    (x_position + 1 + modifiers[0]) * pixel_size,
-                    (glyph.height - y_position - 1 + ascent + modifiers[1]) * pixel_size,
-                )
+import mcfonts.utils.exporting
+import mcfonts.utils.image
+import mcfonts.utils.unihex
+
+BITMAP_EXPORT_PIXEL_THRESHOLD = 180
+UNIHEX_EXPORT_PIXEL_ON = "1"
+SPACE_EXPORT_MAX_ADVANCE = 12500
+
+
+class Glyph(abc.ABC):
+    """The base Glyph class. Should never be called or instantiated."""
+
+    @abc.abstractmethod
+    def get_width(self) -> int:
+        """Width of the glyph."""
+
+    @abc.abstractmethod
+    def export_to_character(
+        self,
+        font_xml: lxml.etree._Element,
+        character: str,
+        allocated_characters: set[str],
+        char_options: dict | None = None,
+    ) -> None:
+        """
+        Export this glyph to a character in a font XML.
+
+        The font XML is mutated in-place and nothing is returned.
+
+        :param font_xml: The font XML as a :class:`lxml.etree._Element`.
+        :param character: A string of a single character for what Unicode character to export and assign the glyph to.
+        :param allocated_characters: A set of all the characters the `font_xml` already has an allocation for.
+        :param char_options:
+            An optional dictionary of character options.
+            Get this from :meth:`mcfonts.providers.options.OptionsProvider.get_options_for_char`.
+
+            This is deprecated since v0.6 and will be removed in v0.7.
+        :raises mcfonts.exceptions.CharacterPaddingError: If character is a padding character.
+        """
+
+    @abc.abstractmethod
+    def get_ascent(self) -> int:
+        """Ascent of the glyph."""
+
+    @abc.abstractmethod
+    def get_height(self) -> int:
+        """Height of the glyph. This is not always equal to the glyph's image, if applicable."""
+
+    @abc.abstractmethod
+    def get_program(
+        self,
+        char_options: dict | None = None,
+    ) -> list[str, int] | None:
+        """
+        Type 2 charstring program. This is used in exporting and can be cached for better performance.
+
+        :param char_options:
+            A specialized dictionary that should be derived from an instance of
+            :class:`mcfonts.providers.options.OptionsProvider`.
+
+            This is deprecated since v0.6 and will be removed in v0.7.
+        """
+
+    @abc.abstractmethod
+    def construct_program(self, pixel_size: int, options: dict | None = None) -> list[str | int] | None:
+        """
+        Create a Type 2 charstring program.
+
+        If the glyph is empty or has no white pixels, None will be returned.
+        Otherwise, a list *(the program)* will be returned.
+
+        .. warning::
+
+            These charstrings are **not** optimized or checked for overlaps.
+            In FontForge, use :menuselection:`E&lement -> O&verlap -> &Remove Overlap` manually afterward.
+
+        :param pixel_size:
+            How big each pixel should be.
+        :param options:
+            A specialized dictionary that should be derived from an instance of
+            :class:`mcfonts.providers.options.OptionsProvider`.
+
+            Should be in the form of {field*: value}.
+            For example, an Options dictionary of ``{"width": {"a": 4}, "spacing": {"a": 2}}``
+            should transform into ``{"width": 4, "spacing": 2}``;
+            use :meth:`mcfonts.providers.options.OptionsProvider.get_options_for_char` for this.
+
+            This is deprecated since v0.6 and will be removed in v0.7.
+        :returns:
+            A list of strings of the glyph's program, or None if there was no pixel data in ``glyph``.
+        """
+
+
+@dataclasses.dataclass
+class BitmapGlyph(Glyph):
+    """
+    A bitmap glyph.
+
+    Must contain an image and ascent.
+    Height, ascent, and bearings are optional.
+    Bearings and width are lazily-loaded.
+    """
+
+    image: PIL.Image.Image
+    """Required image."""
+    ascent: int
+    """Required ascent."""
+    height: int | None = None
+    """Optional height. Lazy default is 8 if None."""
+    width: int | None = None
+    """Optional width. Lazy default is `self.image.width`."""
+    bearings: tuple[int, int] | None = None
+    """Optional padding from the edges of the canvas."""
+    program: list[str, int] | None = None
+    """Optional Type 2 charstring program of the glyph."""
+
+    def get_bearings(self) -> tuple[int, int]:
+        """
+        From :func:`mcfonts.utils.resources.get_image_bearings`:
+
+        | Bearings are a "padding" from the edge of the canvas to image pixels.
+        | Left bearing is the distance from the left edge of the canvas to the most-left pixel data.
+        | Right bearing is the distance from the right edge of the canvas to the most-right pixel data.
+
+        This is lazily-loaded.
+        """
+        if self.bearings is None:
+            self.bearings = mcfonts.utils.image.get_image_bearings(self.image)
+        return self.bearings
+
+    def get_width(self) -> int:
+        """
+        Width of the glyph's image.
+
+        This is lazily-loaded.
+        """
+        if self.width is None:
+            self.width = self.image.width
+        return self.width
+
+    def get_image(self) -> PIL.Image.Image:
+        """The image of the glyph."""
+        if self.image.mode not in {"RGBA", "LA"}:
+            self.image = self.image.convert("RGBA")
+        return self.image
+
+    def get_height(self) -> int:
+        """
+        The height of the glyph; this is not necessarily the glyph's image width.
+
+        This is lazily-loaded.
+        """
+        if self.height is None:
+            self.height = 8
+        return self.height
+
+    def get_ascent(self) -> int:
+        """The glyph's ascent."""
+        return self.ascent
+
+    def get_program(
+        self,
+        char_options: dict | None = None,
+    ) -> list[str, int] | None:
+        if self.program is None:
+            self.program = self.construct_program(
+                # Em size (1000) divided by 8 (standard width) = 125,
+                # divide this by scale (glyph height / JSON height) to get how big each "pixel" will translate to.
+                125 // (self.image.height // self.get_height()),
+                char_options,
             )
-            # Right X, bottom right
-            pen.lineTo(
-                (
-                    (x_position + modifiers[0]) * pixel_size,
-                    (glyph.height - y_position - 1 + ascent + modifiers[1]) * pixel_size,
-                )
-            )
-            # Done pixel
-            pen.closePath()
-    # Return the pen's resulting program
-    charstring = pen.getCharString()
-    # Set the width correctly
-    charstring.program[0] = int(width)
-
-    mcfonts.logger.debug(f"exporting: made program for glyph, with options: {bool(options)}")
-
-    return charstring.program
-
+        return self.program
 
-def get_glyph_nominals(glyph: PIL.Image.Image) -> tuple[int, int]:
-    """
-    Return the number of pixels away from the left edge of the canvas the glyph is and the
-    glyph's resulting calculated width.
-
-    If return is 0, -1, there is no pixel data, the glyph is all spaces.
-
-    :param glyph: A :class:`PIL.Image.Image` instance.
-    :returns:
-        Left padding and total width.
-        Returns (0, -1) if no pixel data.
-    """
-    try:
-        bbox = glyph.getbbox()
-        return bbox[0], bbox[2]
-    except (TypeError, IndexError):
-        # Pure space, has no width
-        return 0, -1
-
-
-def allocate_char(font_xml: lxml.etree._Element, char: str) -> None:
-    """
-    Allocate a Unicode character in a font.
-    Does not assign any character data or widths.
-
-    :param font_xml: The font XML.
-    :param char: A single character.
-    :returns: Nothing, font is modified in-place.
-    :raises GlyphLimitError: If there are more than 65,535 glyphs in the font; can't add more.
-    """
-    codepoint = ord(char)
-    uni = f"u{codepoint:04X}"
-
-    if (metrics_num := int((metrics := font_xml.find("hhea/numberOfHMetrics")).get("value"))) >= 65535:
-        raise mcfonts.exceptions.GlyphLimitError
-    metrics.set("value", str(metrics_num + 1))
-
-    num_glyphs = font_xml.find("maxp/numGlyphs")
-    num_glyphs.set("value", str(int(num_glyphs.get("value")) + 1))
-
-    cmap = font_xml.find("cmap")
-
-    if (cmap_12 := cmap.find("cmap_format_12")) is None:
-        lxml.etree.SubElement(
-            cmap,
-            "cmap_format_12",
-            {
-                "platformID": "0",
-                "platEncID": "4",
-                "language": "0",
-                "length": "4120",
-                "nGroups": "323",
-                "format": "12",
-                "reserved": "0",
-            },
-        )
-        cmap_12 = cmap.find("cmap_format_12")
-    # Inside the BMP
-    if codepoint <= 0xFFFF:
-        # No format table exists yet, add it
-        if (cmap_4 := cmap.find("cmap_format_4")) is None:
-            lxml.etree.SubElement(
-                cmap,
-                "cmap_format_4",
-                {
-                    "platformID": "3",
-                    "platEncID": "4",
-                    "language": "0",
-                },
+    def export_to_character(
+        self,
+        font_xml: lxml.etree._Element,
+        character: str,
+        allocated_characters: set[str] | None = None,
+        char_options: dict | None = None,
+    ) -> None:
+        if allocated_characters is None:
+            allocated_characters = set()
+        if character in mcfonts.constants.PADDING_CHARS:
+            raise mcfonts.exceptions.CharacterPaddingError()
+        if character not in allocated_characters:
+            mcfonts.utils.exporting.allocate_char(font_xml, character)
+        if program := self.get_program(char_options):  # If we have a program.
+            mcfonts.utils.exporting.set_program_to_char(font_xml, program, character)
+        else:
+            # Nothing here; it was a space.
+            mcfonts.utils.exporting.set_space_to_char(font_xml, character, 1)
+
+    def construct_program(self, pixel_size: int, options: dict | None = None) -> list[str | int] | None:
+        if options is None:
+            options = {}
+        if (bearings := self.get_bearings()) == (0, 0):
+            return None
+        pen = fontTools.pens.t2CharStringPen.T2CharStringPen(0, {})
+        modifiers = [0, 0]
+        width = bearings[1]
+        spacing = 1
+        if options.get("fullwidth", False) is True:
+            width = self.get_width()
+        # If shift is [0, 0], ignore it.
+        if options.get("shift", [0, 0]) != [0, 0]:
+            modifiers = options["shift"]
+        if options.get("spacing") is not None:
+            spacing = options["spacing"]
+        if options.get("width") is not None:
+            width = options["width"]
+
+        ascent = self.get_ascent()
+        height = self.get_image().height
+
+        for index, pixel in enumerate(self.get_image().convert("LA").getdata(1)):
+            if pixel >= BITMAP_EXPORT_PIXEL_THRESHOLD:
+                glyph_width = self.get_image().width
+                x_real = (index % glyph_width) + modifiers[0]
+                y_real = height - (index // glyph_width) + ascent + modifiers[1]
+                pen.moveTo(
+                    (
+                        x_real * pixel_size,
+                        y_real * pixel_size,
+                    )
+                )  # Left X, top right.
+
+                pen.lineTo(
+                    (
+                        (x_real + 1) * pixel_size,
+                        y_real * pixel_size,
+                    )
+                )  # Down Y, bottom left.
+
+                pen.lineTo(
+                    (
+                        (x_real + 1) * pixel_size,
+                        (y_real - 1) * pixel_size,
+                    )
+                )  # Right X, bottom right.
+
+                pen.lineTo(
+                    (
+                        x_real * pixel_size,
+                        (y_real - 1) * pixel_size,
+                    )
+                )  # Done with pixel.
+
+                pen.closePath()
+        program: list[int | str] = pen.getCharString().program
+        program[0] = (width + spacing) * pixel_size  # Set the width correctly.
+        return program
+
+
+@dataclasses.dataclass
+class SpaceGlyph(Glyph):
+    """
+    A space glyph.
+
+    Contans one required field, the glyph's width.
+    """
+
+    width: int
+    """The width of the glyph."""
+    program: list[str, int] | None = None
+    """Optional Type 2 charstring program of the glyph."""
+
+    def export_to_character(
+        self,
+        font_xml: lxml.etree._Element,
+        character: str,
+        allocated_characters: set[str],
+        char_options: dict | None = None,
+    ) -> None:
+        width = self.get_width()
+        if math.isinf(width) or math.isnan(width):
+            width = 20
+        if character not in allocated_characters:
+            mcfonts.utils.exporting.allocate_char(font_xml, character)
+        mcfonts.utils.exporting.set_space_to_char(font_xml, character, width)
+
+    def get_width(self) -> int:
+        return self.width
+
+    def get_ascent(self) -> int:
+        return 1
+
+    def get_height(self) -> int:
+        return 8
+
+    def get_program(
+        self,
+        char_options: dict | None = None,
+    ) -> list[str, int] | None:
+        if self.program is None:
+            self.program = self.construct_program(125)
+        return self.program
+
+    def construct_program(self, pixel_size: float, options: dict | None = None) -> list[str | int] | None:
+        return [int(min(abs((self.get_width() * pixel_size)), SPACE_EXPORT_MAX_ADVANCE)), "endchar"]
+
+
+@dataclasses.dataclass
+class UnihexGlyph(Glyph):
+    """
+    A unihex glyph.
+
+    Must contain a bit string.
+    Width, image, and bearings are optional.
+    Width, image, and bearings are lazily-loaded.
+
+    TODO more stuff here about what it is, what it does, etc.
+    """
+
+    bit_string: str
+    """The bit string; does not include the `codepoint:` starting portion."""
+    width: int | None
+    """The width of the glyph. Equal to ``len(self.bit_string) // 4``."""
+    image: PIL.Image.Image | None
+    """
+    An optional image of the glyph, comparable to a :class:`BitmapGlyph`.
+    If possible, try not to use this.
+    """
+    bearings: tuple[int, int] | None
+    """An optional tuple of the glyph's bearings, comparable to a :class:`BitmapGlyph`."""
+    size_override: tuple[int, int] | None
+    """
+    An optional tuple of the glyph's size override.
+    
+    The first value is the starting column, and the second value is the ending column.
+    When exporting, data outside of these columns will be discarded.
+    If this is None, this is lazily-calculated to be ``(0, self.get_width())``.
+    """
+    program: list[str, int] | None = None
+    """Optional Type 2 charstring program of the glyph."""
+
+    def export_to_character(
+        self,
+        font_xml: lxml.etree._Element,
+        character: str,
+        allocated_characters: set[str],
+        char_options: dict | None = None,
+    ) -> None:
+        if character not in allocated_characters:
+            mcfonts.utils.exporting.allocate_char(font_xml, character)
+        if program := self.get_program(char_options):  # If we have a program.
+            mcfonts.utils.exporting.set_program_to_char(font_xml, program, character, False)
+        else:
+            # Nothing here; it was a space.
+            mcfonts.utils.exporting.set_space_to_char(font_xml, character, 1, False)
+
+    def get_width(self) -> int:
+        if self.width is None:
+            self.width = len(self.bit_string) >> 2
+        return self.width
+
+    def get_image(self) -> PIL.Image.Image:
+        """
+        The image of the glyph.
+
+        This is lazily-loaded.
+        """
+        if self.image is None:
+            self.image = mcfonts.utils.unihex.bit_string_to_image(self.bit_string)
+        return self.image
+
+    def get_bit_string(self) -> str:
+        """The bit string is the portion after the ``codepoint:``."""
+        return self.bit_string
+
+    def get_bearings(self) -> tuple[int, int]:
+        """See :func:`mcfonts.utils.unihex.get_unihex_bearings`."""
+        if self.bearings is None:
+            self.bearings = mcfonts.utils.unihex.get_unihex_bearings(self.get_bit_string())
+        return self.bearings
+
+    def get_ascent(self) -> int:
+        return 1
+
+    def get_height(self) -> int:
+        return 8
+
+    def get_program(
+        self,
+        char_options: dict | None = None,
+    ) -> list[str, int] | None:
+        if self.program is None:
+            self.program = self.construct_program(
+                # Em size (1000) divided by 10 = 100
+                # divide this by scale (glyph height / JSON height) to get how big each "pixel" will translate to.
+                125,
+                char_options,
             )
-            cmap_4 = cmap.find("cmap_format_4")
-        lxml.etree.SubElement(cmap_4, "map", {"code": f"0x{codepoint:X}", "name": uni, "language": "0"})
-    lxml.etree.SubElement(cmap_12, "map", {"code": f"0x{codepoint:X}", "name": uni, "language": "0"})
-
-    lxml.etree.SubElement(font_xml.find("GDEF/GlyphClassDef"), "ClassDef", {"glyph": uni, "class": "1"})
-
-    lxml.etree.SubElement(font_xml.find("GlyphOrder"), "GlyphID", {"name": uni})
-    mcfonts.logger.debug(f"exporting: allocated char {mcfonts.utils.unicode.pretty_print_char(char)}")
+        return self.program
 
-
-def set_program_to_char(font_xml: lxml.etree._Element, program: list[str], char: str, replace: bool = True) -> None:
-    """
-    Set a program to a character.
-    This is how character data is added to the font.
-    The character must be allocated already.
-    That is not done in this function.
-
-    If the character is not in the font, add it.
-    If it is and ``replace`` is True, set it to the new character data.
-    Otherwise, do nothing.
-
-    :param font_xml: The font XML.
-    :param program: A list of strings of the glyph's program.
-    :param char: A single character.
-    :param replace: If the character already has data, overwrite.
-    :returns: Nothing, font is modified in-place.
-    :raises GlyphLimitError: If there are more than 65,535 glyphs in the font; can't add more.
-    """
-    uni = f"u{ord(char):04X}"
-    charstrings = font_xml.find("CFF/CFFFont/CharStrings")
-    charstring_xml = font_xml.find(f"{charstrings}/CharString[@name='{uni}']")
-    if charstring_xml is None:
-        # Doesn't exist
-        lxml.etree.SubElement(charstrings, "CharString", {"name": uni}).text = " ".join(str(x) for x in program)
-        lxml.etree.SubElement(font_xml.find("hmtx"), "mtx", {"name": uni, "width": str(program[0]), "lsb": "0"})
-    elif replace:
-        # Exists already in the charstrings, replace it too
-        charstring_xml.text = " ".join(str(x) for x in program)
-        font_xml.find(f"hmtx/mtx[@name='{uni}']").set("width", str(program[0]))
-    mcfonts.logger.debug(
-        f"exporting: set program to char {mcfonts.utils.unicode.pretty_print_char(char)}, replaced: {replace}"
-    )
+    def construct_program(self, pixel_size: int, options: dict | None = None) -> list[str | int] | None:
+        pen = fontTools.pens.t2CharStringPen.T2CharStringPen(0, {})
+        glyph_width = self.get_width()
+        size = self.get_size_override()
+        index = 0
+        bearings = self.get_bearings()
+        for row in mcfonts.utils.unihex.bit_string_to_rows(self.get_bit_string()):
+            for pixel in row:
+                if pixel == UNIHEX_EXPORT_PIXEL_ON:
+                    x_real = index % glyph_width
+                    # - 1 to correct for baseline
+                    y_real = (index // glyph_width) - 1
+                    if x_real < min(size[0], 0) or x_real > min(size[1], glyph_width):
+                        # Size overrides say to cut it off
+                        continue
+                    x_real -= bearings[0]
+                    pen.moveTo(
+                        (
+                            x_real * pixel_size,
+                            y_real * pixel_size,
+                        )
+                    )  # Left X, top right.
+
+                    pen.lineTo(
+                        (
+                            (x_real + 1) * pixel_size,
+                            y_real * pixel_size,
+                        )
+                    )  # Down Y, bottom left.
+
+                    pen.lineTo(
+                        (
+                            (x_real + 1) * pixel_size,
+                            (y_real - 1) * pixel_size,
+                        )
+                    )  # Right X, bottom right.
+
+                    pen.lineTo(
+                        (
+                            x_real * pixel_size,
+                            (y_real - 1) * pixel_size,
+                        )
+                    )  # Done with pixel.
+
+                    pen.closePath()
+                index += 1
+        program: list[int | str] = pen.getCharString().program
+        program[0] = (bearings[1] - bearings[0] + 1) * pixel_size  # Set the width correctly.
+        return program
+
+    def get_size_override(self) -> tuple[int, int]:
+        """Size override is a tuple of 2 integers of the starting and ending columns for a glyph."""
+        if self.size_override is None:
+            self.size_override = (0, self.get_width())
+        return self.size_override
 
 
-def set_space_to_char(font_xml: lxml.etree._Element, char: str, width: int, replace: bool = True) -> None:
-    """
-    Add/set a whitespace character to the font, only defining its width.
-    The charcter must be allocated already. That is not done in this function.
-
-    If the glyph is not in the font, add it.
-    If it is and ``replace`` is True, set it to the new value.
-    Otherwise, do nothing.
-
-    :param font_xml: The font XML.
-    :param char: A single character.
-    :param width: The width of the whitespace, unscaled.
-    :param replace: If the character already has data, overwrite.
-    :returns: Nothing, font is modified in-place.
-    :raises GlyphLimitError: If there are more than 65,535 glyphs in the font; can't add more.
-    """
-    uni = f"u{ord(char):04X}"
-    charstrings = font_xml.find("CFF/CFFFont/CharStrings")
-    width *= 125
-
-    if (charstring_xml := font_xml.find(f"{charstrings}/CharString[@name='{uni}']")) is None:
-        # Doesn't exist
-        lxml.etree.SubElement(charstrings, "CharString", {"name": uni}).text = f"{width} endchar"
-        lxml.etree.SubElement(font_xml.find("hmtx"), "mtx", {"name": uni, "width": str(width), "lsb": "0"})
-    elif replace:
-        # Exists already in the charstrings, replace it too
-        charstring_xml.text = f"{width} endchar"
-        font_xml.find(f"hmtx/mtx[@name='{uni}']").set("width", str(width))
-    mcfonts.logger.debug(
-        f"exporting: set space to char {mcfonts.utils.unicode.pretty_print_char(char)}, "
-        f"replaced: {replace}, width: {width}"
-    )
-
-
-def add_namerecord_to_font(font_xml: lxml.etree._Element, data: str, name_id: int) -> None:
-    """
-    Set a namerecord in a font.
-    Does not check if such a namerecord already exists, and will add new namerecords.
-
-    * 0 -> Copyright
-    * 1 -> Font family
-    * 2 -> Font subfamily
-    * 3 -> Unique font ID
-    * 4 -> Full font name, ID 1 + 2
-    * 5 -> Version: "Version maj.min"
-    * 6 -> PostScript name
-    * 7 -> Trademark
-    * 8 -> Manufacturer
-    * 9 -> Designer
-    * 10 -> Descriptions
-
-    See more at https://docs.microsoft.com/en-us/typography/opentype/spec/name#name-ids.
-
-    All are encoded at (0, 4) and (3, 1), Unicode 2.0+ full.
-
-    :param font_xml: The font XML.
-    :param data: Whatever string to add.
-    :param name_id: The ID of the namerecord.
-    :returns: Nothing, font is modified in-place.
-    """
-    lxml.etree.SubElement(
-        font_xml.find("name"),
-        "namerecord",
-        {"platformID": "0", "platEncID": "4", "nameID": str(name_id), "langID": "0x0"},
-    ).text = data
-    lxml.etree.SubElement(
-        font_xml.find("name"),
-        "namerecord",
-        {"platformID": "3", "platEncID": "1", "nameID": str(name_id), "langID": "0x409"},
-    ).text = data
-    mcfonts.logger.debug(f"exporting: added namerecord {name_id}: {data}")
-
-
-def set_cfffont_name(font_xml: lxml.etree._Element, font_name: str, family_name: str) -> None:
-    """
-    Sets the font's appropriate CFF name in 'CFF ' tables.
-    This is not the same as changing the 'name' tables, see :func:`add_namerecord_to_font` instead.
-
-    :param font_xml: The font XML.
-    :param font_name: The name of the font (do not include "Regular" or related weights).
-    :param family_name: The family name of the font (do not include "Regular" or related weights).
-    :returns: Nothing, font is modified in-place.
-    """
-    cfffont = font_xml.find("CFF/CFFFont")
-    cfffont.set("name", mcfonts.utils.sanitize_font_name(font_name))
-    cfffont.find("FullName").set("value", font_name)
-    cfffont.find("FamilyName").set("value", family_name)
-    mcfonts.logger.debug(f"exporting: set CFF font name to {font_name}, family {family_name}")
-
-
-def set_font_times(font_xml: lxml.etree._Element) -> None:
-    """
-    Sets the font's created and modified times,
-    in the format of ``%a %b %d %X %Y``.
-
-    :param font_xml: The font XML.
-    :returns: Nothing, font is modified in-place.
-    """
-    time = datetime.datetime.now().strftime("%a %b %d %X %Y")
-    font_xml.find("head/created").set("value", time)
-    font_xml.find("head/modified").set("value", time)
-    mcfonts.logger.debug("exporting: set font times")
-
-
-def set_notdef_in_font(font_xml: lxml.etree._Element, program: list[str]) -> None:
-    """
-    Set the .notdef character of the font.
-    The font already has a default notdef, use for setting to something else.
-
-    :param font_xml: The font XML.
-    :param program: A list of strings of the glyph's program.
-    :returns: Nothing, font is modified in-place.
-    """
-    font_xml.find("CFF/CFFFont/CharStrings/CharString[@name='.notdef']").text = " ".join(str(x) for x in program)
-    font_xml.find("hmtx/mtx[@name='.notdef']").set("width", str(program[0]))
-    mcfonts.logger.debug("exporting: set notdef")
-
-
-def set_font_name(font_xml: lxml.etree._Element, font_name: str, include_credits: bool = True) -> None:
-    """
-    Set the font's name to `font_xml` in all appropriate places.
-
-    This not the same as :func:`set_cfffont_name`, which sets the name for only CFF tables.
+AnyGlyph = BitmapGlyph | SpaceGlyph | UnihexGlyph
+"""
+Any glyph, either Bitmap, Space, or Unihex.
 
-    :param font_xml: The font XML.
-    :param font_name: The name of the font.
-    :param include_credits: If credits and links to mcfonts are included in the namerecords.
-    """
-    mcfonts.utils.exporting.add_namerecord_to_font(font_xml, font_name, 1)
-    mcfonts.utils.exporting.set_cfffont_name(font_xml, font_name, font_name)
-    mcfonts.utils.exporting.add_namerecord_to_font(font_xml, "Regular", 2)
-    if include_credits:
-        mcfonts.utils.exporting.add_namerecord_to_font(font_xml, "🄯 Public domain", 0)
-        mcfonts.utils.exporting.add_namerecord_to_font(font_xml, f"mcfonts: {font_name} Regular: {hash(font_xml)}", 3)
-        mcfonts.utils.exporting.add_namerecord_to_font(font_xml, "mcfonts", 8)
-        mcfonts.utils.exporting.add_namerecord_to_font(font_xml, f"{font_name} has no trademark.", 7)
-        mcfonts.utils.exporting.add_namerecord_to_font(font_xml, "https://gitlab.com/whoatemybutter/mcfonts", 11)
-        mcfonts.utils.exporting.add_namerecord_to_font(
-            font_xml,
-            "This font is under no explicit licensing. "
-            "This font's author may have additional licensing terms, contact them.",
-            13,
-        )
-    else:
-        mcfonts.utils.exporting.add_namerecord_to_font(font_xml, f"{font_name} Regular: {hash(font_xml)}", 3)
-    mcfonts.utils.exporting.add_namerecord_to_font(font_xml, f"{font_name} Regular", 4)
-    mcfonts.utils.exporting.add_namerecord_to_font(
-        font_xml,
-        f"Version 1.0; {datetime.date.strftime(datetime.date.today(), '%B %d, %Y')}",
-        5,
-    )
-    mcfonts.utils.exporting.add_namerecord_to_font(font_xml, mcfonts.utils.sanitize_font_name(font_name), 6)
-    mcfonts.utils.exporting.set_font_times(font_xml)
-    mcfonts.logger.debug(f"exporting: set font name to {font_name}, credits: {include_credits}")
+However, the method names will obviously vary. Check instances first.
+All of these inherit from the metaclass :class:`Glyph`.
+"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mcfonts-0.5.2/mcfonts.egg-info/PKG-INFO` & `mcfonts-0.6/mcfonts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcfonts
-Version: 0.5.2
+Version: 0.6
 Summary: A module for exporting, manipulating, and working with Minecraft fonts
 Author: WhoAteMyButter
 License: MIT
 Project-URL: Documentation, https://mcfonts.readthedocs.io
 Project-URL: Source, https://gitlab.com/whoatemybutter/mcfonts
 Project-URL: Changelog, https://gitlab.com/whoatemybutter/mcfonts/-/blob/master/CHANGELOG.md
 Project-URL: Issues, https://gitlab.com/whoatemybutter/mcfonts/-/issues
@@ -19,31 +19,30 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 [![mcfonts](logo.png)](https://gitlab.com/whoatemybutter/mcfonts)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Pylint](https://img.shields.io/badge/pylint-9.98-ffbf48)](https://pylint.pycqa.org/en/latest/)
+[![Pylint](https://img.shields.io/badge/pylint-9.94-ffbf48)](https://pylint.pycqa.org/en/latest/)
 [![License](https://img.shields.io/badge/license-MIT-a51931)](https://spdx.org/licenses/MIT.html)
 [![PyPi](https://img.shields.io/pypi/v/mcfonts)](https://pypi.org/project/mcfonts/)
 [![GitLab Release (latest by SemVer)](https://img.shields.io/gitlab/v/release/38935127?sort=semver)](https://gitlab.com/whoatemybutter/mcfonts/-/releases)
 
 **mcfonts** is a versatile, fast, and extensible package for working with Minecraft fonts.
 <br/>
-mcfonts works with any font JSON and can export every kind of texture & size,
-no matter the amount or complexity.
+mcfonts works with any font JSON and can export every kind of texture & size, no matter the amount or complexity.
 <br/>
 It can be used anywhere in places that deal with Minecraft fonts.
 
 > ⚠️ mcfonts is in beta. API may change at any time, read the changelog carefully.
 
 ---
 
@@ -59,127 +58,146 @@
     - [🚫 Disclaimer](#-disclaimer)
 - [📎 Links](#-links)
 
 ---
 
 ## 📦 Installation
 
-`mcfonts` is available on PyPi.
-It requires a Python version of **at least 3.10.0.**
-
-#### It depends on these packages:
-* [fontTools](https://pypi.org/project/fontTools/): for exporting to OpenType
-* [lxml](https://pypi.org/project/lxml/): for fast XML parsing
-* [Pillow](https://pypi.org/project/Pillow/): for processing font textures
-* [tinyunicodeblock](https://pypi.org/project/tinyunicodeblock/): for font coverage summaries
-* [jsonschema](https://pypi.org/project/jsonschema): for font JSON validation
-
-#### It also has these **optional dependencies**:
-
-`docs`: Generating documentation
-* [sphinx](https://pypi.org/project/sphinx/): for generating documentation
-* [sphinx-autoapi](https://pypi.org/project/sphinx-autoapi/): for generating code documentation
-* [furo](https://pypi.org/project/furo/): for documentation theme
+`mcfonts` is available on PyPI.
+It requires a Python version of **at least 3.11.0.**
 
 To install `mcfonts` with pip, run:
 ```shell
 python -m pip install mcfonts
 ```
 
 If you would like the ability to generate documentation alongside it, run:
 ```shell
 python -m pip install mcfonts[docs]
 ```
 
+### "externally-managed-environment"
+
+This error occurs on some Linux distributions such as Fedora 38 and Ubuntu 23.04.
+It can be solved by either:
+
+1. Using a [virtual environment (venv)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)
+2. Using [pipx](https://github.com/pypa/pipx)
+
+### Dependencies
+
+* [fontTools](https://pypi.org/project/fontTools/): for exporting to OpenType
+* [lxml](https://pypi.org/project/lxml/): for fast XML parsing
+* [Pillow](https://pypi.org/project/Pillow/): for processing font textures
+* [tinyunicodeblock](https://pypi.org/project/tinyunicodeblock/): for font coverage summaries
+* [jsonschema](https://pypi.org/project/jsonschema): for the font JSON validation
+* [unirange](https://pypi.org/project/unirange/): for special unirange shortcuts
+
+#### Optional dependencies
+
+`docs`: Generating documentation
+* [sphinx](https://pypi.org/project/sphinx/): for generating documentation
+* [sphinx-autoapi](https://pypi.org/project/sphinx-autoapi/): for generating code documentation
+* [sphinxext-opengraph](https://pypi.org/project/sphinxext-opengraph/): for meta tags
+* [sphinx-immaterial](https://pypi.org/project/sphinx-immaterial/): for documentation theme
+
 ---
 
 ## 🧮 Features
 
 * Handles these providers:
     * `space`
     * `bitmap`
     * `legacy_unicode`
     * `ttf`
+    * `unihex`
+    * `reference`
 * Warns of invalid data
 * Finds oversights that the Vanilla client does not notice
 * Generates optimized and space-saving glyph paths
 * Works with any font, not just Vanilla
 * Works on fonts with double, triple, or quadruple scales
 * Generates summaries of fonts
 * Allows easy inspection of a font's details
 * Contains glyph utilities and compacting functions
+* Works on new 1.20+ `unihex` and `reference` providers
 
 ---
 
 ## 🛠 Usage
 Using `mcfonts` is simple.
-Most functionality begins by using a function in the `mcfonts.importing` module.
 
 ```python
-import mcfonts.importing
-font = mcfonts.importing.from_java_font_file("path/to/font.json")
+import mcfonts
+
+font = mcfonts.from_java_font_file("path/to/font.json")
 # Do stuff with `font`...
 ```
 
 ### Exporting
 
 To export to OpenType:
 
 ```python
-import mcfonts.importing
-font = mcfonts.importing.from_java_font_file("path/to/font.json")
+import mcfonts
+
+font = mcfonts.from_java_font_file("path/to/font.json")
 font.export("My cool font").save("My cool font.otf")
 ```
 That's it. Your font is at `./My cool font.otf`.
 
 If you have a font with ~200 characters, it generated in ~0.3 seconds.
 <br/>
-If you have a font with ~2,000 characters, it generated in ~4.9 seconds.
+If you have a font with ~2,000 characters, it generated in ~3.2 seconds.
 <br/>
-If you have a font with ~15,000 characters, it generated in ~33.7 seconds.
+If you have a font with ~13,000 characters, it generated in ~9.9 seconds.
 <br/>
 If you have a font with ~60,000 characters, you've made a mistake.
-<small>(your font generated in ~2 minutes, 5 seconds.)</small>
+<small>(your font generated in ~1 minute, 14 seconds.)</small>
 
 > ❗ Note: Only OpenType fonts are supported for exporting.</br>
 > Use other utilities such as [FontForge](https://fontforge.org/en-US/) to convert between formats.
 
 ---
 
 ## ❓ Why?
 ### ⏳ It's fast
 
 In the time it has taken you to read this sentence,
 a font with 1,000 glyphs has already been generated.
 
-A 13,000 glyph font takes ~30 seconds.
+A 13,000 glyph font takes 10 seconds.
 
-A simple 100 glyph font? A fraction of a second; it takes 1/100s.
+A simple 100 glyph font? A fraction of a second; it takes 0.1s.
 
 ### ➿ It's versatile
 
 `mcfonts` works on fonts of any height, ascent, and size.
-It correctly compensates for oversized characters,
+
+It correctly compensates & warns about oversized characters,
 translucent textures, and invalid data.
 
 ### 🧠 It makes sense
 
 Fonts are organized by a class, instead of using individual functions.
+
 Providers, too, have their own classes.
-Exporting and compacting are separated into their own functions,
-which makes debugging & modification easy.
 
-**`mcfonts` does not fix mistakes in fonts.**
+Exporting and compacting are separated into their own functions, which makes debugging & modification easy.
+
+> **`mcfonts` does not fix mistakes in fonts.**
+
 It will extrapolate missing data, but empty/corrupt textures, invalid numbers,
-or extreme cases, result in an error when trying to create a `MinecraftFont` instance.
+or extreme cases will result in an error when trying to create a `MinecraftFont` instance with them.
 
 This gives you the ability to correct these problems, instead of silently making them work
 (sometimes with limited effectiveness) and keeping you in the dark about future issues.
 
 ### 📜 It's documented
+
 `mcfonts` has extensive documentation, both externally and in the source code.
 Functions are carefully written with rST-style docstrings,
 and module variables are given precise descriptions.
 
 ---
 
 ## 📒 Documentation
@@ -187,53 +205,53 @@
 Documentation for `mcfonts` is available at https://mcfonts.readthedocs.io.
 
 ### Building locally
 You can build the documentation yourself by grabbing a copy of the source code:
 
 ```shell
 git clone https://gitlab.com/whoatemybutter/mcfonts.git
+cd mcfonts/docs
 ```
 
 The documenation has a few requirements, install them all with:
 ```shell
-python -m pip install furo Sphinx sphinx-autoapi
+python -m pip install -r requirements.txt
 ```
 
-There should be a `docs` directory; go to it.
 Run `make html` to begin building the documentation.
 It will be at `_build/html/index.html`.
 
 ---
 
 ## 📰 Changelog
 
 The changelog is at [CHANGELOG.md](CHANGELOG.md).
 
 ---
 
 ## 📜 License
 
-`mcfonts` is licensed under
-[MIT](https://spdx.org/licenses/MIT.html).
+`mcfonts` is licensed under the [MIT license](https://spdx.org/licenses/MIT.html).
 <br/>
 Fonts created with this tool are under **no explicit license**; you can license them in any way you want.
 This includes under a paid license.<br/>
 *By default, fonts created by this tool are under the public domain.*
 
 Although credit is embedded in exported fonts, *removing this credit **is** allowed*,
-and the function parameter `MinecraftFont.export(include_credit)` may be set to `False`.
+and the function parameter `mcfonts.MinecraftFont.export(include_credit)` may be set to `False`.
 <br/>
 
-**Keeping it is greatly appreciated and helps make `mcfonts` better.
+**Keeping it in is greatly appreciated and helps make `mcfonts` better.
 There is no disadvantage to leaving the credit in.**
 
 ### 🚫 Disclaimer
 
 > **mcfonts is not affiliated, endorsed, created, supported, or an official product
-> by Mojang Studios or by Microsoft Corporation in any way.**
+> by Mojang Studios or by Microsoft Corporation or by any of their associates in any way.**
 
 ---
 
 ## 📎 Links
 
 * [Minecraft Wiki - Fonts](https://minecraft.fandom.com/wiki/Resource_Pack#Fonts)
 * [OpenType specification](https://docs.microsoft.com/en-us/typography/opentype/spec/)
+* [FontForge](https://fontforge.org/)
```

### Comparing `mcfonts-0.5.2/pyproject.toml` & `mcfonts-0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mcfonts"
 description = "A module for exporting, manipulating, and working with Minecraft fonts"
 readme = "README.md"
-requires-python = ">=3.10"
-version = "0.5.2"
+requires-python = ">=3.11"
+version = "0.6"
 license = {text = "MIT"}
 authors = [{name = "WhoAteMyButter"}]
 keywords = [
     "minecraft",
     "fonts",
     "minecraft fonts",
     "font exporting",
@@ -39,41 +39,89 @@
     "Natural Language :: English"
 ]
 dependencies = [
     "fontTools >= 4.35.0",
     "Pillow >= 9.3.0",
     "lxml >= 4.9.0",
     "tinyunicodeblock >= 1.1.0",
-    "jsonschema >= 4.17.3"
+    "jsonschema >= 4.17.3",
+    "unirange >= 1.0"
 ]
 
 [project.optional-dependencies]
 docs = [
     "Sphinx >= 5.3.0",
     "sphinx-autoapi >= 2.0.0",
-    "furo >= 2022.12"
+    "sphinxext-opengraph >= 0.8.2",
+    "sphinx-immaterial >= 0.11.3"
 ]
 
 [project.urls]
 Documentation = "https://mcfonts.readthedocs.io"
 Source = "https://gitlab.com/whoatemybutter/mcfonts"
 Changelog = "https://gitlab.com/whoatemybutter/mcfonts/-/blob/master/CHANGELOG.md"
 Issues = "https://gitlab.com/whoatemybutter/mcfonts/-/issues"
 
 [tool.black]
 line-length = 120
+target-version = ["py311"]
 
 [tool.pylint."MASTER"]
-jobs = 8
-py-version = "3.10"
+jobs = 0
+py-version = "3.11"
+suggestion-mode = true
 max-line-length = 120
 # Needed for lxml not playing nice with pylint
 extension-pkg-allow-list = ["lxml.etree"]
+fail-on = "I"
+# Enable many optional extensions:
+load-plugins = [
+   "pylint.extensions.bad_builtin",
+   "pylint.extensions.code_style",
+   "pylint.extensions.comparison_placement",
+   "pylint.extensions.consider_refactoring_into_while_condition",
+   "pylint.extensions.docparams",
+   "pylint.extensions.dunder",
+   "pylint.extensions.eq_without_hash",
+   "pylint.extensions.for_any_all",
+   "pylint.extensions.magic_value",
+   "pylint.extensions.mccabe",
+   "pylint.extensions.no_self_use",
+   "pylint.extensions.overlapping_exceptions",
+   "pylint.extensions.private_import",
+   "pylint.extensions.redefined_loop_name",
+   "pylint.extensions.redefined_variable_type",
+   "pylint.extensions.set_membership",
+   "pylint.extensions.typing",
+   "pylint.extensions.while_used"
+]
 [tool.pylint."MESSAGES CONTROL"]
 disable = ["logging-fstring-interpolation"]
+enable = [
+    "bad-inline-option",
+    "deprecated-pragma",
+    "file-ignored",
+    "use-symbolic-message-instead",
+    "useless-suppression"
+]
+include-naming-hint = true
+[tool.pylint."STRING CONSTANT"]
+check-quote-consistency = true
+
+
+# Include some helpful details on errors messages for naming rules:
+include-naming-hint = "yes"
 confidence = []
+[tool.pylint."STRING_CONSTANT"]
+check-quote-consistency = "yes"
+[tool.pylint."VARIABLES"]
+allow-global-unused-variables = "yes"
 
-[tool.mypy]
-ignore_missing_imports = true
+[tool.pydocstyle]
+convention = "pep257"
 
 [tool.setuptools.package-data]
 mcfonts = ["template_hexchar_textures/*.png", "py.typed", "LICENSE.txt"]
+
+[tool.mypy]
+show_error_codes = true
+pretty = true
```

