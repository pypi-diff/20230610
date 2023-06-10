# Comparing `tmp/circuitree-0.1.1.tar.gz` & `tmp/circuitree-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.1.1.tar", max compression
+gzip compressed data, was "circuitree-0.1.2.tar", max compression
```

## Comparing `circuitree-0.1.1.tar` & `circuitree-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.1.1/LICENSE
--rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.1.1/README.md
--rwxr-xr-x   0        0        0      117 2023-05-26 21:21:11.249063 circuitree-0.1.1/circuitree/__init__.py
--rwxr-xr-x   0        0        0    15789 2023-06-09 16:17:43.194776 circuitree-0.1.1/circuitree/circuitree.py
--rwxr-xr-x   0        0        0     5381 2023-06-01 21:21:07.888185 circuitree-0.1.1/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.1.1/circuitree/modularity.py
--rw-r--r--   0        0        0     8695 2023-06-08 20:21:23.933282 circuitree-0.1.1/circuitree/parallel.py
--rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.1.1/circuitree/regret.py
--rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.1.1/circuitree/rewards.py
--rw-r--r--   0        0        0      224 2023-06-09 00:12:32.253104 circuitree-0.1.1/circuitree/utils.py
--rw-r--r--   0        0        0      407 2023-05-26 18:26:21.149205 circuitree-0.1.1/circuitree/viz.py
--rw-r--r--   0        0        0     1469 2023-06-10 00:47:54.514133 circuitree-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 circuitree-0.1.1/setup.py
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 circuitree-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.1.2/README.md
+-rwxr-xr-x   0        0        0      117 2023-05-26 21:21:11.249063 circuitree-0.1.2/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    15789 2023-06-09 16:17:43.194776 circuitree-0.1.2/circuitree/circuitree.py
+-rwxr-xr-x   0        0        0     5381 2023-06-01 21:21:07.888185 circuitree-0.1.2/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.1.2/circuitree/modularity.py
+-rw-r--r--   0        0        0     8695 2023-06-08 20:21:23.933282 circuitree-0.1.2/circuitree/parallel.py
+-rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.1.2/circuitree/regret.py
+-rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.1.2/circuitree/rewards.py
+-rw-r--r--   0        0        0      224 2023-06-09 00:12:32.253104 circuitree-0.1.2/circuitree/utils.py
+-rw-r--r--   0        0        0      407 2023-05-26 18:26:21.149205 circuitree-0.1.2/circuitree/viz.py
+-rw-r--r--   0        0        0     1469 2023-06-10 07:29:13.219330 circuitree-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 circuitree-0.1.2/setup.py
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 circuitree-0.1.2/PKG-INFO
```

### Comparing `circuitree-0.1.1/LICENSE` & `circuitree-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.1/README.md` & `circuitree-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.1/circuitree/circuitree.py` & `circuitree-0.1.2/circuitree/circuitree.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.1/circuitree/models.py` & `circuitree-0.1.2/circuitree/models.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.1/circuitree/modularity.py` & `circuitree-0.1.2/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.1/circuitree/parallel.py` & `circuitree-0.1.2/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.1/circuitree/rewards.py` & `circuitree-0.1.2/circuitree/rewards.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.1/pyproject.toml` & `circuitree-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.1.1"
+version = "0.1.2"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `circuitree-0.1.1/setup.py` & `circuitree-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['networkx>=3.1,<4.0', 'numpy>=1.23.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.1.1/PKG-INFO` & `circuitree-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.1.1
+Version: 0.1.2
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

