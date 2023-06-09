# Comparing `tmp/contact_magic-0.1.0.tar.gz` & `tmp/contact_magic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.1.0.tar", max compression
+gzip compressed data, was "contact_magic-0.2.0.tar", max compression
```

## Comparing `contact_magic-0.1.0.tar` & `contact_magic-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0     4420 2023-06-09 17:09:31.138259 contact_magic-0.1.0/README.md
--rw-r--r--   0        0        0      104 2023-06-09 23:00:37.834076 contact_magic-0.1.0/contact_magic/__init__.py
--rw-r--r--   0        0        0     3340 2023-06-08 17:49:52.148765 contact_magic-0.1.0/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.1.0/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2132 2023-06-09 12:24:31.763283 contact_magic-0.1.0/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1309 2023-06-09 12:43:56.850054 contact_magic-0.1.0/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1428 2023-06-07 09:00:52.922224 contact_magic-0.1.0/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.1.0/contact_magic/logger.py
--rw-r--r--   0        0        0    11252 2023-06-09 13:05:03.101403 contact_magic-0.1.0/contact_magic/models.py
--rw-r--r--   0        0        0     2773 2023-06-09 12:44:06.238751 contact_magic-0.1.0/contact_magic/utils.py
--rw-r--r--   0        0        0     1710 2023-06-09 21:02:50.225656 contact_magic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 contact_magic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4420 2023-06-09 17:09:31.138259 contact_magic-0.2.0/README.md
+-rw-r--r--   0        0        0      104 2023-06-09 23:29:32.059389 contact_magic-0.2.0/contact_magic/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-09 23:24:56.292562 contact_magic-0.2.0/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     4667 2023-06-09 23:40:08.296999 contact_magic-0.2.0/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-09 23:24:56.315289 contact_magic-0.2.0/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.2.0/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2151 2023-06-09 23:24:56.298589 contact_magic-0.2.0/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1328 2023-06-09 23:24:56.296537 contact_magic-0.2.0/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.2.0/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.2.0/contact_magic/logger.py
+-rw-r--r--   0        0        0    11271 2023-06-09 23:24:56.313283 contact_magic-0.2.0/contact_magic/models.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.2.0/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1593 2023-06-09 23:26:11.761609 contact_magic-0.2.0/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.2.0/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-09 23:26:11.764227 contact_magic-0.2.0/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-09 23:26:11.765943 contact_magic-0.2.0/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     2773 2023-06-09 12:44:06.238751 contact_magic-0.2.0/contact_magic/utils.py
+-rw-r--r--   0        0        0     1683 2023-06-09 23:33:26.636024 contact_magic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 contact_magic-0.2.0/PKG-INFO
```

### Comparing `contact_magic-0.1.0/README.md` & `contact_magic-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.1.0/contact_magic/helpers.py` & `contact_magic-0.2.0/contact_magic/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gspread
 import numpy as np
 import pandas as pd
 
 from contact_magic.integrations.sheets import get_worksheet_from_spreadsheet
 from contact_magic.models import PersonalizationSettings
-from settings import SETTINGS
+from contact_magic.conf.settings import SETTINGS
 
 
 def prepare_data_for_gsheet(
     df: pd.DataFrame, mapping: dict = None, enforced_columns: list = None
 ):
     """
     Converts a dataframe to a list of list to be passed to Gspread or Sheet alternative.
```

### Comparing `contact_magic-0.1.0/contact_magic/integrations/copyfactory.py` & `contact_magic-0.2.0/contact_magic/integrations/copyfactory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 
 import httpx
 
 from contact_magic.utils import find_item
-from settings import SETTINGS
+from contact_magic.conf.settings import SETTINGS
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
 endpoint = "https://app.copyfactory.io/api/v2/generate/"
 
 headers = {"Accept": "application/json", "Authorization": SETTINGS.COPYFACTORY_API_KEY}
```

### Comparing `contact_magic-0.1.0/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.2.0/contact_magic/integrations/sales_scrapers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 
 import httpx
 
 from contact_magic.utils import fix_website
-from settings import SETTINGS
+from contact_magic.conf.settings import SETTINGS
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 base_url = "https://salesscrapers.dev/api/"
 
 headers = {"Accept": "application/json", "X-API-Key": SETTINGS.SALES_SCRAPERS_API_KEY}
```

### Comparing `contact_magic-0.1.0/contact_magic/integrations/sheets.py` & `contact_magic-0.2.0/contact_magic/integrations/sheets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import sleep
 
 import gspread
 from gspread.exceptions import APIError
 from oauth2client.service_account import ServiceAccountCredentials
 
-from settings import SETTINGS
+from contact_magic.conf.settings import SETTINGS
 
 
 def retry_req(func: callable, *args):
     sleepy_time = 1
     for _ in range(20):
         sleepy_time *= 2
         try:
```

### Comparing `contact_magic-0.1.0/contact_magic/models.py` & `contact_magic-0.2.0/contact_magic/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from contact_magic.integrations import (
     make_copyfactory_request,
     make_sales_scraper_request,
 )
 from contact_magic.logger import logger
 from contact_magic.utils import get_id_from_url, is_valid_premise_url, replace_keys
-from settings import SETTINGS
+from contact_magic.conf.settings import SETTINGS
 
 
 class DataRow(BaseModel):
     """
     A class to hold a row of data and it's index number
     to sort by after. Converts set data to a dict.
     """
```

### Comparing `contact_magic-0.1.0/contact_magic/utils.py` & `contact_magic-0.2.0/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.1.0/pyproject.toml` & `contact_magic-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.1.0"
+version = "0.2.0"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 license = "MIT"
-packages = [{include = "contact_magic"}]
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
     "Topic :: Internet",
@@ -43,12 +42,12 @@
 
 [tool.flit.metadata.requires-extra]
 dev = [
     "pre-commit >=2.17.0,<3.0.0",
 ]
 
 [tool.poetry.scripts]
-contact-magic = "scripts.agency:app"
+contact-magic = "contact_magic.scripts.agency:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `contact_magic-0.1.0/PKG-INFO` & `contact_magic-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.1.0
+Version: 0.2.0
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

