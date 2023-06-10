# Comparing `tmp/setuptools_golang-2.7.0.tar.gz` & `tmp/setuptools_golang-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools_golang-2.7.0.tar", last modified: Mon Oct  4 23:21:55 2021, max compression
+gzip compressed data, was "setuptools_golang-2.8.0.tar", last modified: Sat Jun 10 19:08:29 2023, max compression
```

## Comparing `setuptools_golang-2.7.0.tar` & `setuptools_golang-2.8.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-10-04 23:21:55.580727 setuptools_golang-2.7.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2021-10-04 22:25:09.000000 setuptools_golang-2.7.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5480 2021-10-04 23:21:55.580727 setuptools_golang-2.7.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4605 2021-10-04 22:25:09.000000 setuptools_golang-2.7.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1520 2021-10-04 23:21:55.580727 setuptools_golang-2.7.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2021-10-04 22:25:09.000000 setuptools_golang-2.7.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-10-04 23:21:55.580727 setuptools_golang-2.7.0/setuptools_golang.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5480 2021-10-04 23:21:55.000000 setuptools_golang-2.7.0/setuptools_golang.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      265 2021-10-04 23:21:55.000000 setuptools_golang-2.7.0/setuptools_golang.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2021-10-04 23:21:55.000000 setuptools_golang-2.7.0/setuptools_golang.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      178 2021-10-04 23:21:55.000000 setuptools_golang-2.7.0/setuptools_golang.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       18 2021-10-04 23:21:55.000000 setuptools_golang-2.7.0/setuptools_golang.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8044 2021-10-04 23:21:39.000000 setuptools_golang-2.7.0/setuptools_golang.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4800 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4147 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1367 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/setuptools_golang.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4800 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      305 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      177 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       18 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7966 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/setuptools_golang.py
```

### Comparing `setuptools_golang-2.7.0/LICENSE` & `setuptools_golang-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_golang-2.7.0/PKG-INFO` & `setuptools_golang-2.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 Metadata-Version: 2.1
 Name: setuptools_golang
-Version: 2.7.0
+Version: 2.8.0
 Summary: A setuptools extension for building cpython extensions written in golang.
 Home-page: https://github.com/asottile/setuptools-golang
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.1
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setuptools-golang?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=52&branchName=master)
-[![Build status](https://ci.appveyor.com/api/projects/status/j4i2pc4o7pby3wdn/branch/master?svg=true)](https://ci.appveyor.com/project/asottile/setuptools-golang/branch/master)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/52/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=52&branchName=master)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/master.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/master)
+[![build status](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/main)
 
 setuptools-golang
 =================
 
 A setuptools extension for building cpython extensions written in golang.
 
 ## Requirements
 
-This requires golang >= 1.5.  It is currently tested against 1.16 and 1.17.
+This requires golang >= 1.5.
 
-This requires python >= 3.6.  It is currently tested against python3 and pypy3.
+This requires python >= 3.7.  It is currently tested against python3 and pypy3.
 
 ## Platform Support
 
 - linux
 - macOS
 - win32 (32 bit cpython, 32 bit go 1.10+)
 
@@ -140,9 +133,7 @@
 -rw-r--r--  1 1000 1000 2064862 Feb  1 04:16 setuptools_golang_examples-0.1.1-cp35-cp35m-manylinux1_x86_64.whl
 -rw-r--r--  1 1000 1000 2064873 Feb  1 04:16 setuptools_golang_examples-0.1.1-cp36-cp36m-manylinux1_x86_64.whl
 -rw-rw-r--  1 1000 1000    4273 Feb  1 04:14 setuptools-golang-examples-0.1.1.tar.gz
 *******************************************************************************
 Your wheels have been built into ./dist
 *******************************************************************************
 ```
-
-
```

### Comparing `setuptools_golang-2.7.0/README.md` & `setuptools_golang-2.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setuptools-golang?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=52&branchName=master)
-[![Build status](https://ci.appveyor.com/api/projects/status/j4i2pc4o7pby3wdn/branch/master?svg=true)](https://ci.appveyor.com/project/asottile/setuptools-golang/branch/master)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/52/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=52&branchName=master)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/master.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/master)
+[![build status](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/main)
 
 setuptools-golang
 =================
 
 A setuptools extension for building cpython extensions written in golang.
 
 ## Requirements
 
-This requires golang >= 1.5.  It is currently tested against 1.16 and 1.17.
+This requires golang >= 1.5.
 
-This requires python >= 3.6.  It is currently tested against python3 and pypy3.
+This requires python >= 3.7.  It is currently tested against python3 and pypy3.
 
 ## Platform Support
 
 - linux
 - macOS
 - win32 (32 bit cpython, 32 bit go 1.10+)
```

### Comparing `setuptools_golang-2.7.0/setup.cfg` & `setuptools_golang-2.8.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [metadata]
 name = setuptools_golang
-version = 2.7.0
+version = 2.8.0
 description = A setuptools extension for building cpython extensions written in golang.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/setuptools-golang
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = setuptools_golang
-python_requires = >=3.6.1
+install_requires = 
+	setuptools
+python_requires = >=3.7
 
 [options.entry_points]
 console_scripts = 
 	setuptools-golang-build-manylinux-wheels = setuptools_golang:build_manylinux_wheels
 distutils.setup_keywords = 
 	build_golang = setuptools_golang:set_build_ext
 
@@ -40,15 +38,14 @@
 data_file = $PWD/.coverage
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

### Comparing `setuptools_golang-2.7.0/setuptools_golang.egg-info/PKG-INFO` & `setuptools_golang-2.8.0/setuptools_golang.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 Metadata-Version: 2.1
 Name: setuptools-golang
-Version: 2.7.0
+Version: 2.8.0
 Summary: A setuptools extension for building cpython extensions written in golang.
 Home-page: https://github.com/asottile/setuptools-golang
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.1
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setuptools-golang?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=52&branchName=master)
-[![Build status](https://ci.appveyor.com/api/projects/status/j4i2pc4o7pby3wdn/branch/master?svg=true)](https://ci.appveyor.com/project/asottile/setuptools-golang/branch/master)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/52/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=52&branchName=master)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/master.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/master)
+[![build status](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/main)
 
 setuptools-golang
 =================
 
 A setuptools extension for building cpython extensions written in golang.
 
 ## Requirements
 
-This requires golang >= 1.5.  It is currently tested against 1.16 and 1.17.
+This requires golang >= 1.5.
 
-This requires python >= 3.6.  It is currently tested against python3 and pypy3.
+This requires python >= 3.7.  It is currently tested against python3 and pypy3.
 
 ## Platform Support
 
 - linux
 - macOS
 - win32 (32 bit cpython, 32 bit go 1.10+)
 
@@ -140,9 +133,7 @@
 -rw-r--r--  1 1000 1000 2064862 Feb  1 04:16 setuptools_golang_examples-0.1.1-cp35-cp35m-manylinux1_x86_64.whl
 -rw-r--r--  1 1000 1000 2064873 Feb  1 04:16 setuptools_golang_examples-0.1.1-cp36-cp36m-manylinux1_x86_64.whl
 -rw-rw-r--  1 1000 1000    4273 Feb  1 04:14 setuptools-golang-examples-0.1.1.tar.gz
 *******************************************************************************
 Your wheels have been built into ./dist
 *******************************************************************************
 ```
-
-
```

### Comparing `setuptools_golang-2.7.0/setuptools_golang.py` & `setuptools_golang-2.8.0/setuptools_golang.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,38 @@
+from __future__ import annotations
+
 import argparse
 import contextlib
 import copy
 import errno
 import os
 import shlex
 import shutil
 import stat
 import subprocess
 import sys
 import tempfile
-from distutils.ccompiler import CCompiler
-from distutils.dist import Distribution
 from types import TracebackType
 from typing import Any
 from typing import Callable
-from typing import Dict
 from typing import Generator
-from typing import Optional
 from typing import Sequence
-from typing import Tuple
-from typing import Type
 
+from distutils.ccompiler import CCompiler
+from distutils.dist import Distribution
 from setuptools import Extension
 from setuptools.command.build_ext import build_ext as _build_ext
 
 
 def rmtree(path: str) -> None:
     """Newer golang uses readonly dirs & files for module cache."""
     def handle_remove_readonly(
             func: Callable[..., Any],
             path: str,
-            exc: Tuple[Type[OSError], OSError, TracebackType],
+            exc: tuple[type[OSError], OSError, TracebackType],
     ) -> None:
         excvalue = exc[1]
         if (
                 func in (os.rmdir, os.remove, os.unlink) and
                 excvalue.errno == errno.EACCES
         ):
             for p in (path, os.path.dirname(path)):
@@ -52,15 +50,15 @@
         yield tempdir
     finally:
         rmtree(tempdir)
 
 
 def _get_cflags(
         compiler: CCompiler,
-        macros: Sequence[Tuple[str, Optional[str]]],
+        macros: Sequence[tuple[str, str | None]],
 ) -> str:
     args = [f'-I{p}' for p in compiler.include_dirs]
     for macro_name, macro_value in macros:
         if macro_value is None:
             args.append(f'-D{macro_name}')
         else:
             args.append(f'-D{macro_name}={macro_value}')
@@ -73,15 +71,15 @@
 
 
 def _get_ldflags() -> str:
     """Determine the correct link flags.  This attempts compiles similar
     to how autotools does feature detection.
     """
     # windows gcc does not support linking with unresolved symbols
-    if sys.platform == 'win32':  # pragma: no cover (windows)
+    if sys.platform == 'win32':  # pragma: win32 cover
         prefix = getattr(sys, 'real_prefix', sys.prefix)
         libs = os.path.join(prefix, 'libs')
         return '-L{} -lpython{}{}'.format(libs, *sys.version_info[:2])
 
     cc = subprocess.check_output(('go', 'env', 'CC')).decode('UTF-8').strip()
 
     with _tmpdir() as tmpdir:
@@ -97,25 +95,25 @@
                 pass
         else:  # pragma: no cover (platform specific)
             # wellp, none of them worked, fall back to gcc and they'll get a
             # hopefully reasonable error message
             return LFLAG_GCC
 
 
-def _check_call(cmd: Tuple[str, ...], cwd: str, env: Dict[str, str]) -> None:
+def _check_call(cmd: tuple[str, ...], cwd: str, env: dict[str, str]) -> None:
     envparts = [f'{k}={shlex.quote(v)}' for k, v in sorted(tuple(env.items()))]
     print(
         '$ {}'.format(' '.join(envparts + [shlex.quote(p) for p in cmd])),
         file=sys.stderr,
     )
     subprocess.check_call(cmd, cwd=cwd, env=dict(os.environ, **env))
 
 
 def _get_build_extension_method(
-        base: Type[_build_ext],
+        base: type[_build_ext],
         root: str,
         strip: bool,
 ) -> Callable[[_build_ext, Extension], None]:
     def build_extension(self: _build_ext, ext: Extension) -> None:
         # If there are no .go files then the parent should handle this
         if not any(source.endswith('.go') for source in ext.sources):
             # the base class may mutate `self.compiler`
@@ -157,41 +155,41 @@
             env.update({
                 'CGO_CFLAGS': _get_cflags(
                     self.compiler, ext.define_macros or (),
                 ),
                 'CGO_LDFLAGS': _get_ldflags(),
             })
 
-            cmd_build: Tuple[str, ...] = (
+            cmd_build: tuple[str, ...] = (
                 'go', 'build', '-buildmode=c-shared',
                 '-o', os.path.abspath(self.get_ext_fullpath(ext.name)),
             )
             # "-s" omits the symbol table and debug information
             # "-w" omits DWARF debugging information
             if strip:
                 cmd_build = (*cmd_build, '-ldflags=-s -w')
 
             _check_call(cmd_build, cwd=pkg_path, env=env)
 
     return build_extension
 
 
 def _get_build_ext_cls(
-        base: Type[_build_ext],
+        base: type[_build_ext],
         root: str,
         strip: bool = True,
-) -> Type[_build_ext]:
+) -> type[_build_ext]:
     attrs = {'build_extension': _get_build_extension_method(base, root, strip)}
     return type('build_ext', (base,), attrs)
 
 
 def set_build_ext(
         dist: Distribution,
         attr: str,
-        value: Dict[str, Any],
+        value: dict[str, Any],
 ) -> None:
     base = dist.cmdclass.get('build_ext', _build_ext)
     dist.cmdclass['build_ext'] = _get_build_ext_cls(base, **value)
 
 
 GOLANG = 'https://storage.googleapis.com/golang/go{}.linux-amd64.tar.gz'
 SCRIPT = '''\
@@ -203,23 +201,23 @@
 done
 ls *.whl | xargs -n1 --verbose auditwheel repair --wheel-dir /dist
 ls -al /dist
 '''
 
 
 def build_manylinux_wheels(
-        argv: Optional[Sequence[str]] = None,
+        argv: Sequence[str] | None = None,
 ) -> int:  # pragma: no cover
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '--golang', default='1.17.1',
         help='Override golang version (default %(default)s)',
     )
     parser.add_argument(
-        '--pythons', default='cp36-cp36m',
+        '--pythons', default='cp37-cp37m',
         help='Override pythons to build (default %(default)s)',
     )
     args = parser.parse_args(argv)
 
     golang = GOLANG.format(args.golang)
     pythons = ' '.join(args.pythons.split(','))
```

