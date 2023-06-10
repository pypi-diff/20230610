# Comparing `tmp/gpru-0.0.2.tar.gz` & `tmp/gpru-0.0.3.tar.gz`

## Comparing `gpru-0.0.2.tar` & `gpru-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/_client.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/__init__.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/_api.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/_utils.py
--rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/preview_2022_03_01.py
--rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/preview_2022_06_01.py
--rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/preview_2023_03_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/py.typed
--rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/stable_2022_12_01.py
--rw-r--r--   0        0        0    49072 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/stable_2023_05_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/openai/__init__.py
--rw-r--r--   0        0        0    55082 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/openai/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/openai/py.typed
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.0.2/LICENSE
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 gpru-0.0.2/README.md
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 gpru-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 gpru-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/__about__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/__init__.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/_client.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/_logger.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/__init__.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/_api.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/_utils.py
+-rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/preview_2022_03_01.py
+-rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/preview_2022_06_01.py
+-rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/preview_2023_03_15.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/py.typed
+-rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/stable_2022_12_01.py
+-rw-r--r--   0        0        0    49072 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/stable_2023_05_15.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/openai/__init__.py
+-rw-r--r--   0        0        0    55082 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/openai/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/openai/py.typed
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 gpru-0.0.3/README.md
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 gpru-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 gpru-0.0.3/PKG-INFO
```

### Comparing `gpru-0.0.2/gpru/_client.py` & `gpru-0.0.3/gpru/_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,73 @@
+import logging
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Dict, Generator, Type, TypeVar
 
 import httpx
-from httpx._exceptions import HTTPError, StreamError
+from httpx._exceptions import HTTPError, ReadTimeout, StreamError
 from pydantic import BaseModel
 from pydantic.error_wrappers import ValidationError
+from tenacity import (
+    before_log,
+    retry,
+    retry_if_exception,
+    stop_after_attempt,
+    wait_random_exponential,
+)
 
+from gpru.__about__ import __version__
+from gpru._logger import logger
 from gpru.exceptions import ApiError, IncorrectImplementationError
 
 T = TypeVar("T", bound=BaseModel)
 
+_API_FAILED = "API request failed."
+_IMPLEMENTATION_ERROR = f"Implementation error in gpru@{__version__}."
+
 
 def _raise_api_error(error_response_model: Type[T], response: httpx.Response) -> None:
+    logger.error(_API_FAILED)
     error_response = error_response_model.parse_obj(response.json())
     error = error_response.error if hasattr(error_response, "error") else error_response
     raise ApiError(response.status_code, error)
 
 
+def _retry_condition(e: BaseException) -> bool:
+    if type(e) == ApiError:
+        return isinstance(e.error, ReadTimeout)
+
+    return False
+
+
 def request_factory(
     error_response_model: Type[T], **client_kwargs: Any
 ) -> Callable[..., httpx.Response]:
+    @retry(  # type: ignore[misc]
+        stop=stop_after_attempt(6),
+        wait=wait_random_exponential(min=1, max=20),
+        retry=retry_if_exception(_retry_condition),
+        before=before_log(logger, logging.DEBUG),
+        reraise=True,
+    )
     def request(method: str, path: str, **kwargs: Any) -> httpx.Response:
         try:
             with httpx.Client(**client_kwargs) as client:
                 response = client.request(method, path, **kwargs)
                 if not response.is_success:
                     _raise_api_error(error_response_model, response)
                 return response
         except HTTPError as e:
+            logger.exception(_API_FAILED)
             raise ApiError(None, e) from e
         except ValidationError as e:
+            logger.exception(_IMPLEMENTATION_ERROR)
             raise IncorrectImplementationError from e
 
-    return request
+    return request  # type: ignore[no-any-return]
 
 
 def _generate_chunk_models(
     response: httpx.Response, response_model: Type[T]
 ) -> Generator[T, None, None]:
     for chunk in response.iter_raw():
         for line in chunk.splitlines():
@@ -63,16 +93,18 @@
         try:
             with httpx.Client(**client_kwargs) as client:  # noqa: SIM117
                 with client.stream(method, path, **kwargs) as response:
                     if not response.is_success:
                         _raise_api_error(error_response_model, response)
                     yield from _generate_chunk_models(response, response_model)
         except (HTTPError, StreamError) as e:
+            logger.exception(_API_FAILED)
             raise ApiError(None, e) from e
         except ValidationError as e:
+            logger.exception(_IMPLEMENTATION_ERROR)
             raise IncorrectImplementationError from e
 
     return stream
 
 
 def kwargs_for_uploading(request_model: T) -> Dict[str, Any]:
     data: Dict[str, Any] = {}
```

### Comparing `gpru-0.0.2/gpru/exceptions.py` & `gpru-0.0.3/gpru/exceptions.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/gpru/azure/_api.py` & `gpru-0.0.3/gpru/azure/_api.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/gpru/azure/preview_2022_03_01.py` & `gpru-0.0.3/gpru/azure/preview_2022_03_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/gpru/azure/preview_2022_06_01.py` & `gpru-0.0.3/gpru/azure/preview_2022_06_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/gpru/azure/preview_2023_03_15.py` & `gpru-0.0.3/gpru/azure/preview_2023_03_15.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/gpru/azure/stable_2022_12_01.py` & `gpru-0.0.3/gpru/azure/stable_2022_12_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/gpru/azure/stable_2023_05_15.py` & `gpru-0.0.3/gpru/azure/stable_2023_05_15.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/gpru/openai/api.py` & `gpru-0.0.3/gpru/openai/api.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/.gitignore` & `gpru-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/LICENSE` & `gpru-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/README.md` & `gpru-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpru-0.0.2/pyproject.toml` & `gpru-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,17 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Communications :: Chat",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
-  "httpx[http2]>=0.24.0",
-  "pydantic>=1.10.7",
+  "httpx[http2]>=0.24.1",
+  "pydantic>=1.10.9",
+  "tenacity>=8.2.2",
 ]
 description = "Unofficial Python client library for the OpenAI and Azure OpenAI APIs"
 dynamic = ["version"]
 keywords = ["openai", "azure", "chatgpt", "gpt", "gpt-3", "gpt-4", "asyncio", "pydantic"]
 license = "MIT"
 name = "gpru"
 readme = "README.md"
@@ -45,15 +46,15 @@
 [tool.hatch.build.targets.sdist]
 packages = ["src/gpru"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/gpru"]
 
 [tool.hatch.version]
-path = "src/gpru/__init__.py"
+path = "src/gpru/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]",
   "datamodel-code-generator[http]<0.18", # https://docs.pydantic.dev/latest/datamodel_code_generator/
   "pre-commit",
   "pytest",
@@ -65,16 +66,14 @@
   "cov-report",
 ]
 cov-report = [
   "- coverage combine",
   "coverage report --show-missing",
 ]
 gen-model = "datamodel-codegen --openapi-scopes=schemas --snake-case-field --use-schema-description --use-field-description --reuse-model --capitalise-enum-members --use-subclass-enum --target-python-version=3.7 --wrap-string-literal --output=models.py {args:}"
-pc-run = "pre-commit run --all-files"
-pc-update = "pre-commit autoupdate"
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 
 [[tool.hatch.envs.all.matrix]]
 # If you are using pyenv, just run `pyenv global 3.7 3.8 3.9 3.10 3.11` beforehand.
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
@@ -102,27 +101,27 @@
 detached = true
 python = "3.11"
 
 [tool.hatch.envs.lint.scripts]
 check = [
   "black --check --diff {args:.}",
   "isort --check {args:.}",
-  "docformatter {args:--check .}",
+  "docformatter --check {args:.}",
   "ruff {args:.}",
   "typing",
 ]
 format = [
   "black {args:.}",
   "isort {args:.}",
-  "docformatter {args:--in-place .}",
+  "docformatter --in-place {args:.}",
   "ruff --fix {args:.}",
   "typing",
 ]
 typing = [
-  "mypy --install-types --non-interactive {args:examples src tests}",
+  "mypy {args:examples src tests}",
 ]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 source_pkgs = ["gpru"]
 
@@ -157,20 +156,22 @@
 [tool.isort]
 include_trailing_comma = true
 line_length = 88
 multi_line_output = 3
 profile = "black"
 
 [tool.mypy]
+install_types = true
+non_interactive = true
 plugins = ["pydantic.mypy"] # https://docs.pydantic.dev/latest/mypy_plugin/#enabling-the-plugin
 strict = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
-module = "httpx.*"
+module = ["httpx.*", "tenacity.*"]
 
 [tool.ruff]
 ignore = [
   "D10", # TODO: write docstrings and remove this line
   "D200",
   "D205",
   "ANN",
```

### Comparing `gpru-0.0.2/PKG-INFO` & `gpru-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpru
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Python client library for the OpenAI and Azure OpenAI APIs
 Project-URL: Documentation, https://github.com/sincekmori/gpru#readme
 Project-URL: Issues, https://github.com/sincekmori/gpru/issues
 Project-URL: Source, https://github.com/sincekmori/gpru
 Author-email: Shinsuke Mori <sincekmori@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -23,16 +23,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
-Requires-Dist: httpx[http2]>=0.24.0
-Requires-Dist: pydantic>=1.10.7
+Requires-Dist: httpx[http2]>=0.24.1
+Requires-Dist: pydantic>=1.10.9
+Requires-Dist: tenacity>=8.2.2
 Description-Content-Type: text/markdown
 
 # GPRU: Unofficial Python Client Library for the OpenAI and Azure OpenAI APIs
 
 **PyPI**
 [![PyPI - Version](https://img.shields.io/pypi/v/gpru.svg)](https://pypi.org/project/gpru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gpru.svg)](https://pypi.org/project/gpru)
```

