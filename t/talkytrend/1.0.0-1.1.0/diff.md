# Comparing `tmp/talkytrend-1.0.0.tar.gz` & `tmp/talkytrend-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.0.0.tar", max compression
+gzip compressed data, was "talkytrend-1.1.0.tar", max compression
```

## Comparing `talkytrend-1.0.0.tar` & `talkytrend-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-08 17:26:23.900876 talkytrend-1.0.0/LICENSE
--rw-r--r--   0        0        0     1450 2023-06-08 17:26:23.900876 talkytrend-1.0.0/README.md
--rw-r--r--   0        0        0     1686 2023-06-08 17:26:48.112966 talkytrend-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-08 17:26:48.112966 talkytrend-1.0.0/talkytrend/__init__.py
--rw-r--r--   0        0        0      630 2023-06-08 17:26:23.900876 talkytrend-1.0.0/talkytrend/config.py
--rw-r--r--   0        0        0      293 2023-06-08 17:26:23.900876 talkytrend-1.0.0/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     1733 2023-06-08 17:26:23.900876 talkytrend-1.0.0/talkytrend/main.py
--rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 talkytrend-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-10 15:02:55.563721 talkytrend-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1456 2023-06-10 15:02:55.563721 talkytrend-1.1.0/README.md
+-rw-r--r--   0        0        0     1669 2023-06-10 15:03:15.520003 talkytrend-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-06-10 15:03:15.520003 talkytrend-1.1.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-10 15:02:55.563721 talkytrend-1.1.0/talkytrend/config.py
+-rw-r--r--   0        0        0      489 2023-06-10 15:02:55.563721 talkytrend-1.1.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     2922 2023-06-10 15:02:55.563721 talkytrend-1.1.0/talkytrend/main.py
+-rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 talkytrend-1.1.0/PKG-INFO
```

### Comparing `talkytrend-1.0.0/LICENSE` & `talkytrend-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.0.0/README.md` & `talkytrend-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TalkyTrend 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"> | A python package to retrieve asset trend and economic data. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) ![Version](https://img.shields.io/pypi/v/talkytrend)<br>  ![Pypi](https://img.shields.io/pypi/dm/talkytrend)<br> [![Build](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) | Find Trend |
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) ![Version](https://img.shields.io/pypi/v/talkytrend)<br>  ![Pypi](https://img.shields.io/pypi/dm/talkytrend)<br> [![Build](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) | Find Asset Trend |
 
 Key features:
 
 - trading view connectivity
 
 ## Install
```

### Comparing `talkytrend-1.0.0/pyproject.toml` & `talkytrend-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.0.0"
-description = "A python package to retrieve key economic data such as Trend, Key economic data for any financial symbol."
+version = "1.1.0"
+description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
 ]
@@ -18,18 +18,17 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 asyncio = "*"
 dynaconf = "*"
 tradingview_ta = "*"
 
-
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
-pytest = "*"
+pytest = "^7.0.0"
 pytest-cov = "*"
 pytest-asyncio = "*"
 pytest-mock = "*"
 coverage = "*"
 
 [tool.pytest.ini_options]
 pythonpath = "."
@@ -54,8 +53,8 @@
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
 major_emoji = "💥"
 minor_emoji = "🥚,🚀,💄,✨"
-patch_emoji = "🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊"
+patch_emoji = "🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊"
```

### Comparing `talkytrend-1.0.0/talkytrend/config.py` & `talkytrend-1.1.0/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.0.0/PKG-INFO` & `talkytrend-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.0.0
-Summary: A python package to retrieve key economic data such as Trend, Key economic data for any financial symbol.
+Version: 1.1.0
+Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
 Description-Content-Type: text/markdown
 
 # TalkyTrend 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"> | A python package to retrieve asset trend and economic data. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) ![Version](https://img.shields.io/pypi/v/talkytrend)<br>  ![Pypi](https://img.shields.io/pypi/dm/talkytrend)<br> [![Build](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) | Find Trend |
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) ![Version](https://img.shields.io/pypi/v/talkytrend)<br>  ![Pypi](https://img.shields.io/pypi/dm/talkytrend)<br> [![Build](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) | Find Asset Trend |
 
 Key features:
 
 - trading view connectivity
 
 ## Install
```

