# Comparing `tmp/cvss_rescore-0.0.4.tar.gz` & `tmp/cvss_rescore-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvss_rescore-0.0.4.tar", last modified: Sun Feb 12 15:38:31 2023, max compression
+gzip compressed data, was "cvss_rescore-0.0.5.tar", last modified: Sat Jun 10 15:31:08 2023, max compression
```

## Comparing `cvss_rescore-0.0.4.tar` & `cvss_rescore-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.811028 cvss_rescore-0.0.4/
--rw-rw-rw-   0        0        0      623 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/.coveragerc
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.746123 cvss_rescore-0.0.4/.github/
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.749133 cvss_rescore-0.0.4/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      857 2023-02-04 17:41:26.000000 cvss_rescore-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      615 2023-02-04 17:41:26.000000 cvss_rescore-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-rw-   0        0        0      444 2023-02-04 17:41:26.000000 cvss_rescore-0.0.4/.github/dependabot.yml
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.760123 cvss_rescore-0.0.4/.github/workflows/
--rw-rw-rw-   0        0        0     3498 2023-01-29 21:41:14.000000 cvss_rescore-0.0.4/.github/workflows/bump_version.py
--rw-rw-rw-   0        0        0      807 2023-02-11 13:43:39.000000 cvss_rescore-0.0.4/.github/workflows/bump_version_action.yml
--rw-rw-rw-   0        0        0      360 2023-01-29 21:41:14.000000 cvss_rescore-0.0.4/.github/workflows/bump_version_requirements.txt
--rw-rw-rw-   0        0        0      721 2023-02-11 13:42:00.000000 cvss_rescore-0.0.4/.github/workflows/testpypi_package_deploy.yml
--rw-rw-rw-   0        0        0      632 2023-02-11 14:00:03.000000 cvss_rescore-0.0.4/.gitignore
--rw-rw-rw-   0        0        0      513 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/.readthedocs.yml
--rw-rw-rw-   0        0        0       77 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0      141 2023-02-11 14:13:00.000000 cvss_rescore-0.0.4/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14233 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1098 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      564 2023-02-12 15:20:11.000000 cvss_rescore-0.0.4/MAINTAINERS.md
--rw-rw-rw-   0        0        0     3415 2023-02-12 15:38:31.811028 cvss_rescore-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2723 2023-02-12 14:54:19.000000 cvss_rescore-0.0.4/README.rst
--rw-rw-rw-   0        0        0     2407 2023-02-11 13:40:35.000000 cvss_rescore-0.0.4/RULES.rst
--rw-rw-rw-   0        0        0     2361 2023-02-12 15:35:59.000000 cvss_rescore-0.0.4/SAMPLECODE.rst
--rw-rw-rw-   0        0        0      409 2023-02-11 13:42:00.000000 cvss_rescore-0.0.4/SECURITY.md
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.779862 cvss_rescore-0.0.4/docs/
--rw-rw-rw-   0        0        0     1183 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.781865 cvss_rescore-0.0.4/docs/_static/
--rw-rw-rw-   0        0        0       19 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/_static/.gitignore
--rw-rw-rw-   0        0        0       43 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/changelog.rst
--rw-rw-rw-   0        0        0    10041 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/contributing.rst
--rw-rw-rw-   0        0        0     1461 2023-02-12 14:58:19.000000 cvss_rescore-0.0.4/docs/index.rst
--rw-rw-rw-   0        0        0       74 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/license.rst
--rw-rw-rw-   0        0        0       41 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/readme.rst
--rw-rw-rw-   0        0        0      238 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/docs/requirements.txt
--rw-rw-rw-   0        0        0       27 2023-01-29 23:58:26.000000 cvss_rescore-0.0.4/docs/rules.rst
--rw-rw-rw-   0        0        0       32 2023-01-29 23:58:26.000000 cvss_rescore-0.0.4/docs/samplecode.rst
--rw-rw-rw-   0        0        0      563 2023-02-12 14:55:22.000000 cvss_rescore-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      682 2023-01-22 22:38:00.000000 cvss_rescore-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0     1443 2023-02-12 15:38:31.813028 cvss_rescore-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.784864 cvss_rescore-0.0.4/src/
--rw-rw-rw-   0        0        0       67 2023-01-23 00:19:00.000000 cvss_rescore-0.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.791356 cvss_rescore-0.0.4/src/cvss_rescore/
--rw-rw-rw-   0        0        0      593 2023-01-23 00:17:27.000000 cvss_rescore-0.0.4/src/cvss_rescore/__init__.py
--rw-rw-rw-   0        0        0     4533 2023-02-12 14:57:16.000000 cvss_rescore-0.0.4/src/cvss_rescore/cvsslib.py
--rw-rw-rw-   0        0        0      118 2023-01-22 16:01:23.000000 cvss_rescore-0.0.4/src/cvss_rescore/manualVettingException.py
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.804022 cvss_rescore-0.0.4/src/cvss_rescore.egg-info/
--rw-rw-rw-   0        0        0     3415 2023-02-12 15:38:31.000000 cvss_rescore-0.0.4/src/cvss_rescore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-02-12 15:38:31.000000 cvss_rescore-0.0.4/src/cvss_rescore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 15:38:31.000000 cvss_rescore-0.0.4/src/cvss_rescore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-12 15:38:29.000000 cvss_rescore-0.0.4/src/cvss_rescore.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      131 2023-02-12 15:38:31.000000 cvss_rescore-0.0.4/src/cvss_rescore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-12 15:38:31.000000 cvss_rescore-0.0.4/src/cvss_rescore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.807029 cvss_rescore-0.0.4/tests/
--rw-rw-rw-   0        0        0      290 2023-01-22 21:44:29.000000 cvss_rescore-0.0.4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-12 15:38:31.809029 cvss_rescore-0.0.4/tests/cvss_rescore/
--rw-rw-rw-   0        0        0     6108 2023-02-12 14:52:27.000000 cvss_rescore-0.0.4/tests/cvss_rescore/test_cvsslib.py
--rw-rw-rw-   0        0        0     4851 2023-01-24 10:01:02.000000 cvss_rescore-0.0.4/tests/rules_actions.json
--rw-rw-rw-   0        0        0     2781 2023-02-05 19:00:55.000000 cvss_rescore-0.0.4/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.800274 cvss_rescore-0.0.5/
+-rw-rw-rw-   0        0        0      623 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/.coveragerc
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.740385 cvss_rescore-0.0.5/.github/
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.743385 cvss_rescore-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      857 2023-02-04 17:41:26.000000 cvss_rescore-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      615 2023-02-04 17:41:26.000000 cvss_rescore-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-rw-   0        0        0      444 2023-02-04 17:41:26.000000 cvss_rescore-0.0.5/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.752467 cvss_rescore-0.0.5/.github/workflows/
+-rw-rw-rw-   0        0        0     1162 2023-06-10 14:26:39.000000 cvss_rescore-0.0.5/.github/workflows/Publish_Pypi_Github.yml
+-rw-rw-rw-   0        0        0     3498 2023-01-29 21:41:14.000000 cvss_rescore-0.0.5/.github/workflows/bump_version.py
+-rw-rw-rw-   0        0        0      807 2023-02-11 13:43:39.000000 cvss_rescore-0.0.5/.github/workflows/bump_version_action.yml
+-rw-rw-rw-   0        0        0      360 2023-06-10 15:21:45.000000 cvss_rescore-0.0.5/.github/workflows/bump_version_requirements.txt
+-rw-rw-rw-   0        0        0      721 2023-02-11 13:42:00.000000 cvss_rescore-0.0.5/.github/workflows/testpypi_package_deploy.yml
+-rw-rw-rw-   0        0        0      632 2023-02-11 14:00:03.000000 cvss_rescore-0.0.5/.gitignore
+-rw-rw-rw-   0        0        0      513 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/.readthedocs.yml
+-rw-rw-rw-   0        0        0       77 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0      204 2023-06-10 15:30:56.000000 cvss_rescore-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0      141 2023-06-10 15:25:09.000000 cvss_rescore-0.0.5/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14233 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1098 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      564 2023-06-10 15:24:52.000000 cvss_rescore-0.0.5/MAINTAINERS.md
+-rw-rw-rw-   0        0        0     3415 2023-06-10 15:31:08.800274 cvss_rescore-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2723 2023-02-12 14:54:19.000000 cvss_rescore-0.0.5/README.rst
+-rw-rw-rw-   0        0        0     2407 2023-02-11 13:40:35.000000 cvss_rescore-0.0.5/RULES.rst
+-rw-rw-rw-   0        0        0     2361 2023-02-12 15:35:59.000000 cvss_rescore-0.0.5/SAMPLECODE.rst
+-rw-rw-rw-   0        0        0      409 2023-02-11 13:42:00.000000 cvss_rescore-0.0.5/SECURITY.md
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.771474 cvss_rescore-0.0.5/docs/
+-rw-rw-rw-   0        0        0     1183 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.773474 cvss_rescore-0.0.5/docs/_static/
+-rw-rw-rw-   0        0        0       19 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0       43 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/changelog.rst
+-rw-rw-rw-   0        0        0    10041 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1461 2023-02-12 14:58:19.000000 cvss_rescore-0.0.5/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/license.rst
+-rw-rw-rw-   0        0        0       41 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/readme.rst
+-rw-rw-rw-   0        0        0      238 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/docs/requirements.txt
+-rw-rw-rw-   0        0        0       27 2023-01-29 23:58:26.000000 cvss_rescore-0.0.5/docs/rules.rst
+-rw-rw-rw-   0        0        0       32 2023-01-29 23:58:26.000000 cvss_rescore-0.0.5/docs/samplecode.rst
+-rw-rw-rw-   0        0        0      748 2023-06-10 15:30:56.000000 cvss_rescore-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      682 2023-06-03 15:13:27.000000 cvss_rescore-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0     1443 2023-06-10 15:31:08.801273 cvss_rescore-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.774475 cvss_rescore-0.0.5/src/
+-rw-rw-rw-   0        0        0       67 2023-01-23 00:19:00.000000 cvss_rescore-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.781275 cvss_rescore-0.0.5/src/cvss_rescore/
+-rw-rw-rw-   0        0        0      593 2023-01-23 00:17:27.000000 cvss_rescore-0.0.5/src/cvss_rescore/__init__.py
+-rw-rw-rw-   0        0        0     4985 2023-06-10 14:22:23.000000 cvss_rescore-0.0.5/src/cvss_rescore/cvsslib.py
+-rw-rw-rw-   0        0        0      118 2023-01-22 16:01:23.000000 cvss_rescore-0.0.5/src/cvss_rescore/manualVettingException.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.792273 cvss_rescore-0.0.5/src/cvss_rescore.egg-info/
+-rw-rw-rw-   0        0        0     3415 2023-06-10 15:31:08.000000 cvss_rescore-0.0.5/src/cvss_rescore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-06-10 15:31:08.000000 cvss_rescore-0.0.5/src/cvss_rescore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 15:31:08.000000 cvss_rescore-0.0.5/src/cvss_rescore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 15:29:02.000000 cvss_rescore-0.0.5/src/cvss_rescore.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      131 2023-06-10 15:31:08.000000 cvss_rescore-0.0.5/src/cvss_rescore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 15:31:08.000000 cvss_rescore-0.0.5/src/cvss_rescore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.796273 cvss_rescore-0.0.5/tests/
+-rw-rw-rw-   0        0        0      290 2023-01-22 21:44:29.000000 cvss_rescore-0.0.5/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:31:08.798280 cvss_rescore-0.0.5/tests/cvss_rescore/
+-rw-rw-rw-   0        0        0     7502 2023-06-10 14:22:23.000000 cvss_rescore-0.0.5/tests/cvss_rescore/test_cvsslib.py
+-rw-rw-rw-   0        0        0     4851 2023-01-24 10:01:02.000000 cvss_rescore-0.0.5/tests/rules_actions.json
+-rw-rw-rw-   0        0        0     2781 2023-02-05 19:00:55.000000 cvss_rescore-0.0.5/tox.ini
```

### Comparing `cvss_rescore-0.0.4/.coveragerc` & `cvss_rescore-0.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `cvss_rescore-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `cvss_rescore-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/.github/workflows/bump_version.py` & `cvss_rescore-0.0.5/.github/workflows/bump_version.py`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/.github/workflows/bump_version_action.yml` & `cvss_rescore-0.0.5/.github/workflows/bump_version_action.yml`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/.github/workflows/testpypi_package_deploy.yml` & `cvss_rescore-0.0.5/.github/workflows/testpypi_package_deploy.yml`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/.gitignore` & `cvss_rescore-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/.readthedocs.yml` & `cvss_rescore-0.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/CONTRIBUTING.rst` & `cvss_rescore-0.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/LICENSE.txt` & `cvss_rescore-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/MAINTAINERS.md` & `cvss_rescore-0.0.5/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/PKG-INFO` & `cvss_rescore-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvss_rescore
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rescore cvss3 and 3.1 results from any json file based on custom rules that you create.
 Home-page: https://github.com/bp4151/cvss-rescore/
 Author: Bruce Parr
 Author-email: bp4151@gmail.com
 License: MIT
 Project-URL: Documentation, https://cvss-rescore.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/bp4151/cvss-rescore/
```

### Comparing `cvss_rescore-0.0.4/README.rst` & `cvss_rescore-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/RULES.rst` & `cvss_rescore-0.0.5/RULES.rst`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/SAMPLECODE.rst` & `cvss_rescore-0.0.5/SAMPLECODE.rst`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/docs/Makefile` & `cvss_rescore-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/docs/conf.py` & `cvss_rescore-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/docs/index.rst` & `cvss_rescore-0.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/pyproject.toml` & `cvss_rescore-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,7 +9,15 @@
 version_scheme = "release-branch-semver"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+tag_format = "v$version"
+version_type = "semver"
+version = "0.0.5"
+update_changelog_on_bump = true
+major_version_zero = true
```

### Comparing `cvss_rescore-0.0.4/requirements.txt` & `cvss_rescore-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/setup.cfg` & `cvss_rescore-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/setup.py` & `cvss_rescore-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/src/cvss_rescore/__init__.py` & `cvss_rescore-0.0.5/src/cvss_rescore/__init__.py`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/src/cvss_rescore/cvsslib.py` & `cvss_rescore-0.0.5/src/cvss_rescore/cvsslib.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,26 @@
         :exception: SymbolResolutionError will log to error if the path in your
             custom rule cannot be found in the source json file
         :exception: RuleSyntaxError will log to error if the rule you have
             defined cannot be parsed.
         :exception: ManualVettingException will be thrown if no rules were matched.
             This can be caught in your parent script
         """
+        # convert the original vector string to a dict
         original_vector_obj = cls.__str2dict(original_vector_string)
-        if original_vector_obj['CVSS'].startswith('3'):
-            cvss_obj = CVSS3(original_vector_string)
-        elif original_vector_obj['CVSS'].startswith('2'):
-            raise ValueError(f'CVSS version {original_vector_obj["CVSS"]} is unsupported, manual vetting required')
+        # check if the vector string contains `CVSS`
+        if original_vector_obj.get('CVSS') is None:
+            raise ValueError('CVSS vector string does not contain CVSS, manual vetting required')
+        else:
+            # if we have a CVSS object and the value is 3.x, use the CVSS3 class
+            # if we have a CVSS object and the value is 2.x, raise an error
+            if original_vector_obj['CVSS'].startswith('3'):
+                cvss_obj = CVSS3(original_vector_string)
+            elif original_vector_obj['CVSS'].startswith('2'):
+                raise ValueError(f'CVSS version {original_vector_obj["CVSS"]} is unsupported, manual vetting required')
         results = []
         rules_applied = []
         result = False
         for rule_action in cls.rules_actions:
             try:
                 rule = Rule(rule_action['rule'])
                 result = rule.matches(record)
```

### Comparing `cvss_rescore-0.0.4/src/cvss_rescore.egg-info/PKG-INFO` & `cvss_rescore-0.0.5/src/cvss_rescore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvss-rescore
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rescore cvss3 and 3.1 results from any json file based on custom rules that you create.
 Home-page: https://github.com/bp4151/cvss-rescore/
 Author: Bruce Parr
 Author-email: bp4151@gmail.com
 License: MIT
 Project-URL: Documentation, https://cvss-rescore.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/bp4151/cvss-rescore/
```

### Comparing `cvss_rescore-0.0.4/src/cvss_rescore.egg-info/SOURCES.txt` & `cvss_rescore-0.0.5/src/cvss_rescore.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .coveragerc
 .gitignore
 .readthedocs.yml
 AUTHORS.rst
+CHANGELOG.md
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 MAINTAINERS.md
 README.rst
 RULES.rst
 SAMPLECODE.rst
@@ -14,14 +15,15 @@
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/Publish_Pypi_Github.yml
 .github/workflows/bump_version.py
 .github/workflows/bump_version_action.yml
 .github/workflows/bump_version_requirements.txt
 .github/workflows/testpypi_package_deploy.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
```

### Comparing `cvss_rescore-0.0.4/tests/cvss_rescore/test_cvsslib.py` & `cvss_rescore-0.0.5/tests/cvss_rescore/test_cvsslib.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,49 @@
     cvsslib = CvssLib(rules_file_path=rules_file)
     try:
         modified_vector_string, modified_environmental_score, modified_severity, rules_applied = cvsslib.get_modified_cvss(record=record, original_vector_string=original_vector_string, logger=logger)
     except ValueError as ve:
         assert True
 
 
+def test_missing_cvss_throws_value_error():
+    record = {
+        "locations": "",
+        "package": {
+            "Package": {
+                "pm": "npm",
+                "group": None,
+                "name": "minimist",
+                "version": "1.2.0",
+                "vendor": None,
+                "fixVersions": ["[1.2.6]"],
+                "impactPaths": [["npm://covert:1.0.0", "npm://minimist:1.2.0"]]
+            },
+            "Vulnerabilities": [{
+                "id": "XRAY-000000",
+                "title": "Critical vulnerability found in component temp_react_core",
+                "description": "Prototype pollution vulnerability in function parseQuery in parseQuery.js in webpack loader-utils 2.0.0 via the name variable in parseQuery.js.",
+                "cvssScore": "10.0",
+                "cvssVector": "AV:N/AC:L/Au:N/C:C/I:C/A:C)",
+                "cve": "CVE-2022-00000"
+            }]
+        }
+    }
+    original_vector_string = record.get('package').get('Vulnerabilities')[0].get('cvssVector')
+    cvsslib = CvssLib(rules_file_path=rules_file)
+    try:
+        modified_vector_string, \
+            modified_environmental_score, \
+            modified_severity, \
+            rules_applied = \
+            cvsslib.get_modified_cvss(record=record, original_vector_string=original_vector_string)
+    except ValueError as ve:
+        assert True
+
+
 def test_cvss3_does_not_throw_exception():
     record = {
         "locations": "",
         "package": {
             "Package": {
                 "pm": "npm",
                 "group": None,
@@ -72,16 +107,15 @@
     original_vector_string = record.get('package').get('Vulnerabilities')[0].get('cvssVector')
     cvsslib = CvssLib(rules_file_path=rules_file)
     modified_vector_string, \
         modified_environmental_score, \
         modified_severity, \
         rules_applied = cvsslib.get_modified_cvss(
         record=record,
-        original_vector_string=original_vector_string,
-        logger=logger)
+        original_vector_string=original_vector_string)
     assert modified_severity[0] == 'Critical'
 
 
 def test_invalid_vector_value():
     record = {
         "locations": "",
         "package": {
```

### Comparing `cvss_rescore-0.0.4/tests/rules_actions.json` & `cvss_rescore-0.0.5/tests/rules_actions.json`

 * *Files identical despite different names*

### Comparing `cvss_rescore-0.0.4/tox.ini` & `cvss_rescore-0.0.5/tox.ini`

 * *Files identical despite different names*

