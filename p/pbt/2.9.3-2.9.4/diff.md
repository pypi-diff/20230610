# Comparing `tmp/pbt-2.9.3.tar.gz` & `tmp/pbt-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbt-2.9.3.tar", max compression
+gzip compressed data, was "pbt-2.9.4.tar", max compression
```

## Comparing `pbt-2.9.3.tar` & `pbt-2.9.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3451 2022-10-15 20:13:53.643158 pbt-2.9.3/README.md
--rw-r--r--   0        0        0        0 2022-10-15 20:13:53.643158 pbt-2.9.3/pbt/__init__.py
--rw-r--r--   0        0        0     1264 2022-10-15 20:13:53.643158 pbt-2.9.3/pbt/__main__.py
--rw-r--r--   0        0        0     5683 2022-10-15 20:13:53.643158 pbt-2.9.3/pbt/config.py
--rw-r--r--   0        0        0        0 2022-10-15 20:13:53.643158 pbt-2.9.3/pbt/console/__init__.py
--rw-r--r--   0        0        0     1929 2022-10-15 20:13:53.643158 pbt-2.9.3/pbt/console/git.py
--rw-r--r--   0        0        0     9501 2022-10-15 20:13:53.643158 pbt-2.9.3/pbt/console/pbt.py
--rw-r--r--   0        0        0     7548 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/diff.py
--rw-r--r--   0        0        0     3816 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/misc.py
--rw-r--r--   0        0        0        0 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/__init__.py
--rw-r--r--   0        0        0     3319 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/graph.py
--rw-r--r--   0        0        0        0 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/manager/__init__.py
--rw-r--r--   0        0        0    16837 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/manager/manager.py
--rw-r--r--   0        0        0    11201 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/manager/maturin.py
--rw-r--r--   0        0        0    13849 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/manager/poetry.py
--rw-r--r--   0        0        0    12970 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/manager/python.py
--rw-r--r--   0        0        0     6754 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/package.py
--rw-r--r--   0        0        0    10304 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/pipeline.py
--rw-r--r--   0        0        0        0 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/registry/__init__.py
--rw-r--r--   0        0        0     2880 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/registry/pypi.py
--rw-r--r--   0        0        0      434 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/package/registry/registry.py
--rw-r--r--   0        0        0        0 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/vcs/__init__.py
--rw-r--r--   0        0        0    10240 2022-10-15 20:13:53.647158 pbt-2.9.3/pbt/vcs/git.py
--rw-r--r--   0        0        0      834 2022-10-15 20:13:53.647158 pbt-2.9.3/pyproject.toml
--rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 pbt-2.9.3/setup.py
--rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 pbt-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0     3451 2022-10-17 20:44:20.747502 pbt-2.9.4/README.md
+-rw-r--r--   0        0        0        0 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/__init__.py
+-rw-r--r--   0        0        0     1264 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/__main__.py
+-rw-r--r--   0        0        0     5683 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/config.py
+-rw-r--r--   0        0        0        0 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/console/__init__.py
+-rw-r--r--   0        0        0     1929 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/console/git.py
+-rw-r--r--   0        0        0     9463 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/console/pbt.py
+-rw-r--r--   0        0        0     7548 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/diff.py
+-rw-r--r--   0        0        0     3816 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/misc.py
+-rw-r--r--   0        0        0        0 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/__init__.py
+-rw-r--r--   0        0        0     3319 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/graph.py
+-rw-r--r--   0        0        0        0 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/manager/__init__.py
+-rw-r--r--   0        0        0    16837 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/manager/manager.py
+-rw-r--r--   0        0        0    11201 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/manager/maturin.py
+-rw-r--r--   0        0        0    13849 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/manager/poetry.py
+-rw-r--r--   0        0        0    12970 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/manager/python.py
+-rw-r--r--   0        0        0     6754 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/package.py
+-rw-r--r--   0        0        0    10304 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/pipeline.py
+-rw-r--r--   0        0        0        0 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/registry/__init__.py
+-rw-r--r--   0        0        0     2880 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/registry/pypi.py
+-rw-r--r--   0        0        0      434 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/package/registry/registry.py
+-rw-r--r--   0        0        0        0 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/vcs/__init__.py
+-rw-r--r--   0        0        0    10240 2022-10-17 20:44:20.751502 pbt-2.9.4/pbt/vcs/git.py
+-rw-r--r--   0        0        0      834 2022-10-17 20:44:20.751502 pbt-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 pbt-2.9.4/setup.py
+-rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 pbt-2.9.4/PKG-INFO
```

### Comparing `pbt-2.9.3/README.md` & `pbt-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/__main__.py` & `pbt-2.9.4/pbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/config.py` & `pbt-2.9.4/pbt/config.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/console/git.py` & `pbt-2.9.4/pbt/console/git.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/console/pbt.py` & `pbt-2.9.4/pbt/console/pbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,18 +221,18 @@
     verbose: bool = False,
 ):
     """Install a local python package in editable mode without building it. This works by adding .pth file containing the path
     to the package to the site-packages directory.
 
     This is a temporary solution for package requiring extension binary but we cannot build the binary,
     so we have to download the prebuilt binary and put it to the src directory before running this command.
+
+    Note: this command won't enforce version consistency as it is intended to be used in hacky situations.
     """
     pl, cfg, pkgs = init(cwd, [package], verbose)
-    pl.enforce_version_consistency(freeze_packages=cfg.freeze_packages)
-
     pkg = pl.pkgs[package]
     dep_pkg = pl.pkgs[dep]
 
     manager = pl.managers[pkg.type]
     assert isinstance(manager, PythonPkgManager) and isinstance(
         pl.managers[dep_pkg.type], PythonPkgManager
     )
@@ -291,16 +291,14 @@
     package: str,
     cwd: str = ".",
     verbose: bool = False,
     source: Literal["build", "pypi"] = "build",
     clean: bool = False,
 ):
     pl, cfg, pkgs = init(cwd, [package], verbose)
-    pl.enforce_version_consistency(freeze_packages=cfg.freeze_packages)
-
     pkg = pl.pkgs[package]
 
     manager = pl.managers[pkg.type]
     assert isinstance(manager, PythonPkgManager)
 
     dist_dir = (pkg.location / cfg.distribution_dir).absolute()
     shutil.rmtree(dist_dir, ignore_errors=True)
```

### Comparing `pbt-2.9.3/pbt/diff.py` & `pbt-2.9.4/pbt/diff.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/misc.py` & `pbt-2.9.4/pbt/misc.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/graph.py` & `pbt-2.9.4/pbt/package/graph.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/manager/manager.py` & `pbt-2.9.4/pbt/package/manager/manager.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/manager/maturin.py` & `pbt-2.9.4/pbt/package/manager/maturin.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/manager/poetry.py` & `pbt-2.9.4/pbt/package/manager/poetry.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/manager/python.py` & `pbt-2.9.4/pbt/package/manager/python.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/package.py` & `pbt-2.9.4/pbt/package/package.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/pipeline.py` & `pbt-2.9.4/pbt/package/pipeline.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/package/registry/pypi.py` & `pbt-2.9.4/pbt/package/registry/pypi.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pbt/vcs/git.py` & `pbt-2.9.4/pbt/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pbt-2.9.3/pyproject.toml` & `pbt-2.9.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbt"
-version = "2.9.3"
+version = "2.9.4"
 description = "A build tool for multiple Python projects in a single repository"
 authors = ["Binh Vu <binh@toan2.com>"]
 homepage = "https://github.com/binh-vu/pbt"
 repository = "https://github.com/binh-vu/pbt"
 readme = "README.md"
 license = "MIT"
```

### Comparing `pbt-2.9.3/setup.py` & `pbt-2.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'typing-extensions>=4.4.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['pab = pbt.__main__:cli', 'pbt = pbt.__main__:cli']}
 
 setup_kwargs = {
     'name': 'pbt',
-    'version': '2.9.3',
+    'version': '2.9.4',
     'description': 'A build tool for multiple Python projects in a single repository',
     'long_description': '<h1 align="center">PBT</h1>\n\n<div align="center">\n<b>pbt</b> — A build tool for multiple Python projects in a single repository\n    \n![PyPI](https://img.shields.io/pypi/v/pbt)\n![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)\n[![GitHub Issues](https://img.shields.io/github/issues/binh-vu/pbt.svg)](https://github.com/binh-vu/pbt/issues)\n![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)\n[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n\n</div>\n\n## Introduction\n\nHaving all packages in the same repository make it much easier to develop, share, reuse, and refactor code. Building and publishing the packages should not be done manually because it is time-consuming and may be frustrated if the projects are depending on each other. [pbt](https://github.com/binh-vu/pbt) is a tool designed to help make the process easier and faster. It supports building, installing, and updating versions of your packages and their dependencies consistently. It also provides utility commands to help you work with your packages in multi-repositories as if you are working with a monorepo.\n\n## Installation\n\n```bash\npip install -U pbt\n```\n\n## Usage\n\nNote: currently, [pbt](https://github.com/binh-vu/pbt) supports Python packages configured with Poetry (an awesome dependency management that you should consider using).\n\nAssuming that you organized your packages to different sub-folders, each has their own project configuration file (e.g., `pyproject.toml`). You can run the following commands in the root directory (containing your projects). Note: [pbt](https://github.com/binh-vu/pbt) will discover the project based on the project name in its configuration file not the folder name.\n\nYou can also discover the list of commands by running `pbt --help`. Many commands have an option `--cwd` to override the current working directory.\n\n1. **List all packages in the current project, and their dependencies if required**\n\n```bash\npbt list [-d]\n```\n\n- `-d`, `--dev`: Whether to print to the local (inter-) dependencies\n\n2. **Create virtual environment of a package and install its dependencies**\n\n```bash\npbt install [-d] [-v] [-p <package>]\n```\n\n- `-d`: also install dev-dependencies of the package\n- `-v`: verbose\n- `-p`: specify the package we want to build, if empty build all packages.\n\nIf you have encounter some errors during the installation, you can checkout the `pyproject.failed.toml` file that is generated by pbt in `./cache/<package>` folder (relative to your current working directory). For example, on M1 chip, if your python version is `^3.8`, you can\'t use the newer scipy (e.g., >1.8 as it requires python `<3.11`), poetry lock chooses to use an old version `1.6.0`, which typically can\'t build on M1 due to no pre-built numpy for it.\n\n3. **Update all package inter-dependencies**\n\n```bash\npbt update\n```\n\n4. **Clean packages\' build & lock files**\n\n```bash\npbt clean [-p <package>]\n```\n\n- `-p`: specify the package we want to build, if empty build all packages.\n\n6. **Git clone a multi-repository project**\n\n```bash\npbt git clone --repo <repo_url>\n```\n\nClone a repository and check out all of its submodules to their correct branches that we were using last time.\n\n7. **Git update a multi-repository project**\n\n```bash\npbt git update\n```\n\nPull latest changes from the repository, and check out all of its submodules to their correct branches.\n',
     'author': 'Binh Vu',
     'author_email': 'binh@toan2.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/binh-vu/pbt',
```

### Comparing `pbt-2.9.3/PKG-INFO` & `pbt-2.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbt
-Version: 2.9.3
+Version: 2.9.4
 Summary: A build tool for multiple Python projects in a single repository
 Home-page: https://github.com/binh-vu/pbt
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

