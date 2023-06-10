# Comparing `tmp/platformdirs-3.5.1.tar.gz` & `tmp/platformdirs-3.5.2.tar.gz`

## Comparing `platformdirs-3.5.1.tar` & `platformdirs-3.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tox.ini
--rw-r--r--   0        0        0    18902 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/android.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/api.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/py.typed
--rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/version.py
--rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/windows.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/conftest.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_android.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_api.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_main.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.1/LICENSE
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 platformdirs-3.5.1/README.rst
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 platformdirs-3.5.1/pyproject.toml
--rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 platformdirs-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tox.ini
+-rw-r--r--   0        0        0    19758 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/android.py
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/version.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_android.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_api.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_main.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.2/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.2/LICENSE
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 platformdirs-3.5.2/README.rst
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 platformdirs-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 platformdirs-3.5.2/PKG-INFO
```

### Comparing `platformdirs-3.5.1/tox.ini` & `platformdirs-3.5.2/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -37,37 +37,37 @@
       --cov-report html:{envtmpdir}{/}htmlcov --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
 
 [testenv:fix]
 description = run static analysis and style check using flake8
 skip_install = true
 deps =
-    pre-commit>=3.3.1
+    pre-commit>=3.3.2
 pass_env =
     HOMEPATH
     PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.2
+    mypy==1.3
 set_env =
     {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy --strict src
     mypy --strict tests
 
 [testenv:coverage]
 description = combine coverage files and generate diff (against DIFF_AGAINST defaulting to origin/main)
 skip_install = true
 deps =
     covdefaults>=2.3
-    coverage[toml]>=7.2.5
+    coverage[toml]>=7.2.7
     diff-cover>=7.5
 extras =
 parallel_show_output = true
 pass_env =
     DIFF_AGAINST
 set_env =
     COVERAGE_FILE = {toxworkdir}/.coverage
```

### Comparing `platformdirs-3.5.1/src/platformdirs/__init__.py` & `platformdirs-3.5.2/src/platformdirs/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 Utilities for determining application-specific dirs. See <https://github.com/platformdirs/platformdirs> for details and
 usage.
 """
 from __future__ import annotations
 
 import os
 import sys
-from pathlib import Path
-
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from typing import Literal
-else:  # pragma: no cover (py38+)
-    from typing_extensions import Literal
+from typing import TYPE_CHECKING
 
 from .api import PlatformDirsABC
 from .version import __version__
 from .version import __version_tuple__ as __version_info__
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
+        from typing import Literal
+    else:  # pragma: no cover (py38+)
+        from typing_extensions import Literal
+
 
 def _set_platform_dir_class() -> type[PlatformDirsABC]:
     if sys.platform == "win32":
         from platformdirs.windows import Windows as Result
     elif sys.platform == "darwin":
         from platformdirs.macos import MacOS as Result
     else:
@@ -44,16 +47,16 @@
 AppDirs = PlatformDirs  #: Backwards compatibility with appdirs
 
 
 def user_data_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    roaming: bool = False,
-    ensure_exists: bool = False,
+    roaming: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param roaming: See `roaming <platformdirs.api.PlatformDirsABC.roaming>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -68,16 +71,16 @@
     ).user_data_dir
 
 
 def site_data_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    multipath: bool = False,
-    ensure_exists: bool = False,
+    multipath: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param multipath: See `roaming <platformdirs.api.PlatformDirsABC.multipath>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -92,16 +95,16 @@
     ).site_data_dir
 
 
 def user_config_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    roaming: bool = False,
-    ensure_exists: bool = False,
+    roaming: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param roaming: See `roaming <platformdirs.api.PlatformDirsABC.roaming>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -116,16 +119,16 @@
     ).user_config_dir
 
 
 def site_config_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    multipath: bool = False,
-    ensure_exists: bool = False,
+    multipath: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param multipath: See `roaming <platformdirs.api.PlatformDirsABC.multipath>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -140,16 +143,16 @@
     ).site_config_dir
 
 
 def user_cache_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `roaming <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -164,16 +167,16 @@
     ).user_cache_dir
 
 
 def site_cache_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `opinion <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -188,16 +191,16 @@
     ).site_cache_dir
 
 
 def user_state_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    roaming: bool = False,
-    ensure_exists: bool = False,
+    roaming: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param roaming: See `roaming <platformdirs.api.PlatformDirsABC.roaming>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -212,16 +215,16 @@
     ).user_state_dir
 
 
 def user_log_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `roaming <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -233,47 +236,39 @@
         version=version,
         opinion=opinion,
         ensure_exists=ensure_exists,
     ).user_log_dir
 
 
 def user_documents_dir() -> str:
-    """
-    :returns: documents directory tied to the user
-    """
+    """:returns: documents directory tied to the user"""
     return PlatformDirs().user_documents_dir
 
 
 def user_pictures_dir() -> str:
-    """
-    :returns: pictures directory tied to the user
-    """
+    """:returns: pictures directory tied to the user"""
     return PlatformDirs().user_pictures_dir
 
 
 def user_videos_dir() -> str:
-    """
-    :returns: videos directory tied to the user
-    """
+    """:returns: videos directory tied to the user"""
     return PlatformDirs().user_videos_dir
 
 
 def user_music_dir() -> str:
-    """
-    :returns: music directory tied to the user
-    """
+    """:returns: music directory tied to the user"""
     return PlatformDirs().user_music_dir
 
 
 def user_runtime_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> str:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `opinion <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -288,16 +283,16 @@
     ).user_runtime_dir
 
 
 def user_data_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    roaming: bool = False,
-    ensure_exists: bool = False,
+    roaming: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param roaming: See `roaming <platformdirs.api.PlatformDirsABC.roaming>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -312,16 +307,16 @@
     ).user_data_path
 
 
 def site_data_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    multipath: bool = False,
-    ensure_exists: bool = False,
+    multipath: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param multipath: See `multipath <platformdirs.api.PlatformDirsABC.multipath>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -336,16 +331,16 @@
     ).site_data_path
 
 
 def user_config_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    roaming: bool = False,
-    ensure_exists: bool = False,
+    roaming: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param roaming: See `roaming <platformdirs.api.PlatformDirsABC.roaming>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -360,16 +355,16 @@
     ).user_config_path
 
 
 def site_config_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    multipath: bool = False,
-    ensure_exists: bool = False,
+    multipath: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param multipath: See `roaming <platformdirs.api.PlatformDirsABC.multipath>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -384,16 +379,16 @@
     ).site_config_path
 
 
 def site_cache_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `opinion <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -408,16 +403,16 @@
     ).site_cache_path
 
 
 def user_cache_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `roaming <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -432,16 +427,16 @@
     ).user_cache_path
 
 
 def user_state_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    roaming: bool = False,
-    ensure_exists: bool = False,
+    roaming: bool = False,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param roaming: See `roaming <platformdirs.api.PlatformDirsABC.roaming>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -456,16 +451,16 @@
     ).user_state_path
 
 
 def user_log_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `roaming <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
@@ -477,47 +472,39 @@
         version=version,
         opinion=opinion,
         ensure_exists=ensure_exists,
     ).user_log_path
 
 
 def user_documents_path() -> Path:
-    """
-    :returns: documents path tied to the user
-    """
+    """:returns: documents path tied to the user"""
     return PlatformDirs().user_documents_path
 
 
 def user_pictures_path() -> Path:
-    """
-    :returns: pictures path tied to the user
-    """
+    """:returns: pictures path tied to the user"""
     return PlatformDirs().user_pictures_path
 
 
 def user_videos_path() -> Path:
-    """
-    :returns: videos path tied to the user
-    """
+    """:returns: videos path tied to the user"""
     return PlatformDirs().user_videos_path
 
 
 def user_music_path() -> Path:
-    """
-    :returns: music path tied to the user
-    """
+    """:returns: music path tied to the user"""
     return PlatformDirs().user_music_path
 
 
 def user_runtime_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
-    opinion: bool = True,
-    ensure_exists: bool = False,
+    opinion: bool = True,  # noqa: FBT001, FBT002
+    ensure_exists: bool = False,  # noqa: FBT001, FBT002
 ) -> Path:
     """
     :param appname: See `appname <platformdirs.api.PlatformDirsABC.appname>`.
     :param appauthor: See `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`.
     :param version: See `version <platformdirs.api.PlatformDirsABC.version>`.
     :param opinion: See `opinion <platformdirs.api.PlatformDirsABC.opinion>`.
     :param ensure_exists: See `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
```

### Comparing `platformdirs-3.5.1/src/platformdirs/__main__.py` & `platformdirs-3.5.2/src/platformdirs/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Main entry point."""
 from __future__ import annotations
 
 from platformdirs import PlatformDirs, __version__
 
 PROPS = (
     "user_data_dir",
     "user_config_dir",
@@ -16,35 +17,36 @@
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
 )
 
 
 def main() -> None:
+    """Run main entry point."""
     app_name = "MyApp"
     app_author = "MyCompany"
 
-    print(f"-- platformdirs {__version__} --")
+    print(f"-- platformdirs {__version__} --")  # noqa: T201
 
-    print("-- app dirs (with optional 'version')")
+    print("-- app dirs (with optional 'version')")  # noqa: T201
     dirs = PlatformDirs(app_name, app_author, version="1.0")
     for prop in PROPS:
-        print(f"{prop}: {getattr(dirs, prop)}")
+        print(f"{prop}: {getattr(dirs, prop)}")  # noqa: T201
 
-    print("\n-- app dirs (without optional 'version')")
+    print("\n-- app dirs (without optional 'version')")  # noqa: T201
     dirs = PlatformDirs(app_name, app_author)
     for prop in PROPS:
-        print(f"{prop}: {getattr(dirs, prop)}")
+        print(f"{prop}: {getattr(dirs, prop)}")  # noqa: T201
 
-    print("\n-- app dirs (without optional 'appauthor')")
+    print("\n-- app dirs (without optional 'appauthor')")  # noqa: T201
     dirs = PlatformDirs(app_name)
     for prop in PROPS:
-        print(f"{prop}: {getattr(dirs, prop)}")
+        print(f"{prop}: {getattr(dirs, prop)}")  # noqa: T201
 
-    print("\n-- app dirs (with disabled 'appauthor')")
+    print("\n-- app dirs (with disabled 'appauthor')")  # noqa: T201
     dirs = PlatformDirs(app_name, appauthor=False)
     for prop in PROPS:
-        print(f"{prop}: {getattr(dirs, prop)}")
+        print(f"{prop}: {getattr(dirs, prop)}")  # noqa: T201
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `platformdirs-3.5.1/src/platformdirs/android.py` & `platformdirs-3.5.2/src/platformdirs/android.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Android."""
 from __future__ import annotations
 
 import os
 import re
 import sys
 from functools import lru_cache
 from typing import cast
@@ -26,15 +27,16 @@
     def site_data_dir(self) -> str:
         """:return: data directory shared by users, same as `user_data_dir`"""
         return self.user_data_dir
 
     @property
     def user_config_dir(self) -> str:
         """
-        :return: config directory tied to the user, e.g. ``/data/user/<userid>/<packagename>/shared_prefs/<AppName>``
+        :return: config directory tied to the user, e.g. \
+        ``/data/user/<userid>/<packagename>/shared_prefs/<AppName>``
         """
         return self._append_app_name_and_version(cast(str, _android_folder()), "shared_prefs")
 
     @property
     def site_config_dir(self) -> str:
         """:return: config directory shared by the users, same as `user_config_dir`"""
         return self.user_config_dir
@@ -58,67 +60,59 @@
     def user_log_dir(self) -> str:
         """
         :return: log directory tied to the user, same as `user_cache_dir` if not opinionated else ``log`` in it,
           e.g. ``/data/user/<userid>/<packagename>/cache/<AppName>/log``
         """
         path = self.user_cache_dir
         if self.opinion:
-            path = os.path.join(path, "log")
+            path = os.path.join(path, "log")  # noqa: PTH118
         return path
 
     @property
     def user_documents_dir(self) -> str:
-        """
-        :return: documents directory tied to the user e.g. ``/storage/emulated/0/Documents``
-        """
+        """:return: documents directory tied to the user e.g. ``/storage/emulated/0/Documents``"""
         return _android_documents_folder()
 
     @property
     def user_pictures_dir(self) -> str:
-        """
-        :return: pictures directory tied to the user e.g. ``/storage/emulated/0/Pictures``
-        """
+        """:return: pictures directory tied to the user e.g. ``/storage/emulated/0/Pictures``"""
         return _android_pictures_folder()
 
     @property
     def user_videos_dir(self) -> str:
-        """
-        :return: videos directory tied to the user e.g. ``/storage/emulated/0/DCIM/Camera``
-        """
+        """:return: videos directory tied to the user e.g. ``/storage/emulated/0/DCIM/Camera``"""
         return _android_videos_folder()
 
     @property
     def user_music_dir(self) -> str:
-        """
-        :return: music directory tied to the user e.g. ``/storage/emulated/0/Music``
-        """
+        """:return: music directory tied to the user e.g. ``/storage/emulated/0/Music``"""
         return _android_music_folder()
 
     @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, same as `user_cache_dir` if not opinionated else ``tmp`` in it,
           e.g. ``/data/user/<userid>/<packagename>/cache/<AppName>/tmp``
         """
         path = self.user_cache_dir
         if self.opinion:
-            path = os.path.join(path, "tmp")
+            path = os.path.join(path, "tmp")  # noqa: PTH118
         return path
 
 
 @lru_cache(maxsize=1)
 def _android_folder() -> str | None:
-    """:return: base folder for the Android OS or None if cannot be found"""
+    """:return: base folder for the Android OS or None if it cannot be found"""
     try:
         # First try to get path to android app via pyjnius
         from jnius import autoclass
 
-        Context = autoclass("android.content.Context")  # noqa: N806
-        result: str | None = Context.getFilesDir().getParentFile().getAbsolutePath()
-    except Exception:
+        context = autoclass("android.content.Context")
+        result: str | None = context.getFilesDir().getParentFile().getAbsolutePath()
+    except Exception:  # noqa: BLE001
         # if fails find an android folder looking path on the sys.path
         pattern = re.compile(r"/data/(data|user/\d+)/(.+)/files")
         for path in sys.path:
             if pattern.match(path):
                 result = path.split("/files")[0]
                 break
         else:
@@ -129,66 +123,66 @@
 @lru_cache(maxsize=1)
 def _android_documents_folder() -> str:
     """:return: documents folder for the Android OS"""
     # Get directories with pyjnius
     try:
         from jnius import autoclass
 
-        Context = autoclass("android.content.Context")  # noqa: N806
-        Environment = autoclass("android.os.Environment")  # noqa: N806
-        documents_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_DOCUMENTS).getAbsolutePath()
-    except Exception:
+        context = autoclass("android.content.Context")
+        environment = autoclass("android.os.Environment")
+        documents_dir: str = context.getExternalFilesDir(environment.DIRECTORY_DOCUMENTS).getAbsolutePath()
+    except Exception:  # noqa: BLE001
         documents_dir = "/storage/emulated/0/Documents"
 
     return documents_dir
 
 
 @lru_cache(maxsize=1)
 def _android_pictures_folder() -> str:
     """:return: pictures folder for the Android OS"""
     # Get directories with pyjnius
     try:
         from jnius import autoclass
 
-        Context = autoclass("android.content.Context")  # noqa: N806
-        Environment = autoclass("android.os.Environment")  # noqa: N806
-        pictures_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_PICTURES).getAbsolutePath()
-    except Exception:
+        context = autoclass("android.content.Context")
+        environment = autoclass("android.os.Environment")
+        pictures_dir: str = context.getExternalFilesDir(environment.DIRECTORY_PICTURES).getAbsolutePath()
+    except Exception:  # noqa: BLE001
         pictures_dir = "/storage/emulated/0/Pictures"
 
     return pictures_dir
 
 
 @lru_cache(maxsize=1)
 def _android_videos_folder() -> str:
     """:return: videos folder for the Android OS"""
     # Get directories with pyjnius
     try:
         from jnius import autoclass
 
-        Context = autoclass("android.content.Context")  # noqa: N806
-        Environment = autoclass("android.os.Environment")  # noqa: N806
-        videos_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_DCIM).getAbsolutePath()
-    except Exception:
+        context = autoclass("android.content.Context")
+        environment = autoclass("android.os.Environment")
+        videos_dir: str = context.getExternalFilesDir(environment.DIRECTORY_DCIM).getAbsolutePath()
+    except Exception:  # noqa: BLE001
         videos_dir = "/storage/emulated/0/DCIM/Camera"
 
     return videos_dir
 
 
 @lru_cache(maxsize=1)
 def _android_music_folder() -> str:
     """:return: music folder for the Android OS"""
     # Get directories with pyjnius
     try:
         from jnius import autoclass
 
-        Context = autoclass("android.content.Context")  # noqa: N806
-        Environment = autoclass("android.os.Environment")  # noqa: N806
-        music_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_MUSIC).getAbsolutePath()
-    except Exception:
+        context = autoclass("android.content.Context")
+        environment = autoclass("android.os.Environment")
+        music_dir: str = context.getExternalFilesDir(environment.DIRECTORY_MUSIC).getAbsolutePath()
+    except Exception:  # noqa: BLE001
         music_dir = "/storage/emulated/0/Music"
 
     return music_dir
 
 
 __all__ = [
     "Android",
```

### Comparing `platformdirs-3.5.1/src/platformdirs/api.py` & `platformdirs-3.5.2/src/platformdirs/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+"""Base API."""
 from __future__ import annotations
 
 import os
-import sys
 from abc import ABC, abstractmethod
 from pathlib import Path
+from typing import TYPE_CHECKING
 
-if sys.version_info >= (3, 8):  # pragma: no branch
-    from typing import Literal  # pragma: no cover
+if TYPE_CHECKING:
+    import sys
+
+    if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
+        from typing import Literal
+    else:  # pragma: no cover (py38+)
+        from typing_extensions import Literal
 
 
 class PlatformDirsABC(ABC):
-    """
-    Abstract base class for platform directories.
-    """
+    """Abstract base class for platform directories."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         appname: str | None = None,
         appauthor: str | None | Literal[False] = None,
         version: str | None = None,
-        roaming: bool = False,
-        multipath: bool = False,
-        opinion: bool = True,
-        ensure_exists: bool = False,
-    ):
+        roaming: bool = False,  # noqa: FBT001, FBT002
+        multipath: bool = False,  # noqa: FBT001, FBT002
+        opinion: bool = True,  # noqa: FBT001, FBT002
+        ensure_exists: bool = False,  # noqa: FBT001, FBT002
+    ) -> None:
         """
         Create a new platform directory.
 
         :param appname: See `appname`.
         :param appauthor: See `appauthor`.
         :param version: See `version`.
         :param roaming: See `roaming`.
@@ -66,15 +70,15 @@
 
     def _append_app_name_and_version(self, *base: str) -> str:
         params = list(base[1:])
         if self.appname:
             params.append(self.appname)
             if self.version:
                 params.append(self.version)
-        path = os.path.join(base[0], *params)
+        path = os.path.join(base[0], *params)  # noqa: PTH118
         self._optionally_create_directory(path)
         return path
 
     def _optionally_create_directory(self, path: str) -> None:
         if self.ensure_exists:
             Path(path).mkdir(parents=True, exist_ok=True)
```

### Comparing `platformdirs-3.5.1/src/platformdirs/macos.py` & `platformdirs-3.5.2/src/platformdirs/macos.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+"""macOS."""
 from __future__ import annotations
 
-import os
+import os.path
 
 from .api import PlatformDirsABC
 
 
 class MacOS(PlatformDirsABC):
     """
     Platform directories for the macOS operating system. Follows the guidance from `Apple documentation
@@ -13,15 +14,15 @@
     `version <platformdirs.api.PlatformDirsABC.version>`,
     `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
     """
 
     @property
     def user_data_dir(self) -> str:
         """:return: data directory tied to the user, e.g. ``~/Library/Application Support/$appname/$version``"""
-        return self._append_app_name_and_version(os.path.expanduser("~/Library/Application Support"))
+        return self._append_app_name_and_version(os.path.expanduser("~/Library/Application Support"))  # noqa: PTH111
 
     @property
     def site_data_dir(self) -> str:
         """:return: data directory shared by users, e.g. ``/Library/Application Support/$appname/$version``"""
         return self._append_app_name_and_version("/Library/Application Support")
 
     @property
@@ -33,53 +34,53 @@
     def site_config_dir(self) -> str:
         """:return: config directory shared by the users, same as `site_data_dir`"""
         return self.site_data_dir
 
     @property
     def user_cache_dir(self) -> str:
         """:return: cache directory tied to the user, e.g. ``~/Library/Caches/$appname/$version``"""
-        return self._append_app_name_and_version(os.path.expanduser("~/Library/Caches"))
+        return self._append_app_name_and_version(os.path.expanduser("~/Library/Caches"))  # noqa: PTH111
 
     @property
     def site_cache_dir(self) -> str:
         """:return: cache directory shared by users, e.g. ``/Library/Caches/$appname/$version``"""
         return self._append_app_name_and_version("/Library/Caches")
 
     @property
     def user_state_dir(self) -> str:
         """:return: state directory tied to the user, same as `user_data_dir`"""
         return self.user_data_dir
 
     @property
     def user_log_dir(self) -> str:
         """:return: log directory tied to the user, e.g. ``~/Library/Logs/$appname/$version``"""
-        return self._append_app_name_and_version(os.path.expanduser("~/Library/Logs"))
+        return self._append_app_name_and_version(os.path.expanduser("~/Library/Logs"))  # noqa: PTH111
 
     @property
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user, e.g. ``~/Documents``"""
-        return os.path.expanduser("~/Documents")
+        return os.path.expanduser("~/Documents")  # noqa: PTH111
 
     @property
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user, e.g. ``~/Pictures``"""
-        return os.path.expanduser("~/Pictures")
+        return os.path.expanduser("~/Pictures")  # noqa: PTH111
 
     @property
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user, e.g. ``~/Movies``"""
-        return os.path.expanduser("~/Movies")
+        return os.path.expanduser("~/Movies")  # noqa: PTH111
 
     @property
     def user_music_dir(self) -> str:
         """:return: music directory tied to the user, e.g. ``~/Music``"""
-        return os.path.expanduser("~/Music")
+        return os.path.expanduser("~/Music")  # noqa: PTH111
 
     @property
     def user_runtime_dir(self) -> str:
         """:return: runtime directory tied to the user, e.g. ``~/Library/Caches/TemporaryItems/$appname/$version``"""
-        return self._append_app_name_and_version(os.path.expanduser("~/Library/Caches/TemporaryItems"))
+        return self._append_app_name_and_version(os.path.expanduser("~/Library/Caches/TemporaryItems"))  # noqa: PTH111
 
 
 __all__ = [
     "MacOS",
 ]
```

### Comparing `platformdirs-3.5.1/src/platformdirs/unix.py` & `platformdirs-3.5.2/src/platformdirs/unix.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+"""Unix."""
 from __future__ import annotations
 
 import os
 import sys
 from configparser import ConfigParser
 from pathlib import Path
 
 from .api import PlatformDirsABC
 
 if sys.platform == "win32":
 
     def getuid() -> int:
-        raise RuntimeError("should only be used on Unix")
+        msg = "should only be used on Unix"
+        raise RuntimeError(msg)
 
 else:
     from os import getuid
 
 
 class Unix(PlatformDirsABC):
     """
@@ -33,15 +35,15 @@
     def user_data_dir(self) -> str:
         """
         :return: data directory tied to the user, e.g. ``~/.local/share/$appname/$version`` or
          ``$XDG_DATA_HOME/$appname/$version``
         """
         path = os.environ.get("XDG_DATA_HOME", "")
         if not path.strip():
-            path = os.path.expanduser("~/.local/share")
+            path = os.path.expanduser("~/.local/share")  # noqa: PTH111
         return self._append_app_name_and_version(path)
 
     @property
     def site_data_dir(self) -> str:
         """
         :return: data directories shared by users (if `multipath <platformdirs.api.PlatformDirsABC.multipath>` is
          enabled and ``XDG_DATA_DIR`` is set and a multi path the response is also a multi path separated by the OS
@@ -53,26 +55,26 @@
             path = f"/usr/local/share{os.pathsep}/usr/share"
         return self._with_multi_path(path)
 
     def _with_multi_path(self, path: str) -> str:
         path_list = path.split(os.pathsep)
         if not self.multipath:
             path_list = path_list[0:1]
-        path_list = [self._append_app_name_and_version(os.path.expanduser(p)) for p in path_list]
+        path_list = [self._append_app_name_and_version(os.path.expanduser(p)) for p in path_list]  # noqa: PTH111
         return os.pathsep.join(path_list)
 
     @property
     def user_config_dir(self) -> str:
         """
         :return: config directory tied to the user, e.g. ``~/.config/$appname/$version`` or
          ``$XDG_CONFIG_HOME/$appname/$version``
         """
         path = os.environ.get("XDG_CONFIG_HOME", "")
         if not path.strip():
-            path = os.path.expanduser("~/.config")
+            path = os.path.expanduser("~/.config")  # noqa: PTH111
         return self._append_app_name_and_version(path)
 
     @property
     def site_config_dir(self) -> str:
         """
         :return: config directories shared by users (if `multipath <platformdirs.api.PlatformDirsABC.multipath>`
          is enabled and ``XDG_DATA_DIR`` is set and a multi path the response is also a multi path separated by the OS
@@ -88,71 +90,59 @@
     def user_cache_dir(self) -> str:
         """
         :return: cache directory tied to the user, e.g. ``~/.cache/$appname/$version`` or
          ``~/$XDG_CACHE_HOME/$appname/$version``
         """
         path = os.environ.get("XDG_CACHE_HOME", "")
         if not path.strip():
-            path = os.path.expanduser("~/.cache")
+            path = os.path.expanduser("~/.cache")  # noqa: PTH111
         return self._append_app_name_and_version(path)
 
     @property
     def site_cache_dir(self) -> str:
-        """
-        :return: cache directory shared by users, e.g. ``/var/tmp/$appname/$version``
-        """
-        return self._append_app_name_and_version("/var/tmp")
+        """:return: cache directory shared by users, e.g. ``/var/tmp/$appname/$version``"""
+        return self._append_app_name_and_version("/var/tmp")  # noqa: S108
 
     @property
     def user_state_dir(self) -> str:
         """
         :return: state directory tied to the user, e.g. ``~/.local/state/$appname/$version`` or
          ``$XDG_STATE_HOME/$appname/$version``
         """
         path = os.environ.get("XDG_STATE_HOME", "")
         if not path.strip():
-            path = os.path.expanduser("~/.local/state")
+            path = os.path.expanduser("~/.local/state")  # noqa: PTH111
         return self._append_app_name_and_version(path)
 
     @property
     def user_log_dir(self) -> str:
-        """
-        :return: log directory tied to the user, same as `user_state_dir` if not opinionated else ``log`` in it
-        """
+        """:return: log directory tied to the user, same as `user_state_dir` if not opinionated else ``log`` in it"""
         path = self.user_state_dir
         if self.opinion:
-            path = os.path.join(path, "log")
+            path = os.path.join(path, "log")  # noqa: PTH118
         return path
 
     @property
     def user_documents_dir(self) -> str:
-        """
-        :return: documents directory tied to the user, e.g. ``~/Documents``
-        """
+        """:return: documents directory tied to the user, e.g. ``~/Documents``"""
         return _get_user_media_dir("XDG_DOCUMENTS_DIR", "~/Documents")
 
     @property
     def user_pictures_dir(self) -> str:
-        """
-        :return: pictures directory tied to the user, e.g. ``~/Pictures``
-        """
+        """:return: pictures directory tied to the user, e.g. ``~/Pictures``"""
         return _get_user_media_dir("XDG_PICTURES_DIR", "~/Pictures")
 
     @property
     def user_videos_dir(self) -> str:
-        """
-        :return: videos directory tied to the user, e.g. ``~/Videos``
-        """
+        """:return: videos directory tied to the user, e.g. ``~/Videos``"""
         return _get_user_media_dir("XDG_VIDEOS_DIR", "~/Videos")
 
     @property
     def user_music_dir(self) -> str:
-        """
-        :return: music directory tied to the user, e.g. ``~/Music``
-        """
+        """:return: music directory tied to the user, e.g. ``~/Music``"""
         return _get_user_media_dir("XDG_MUSIC_DIR", "~/Music")
 
     @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g. ``/run/user/$(id -u)/$appname/$version`` or
          ``$XDG_RUNTIME_DIR/$appname/$version``
@@ -185,35 +175,35 @@
 
 
 def _get_user_media_dir(env_var: str, fallback_tilde_path: str) -> str:
     media_dir = _get_user_dirs_folder(env_var)
     if media_dir is None:
         media_dir = os.environ.get(env_var, "").strip()
         if not media_dir:
-            media_dir = os.path.expanduser(fallback_tilde_path)
+            media_dir = os.path.expanduser(fallback_tilde_path)  # noqa: PTH111
 
     return media_dir
 
 
 def _get_user_dirs_folder(key: str) -> str | None:
-    """Return directory from user-dirs.dirs config file. See https://freedesktop.org/wiki/Software/xdg-user-dirs/"""
-    user_dirs_config_path = os.path.join(Unix().user_config_dir, "user-dirs.dirs")
-    if os.path.exists(user_dirs_config_path):
+    """Return directory from user-dirs.dirs config file. See https://freedesktop.org/wiki/Software/xdg-user-dirs/."""
+    user_dirs_config_path = Path(Unix().user_config_dir) / "user-dirs.dirs"
+    if user_dirs_config_path.exists():
         parser = ConfigParser()
 
-        with open(user_dirs_config_path) as stream:
+        with user_dirs_config_path.open() as stream:
             # Add fake section header, so ConfigParser doesn't complain
             parser.read_string(f"[top]\n{stream.read()}")
 
         if key not in parser["top"]:
             return None
 
         path = parser["top"][key].strip('"')
         # Handle relative home paths
-        path = path.replace("$HOME", os.path.expanduser("~"))
+        path = path.replace("$HOME", os.path.expanduser("~"))  # noqa: PTH111
         return path
 
     return None
 
 
 __all__ = [
     "Unix",
```

### Comparing `platformdirs-3.5.1/src/platformdirs/windows.py` & `platformdirs-3.5.2/src/platformdirs/windows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+"""Windows."""
 from __future__ import annotations
 
 import ctypes
 import os
 import sys
 from functools import lru_cache
-from typing import Callable
+from typing import TYPE_CHECKING
 
 from .api import PlatformDirsABC
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
 
 class Windows(PlatformDirsABC):
-    """`MSDN on where to store app data files
+    """
+    `MSDN on where to store app data files
     <http://support.microsoft.com/default.aspx?scid=kb;en-us;310294#XSLTH3194121123120121120120>`_.
     Makes use of the
     `appname <platformdirs.api.PlatformDirsABC.appname>`,
     `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`,
     `version <platformdirs.api.PlatformDirsABC.version>`,
     `roaming <platformdirs.api.PlatformDirsABC.roaming>`,
     `opinion <platformdirs.api.PlatformDirsABC.opinion>`,
@@ -39,15 +44,15 @@
                 author = self.appauthor or self.appname
                 params.append(author)
             params.append(self.appname)
             if opinion_value is not None and self.opinion:
                 params.append(opinion_value)
             if self.version:
                 params.append(self.version)
-        path = os.path.join(path, *params)
+        path = os.path.join(path, *params)  # noqa: PTH118
         self._optionally_create_directory(path)
         return path
 
     @property
     def site_data_dir(self) -> str:
         """:return: data directory shared by users, e.g. ``C:\\ProgramData\\$appauthor\\$appname``"""
         path = os.path.normpath(get_win_folder("CSIDL_COMMON_APPDATA"))
@@ -81,58 +86,48 @@
     @property
     def user_state_dir(self) -> str:
         """:return: state directory tied to the user, same as `user_data_dir`"""
         return self.user_data_dir
 
     @property
     def user_log_dir(self) -> str:
-        """
-        :return: log directory tied to the user, same as `user_data_dir` if not opinionated else ``Logs`` in it
-        """
+        """:return: log directory tied to the user, same as `user_data_dir` if not opinionated else ``Logs`` in it"""
         path = self.user_data_dir
         if self.opinion:
-            path = os.path.join(path, "Logs")
+            path = os.path.join(path, "Logs")  # noqa: PTH118
             self._optionally_create_directory(path)
         return path
 
     @property
     def user_documents_dir(self) -> str:
-        """
-        :return: documents directory tied to the user e.g. ``%USERPROFILE%\\Documents``
-        """
+        """:return: documents directory tied to the user e.g. ``%USERPROFILE%\\Documents``"""
         return os.path.normpath(get_win_folder("CSIDL_PERSONAL"))
 
     @property
     def user_pictures_dir(self) -> str:
-        """
-        :return: pictures directory tied to the user e.g. ``%USERPROFILE%\\Pictures``
-        """
+        """:return: pictures directory tied to the user e.g. ``%USERPROFILE%\\Pictures``"""
         return os.path.normpath(get_win_folder("CSIDL_MYPICTURES"))
 
     @property
     def user_videos_dir(self) -> str:
-        """
-        :return: videos directory tied to the user e.g. ``%USERPROFILE%\\Videos``
-        """
+        """:return: videos directory tied to the user e.g. ``%USERPROFILE%\\Videos``"""
         return os.path.normpath(get_win_folder("CSIDL_MYVIDEO"))
 
     @property
     def user_music_dir(self) -> str:
-        """
-        :return: music directory tied to the user e.g. ``%USERPROFILE%\\Music``
-        """
+        """:return: music directory tied to the user e.g. ``%USERPROFILE%\\Music``"""
         return os.path.normpath(get_win_folder("CSIDL_MYMUSIC"))
 
     @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g.
          ``%USERPROFILE%\\AppData\\Local\\Temp\\$appauthor\\$appname``
         """
-        path = os.path.normpath(os.path.join(get_win_folder("CSIDL_LOCAL_APPDATA"), "Temp"))
+        path = os.path.normpath(os.path.join(get_win_folder("CSIDL_LOCAL_APPDATA"), "Temp"))  # noqa: PTH118
         return self._append_parts(path)
 
 
 def get_win_folder_from_env_vars(csidl_name: str) -> str:
     """Get folder from environment variables."""
     result = get_win_folder_if_csidl_name_not_env_var(csidl_name)
     if result is not None:
@@ -140,55 +135,58 @@
 
     env_var_name = {
         "CSIDL_APPDATA": "APPDATA",
         "CSIDL_COMMON_APPDATA": "ALLUSERSPROFILE",
         "CSIDL_LOCAL_APPDATA": "LOCALAPPDATA",
     }.get(csidl_name)
     if env_var_name is None:
-        raise ValueError(f"Unknown CSIDL name: {csidl_name}")
+        msg = f"Unknown CSIDL name: {csidl_name}"
+        raise ValueError(msg)
     result = os.environ.get(env_var_name)
     if result is None:
-        raise ValueError(f"Unset environment variable: {env_var_name}")
+        msg = f"Unset environment variable: {env_var_name}"
+        raise ValueError(msg)
     return result
 
 
 def get_win_folder_if_csidl_name_not_env_var(csidl_name: str) -> str | None:
     """Get folder for a CSIDL name that does not exist as an environment variable."""
     if csidl_name == "CSIDL_PERSONAL":
-        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")  # noqa: PTH118
 
     if csidl_name == "CSIDL_MYPICTURES":
-        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Pictures")
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Pictures")  # noqa: PTH118
 
     if csidl_name == "CSIDL_MYVIDEO":
-        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Videos")
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Videos")  # noqa: PTH118
 
     if csidl_name == "CSIDL_MYMUSIC":
-        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Music")
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Music")  # noqa: PTH118
     return None
 
 
 def get_win_folder_from_registry(csidl_name: str) -> str:
-    """Get folder from the registry.
+    """
+    Get folder from the registry.
 
-    This is a fallback technique at best. I'm not sure if using the
-    registry for this guarantees us the correct answer for all CSIDL_*
-    names.
+    This is a fallback technique at best. I'm not sure if using the registry for these guarantees us the correct answer
+    for all CSIDL_* names.
     """
     shell_folder_name = {
         "CSIDL_APPDATA": "AppData",
         "CSIDL_COMMON_APPDATA": "Common AppData",
         "CSIDL_LOCAL_APPDATA": "Local AppData",
         "CSIDL_PERSONAL": "Personal",
         "CSIDL_MYPICTURES": "My Pictures",
         "CSIDL_MYVIDEO": "My Video",
         "CSIDL_MYMUSIC": "My Music",
     }.get(csidl_name)
     if shell_folder_name is None:
-        raise ValueError(f"Unknown CSIDL name: {csidl_name}")
+        msg = f"Unknown CSIDL name: {csidl_name}"
+        raise ValueError(msg)
     if sys.platform != "win32":  # only needed for mypy type checker to know that this code runs only on Windows
         raise NotImplementedError
     import winreg
 
     key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders")
     directory, _ = winreg.QueryValueEx(key, shell_folder_name)
     return str(directory)
@@ -202,22 +200,23 @@
         "CSIDL_LOCAL_APPDATA": 28,
         "CSIDL_PERSONAL": 5,
         "CSIDL_MYPICTURES": 39,
         "CSIDL_MYVIDEO": 14,
         "CSIDL_MYMUSIC": 13,
     }.get(csidl_name)
     if csidl_const is None:
-        raise ValueError(f"Unknown CSIDL name: {csidl_name}")
+        msg = f"Unknown CSIDL name: {csidl_name}"
+        raise ValueError(msg)
 
     buf = ctypes.create_unicode_buffer(1024)
     windll = getattr(ctypes, "windll")  # noqa: B009 # using getattr to avoid false positive with mypy type checker
     windll.shell32.SHGetFolderPathW(None, csidl_const, None, 0, buf)
 
     # Downgrade to short path name if it has highbit chars.
-    if any(ord(c) > 255 for c in buf):
+    if any(ord(c) > 255 for c in buf):  # noqa: PLR2004
         buf2 = ctypes.create_unicode_buffer(1024)
         if windll.kernel32.GetShortPathNameW(buf.value, buf2, 1024):
             buf = buf2
 
     return buf.value
```

### Comparing `platformdirs-3.5.1/tests/conftest.py` & `platformdirs-3.5.2/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
-from typing import cast
+from typing import TYPE_CHECKING, cast
 
 import pytest
-from _pytest.fixtures import SubRequest
+
+if TYPE_CHECKING:
+    from _pytest.fixtures import SubRequest
 
 PROPS = (
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
```

### Comparing `platformdirs-3.5.1/tests/test_android.py` & `platformdirs-3.5.2/tests/test_android.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import sys
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from unittest.mock import MagicMock
 
 import pytest
-from _pytest.monkeypatch import MonkeyPatch
-from pytest_mock import MockerFixture
 
 from platformdirs.android import Android
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
 
 @pytest.mark.parametrize(
     "params",
     [
         {},
         {"appname": "foo"},
         {"appname": "foo", "appauthor": "bar"},
@@ -38,28 +39,29 @@
         suffix_elements.append(params["appname"])
     if "version" in params:
         suffix_elements.append(params["version"])
     if suffix_elements:
         suffix_elements.insert(0, "")
     suffix = "/".join(suffix_elements)
 
+    val = "/tmp"  # noqa: S108
     expected_map = {
         "user_data_dir": f"/data/data/com.example/files{suffix}",
         "site_data_dir": f"/data/data/com.example/files{suffix}",
         "user_config_dir": f"/data/data/com.example/shared_prefs{suffix}",
         "site_config_dir": f"/data/data/com.example/shared_prefs{suffix}",
         "user_cache_dir": f"/data/data/com.example/cache{suffix}",
         "site_cache_dir": f"/data/data/com.example/cache{suffix}",
         "user_state_dir": f"/data/data/com.example/files{suffix}",
         "user_log_dir": f"/data/data/com.example/cache{suffix}{'' if params.get('opinion', True) is False else '/log'}",
         "user_documents_dir": "/storage/emulated/0/Documents",
         "user_pictures_dir": "/storage/emulated/0/Pictures",
         "user_videos_dir": "/storage/emulated/0/DCIM/Camera",
         "user_music_dir": "/storage/emulated/0/Music",
-        "user_runtime_dir": f"/data/data/com.example/cache{suffix}{'' if not params.get('opinion', True) else '/tmp'}",
+        "user_runtime_dir": f"/data/data/com.example/cache{suffix}{'' if not params.get('opinion', True) else val}",
     }
     expected = expected_map[func]
 
     assert result == expected
 
 
 def test_android_folder_from_jnius(mocker: MockerFixture) -> None:
@@ -91,27 +93,27 @@
 @pytest.mark.parametrize(
     "path",
     [
         "/data/user/1/a/files",
         "/data/data/a/files",
     ],
 )
-def test_android_folder_from_sys_path(mocker: MockerFixture, path: str, monkeypatch: MonkeyPatch) -> None:
+def test_android_folder_from_sys_path(mocker: MockerFixture, path: str, monkeypatch: pytest.MonkeyPatch) -> None:
     mocker.patch.dict(sys.modules, {"jnius": MagicMock(autoclass=MagicMock(side_effect=ModuleNotFoundError))})
 
     from platformdirs.android import _android_folder
 
     _android_folder.cache_clear()
     monkeypatch.setattr(sys, "path", ["/A", "/B", path])
 
     result = _android_folder()
     assert result == path[: -len("/files")]
 
 
-def test_android_folder_not_found(mocker: MockerFixture, monkeypatch: MonkeyPatch) -> None:
+def test_android_folder_not_found(mocker: MockerFixture, monkeypatch: pytest.MonkeyPatch) -> None:
     mocker.patch.dict(sys.modules, {"jnius": MagicMock(autoclass=MagicMock(side_effect=ModuleNotFoundError))})
 
     from platformdirs.android import _android_folder
 
     _android_folder.cache_clear()
     monkeypatch.setattr(sys, "path", [])
     assert _android_folder() is None
```

### Comparing `platformdirs-3.5.1/tests/test_api.py` & `platformdirs-3.5.2/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import inspect
 import sys
 from pathlib import Path
 
 import pytest
-from _pytest.monkeypatch import MonkeyPatch
 
 import platformdirs
 from platformdirs.android import Android
 
 
 def test_package_metadata() -> None:
     assert hasattr(platformdirs, "__version__")
@@ -51,16 +50,16 @@
 
 
 @pytest.mark.parametrize("root", ["A", "/system", None])
 @pytest.mark.parametrize("data", ["D", "/data", None])
 @pytest.mark.parametrize("path", ["/data/data/a/files", "/C"])
 @pytest.mark.parametrize("shell", ["/data/data/com.app/files/usr/bin/sh", "/usr/bin/sh", None])
 @pytest.mark.parametrize("prefix", ["/data/data/com.termux/files/usr", None])
-def test_android_active(
-    monkeypatch: MonkeyPatch,
+def test_android_active(  # noqa: PLR0913
+    monkeypatch: pytest.MonkeyPatch,
     root: str | None,
     data: str | None,
     path: str,
     shell: str | None,
     prefix: str | None,
 ) -> None:
     for env_var, value in {"ANDROID_DATA": data, "ANDROID_ROOT": root, "SHELL": shell, "PREFIX": prefix}.items():
@@ -74,10 +73,10 @@
     _android_folder.cache_clear()
     monkeypatch.setattr(sys, "path", ["/A", "/B", path])
 
     expected = (
         root == "/system" and data == "/data" and shell is None and prefix is None and _android_folder() is not None
     )
     if expected:
-        assert platformdirs._set_platform_dir_class() is Android
+        assert platformdirs._set_platform_dir_class() is Android  # noqa: SLF001
     else:
-        assert platformdirs._set_platform_dir_class() is not Android
+        assert platformdirs._set_platform_dir_class() is not Android  # noqa: SLF001
```

### Comparing `platformdirs-3.5.1/tests/test_comp_with_appdirs.py` & `platformdirs-3.5.2/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.1/tests/test_macos.py` & `platformdirs-3.5.2/tests/test_macos.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
         pytest.param({"appname": "foo"}, id="app_name"),
         pytest.param({"appname": "foo", "version": "v1.0"}, id="app_name_version"),
     ],
 )
 def test_macos(params: dict[str, Any], func: str) -> None:
     result = getattr(MacOS(**params), func)
 
-    home = os.path.expanduser("~")
+    home = os.path.expanduser("~")  # noqa: PTH111
     suffix_elements = tuple(params[i] for i in ("appname", "version") if i in params)
-    suffix = os.sep.join(("",) + suffix_elements) if suffix_elements else ""
+    suffix = os.sep.join(("", *suffix_elements)) if suffix_elements else ""
 
     expected_map = {
         "user_data_dir": f"{home}/Library/Application Support{suffix}",
         "site_data_dir": f"/Library/Application Support{suffix}",
         "user_config_dir": f"{home}/Library/Application Support{suffix}",
         "site_config_dir": f"/Library/Application Support{suffix}",
         "user_cache_dir": f"{home}/Library/Caches{suffix}",
```

### Comparing `platformdirs-3.5.1/tests/test_unix.py` & `platformdirs-3.5.2/tests/test_unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import importlib
 import os
 import sys
 import typing
-from pathlib import Path
 
 import pytest
-from _pytest.monkeypatch import MonkeyPatch
-from pytest_mock import MockerFixture
 
 from platformdirs import unix
 from platformdirs.unix import Unix
 
+if typing.TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
 
 @pytest.mark.parametrize("prop", ["user_documents_dir", "user_pictures_dir", "user_videos_dir", "user_music_dir"])
 def test_user_media_dir(mocker: MockerFixture, prop: str) -> None:
     example_path = "/home/example/ExampleMediaFolder"
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = example_path
     assert getattr(Unix(), prop) == example_path
@@ -93,54 +95,54 @@
 
 @pytest.fixture()
 def _getuid(mocker: MockerFixture) -> None:
     mocker.patch("platformdirs.unix.getuid", return_value=1234)
 
 
 @pytest.mark.usefixtures("_getuid")
-def test_xdg_variable_not_set(monkeypatch: MonkeyPatch, dirs_instance: Unix, func: str) -> None:
+def test_xdg_variable_not_set(monkeypatch: pytest.MonkeyPatch, dirs_instance: Unix, func: str) -> None:
     xdg_variable = _func_to_path(func)
     if xdg_variable is None:
         return
 
     monkeypatch.delenv(xdg_variable.name, raising=False)
     result = getattr(dirs_instance, func)
-    assert result == os.path.expanduser(xdg_variable.default_value)
+    assert result == os.path.expanduser(xdg_variable.default_value)  # noqa: PTH111
 
 
 @pytest.mark.usefixtures("_getuid")
-def test_xdg_variable_empty_value(monkeypatch: MonkeyPatch, dirs_instance: Unix, func: str) -> None:
+def test_xdg_variable_empty_value(monkeypatch: pytest.MonkeyPatch, dirs_instance: Unix, func: str) -> None:
     xdg_variable = _func_to_path(func)
     if xdg_variable is None:
         return
 
     monkeypatch.setenv(xdg_variable.name, "")
     result = getattr(dirs_instance, func)
-    assert result == os.path.expanduser(xdg_variable.default_value)
+    assert result == os.path.expanduser(xdg_variable.default_value)  # noqa: PTH111
 
 
 @pytest.mark.usefixtures("_getuid")
-def test_xdg_variable_custom_value(monkeypatch: MonkeyPatch, dirs_instance: Unix, func: str) -> None:
+def test_xdg_variable_custom_value(monkeypatch: pytest.MonkeyPatch, dirs_instance: Unix, func: str) -> None:
     xdg_variable = _func_to_path(func)
     if xdg_variable is None:
         return
 
-    monkeypatch.setenv(xdg_variable.name, "/tmp/custom-dir")
+    monkeypatch.setenv(xdg_variable.name, "/custom-dir")
     result = getattr(dirs_instance, func)
-    assert result == "/tmp/custom-dir"
+    assert result == "/custom-dir"
 
 
-def test_platform_on_win32(monkeypatch: MonkeyPatch, mocker: MockerFixture) -> None:
+def test_platform_on_win32(monkeypatch: pytest.MonkeyPatch, mocker: MockerFixture) -> None:
     monkeypatch.delenv("XDG_RUNTIME_DIR", raising=False)
     mocker.patch("sys.platform", "win32")
     prev_unix = unix
     importlib.reload(unix)
     try:
         with pytest.raises(RuntimeError, match="should only be used on Unix"):
-            unix.Unix().user_runtime_dir
+            unix.Unix().user_runtime_dir  # noqa: B018
     finally:
         sys.modules["platformdirs.unix"] = prev_unix
 
 
 def test_ensure_exists_creates_folder(mocker: MockerFixture, tmp_path: Path) -> None:
     mocker.patch.dict(os.environ, {"XDG_DATA_HOME": str(tmp_path)})
     data_path = Unix(appname="acme", ensure_exists=True).user_data_path
```

### Comparing `platformdirs-3.5.1/LICENSE` & `platformdirs-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.1/README.rst` & `platformdirs-3.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.1/PKG-INFO` & `platformdirs-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.5.1
+Version: 3.5.2
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
@@ -17,29 +17,28 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: typing-extensions>=4.5; python_version < '3.8'
+Requires-Dist: typing-extensions>=4.6.3; python_version < '3.8'
 Provides-Extra: docs
-Requires-Dist: furo>=2023.3.27; extra == 'docs'
+Requires-Dist: furo>=2023.5.20; extra == 'docs'
 Requires-Dist: proselint>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
-Requires-Dist: sphinx>=6.2.1; extra == 'docs'
+Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: appdirs==1.4.4; extra == 'test'
 Requires-Dist: covdefaults>=2.3; extra == 'test'
-Requires-Dist: pytest-cov>=4; extra == 'test'
+Requires-Dist: pytest-cov>=4.1; extra == 'test'
 Requires-Dist: pytest-mock>=3.10; extra == 'test'
 Requires-Dist: pytest>=7.3.1; extra == 'test'
 Description-Content-Type: text/x-rst
 
 The problem
 ===========
```

