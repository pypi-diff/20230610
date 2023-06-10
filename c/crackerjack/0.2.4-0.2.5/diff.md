# Comparing `tmp/crackerjack-0.2.4.tar.gz` & `tmp/crackerjack-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.2.4.tar", last modified: Fri Jun  2 10:00:54 2023, max compression
+gzip compressed data, was "crackerjack-0.2.5.tar", last modified: Sat Jun 10 16:59:02 2023, max compression
```

## Comparing `crackerjack-0.2.4.tar` & `crackerjack-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.4/LICENSE
--rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-06-02 09:59:42.631901 crackerjack-0.2.4/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      163 2023-06-02 09:59:42.607073 crackerjack-0.2.4/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-06-02 09:59:42.625124 crackerjack-0.2.4/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     1723 2023-06-02 09:59:42.614915 crackerjack-0.2.4/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.4/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.4/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.4/crackerjack/__init__.py
--rw-r--r--   0        0        0     1238 2023-05-27 10:07:36.046052 crackerjack-0.2.4/crackerjack/__main__.py
--rw-r--r--   0        0        0     5570 2023-05-28 14:53:32.418909 crackerjack-0.2.4/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1603 2023-06-02 09:59:43.739879 crackerjack-0.2.4/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     1828 2023-06-02 10:00:54.189526 crackerjack-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4212 1970-01-01 00:00:00.000000 crackerjack-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 16:58:33.090106 crackerjack-0.2.5/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      163 2023-06-10 16:58:33.038512 crackerjack-0.2.5/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-06-10 16:58:33.073814 crackerjack-0.2.5/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     1723 2023-06-10 16:58:33.053914 crackerjack-0.2.5/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.5/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.5/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.5/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-10 14:55:58.374530 crackerjack-0.2.5/crackerjack/__main__.py
+-rw-r--r--   0        0        0     5370 2023-06-10 16:43:42.483425 crackerjack-0.2.5/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1644 2023-06-10 16:58:33.805909 crackerjack-0.2.5/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     1644 2023-06-10 16:59:02.502818 crackerjack-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 crackerjack-0.2.5/PKG-INFO
```

### Comparing `crackerjack-0.2.4/LICENSE` & `crackerjack-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.4/README.md` & `crackerjack-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.4/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.2.5/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.4/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.2.5/crackerjack/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         name: check-added-large-files
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+    rev: v0.0.272
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
     rev: v2.6.1
     hooks:
       - id: creosote
         args:
@@ -35,29 +35,29 @@
     hooks:
       - id: flynt
   - repo: https://github.com/dosisod/refurb
     rev: v1.16.0
     hooks:
       - id: refurb
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.311
+    rev: v1.1.313
     hooks:
       - id: pyright
   #  - repo: https://github.com/pdoc3/pdoc
   #    rev: master
   #    hooks:
   #      - id: pdoc
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+    rev: v0.0.272
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
```

### Comparing `crackerjack-0.2.4/crackerjack/__main__.py` & `crackerjack-0.2.5/crackerjack/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,41 +4,45 @@
 from click import help_option
 from click import option
 from crackerjack import crackerjack_it
 from pydantic import BaseModel
 
 
 class Options(BaseModel):
-    commit = False
-    interactive = False
-    doc = False
-    do_not_update_configs = False
+    commit: bool = False
+    interactive: bool = False
+    doc: bool = False
+    do_not_update_configs: bool = False
     publish: str | bool = False
-    verbose = False
+    verbose: bool = False
+    update_precommit: bool = False
 
 
 options = Options()
 
 
 @command()
 @help_option("-h", is_flag=True, help="help")
 @option("-c", is_flag=True, help="commit")
 @option("-i", is_flag=True, help="interactive")
 @option("-d", is_flag=True, help="doc")
 @option("-x", is_flag=True, help="do not update configs")
+@option("-u", is_flag=True, help="update pre-commit")
 @option("-v", is_flag=True, help="verbose")
 @option("-p", help="publish: -p [micro, minor, major]")
 # @option("-f", help="format: -f [module]")
-def crackerjack(c: bool, i: bool, d: bool, v: bool, x: bool, p: str) -> None:
+def crackerjack(c: bool, i: bool, d: bool, u: bool, v: bool, x: bool, p: str) -> None:
     if c:
         options.commit = c
     if i:
         options.interactive = i
     if d:
         options.doc = d
+    if u:
+        options.update_precommit = u
     if x:
         options.do_not_update_configs = x
     if p in ("micro", "minor", "major"):
         options.publish = p
     if v:
         print("-v not currently implemented")
         options.verbose = v
```

### Comparing `crackerjack-0.2.4/crackerjack/crackerjack.py` & `crackerjack-0.2.5/crackerjack/crackerjack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,60 @@
 import sys
 import typing as t
 from subprocess import call
 from subprocess import check_output
 from subprocess import run
 
-import pdm_bump
-import pdoc
 from acb.actions import dump
 from acb.actions import load
 
-# from addict import Dict
+import pdm_bump
+import pdoc
+
 from aioconsole import ainput
 from aiopath import AsyncPath
-from inflection import underscore
-from inflection import camelize
 from pydantic import BaseModel
-from pydantic import create_model
-from pydantic import Extra
+from pydantic import ConfigDict
 
 for mod in (pdm_bump, pdoc):  # look ruff / isort to get rid of this
     pass
 
 
 # Crackerjack
 
 
 class Crakerjack(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
     our_path: AsyncPath = AsyncPath(__file__)
     pkg_path: AsyncPath = AsyncPath.cwd()
     pkg_dir: t.Optional[AsyncPath] = None
     pkg_name: str = "crackerjack"
     our_toml: t.Optional[dict] = None
     pkg_toml: t.Optional[dict] = None
     our_toml_path: t.Optional[AsyncPath] = None
     pkg_toml_path: t.Optional[AsyncPath] = None
     poetry_pip_env: bool = False
 
-    async def get_toml_config(self, path: AsyncPath) -> BaseModel:
-        class Config(BaseModel.Config):  # type: ignore
-            extra = Extra.allow
-
-        return create_model(
-            camelize(path.stem),
-            __config__=Config,
-            **(await load.toml(path)),
-        )()
-
     async def update_pyproject_configs(self) -> None:
-        our_toml_config = await self.get_toml_config(self.our_toml_path)
-        pkg_toml_config = await self.get_toml_config(self.pkg_toml_path)
+        toml_file = "pyproject.toml"
+        self.our_toml_path = self.our_path.parent / toml_file
+        self.pkg_toml_path = self.pkg_path / toml_file
+        our_toml_config = await load.toml(self.our_toml_path)  # type: ignore
+        pkg_toml_config = await load.toml(self.pkg_toml_path)  # type: ignore
         if self.poetry_pip_env:
-            del pkg_toml_config.tool.poetry
-        pkg_deps = pkg_toml_config.tool["pdm"]["dev-dependencies"]
-        pkg_toml_config.tool = our_toml_config.tool
-        pkg_toml_config.tool["pdm"]["dev-dependencies"] = pkg_deps
+            del pkg_toml_config["tool"]["poetry"]
+        pkg_deps = pkg_toml_config["tool"]["pdm"]["dev-dependencies"]
+        pkg_toml_config.setdefault("tool", our_toml_config.get("tool", {}))
+        pkg_toml_config["tool"]["pdm"]["dev-dependencies"] = pkg_deps
         if self.pkg_path.stem == "crackerjack":
-            await dump.toml(pkg_toml_config.dict(), self.our_toml_path)
+            await dump.toml(pkg_toml_config, self.our_toml_path)  # type: ignore
         else:
-            await dump.toml(pkg_toml_config.dict(), self.pkg_toml_path)
+            await dump.toml(pkg_toml_config, self.pkg_toml_path)  # type: ignore
 
-    async def clean_poetry_pip_env(self) -> None:
+    async def clean_poetry_pipenv(self) -> None:
         root_files = [
             file
             async for file in self.pkg_path.iterdir()
             if ("poetry" or "Pip") in file.name
         ]
         if root_files:
             self.poetry_pip_env = True
@@ -84,56 +75,55 @@
                 await config_path.write_text(await pkg_config_path.read_text())
             # if poetry_pip_env:
             #     await config_pkg_path.unlink()
             config_text = await config_path.read_text()
             await pkg_config_path.write_text(
                 config_text.replace("crackerjack", self.pkg_name)
             )
+            run(["git", "add", config])
 
     @staticmethod
     async def run_interactive(hook: str) -> None:
         success = False
         while not success:
             fail = call(["pre-commit", "run", hook.lower(), "--all-files"])
             if fail > 0:
                 retry = await ainput(f"\n{hook} failed. Retry? (y/n): ")
                 if retry.lower() == "y":
                     continue
                 sys.exit()
             success = True
 
     async def update_pkg_configs(self) -> None:
-        await self.clean_poetry_pip_env()
+        await self.clean_poetry_pipenv()
         await self.copy_configs()
-        toml_file = "pyproject.toml"
-        self.our_toml_path = self.our_path.parent / toml_file
-        self.pkg_toml_path = self.pkg_path / toml_file
-        if not await self.pkg_toml_path.exists():
-            run(["pdm", "init"])
-            run(["pdm", "self", "add", "keyring"])
-            run(["git", "add", "pyproject.toml"])
         installed_pkgs = check_output(
             ["pdm", "list", "--freeze"],
             universal_newlines=True,
         ).splitlines()
         if not len([pkg for pkg in installed_pkgs if "pre-commit" in pkg]):
+            run(["pdm", "--pep582"])
+            run(["pdm", "self", "add", "keyring"])
+            run(["git", "init"])
+            run(["git", "branch", "-m", "main"])
+            run(["git", "add", "pyproject.toml"])
             run(["pdm", "add", "-d", "pre_commit"])
             run(["pre-commit", "install"])
             run(["git", "add", "pdm.lock"])
         await self.update_pyproject_configs()
 
     async def process(self, options: t.Any) -> None:
         imp_dir = self.pkg_path / "__pypackages__"
         sys.path.append(str(imp_dir))
-        self.pkg_name = underscore(self.pkg_path.stem.lower())
+        self.pkg_name = self.pkg_path.stem.lower()
+        # self.pkg_name = underscore(self.pkg_path.stem.lower())
         self.pkg_dir = self.pkg_path / self.pkg_name
         await self.pkg_dir.mkdir(exist_ok=True)
         print("\nCrackerjacking...\n")
-        if self.pkg_path.stem == "crackerjack":
-            run(["git", "add", ".pre-commit-config.yaml"])
+        if self.pkg_path.stem == "crackerjack" and options.update_precommit:
             run(["pre-commit", "autoupdate"])
         if options.publish:
             check_output(["pdm", "bump", options.publish])
         if not options.do_not_update_configs:
             await self.update_pkg_configs()
         if options.interactive:
             for hook in ("refurb", "pyright"):
```

### Comparing `crackerjack-0.2.4/crackerjack/pyproject.toml` & `crackerjack-0.2.5/crackerjack/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-[tool]
 [tool.pdm.dev-dependencies]
-dev = ["pytest>=7.3.0", "icecream>=2.1.3", "pre-commit>=3.2.2"]
+dev = [
+    "pytest>=7.3.0",
+    "icecream>=2.1.3",
+    "pre-commit>=3.2.2",
+    "-e file:///${PROJECT_ROOT}/../acb#egg=acb",
+]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
 show-source = true
@@ -15,56 +19,70 @@
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.black]
-target-version = ["py311"]
-
-[tool.mypy]
-strict = false
-pretty = true
-ignore_missing_imports = false
-plugins = ["pydantic.mypy"]
+target-version = [
+    "py311",
+]
 
 [tool.refurb]
 enable_all = true
 
-[tool.pytype]
-inputs = ["package_name"]
+[tool.pyright]
+include = [
+    "crackerjack",
+]
+reportMissingImports = true
+reportMissingTypeStubs = false
+pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.4"
+version = "0.2.5"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
-keywords = ["black", "ruff", "mypy", "creosote", "refurb"]
-classifiers = ["Environment :: Console", "Operating System :: OS Independent", "Programming Language :: Python", "Programming Language :: Python :: 3.11"]
-dependencies = ["click>=8.1.3", "pdoc3>=0.10.0", "pdm-bump>=0.7.0", "pydantic>=1.10.7", "aiopath>=0.6.11", "acb>=0.1.2", "aioconsole>=0.6.1", "inflection>=0.5.1"]
-
-[[project.authors]]
-name = "lesleslie"
-email = "les@wedgwoodwebworks.com"
-
-[[project.maintainers]]
-name = "lesleslie"
-email = "les@wedgwoodwebworks.com"
+keywords = [
+    "black",
+    "ruff",
+    "mypy",
+    "creosote",
+    "refurb",
+]
+classifiers = [
+    "Environment :: Console",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.11",
+]
+dependencies = [
+    "click>=8.1.3",
+    "pdoc3>=0.10.0",
+    "pdm-bump>=0.7.0",
+    "aiopath>=0.6.11",
+    "aioconsole>=0.6.1",
+    "pydantic>=2.0b2",
+    "acb>=0.1.5",
+]
+authors = [
+    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
+]
+maintainers = [
+    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
+]
 
 [project.license]
 text = "BSD-3-Clause"
 
-[project.optional-dependencies]
-
 [project.urls]
 homepage = "https://github.com/lesleslie/crackerjack"
 documentation = "https://github.com/lesleslie/crackerjack"
 repository = "https://github.com/lesleslie/crackerjack"
 
-[project.scripts]
-
-[project.entry-points]
-
 [build-system]
-requires = ["pdm-backend"]
+requires = [
+    "pdm-backend",
+]
 build-backend = "pdm.backend"
```

### Comparing `crackerjack-0.2.4/pyproject.toml` & `crackerjack-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.0",
     "icecream>=2.1.3",
     "pre-commit>=3.2.2",
+    "-e file:///${PROJECT_ROOT}/../acb#egg=acb",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -22,37 +23,28 @@
 convention = "google"
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
-[tool.mypy]
-strict = false
-pretty = false
-ignore_missing_imports = false
-plugins = [
-    "pydantic.mypy",
-]
-python_version = 3.11
-
 [tool.refurb]
 enable_all = true
 
 [tool.pyright]
 include = [
     "crackerjack",
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.4"
+version = "0.2.5"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -65,39 +57,32 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "click>=8.1.3",
     "pdoc3>=0.10.0",
     "pdm-bump>=0.7.0",
-    "pydantic>=1.10.7",
     "aiopath>=0.6.11",
-    "acb>=0.1.2",
     "aioconsole>=0.6.1",
-    "inflection>=0.5.1",
+    "pydantic>=2.0b2",
+    "acb>=0.1.5",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 
 [project.license]
 text = "BSD-3-Clause"
 
-[project.optional-dependencies]
-
 [project.urls]
 homepage = "https://github.com/lesleslie/crackerjack"
 documentation = "https://github.com/lesleslie/crackerjack"
 repository = "https://github.com/lesleslie/crackerjack"
 
-[project.scripts]
-
-[project.entry-points]
-
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `crackerjack-0.2.4/PKG-INFO` & `crackerjack-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -14,19 +14,18 @@
 Project-URL: Homepage, https://github.com/lesleslie/crackerjack
 Project-URL: Documentation, https://github.com/lesleslie/crackerjack
 Project-URL: Repository, https://github.com/lesleslie/crackerjack
 Requires-Python: >=3.11
 Requires-Dist: click>=8.1.3
 Requires-Dist: pdoc3>=0.10.0
 Requires-Dist: pdm-bump>=0.7.0
-Requires-Dist: pydantic>=1.10.7
 Requires-Dist: aiopath>=0.6.11
-Requires-Dist: acb>=0.1.2
 Requires-Dist: aioconsole>=0.6.1
-Requires-Dist: inflection>=0.5.1
+Requires-Dist: pydantic>=2.0b2
+Requires-Dist: acb>=0.1.5
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
 [![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
```

