# Comparing `tmp/circuitree-0.1.0.tar.gz` & `tmp/circuitree-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.1.0.tar", max compression
+gzip compressed data, was "circuitree-0.1.1.tar", max compression
```

## Comparing `circuitree-0.1.0.tar` & `circuitree-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.1.0/LICENSE
--rw-r--r--   0        0        0     1028 2023-06-02 18:56:19.944710 circuitree-0.1.0/README.md
--rwxr-xr-x   0        0        0      117 2023-05-26 21:21:11.249063 circuitree-0.1.0/circuitree/__init__.py
--rwxr-xr-x   0        0        0    15789 2023-06-09 16:17:43.194776 circuitree-0.1.0/circuitree/circuitree.py
--rwxr-xr-x   0        0        0     5381 2023-06-01 21:21:07.888185 circuitree-0.1.0/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.1.0/circuitree/modularity.py
--rw-r--r--   0        0        0     8695 2023-06-08 20:21:23.933282 circuitree-0.1.0/circuitree/parallel.py
--rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.1.0/circuitree/regret.py
--rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.1.0/circuitree/rewards.py
--rw-r--r--   0        0        0      224 2023-06-09 00:12:32.253104 circuitree-0.1.0/circuitree/utils.py
--rw-r--r--   0        0        0      407 2023-05-26 18:26:21.149205 circuitree-0.1.0/circuitree/viz.py
--rw-r--r--   0        0        0     1468 2023-06-09 00:21:50.053096 circuitree-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 circuitree-0.1.0/setup.py
--rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 circuitree-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.1.1/README.md
+-rwxr-xr-x   0        0        0      117 2023-05-26 21:21:11.249063 circuitree-0.1.1/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    15789 2023-06-09 16:17:43.194776 circuitree-0.1.1/circuitree/circuitree.py
+-rwxr-xr-x   0        0        0     5381 2023-06-01 21:21:07.888185 circuitree-0.1.1/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.1.1/circuitree/modularity.py
+-rw-r--r--   0        0        0     8695 2023-06-08 20:21:23.933282 circuitree-0.1.1/circuitree/parallel.py
+-rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.1.1/circuitree/regret.py
+-rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.1.1/circuitree/rewards.py
+-rw-r--r--   0        0        0      224 2023-06-09 00:12:32.253104 circuitree-0.1.1/circuitree/utils.py
+-rw-r--r--   0        0        0      407 2023-05-26 18:26:21.149205 circuitree-0.1.1/circuitree/viz.py
+-rw-r--r--   0        0        0     1469 2023-06-10 00:47:54.514133 circuitree-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 circuitree-0.1.1/setup.py
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 circuitree-0.1.1/PKG-INFO
```

### Comparing `circuitree-0.1.0/LICENSE` & `circuitree-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.0/README.md` & `circuitree-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # CircuiTree
 Genetic circuit design using Monte Carlo tree search
 
 ## Installation
 
 ### From a package repository
-[Installation with `pip`/`conda` is not yet supported]
+To install using `pip`:
+
+```pip install circuitree```
 
 ### From the GitHub repository
 
 To install and use `circuitree` from the GitHub source code, first clone the repo into a directory.
 
 ```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```
 
-Then, enter the directory and build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). by running `poetry install`. This will install a virtual environment in the virtualenv cache directory `POETRY_CACHE_DIR`. To activate this environment interactively as a nested shell, run `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. 
+Then, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). 
 
-For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`.
+From the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. 
 
 ## Usage
 
 See the [quick-start demo](examples/quick_start.ipynb).
```

### Comparing `circuitree-0.1.0/circuitree/circuitree.py` & `circuitree-0.1.1/circuitree/circuitree.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.0/circuitree/models.py` & `circuitree-0.1.1/circuitree/models.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.0/circuitree/modularity.py` & `circuitree-0.1.1/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.0/circuitree/parallel.py` & `circuitree-0.1.1/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.0/circuitree/rewards.py` & `circuitree-0.1.1/circuitree/rewards.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.1.0/pyproject.toml` & `circuitree-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.1.0"
+version = "0.1.1"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -33,15 +33,15 @@
 sacred = "^0.8.4"
 h5py = "^3.8.0"
 datashader = "^0.14.4"
 hiveplotlib = "^0.21"
 psutil = "^5.9.4"
 matplotlib = "^3.7.1"
 pandas = "^2.0.0"
-numba = "^0.56.4"
+numba = ">=0.57.0"
 scipy = { python = ">=3.10,<3.12", version = "^1.10.1" }
 tqdm = "^4.65.0"
 
 [tool.poetry.extras]
 examples = [
     "scipy",
     "numba",
```

### Comparing `circuitree-0.1.0/setup.py` & `circuitree-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['networkx>=3.1,<4.0', 'numpy>=1.23.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Genetic circuit design using Monte Carlo tree search',
-    'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\n[Installation with `pip`/`conda` is not yet supported]\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, enter the directory and build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). by running `poetry install`. This will install a virtual environment in the virtualenv cache directory `POETRY_CACHE_DIR`. To activate this environment interactively as a nested shell, run `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. \n\nFor instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`.\n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
+    'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `circuitree-0.1.0/PKG-INFO` & `circuitree-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.1.0
+Version: 0.1.1
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -18,23 +18,25 @@
 
 # CircuiTree
 Genetic circuit design using Monte Carlo tree search
 
 ## Installation
 
 ### From a package repository
-[Installation with `pip`/`conda` is not yet supported]
+To install using `pip`:
+
+```pip install circuitree```
 
 ### From the GitHub repository
 
 To install and use `circuitree` from the GitHub source code, first clone the repo into a directory.
 
 ```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```
 
-Then, enter the directory and build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). by running `poetry install`. This will install a virtual environment in the virtualenv cache directory `POETRY_CACHE_DIR`. To activate this environment interactively as a nested shell, run `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. 
+Then, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). 
 
-For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`.
+From the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. 
 
 ## Usage
 
 See the [quick-start demo](examples/quick_start.ipynb).
```

