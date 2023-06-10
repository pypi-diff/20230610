# Comparing `tmp/xcover-python-0.1.0.tar.gz` & `tmp/xcover_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcover-python-0.1.0.tar", max compression
+gzip compressed data, was "xcover_python-0.1.1.tar", max compression
```

## Comparing `xcover-python-0.1.0.tar` & `xcover_python-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     2912 2021-11-26 13:11:25.627695 xcover-python-0.1.0/README.md
--rw-r--r--   0        0        0     1108 2021-11-26 13:11:25.627695 xcover-python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       41 2021-11-26 13:11:25.631695 xcover-python-0.1.0/xcover/__init__.py
--rw-r--r--   0        0        0     1151 2021-11-26 13:11:25.631695 xcover-python-0.1.0/xcover/auth.py
--rw-r--r--   0        0        0     2320 2021-11-26 13:11:25.631695 xcover-python-0.1.0/xcover/config.py
--rw-r--r--   0        0        0      850 2021-11-26 13:11:25.631695 xcover-python-0.1.0/xcover/encoder.py
--rw-r--r--   0        0        0      154 2021-11-26 13:11:25.631695 xcover-python-0.1.0/xcover/exceptions.py
--rw-r--r--   0        0        0      200 2021-11-26 13:11:25.631695 xcover-python-0.1.0/xcover/utils.py
--rw-r--r--   0        0        0     7122 2021-11-26 13:11:25.631695 xcover-python-0.1.0/xcover/xcover.py
--rw-r--r--   0        0        0     3711 2021-11-26 13:11:35.814769 xcover-python-0.1.0/setup.py
--rw-r--r--   0        0        0     3726 2021-11-26 13:11:35.815156 xcover-python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3530 2023-06-10 14:40:53.011071 xcover_python-0.1.1/README.md
+-rw-r--r--   0        0        0     1126 2023-06-10 14:40:53.011071 xcover_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-06-10 14:40:53.015071 xcover_python-0.1.1/xcover/__init__.py
+-rw-r--r--   0        0        0     1151 2023-06-10 14:40:53.015071 xcover_python-0.1.1/xcover/auth.py
+-rw-r--r--   0        0        0     2444 2023-06-10 14:40:53.015071 xcover_python-0.1.1/xcover/config.py
+-rw-r--r--   0        0        0      850 2023-06-10 14:40:53.015071 xcover_python-0.1.1/xcover/encoder.py
+-rw-r--r--   0        0        0      154 2023-06-10 14:40:53.015071 xcover_python-0.1.1/xcover/exceptions.py
+-rw-r--r--   0        0        0      200 2023-06-10 14:40:53.015071 xcover_python-0.1.1/xcover/utils.py
+-rw-r--r--   0        0        0     8973 2023-06-10 14:40:53.015071 xcover_python-0.1.1/xcover/xcover.py
+-rw-r--r--   0        0        0     4345 1970-01-01 00:00:00.000000 xcover_python-0.1.1/PKG-INFO
```

### Comparing `xcover-python-0.1.0/README.md` & `xcover_python-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 ---
 
 ## Installation
 
 `xcover-python` is available on PyPI. To install the latest version run:
 
-    pip install xcover
+    pip install xcover-python
 
 or
 
-    poertry install xcover
+    poertry install xcover-python
 
 ## Features
 
 - Authentication
 - Simple configuration using env variables
 - (WIP) High-level API to perform partner operations on quotes and bookings
 
@@ -53,14 +53,16 @@
 * `XC_BASE_URL` (`XCoverConfig.base_url`): XCover base URL (e.g. `https://api.xcover.com/api/v2/`).
 * `XC_PARTNER_CODE` (`XCoverConfig.partner_code`): Partner code (e.g. `LLODT`).
 * `XC_HTTP_TIMEOUT` (`XCoverConfig.http_timeout`): HTTP timeout in seconds. Default value is `10`.
 * `XC_AUTH_API_KEY` (`XCoverConfig.auth_api_key`): API key to use.
 * `XC_AUTH_API_SECRET` (`XCoverConfig.auth_api_secret`): API secret to use.
 * `XC_AUTH_ALGORITHM` (`XCoverConfig.auth_algorithm`): HMAC encoding algorithm to use. Default is `hmac-sha512`.
 * `XC_AUTH_HEADERS` (`XCoverConfig.auth_headers`): Headers to sign. Default is `(request-target) date`.
+* `XC_RETRY_TOTAL` (`XCoverConfig.retry_total`): Total number of retries. Default is `5`.
+* `XC_RETRY_BACKOFF_FACTOR` (`XCoverConfig.retry_backoff_factor`): Backoff factor for retries timeout. Default is `2`.
 
 ## Usage example
 
 ### Using low-level `call` method
 
 ```python
 import requests
@@ -99,7 +101,16 @@
     url="partners/LLODT/quotes/",
     payload=payload,
 )
 
 quote = response.json()
 print(quote)
 ```
+
+### Retries
+
+This client will automatically retry certain operations when it is considered safe to do this.
+The retry number and intervals could be controlled via XC_RETRY_TOTAL and XC_RETRY_BACKOFF_FACTOR
+environment variables ot the same config options.
+
+Auto retry logic can be enabled/disabled per operation. However, further fine-tuning is possible
+via extending XCover class if required.
```

### Comparing `xcover-python-0.1.0/pyproject.toml` & `xcover_python-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "xcover-python"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python client for XCover API (XCore)."
 authors = ["Artem Kolesnikov <artem@covergenius.com>"]
 maintainers = ["Artem Kolesnikov <artem@covergenius.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.covergenius.com/xcover/"
 repository = "https://github.com/CoverGenius/xcover-python"
 keywords = ["xcover", "api", "api-client", "insurance"]
 packages = [
     { include = "xcover" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = "^2.26"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2"
-pre-commit = "^2.15"
-pytest-dotenv = "^0.5"
-pytest-recording = "^0.12"
-bump2version = "^1.0"
-factory-boy = "^3.2.0"
-pytest-cov = "^2.12.1"
-coverage = {extras = ["toml"], version = "^5.5"}
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+pre-commit = "^3.2.2"
+pytest-dotenv = "^0.5.2"
+pytest-recording = "^0.12.2"
+bump2version = "^1.0.1"
+factory-boy = "^3.2.1"
+pytest-cov = "^4.0.0"
+coverage = {version = "^7.2.3", extras = ["toml"]}
+
 
 [tool.black]
 line-length = 99
 
 [tool.coverage.html]
 directory = "build/coverage"
```

### Comparing `xcover-python-0.1.0/xcover/auth.py` & `xcover_python-0.1.1/xcover/auth.py`

 * *Files identical despite different names*

### Comparing `xcover-python-0.1.0/xcover/config.py` & `xcover_python-0.1.1/xcover/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,19 +52,21 @@
         return self.SUPPORTED_ALGORITHMS.get(self.algorithm)
 
 
 @dataclass
 class XCoverConfig:
     partner_code: str = env("XC_PARTNER_CODE")
     base_url: str = env("XC_BASE_URL")
-    http_timeout: Union[float, Tuple[float, float]] = float(env("XC_HTTP_TIMEOUT", 10))
+    http_timeout: Union[float, Tuple[float, float]] = float(env("XC_HTTP_TIMEOUT", 60))
     auth_api_key: str = env("XC_AUTH_API_KEY")
     auth_api_secret: str = env("XC_AUTH_API_SECRET")
     auth_algorithm: str = env("XC_AUTH_ALGORITHM")
     headers: str = env("XC_AUTH_HEADERS", "(request-target) date")
+    retry_total: int = int(env("XC_RETRY_TOTAL", 5))
+    retry_backoff_factor: int = int(env("XC_RETRY_BACKOFF_FACTOR", 2))
 
     @property
     def auth_config(self):
         algorithm = (
             SignatureAlgorithm(self.auth_algorithm)
             if self.auth_algorithm
             else SignatureAlgorithm.HMAC_SHA512
```

### Comparing `xcover-python-0.1.0/xcover/encoder.py` & `xcover_python-0.1.1/xcover/encoder.py`

 * *Files identical despite different names*

### Comparing `xcover-python-0.1.0/setup.py` & `xcover_python-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,139 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['xcover']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.26,<3.0']
-
-setup_kwargs = {
-    'name': 'xcover-python',
-    'version': '0.1.0',
-    'description': 'Python client for XCover API (XCore).',
-    'long_description': '# &middot; xcover-python &middot;\n[![Supported Versions](https://img.shields.io/pypi/pyversions/xcover-python.svg)](https://pypi.org/project/xcover-python)\n[![codecov](https://codecov.io/gh/CoverGenius/xcover-python/branch/master/graph/badge.svg?token=KINNTVZV07)](https://codecov.io/gh/CoverGenius/xcover-python)\n\n---\n\n`xcover-python` is a Python API Client for [XCover](https://www.covergenius.com/xcover/).\n\n---\n\n## Installation\n\n`xcover-python` is available on PyPI. To install the latest version run:\n\n    pip install xcover\n\nor\n\n    poertry install xcover\n\n## Features\n\n- Authentication\n- Simple configuration using env variables\n- (WIP) High-level API to perform partner operations on quotes and bookings\n\n## Configuration\n\n### Config object\n\nThe library provides `XCoverConfig` dataclass that can be used as shown:\n\n```python\nfrom xcover import XCover, XCoverConfig\n\nclient = XCover(\n    XCoverConfig( # minimal config, check autocomplete for more options\n        base_url="https://api.xcover.com/xcover",\n        partner_code="--PARTNER_CODE--",\n        auth_api_key="--API_KEY--",\n        auth_api_secret="--API_SECRET--",\n    )\n)\n\n```\n\n### Env variables\n\nAlternatively, it is possible to use env variables.\n\nThe full list of configuration options:\n\n* `XC_BASE_URL` (`XCoverConfig.base_url`): XCover base URL (e.g. `https://api.xcover.com/api/v2/`).\n* `XC_PARTNER_CODE` (`XCoverConfig.partner_code`): Partner code (e.g. `LLODT`).\n* `XC_HTTP_TIMEOUT` (`XCoverConfig.http_timeout`): HTTP timeout in seconds. Default value is `10`.\n* `XC_AUTH_API_KEY` (`XCoverConfig.auth_api_key`): API key to use.\n* `XC_AUTH_API_SECRET` (`XCoverConfig.auth_api_secret`): API secret to use.\n* `XC_AUTH_ALGORITHM` (`XCoverConfig.auth_algorithm`): HMAC encoding algorithm to use. Default is `hmac-sha512`.\n* `XC_AUTH_HEADERS` (`XCoverConfig.auth_headers`): Headers to sign. Default is `(request-target) date`.\n\n## Usage example\n\n### Using low-level `call` method\n\n```python\nimport requests\n\nfrom xcover.xcover import XCover\n\n# Env variables are used\nclient = XCover()\n\n# Prepare payload\npayload = {\n    "request": [\n        {\n            "policy_type": "event_ticket_protection",\n            "policy_type_version": 1,\n            "policy_start_date": "2021-12-01T17:59:00.831+00:00",\n            "event_datetime": "2021-12-25T21:00:00+00:00",\n            "event_name": "Ariana Grande",\n            "event_location": "The O2",\n            "number_of_tickets": 2,\n            "tickets": [\n                {"price": 100},\n            ],\n            "resale_ticket": False,\n            "event_country": "GB",\n        }\n    ],\n    "currency": "GBP",\n    "customer_country": "GB",\n    "customer_region": "London",\n    "customer_language": "en",\n}\n# Calling XCover API\nresponse: requests.Response = client.call(\n    method="POST",\n    url="partners/LLODT/quotes/",\n    payload=payload,\n)\n\nquote = response.json()\nprint(quote)\n```\n',
-    'author': 'Artem Kolesnikov',
-    'author_email': 'artem@covergenius.com',
-    'maintainer': 'Artem Kolesnikov',
-    'maintainer_email': 'artem@covergenius.com',
-    'url': 'https://www.covergenius.com/xcover/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+Metadata-Version: 2.1
+Name: xcover-python
+Version: 0.1.1
+Summary: Python client for XCover API (XCore).
+Home-page: https://www.covergenius.com/xcover/
+License: MIT
+Keywords: xcover,api,api-client,insurance
+Author: Artem Kolesnikov
+Author-email: artem@covergenius.com
+Maintainer: Artem Kolesnikov
+Maintainer-email: artem@covergenius.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.26,<3.0)
+Project-URL: Repository, https://github.com/CoverGenius/xcover-python
+Description-Content-Type: text/markdown
+
+# &middot; xcover-python &middot;
+[![Supported Versions](https://img.shields.io/pypi/pyversions/xcover-python.svg)](https://pypi.org/project/xcover-python)
+[![codecov](https://codecov.io/gh/CoverGenius/xcover-python/branch/master/graph/badge.svg?token=KINNTVZV07)](https://codecov.io/gh/CoverGenius/xcover-python)
+
+---
+
+`xcover-python` is a Python API Client for [XCover](https://www.covergenius.com/xcover/).
+
+---
+
+## Installation
+
+`xcover-python` is available on PyPI. To install the latest version run:
+
+    pip install xcover-python
+
+or
+
+    poertry install xcover-python
+
+## Features
+
+- Authentication
+- Simple configuration using env variables
+- (WIP) High-level API to perform partner operations on quotes and bookings
+
+## Configuration
+
+### Config object
+
+The library provides `XCoverConfig` dataclass that can be used as shown:
+
+```python
+from xcover import XCover, XCoverConfig
+
+client = XCover(
+    XCoverConfig( # minimal config, check autocomplete for more options
+        base_url="https://api.xcover.com/xcover",
+        partner_code="--PARTNER_CODE--",
+        auth_api_key="--API_KEY--",
+        auth_api_secret="--API_SECRET--",
+    )
+)
+
+```
+
+### Env variables
+
+Alternatively, it is possible to use env variables.
+
+The full list of configuration options:
+
+* `XC_BASE_URL` (`XCoverConfig.base_url`): XCover base URL (e.g. `https://api.xcover.com/api/v2/`).
+* `XC_PARTNER_CODE` (`XCoverConfig.partner_code`): Partner code (e.g. `LLODT`).
+* `XC_HTTP_TIMEOUT` (`XCoverConfig.http_timeout`): HTTP timeout in seconds. Default value is `10`.
+* `XC_AUTH_API_KEY` (`XCoverConfig.auth_api_key`): API key to use.
+* `XC_AUTH_API_SECRET` (`XCoverConfig.auth_api_secret`): API secret to use.
+* `XC_AUTH_ALGORITHM` (`XCoverConfig.auth_algorithm`): HMAC encoding algorithm to use. Default is `hmac-sha512`.
+* `XC_AUTH_HEADERS` (`XCoverConfig.auth_headers`): Headers to sign. Default is `(request-target) date`.
+* `XC_RETRY_TOTAL` (`XCoverConfig.retry_total`): Total number of retries. Default is `5`.
+* `XC_RETRY_BACKOFF_FACTOR` (`XCoverConfig.retry_backoff_factor`): Backoff factor for retries timeout. Default is `2`.
+
+## Usage example
+
+### Using low-level `call` method
+
+```python
+import requests
+
+from xcover.xcover import XCover
+
+# Env variables are used
+client = XCover()
+
+# Prepare payload
+payload = {
+    "request": [
+        {
+            "policy_type": "event_ticket_protection",
+            "policy_type_version": 1,
+            "policy_start_date": "2021-12-01T17:59:00.831+00:00",
+            "event_datetime": "2021-12-25T21:00:00+00:00",
+            "event_name": "Ariana Grande",
+            "event_location": "The O2",
+            "number_of_tickets": 2,
+            "tickets": [
+                {"price": 100},
+            ],
+            "resale_ticket": False,
+            "event_country": "GB",
+        }
+    ],
+    "currency": "GBP",
+    "customer_country": "GB",
+    "customer_region": "London",
+    "customer_language": "en",
 }
+# Calling XCover API
+response: requests.Response = client.call(
+    method="POST",
+    url="partners/LLODT/quotes/",
+    payload=payload,
+)
+
+quote = response.json()
+print(quote)
+```
+
+### Retries
+
+This client will automatically retry certain operations when it is considered safe to do this.
+The retry number and intervals could be controlled via XC_RETRY_TOTAL and XC_RETRY_BACKOFF_FACTOR
+environment variables ot the same config options.
 
+Auto retry logic can be enabled/disabled per operation. However, further fine-tuning is possible
+via extending XCover class if required.
 
-setup(**setup_kwargs)
```

