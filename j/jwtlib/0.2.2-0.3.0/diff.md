# Comparing `tmp/jwtlib-0.2.2.tar.gz` & `tmp/jwtlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jwtlib-0.2.2.tar", last modified: Thu Nov 11 18:18:39 2021, max compression
+gzip compressed data, was "jwtlib-0.3.0.tar", max compression
```

## Comparing `jwtlib-0.2.2.tar` & `jwtlib-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 18:18:39.000000 jwtlib-0.2.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/jwtlib/
--rw-r--r--   0 root         (0) root         (0)     7682 2021-11-11 18:18:22.000000 jwtlib-0.2.2/src/jwtlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1807 2021-11-11 18:18:22.000000 jwtlib-0.2.2/src/jwtlib/exc.py
--rw-r--r--   0 root         (0) root         (0)     4978 2021-11-11 18:18:22.000000 jwtlib-0.2.2/src/jwtlib/flask_support.py
--rw-r--r--   0 root         (0) root         (0)      184 2021-11-11 18:18:22.000000 jwtlib-0.2.2/src/jwtlib/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/jwtlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1768 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/jwtlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      312 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/jwtlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/jwtlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/jwtlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2021-11-11 18:18:39.000000 jwtlib-0.2.2/src/jwtlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2021-11-11 18:18:22.000000 jwtlib-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       35 2021-11-11 18:18:22.000000 jwtlib-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      922 2021-11-11 18:18:22.000000 jwtlib-0.2.2/README.rst
--rw-r--r--   0 root         (0) root         (0)     1372 2021-11-11 18:18:22.000000 jwtlib-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1152 2021-11-11 18:18:22.000000 jwtlib-0.2.2/setup.py
--rw-r--r--   0 root         (0) root         (0)     1768 2021-11-11 18:18:39.000000 jwtlib-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-11 18:18:39.000000 jwtlib-0.2.2/setup.cfg
+-rw-r--r--   0        0        0      241 2019-09-21 10:57:52.000000 jwtlib-0.3.0/AUTHORS
+-rw-r--r--   0        0        0    11357 2019-09-21 10:57:52.000000 jwtlib-0.3.0/LICENSE
+-rw-r--r--   0        0        0      922 2021-09-05 16:18:34.014623 jwtlib-0.3.0/README.rst
+-rw-r--r--   0        0        0     1695 2023-06-10 12:55:30.383150 jwtlib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-10 12:55:30.383508 jwtlib-0.3.0/src/jwtlib/__init__.py
+-rw-r--r--   0        0        0      344 2023-06-10 12:55:28.827858 jwtlib-0.3.0/src/jwtlib/abstract.py
+-rw-r--r--   0        0        0      857 2023-06-10 12:55:28.828164 jwtlib-0.3.0/src/jwtlib/exc.py
+-rw-r--r--   0        0        0     7370 2023-06-10 12:55:28.828428 jwtlib-0.3.0/src/jwtlib/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 12:55:28.828515 jwtlib-0.3.0/src/jwtlib/py.typed
+-rw-r--r--   0        0        0       87 2023-06-10 12:55:28.828871 jwtlib-0.3.0/src/jwtlib/types.py
+-rw-r--r--   0        0        0     1688 2023-06-10 13:01:24.245196 jwtlib-0.3.0/setup.py
+-rw-r--r--   0        0        0     1754 2023-06-10 13:01:24.245413 jwtlib-0.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jwtlib-0.2.2/LICENSE` & `jwtlib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtlib-0.2.2/README.rst` & `jwtlib-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `jwtlib-0.2.2/pyproject.toml` & `jwtlib-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+[tool]
 [tool.poetry]
 name = "jwtlib"
-version = "0.2.2"
+version = "0.3.0"
 description = "A little helper library to streamline working with JWT in python"
 readme = "README.rst"
 repository = "http://github.com/novopl/jwtlib"
 homepage = "http://novopl.github.com/jwtlib"
 documentation = "http://novopl.github.com/jwtlib"
 authors = ["Mateusz Klos <novopl@gmail.com>"]
 license = "Apache 2.0"
@@ -19,32 +20,54 @@
 packages = [
     { include = "jwtlib", from = "src" },
 ]
 include = ["LICENSE", "AUTHORS", "README.rst"]
 exclude = ["docs/**"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-pyjwt = "^2.0.0"
+python = ">=3.8.1,<4.0"
+pyjwt = ">=2.4.0"
 
 [tool.poetry.dev-dependencies]
-coverage = "~=5.3"
-factory-boy = "~=2.11"
-more-itertools = "<=5.0.0"
-mypy = {version = "==0.790",markers = "python_version >= '3.5'"}
-peltak = "~=0.27.0"
-psutil = "~=5.7.3"
-pycodestyle = "~=2.6.0"
-pylint = "~=2.6.0"
-pytest = "~=6.1.2"
-pytest-cov = "~=2.10.1"
-pytest-sugar = "~=0.9.4"
-Sphinx = ">=3.3.1"
-sphinx-refdoc = "~=0.3.0"
-sphinx_rtd_theme = "~=0.4.2"
-sphinxcontrib-plantuml = "~=0.17.1"
-requests = "~=2.25.0"
-flake8 = "^3.8.4"
+coverage = "^7.2.7"
+factory-boy = "^3.2.1"
+flake8 = "^6.0.0"
+more-itertools = "^9.1.0"
+mypy = "^1.3.0"
+peltak = "^0.30.0"
+pycodestyle = "^2.10.0"
+pylint = "^2.17.4"
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+pytest-sugar = "^0.9.7"
+requests = "^2.25.1"
+Sphinx = ">6.0,<7.0"
+sphinx-refdoc = "^0.3.0"
+sphinx_rtd_theme = "^1.2.2"
+sphinxcontrib-plantuml = "^0.25"
+peltak-todos = "^0.0.10"
+peltak-changelog = "^0.0.4"
+peltak-gitflow = "^0.0.4"
+
+
+[tool.pytest.ini_options]
+addopts = "--durations=3"
+doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ELLIPSIS"
+
+
+[tool.coverage.run]
+branch = true
+source = ['src']
+omit = []
+
+[tool.coverage.report]
+exclude_lines = ['nocov']
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+
+##################
+#     PYTEST     #
+##################
+
```

