# Comparing `tmp/newrelic_sb_sdk-0.5.0.tar.gz` & `tmp/newrelic_sb_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic_sb_sdk-0.5.0.tar", max compression
+gzip compressed data, was "newrelic_sb_sdk-0.6.0.tar", max compression
```

## Comparing `newrelic_sb_sdk-0.5.0.tar` & `newrelic_sb_sdk-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      757 2023-06-06 01:06:19.235403 newrelic_sb_sdk-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1619 2023-04-16 17:39:52.127412 newrelic_sb_sdk-0.5.0/README.md
--rw-r--r--   0        0        0     2477 2023-06-06 01:06:19.231403 newrelic_sb_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-06 01:06:27.335437 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/__init__.py
--rw-r--r--   0        0        0   385992 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/_modidx.py
--rw-r--r--   0        0        0     4902 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/enums.py
--rw-r--r--   0        0        0      769 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/utils.py
--rw-r--r--   0        0        0     1997 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 01:03:08.154578 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/__init__.py
--rw-r--r--   0        0        0      372 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/base.py
--rw-r--r--   0        0        0      747 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/encoders.py
--rw-r--r--   0        0        0     2235 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/mixins.py
--rw-r--r--   0        0        0     1175 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/__init__.py
--rw-r--r--   0        0        0     1095 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/enums.py
--rw-r--r--   0        0        0     1006 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/pages.py
--rw-r--r--   0        0        0      593 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/utils.py
--rw-r--r--   0        0        0     3583 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/widgets.py
--rw-r--r--   0        0        0      200 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/__init__.py
--rw-r--r--   0        0        0   166880 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/enums.py
--rw-r--r--   0        0        0   238133 2023-06-06 01:03:43.658734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/input_objects.py
--rw-r--r--   0        0        0   422865 2023-06-06 01:03:43.658734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/objects.py
--rw-r--r--   0        0        0     6629 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/scalars.py
--rw-r--r--   0        0        0        0 2023-06-06 01:03:08.154578 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/__init__.py
--rw-r--r--   0        0        0      279 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/query.py
--rw-r--r--   0        0        0      787 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/response.py
--rw-r--r--   0        0        0     1901 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/text.py
--rw-r--r--   0        0        0     3174 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-06-10 11:01:12.829926 newrelic_sb_sdk-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1619 2023-04-16 17:39:52.127412 newrelic_sb_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0     2511 2023-06-10 11:01:12.825926 newrelic_sb_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-10 11:01:18.981947 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/__init__.py
+-rw-r--r--   0        0        0   385992 2023-06-10 10:08:43.124672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/_modidx.py
+-rw-r--r--   0        0        0     4902 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-10 10:08:43.124672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/enums.py
+-rw-r--r--   0        0        0      769 2023-06-10 10:08:43.124672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/utils.py
+-rw-r--r--   0        0        0     2060 2023-06-10 10:54:31.636620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/base.py
+-rw-r--r--   0        0        0      747 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/encoders.py
+-rw-r--r--   0        0        0     2235 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/mixins.py
+-rw-r--r--   0        0        0     1175 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/__init__.py
+-rw-r--r--   0        0        0     1095 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/enums.py
+-rw-r--r--   0        0        0     1006 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/pages.py
+-rw-r--r--   0        0        0      593 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/utils.py
+-rw-r--r--   0        0        0     3583 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/widgets.py
+-rw-r--r--   0        0        0      200 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/__init__.py
+-rw-r--r--   0        0        0    58585 2023-06-10 10:54:31.640620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/enums.py
+-rw-r--r--   0        0        0   358452 2023-06-10 10:54:31.636620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/input_objects.py
+-rw-r--r--   0        0        0   751350 2023-06-10 10:54:31.644620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/objects.py
+-rw-r--r--   0        0        0     3054 2023-06-10 10:54:31.644620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/scalars.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-10 10:54:31.636620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/query.py
+-rw-r--r--   0        0        0      787 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/response.py
+-rw-r--r--   0        0        0     1901 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/text.py
+-rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.6.0/PKG-INFO
```

### Comparing `newrelic_sb_sdk-0.5.0/LICENSE.txt` & `newrelic_sb_sdk-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/README.md` & `newrelic_sb_sdk-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/pyproject.toml` & `newrelic_sb_sdk-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "newrelic-sb-sdk"
-version = "0.5.0"
-description = "New Relic SDK to interact with API for data retrieving"
+version = "0.6.0"
+description = "New Relic SDK to interact with Nerdgraph API."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
-homepage = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface"
-repository = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface"
-documentation = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis"
+homepage = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk"
+repository = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk"
+documentation = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/wikis"
 keywords = [
   "Softbutterfly",
   "New Relic",
   "SDK",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -32,15 +32,15 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.5.0/newrelic-sb-sdk-v0.5.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.6.0/newrelic-sb-sdk-v0.6.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 enforce-typing = "^1.0.0.post1"
 python-dotenv = "^1.0.0"
@@ -52,21 +52,25 @@
 autopep8 = "^2.0.2"
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 flake8-black = "^0.3.6"
 importnb = "^2023.1.7"
+ipympl = "^0.9.3"
 isort = "^5.12.0"
 jupyter-book = "^0.15.1"
 jupyterlab = "^4.0.1"
+matplotlib = "^3.7.1"
 mypy = "^1.3.0"
 nbdev = "^2.3.12"
 nbmake = "^1.4.1"
 nbqa = {extras = ["toolchain"], version = "^1.7.0"}
+numpy = "^1.24.3"
+pandas = "^2.0.2"
 pre-commit = "^3.3.2"
 pycodestyle = "^2.10.0"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.4"
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-vcr = "^1.0.2"
```

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/_modidx.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/_modidx.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/__init__.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/enums.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/utils.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/client/__init__.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,18 @@
                 "query": query,
                 "variables": variables,
             },
         )
         return self.post(self.url, data=data, **kwargs)
 
     @staticmethod
-    def build_query(query_string: str, query_params: Dict[str, Any]) -> str:
-        return build_query(query_string, query_params)
+    def build_query(
+        *, query_string: str, query_params: Union[Dict[str, Any], None] = None
+    ) -> str:
+        return build_query(query_string=query_string, query_params=query_params)
 
 
 class NewRelicRestClient(Session):
     """Client for New Relic Rest API."""
 
     url: str = "https://api.newrelic.com/v2/"
```

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/encoders.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/encoders.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/mixins.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/__init__.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/enums.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/pages.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/pages.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/utils.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/widgets.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/widgets.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/response.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/response.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/text.py` & `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/text.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.5.0/PKG-INFO` & `newrelic_sb_sdk-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: newrelic-sb-sdk
-Version: 0.5.0
-Summary: New Relic SDK to interact with API for data retrieving
-Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
+Version: 0.6.0
+Summary: New Relic SDK to interact with Nerdgraph API.
+Home-page: https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk
 License: MIT
 Keywords: Softbutterfly,New Relic,SDK
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: enforce-typing (>=1.0.0.post1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues
-Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.5.0/newrelic-sb-sdk-v0.5.0.tar.gz
-Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
+Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/wikis
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.6.0/newrelic-sb-sdk-v0.6.0.tar.gz
+Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk)
 ![PyPI - Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/newrelic-sb-sdk)
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: newrelic-sb-sdk Version: 0.5.0 Summary: New Relic
-SDK to interact with API for data retrieving Home-page: https://gitlab.com/
-softbutterfly/open-source/wagtail-sb-admin-interface License: MIT Keywords:
+Metadata-Version: 2.1 Name: newrelic-sb-sdk Version: 0.6.0 Summary: New Relic
+SDK to interact with Nerdgraph API. Home-page: https://gitlab.com/
+softbutterfly/open-source/newrelic-sb-sdk License: MIT Keywords:
 Softbutterfly,New Relic,SDK Author: SoftButterfly Development Team Author-
 email: dev@softbutterfly.io Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Requires-Dist: enforce-typing
 (>=1.0.0.post1,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-
 Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0) Project-URL: Bug Tracker, https://
 gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues Project-URL:
-Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-
-interface/-/wikis Project-URL: Download, https://gitlab.com/softbutterfly/open-
-source/newrelic-sb-sdk/-/archive/v0.5.0/newrelic-sb-sdk-v0.5.0.tar.gz Project-
-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-
-interface Description-Content-Type: text/markdown ![Community-Project](https://
+Documentation, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/
+wikis Project-URL: Download, https://gitlab.com/softbutterfly/open-source/
+newrelic-sb-sdk/-/archive/v0.6.0/newrelic-sb-sdk-v0.6.0.tar.gz Project-URL:
+Repository, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk
+Description-Content-Type: text/markdown ![Community-Project](https://
 gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/
 softbutterfly-open-source--banner--community-project.png) ![PyPI - Supported
 versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk) ![PyPI -
 Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk) ![PyPI -
 Downloads](https://img.shields.io/pypi/dm/newrelic-sb-sdk) ![PyPI - MIT
 License](https://img.shields.io/pypi/l/newrelic-sb-sdk) [![Codacy Badge](https:
 //app.codacy.com/project/badge/Grade/1c25dec51e1c4a719be4c2d4ebe7eef6)](https:/
```

