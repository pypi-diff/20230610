# Comparing `tmp/mbstrdecoder-1.1.2.tar.gz` & `tmp/mbstrdecoder-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbstrdecoder-1.1.2.tar", last modified: Sun Feb  5 12:17:09 2023, max compression
+gzip compressed data, was "mbstrdecoder-1.1.3.tar", last modified: Sat Jun 10 08:54:10 2023, max compression
```

## Comparing `mbstrdecoder-1.1.2.tar` & `mbstrdecoder-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 12:17:09.981349 mbstrdecoder-1.1.2/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      198 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     3810 2023-02-05 12:17:09.981349 mbstrdecoder-1.1.2/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     2371 2023-02-05 05:25:55.000000 mbstrdecoder-1.1.2/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 12:17:09.981349 mbstrdecoder-1.1.2/mbstrdecoder/
--rw-r--r--   0 toor      (1000) toor      (1000)      248 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/mbstrdecoder/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-02-05 12:00:53.000000 mbstrdecoder-1.1.2/mbstrdecoder/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3113 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/mbstrdecoder/_binary_ext_checker.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1355 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/mbstrdecoder/_func.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7377 2023-02-05 05:22:06.000000 mbstrdecoder-1.1.2/mbstrdecoder/_mbstrdecoder.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/mbstrdecoder/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 12:17:09.981349 mbstrdecoder-1.1.2/mbstrdecoder.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     3810 2023-02-05 12:17:09.000000 mbstrdecoder-1.1.2/mbstrdecoder.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      545 2023-02-05 12:17:09.000000 mbstrdecoder-1.1.2/mbstrdecoder.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-02-05 12:17:09.000000 mbstrdecoder-1.1.2/mbstrdecoder.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       75 2023-02-05 12:17:09.000000 mbstrdecoder-1.1.2/mbstrdecoder.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-02-05 12:17:09.000000 mbstrdecoder-1.1.2/mbstrdecoder.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1149 2023-02-05 05:43:38.000000 mbstrdecoder-1.1.2/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 12:17:09.981349 mbstrdecoder-1.1.2/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       18 2022-08-11 09:39:50.000000 mbstrdecoder-1.1.2/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       49 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-02-05 12:17:09.981349 mbstrdecoder-1.1.2/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2708 2023-02-05 05:41:55.000000 mbstrdecoder-1.1.2/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 12:17:09.981349 mbstrdecoder-1.1.2/test/
--rw-r--r--   0 toor      (1000) toor      (1000)      741 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/test/test_binary_ext_checker.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1520 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/test/test_func.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2844 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.2/test/test_mbstrdecoder.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1077 2023-02-05 12:00:01.000000 mbstrdecoder-1.1.2/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 08:54:10.824644 mbstrdecoder-1.1.3/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      198 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     3847 2023-06-10 08:54:10.824644 mbstrdecoder-1.1.3/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     2371 2023-02-05 05:25:55.000000 mbstrdecoder-1.1.3/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 08:54:10.814644 mbstrdecoder-1.1.3/mbstrdecoder/
+-rw-r--r--   0 toor      (1000) toor      (1000)      319 2023-06-10 07:30:33.000000 mbstrdecoder-1.1.3/mbstrdecoder/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-10 08:41:55.000000 mbstrdecoder-1.1.3/mbstrdecoder/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3113 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/mbstrdecoder/_binary_ext_checker.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1355 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/mbstrdecoder/_func.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7377 2023-02-05 05:22:06.000000 mbstrdecoder-1.1.3/mbstrdecoder/_mbstrdecoder.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/mbstrdecoder/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 08:54:10.824644 mbstrdecoder-1.1.3/mbstrdecoder.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3847 2023-06-10 08:54:10.000000 mbstrdecoder-1.1.3/mbstrdecoder.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      580 2023-06-10 08:54:10.000000 mbstrdecoder-1.1.3/mbstrdecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-10 08:54:10.000000 mbstrdecoder-1.1.3/mbstrdecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-10 08:54:01.000000 mbstrdecoder-1.1.3/mbstrdecoder.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       75 2023-06-10 08:54:10.000000 mbstrdecoder-1.1.3/mbstrdecoder.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-06-10 08:54:10.000000 mbstrdecoder-1.1.3/mbstrdecoder.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1186 2023-06-04 09:02:29.000000 mbstrdecoder-1.1.3/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 08:54:10.824644 mbstrdecoder-1.1.3/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       18 2022-08-11 09:39:50.000000 mbstrdecoder-1.1.3/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       49 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-10 08:54:10.824644 mbstrdecoder-1.1.3/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2833 2023-06-10 07:19:54.000000 mbstrdecoder-1.1.3/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 08:54:10.824644 mbstrdecoder-1.1.3/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)      741 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/test/test_binary_ext_checker.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1520 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/test/test_func.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2844 2021-03-20 04:14:04.000000 mbstrdecoder-1.1.3/test/test_mbstrdecoder.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1076 2023-06-10 08:35:26.000000 mbstrdecoder-1.1.3/tox.ini
```

### Comparing `mbstrdecoder-1.1.2/LICENSE` & `mbstrdecoder-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/PKG-INFO` & `mbstrdecoder-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mbstrdecoder
-Version: 1.1.2
-Summary: multi-byte character string decoder
+Version: 1.1.3
+Summary: mbstrdecoder is a Python library for multi-byte character string decoder
 Home-page: https://github.com/thombashi/mbstrdecoder
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/mbstrdecoder
 Project-URL: Tracker, https://github.com/thombashi/mbstrdecoder/issues
 Keywords: multi-byte character,unicode,decoder
```

### Comparing `mbstrdecoder-1.1.2/README.rst` & `mbstrdecoder-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/mbstrdecoder/_binary_ext_checker.py` & `mbstrdecoder-1.1.3/mbstrdecoder/_binary_ext_checker.py`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/mbstrdecoder/_func.py` & `mbstrdecoder-1.1.3/mbstrdecoder/_func.py`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/mbstrdecoder/_mbstrdecoder.py` & `mbstrdecoder-1.1.3/mbstrdecoder/_mbstrdecoder.py`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/mbstrdecoder.egg-info/PKG-INFO` & `mbstrdecoder-1.1.3/mbstrdecoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mbstrdecoder
-Version: 1.1.2
-Summary: multi-byte character string decoder
+Version: 1.1.3
+Summary: mbstrdecoder is a Python library for multi-byte character string decoder
 Home-page: https://github.com/thombashi/mbstrdecoder
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/mbstrdecoder
 Project-URL: Tracker, https://github.com/thombashi/mbstrdecoder/issues
 Keywords: multi-byte character,unicode,decoder
```

### Comparing `mbstrdecoder-1.1.2/mbstrdecoder.egg-info/SOURCES.txt` & `mbstrdecoder-1.1.3/mbstrdecoder.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 mbstrdecoder/_binary_ext_checker.py
 mbstrdecoder/_func.py
 mbstrdecoder/_mbstrdecoder.py
 mbstrdecoder/py.typed
 mbstrdecoder.egg-info/PKG-INFO
 mbstrdecoder.egg-info/SOURCES.txt
 mbstrdecoder.egg-info/dependency_links.txt
+mbstrdecoder.egg-info/not-zip-safe
 mbstrdecoder.egg-info/requires.txt
 mbstrdecoder.egg-info/top_level.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
 test/test_binary_ext_checker.py
 test/test_func.py
 test/test_mbstrdecoder.py
```

### Comparing `mbstrdecoder-1.1.2/pyproject.toml` & `mbstrdecoder-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
```

### Comparing `mbstrdecoder-1.1.2/setup.py` & `mbstrdecoder-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "mbstrdecoder"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -39,23 +39,30 @@
 
 setuptools.setup(
     name=MODULE_NAME,
     version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
-    description="multi-byte character string decoder",
+    description=f"{MODULE_NAME} is a Python library for multi-byte character string decoder",
     include_package_data=True,
-    keywords=["multi-byte character", "unicode", "decoder"],
+    keywords=[
+        "multi-byte character",
+        "unicode",
+        "decoder",
+    ],
     license=pkg_info["__license__"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
-    project_urls={"Source": REPOSITORY_URL, "Tracker": f"{REPOSITORY_URL:s}/issues"},
+    project_urls={
+        "Source": REPOSITORY_URL,
+        "Tracker": f"{REPOSITORY_URL:s}/issues",
+    },
     python_requires=">=3.7",
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={"test": tests_require},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
@@ -72,8 +79,9 @@
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Text Processing",
     ],
     cmdclass=get_release_command_class(),
+    zip_safe=False,
 )
```

### Comparing `mbstrdecoder-1.1.2/test/test_binary_ext_checker.py` & `mbstrdecoder-1.1.3/test/test_binary_ext_checker.py`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/test/test_func.py` & `mbstrdecoder-1.1.3/test/test_func.py`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/test/test_mbstrdecoder.py` & `mbstrdecoder-1.1.3/test/test_mbstrdecoder.py`

 * *Files identical despite different names*

### Comparing `mbstrdecoder-1.1.2/tox.ini` & `mbstrdecoder-1.1.3/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tox]
 envlist =
     py{37,38,39,310,311,312}
     pypy3
-    clean
     cov
     fmt
     lint
 
 [testenv]
+passenv = *
 extras =
     test
 commands =
     pytest {posargs:-vv}
 
 [testenv:build]
 deps =
@@ -37,27 +37,27 @@
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:fmt]
 skip_install = true
 deps =
-    autoflake>=1.4
+    autoflake>=2
     black>=23.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
     black setup.py test mbstrdecoder
 
 [testenv:lint]
 skip_install = true
 deps =
-    codespell
-    mypy>=0.991
+    codespell>=2
+    mypy>=1
     pylama>=8.4.1
     types-chardet
 commands =
     python setup.py check
     -codespell mbstrdecoder examples test -q 2 --check-filenames --ignore-words-list followings
     mypy mbstrdecoder setup.py
     pylama
```

