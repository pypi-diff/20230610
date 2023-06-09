# Comparing `tmp/contact_magic-0.2.0.tar.gz` & `tmp/contact_magic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.2.0.tar", max compression
+gzip compressed data, was "contact_magic-0.2.1.tar", max compression
```

## Comparing `contact_magic-0.2.0.tar` & `contact_magic-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4420 2023-06-09 17:09:31.138259 contact_magic-0.2.0/README.md
--rw-r--r--   0        0        0      104 2023-06-09 23:29:32.059389 contact_magic-0.2.0/contact_magic/__init__.py
--rw-r--r--   0        0        0       50 2023-06-09 23:24:56.292562 contact_magic-0.2.0/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     4667 2023-06-09 23:40:08.296999 contact_magic-0.2.0/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-09 23:24:56.315289 contact_magic-0.2.0/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.2.0/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2151 2023-06-09 23:24:56.298589 contact_magic-0.2.0/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1328 2023-06-09 23:24:56.296537 contact_magic-0.2.0/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.2.0/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.2.0/contact_magic/logger.py
--rw-r--r--   0        0        0    11271 2023-06-09 23:24:56.313283 contact_magic-0.2.0/contact_magic/models.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.2.0/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1593 2023-06-09 23:26:11.761609 contact_magic-0.2.0/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.2.0/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4083 2023-06-09 23:26:11.764227 contact_magic-0.2.0/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-09 23:26:11.765943 contact_magic-0.2.0/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     2773 2023-06-09 12:44:06.238751 contact_magic-0.2.0/contact_magic/utils.py
--rw-r--r--   0        0        0     1683 2023-06-09 23:33:26.636024 contact_magic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 contact_magic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4420 2023-06-09 17:09:31.138259 contact_magic-0.2.1/README.md
+-rw-r--r--   0        0        0      209 2023-06-09 23:45:46.576485 contact_magic-0.2.1/contact_magic/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-09 23:24:56.292562 contact_magic-0.2.1/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     4667 2023-06-09 23:40:08.296999 contact_magic-0.2.1/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-09 23:24:56.315289 contact_magic-0.2.1/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.2.1/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2151 2023-06-09 23:24:56.298589 contact_magic-0.2.1/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1328 2023-06-09 23:24:56.296537 contact_magic-0.2.1/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.2.1/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.2.1/contact_magic/logger.py
+-rw-r--r--   0        0        0    11271 2023-06-09 23:24:56.313283 contact_magic-0.2.1/contact_magic/models.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.2.1/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1593 2023-06-09 23:26:11.761609 contact_magic-0.2.1/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.2.1/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-09 23:26:11.764227 contact_magic-0.2.1/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-09 23:26:11.765943 contact_magic-0.2.1/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     2773 2023-06-09 12:44:06.238751 contact_magic-0.2.1/contact_magic/utils.py
+-rw-r--r--   0        0        0     1731 2023-06-09 23:49:40.669901 contact_magic-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 contact_magic-0.2.1/PKG-INFO
```

### Comparing `contact_magic-0.2.0/README.md` & `contact_magic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/conf/settings.py` & `contact_magic-0.2.1/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/helpers.py` & `contact_magic-0.2.1/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/integrations/copyfactory.py` & `contact_magic-0.2.1/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.2.1/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/integrations/sheets.py` & `contact_magic-0.2.1/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/models.py` & `contact_magic-0.2.1/contact_magic/models.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/scripts/agency.py` & `contact_magic-0.2.1/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/scripts/run_workflows.py` & `contact_magic-0.2.1/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.2.1/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/contact_magic/utils.py` & `contact_magic-0.2.1/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.0/pyproject.toml` & `contact_magic-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.2.0"
+version = "0.2.1"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
+packages = [
+    { include = "contact_magic"}
+]
 license = "MIT"
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
```

### Comparing `contact_magic-0.2.0/PKG-INFO` & `contact_magic-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

