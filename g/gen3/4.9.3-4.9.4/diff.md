# Comparing `tmp/gen3-4.9.3.tar.gz` & `tmp/gen3-4.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3-4.9.3.tar", max compression
+gzip compressed data, was "gen3-4.9.4.tar", max compression
```

## Comparing `gen3-4.9.3.tar` & `gen3-4.9.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rwxr-xr-x   0        0        0    11357 2022-05-12 14:29:14.735861 gen3-4.9.3/LICENSE
--rwxr-xr-x   0        0        0      163 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/__init__.py
--rwxr-xr-x   0        0        0    14164 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/auth.py
--rw-r--r--   0        0        0        0 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/__init__.py
--rw-r--r--   0        0        0     2939 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/__main__.py
--rw-r--r--   0        0        0     2283 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/auth.py
--rw-r--r--   0        0        0      864 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/configure.py
--rw-r--r--   0        0        0     2674 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/discovery.py
--rw-r--r--   0        0        0     3974 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/drs_pull.py
--rw-r--r--   0        0        0     8834 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/objects.py
--rw-r--r--   0        0        0      570 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/pfb.py
--rw-r--r--   0        0        0     2123 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/cli/wss.py
--rw-r--r--   0        0        0     2535 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/configure.py
--rwxr-xr-x   0        0        0     4116 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/file.py
--rwxr-xr-x   0        0        0    23827 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/index.py
--rw-r--r--   0        0        0     8292 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/jobs.py
--rw-r--r--   0        0        0    20310 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/metadata.py
--rwxr-xr-x   0        0        0     2129 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/object.py
--rwxr-xr-x   0        0        0     7616 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/query.py
--rwxr-xr-x   0        0        0    26941 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/submission.py
--rw-r--r--   0        0        0        0 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/__init__.py
--rw-r--r--   0        0        0    11698 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/bundle/ingest_manifest.py
--rw-r--r--   0        0        0     6619 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/diff.py
--rw-r--r--   0        0        0        1 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/download/__init__.py
--rw-r--r--   0        0        0    47500 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/download/drs_download.py
--rw-r--r--   0        0        0    14280 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/download/drs_resolvers.py
--rw-r--r--   0        0        0      240 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/indexing/__init__.py
--rw-r--r--   0        0        0    12079 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/indexing/download_manifest.py
--rw-r--r--   0        0        0    28410 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/indexing/index_manifest.py
--rw-r--r--   0        0        0    14184 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/indexing/manifest_columns.py
--rw-r--r--   0        0        0    17078 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/indexing/merge_manifests.py
--rw-r--r--   0        0        0    17092 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/indexing/validate_manifest_format.py
--rw-r--r--   0        0        0    14531 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/indexing/verify_manifest.py
--rw-r--r--   0        0        0    10919 2022-05-12 14:29:14.759873 gen3-4.9.3/gen3/tools/merge.py
--rw-r--r--   0        0        0      235 2022-05-12 14:29:14.763875 gen3-4.9.3/gen3/tools/metadata/__init__.py
--rw-r--r--   0        0        0     7595 2022-05-12 14:29:14.763875 gen3-4.9.3/gen3/tools/metadata/discovery.py
--rw-r--r--   0        0        0    19933 2022-05-12 14:29:14.763875 gen3-4.9.3/gen3/tools/metadata/ingest_manifest.py
--rw-r--r--   0        0        0    10450 2022-05-12 14:29:14.763875 gen3-4.9.3/gen3/tools/metadata/verify_manifest.py
--rw-r--r--   0        0        0     5903 2022-05-12 14:29:14.763875 gen3-4.9.3/gen3/utils.py
--rw-r--r--   0        0        0     6140 2022-05-12 14:29:14.763875 gen3-4.9.3/gen3/wss.py
--rw-r--r--   0        0        0     1644 2022-05-12 14:29:14.763875 gen3-4.9.3/pyproject.toml
--rw-r--r--   0        0        0     1139 2022-05-12 14:31:53.487117 gen3-4.9.3/setup.py
--rw-r--r--   0        0        0     1259 2022-05-12 14:31:53.487401 gen3-4.9.3/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2022-06-06 23:14:00.681649 gen3-4.9.4/LICENSE
+-rwxr-xr-x   0        0        0      163 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/__init__.py
+-rwxr-xr-x   0        0        0    14164 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/auth.py
+-rw-r--r--   0        0        0        0 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/__init__.py
+-rw-r--r--   0        0        0     2939 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/__main__.py
+-rw-r--r--   0        0        0     2283 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/auth.py
+-rw-r--r--   0        0        0      864 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/configure.py
+-rw-r--r--   0        0        0     2674 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/discovery.py
+-rw-r--r--   0        0        0     3975 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/drs_pull.py
+-rw-r--r--   0        0        0     8834 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/objects.py
+-rw-r--r--   0        0        0      570 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/pfb.py
+-rw-r--r--   0        0        0     2123 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/cli/wss.py
+-rw-r--r--   0        0        0     2535 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/configure.py
+-rwxr-xr-x   0        0        0     4116 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/file.py
+-rwxr-xr-x   0        0        0    23827 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/index.py
+-rw-r--r--   0        0        0     8292 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/jobs.py
+-rw-r--r--   0        0        0    19711 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/metadata.py
+-rwxr-xr-x   0        0        0     2129 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/object.py
+-rwxr-xr-x   0        0        0     7616 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/query.py
+-rwxr-xr-x   0        0        0    26941 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/submission.py
+-rw-r--r--   0        0        0        0 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/__init__.py
+-rw-r--r--   0        0        0    11698 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/bundle/ingest_manifest.py
+-rw-r--r--   0        0        0     6619 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/diff.py
+-rw-r--r--   0        0        0        1 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/download/__init__.py
+-rw-r--r--   0        0        0    47501 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/download/drs_download.py
+-rw-r--r--   0        0        0    14281 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/download/drs_resolvers.py
+-rw-r--r--   0        0        0      240 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/indexing/__init__.py
+-rw-r--r--   0        0        0    12079 2022-06-06 23:14:00.709635 gen3-4.9.4/gen3/tools/indexing/download_manifest.py
+-rw-r--r--   0        0        0    28410 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/indexing/index_manifest.py
+-rw-r--r--   0        0        0    14184 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/indexing/manifest_columns.py
+-rw-r--r--   0        0        0    17078 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/indexing/merge_manifests.py
+-rw-r--r--   0        0        0    17092 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/indexing/validate_manifest_format.py
+-rw-r--r--   0        0        0    14531 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/indexing/verify_manifest.py
+-rw-r--r--   0        0        0    10919 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/merge.py
+-rw-r--r--   0        0        0      235 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/metadata/__init__.py
+-rw-r--r--   0        0        0     7595 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/metadata/discovery.py
+-rw-r--r--   0        0        0    19933 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/metadata/ingest_manifest.py
+-rw-r--r--   0        0        0    10450 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/tools/metadata/verify_manifest.py
+-rw-r--r--   0        0        0     5903 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/utils.py
+-rw-r--r--   0        0        0     6140 2022-06-06 23:14:00.713633 gen3-4.9.4/gen3/wss.py
+-rw-r--r--   0        0        0     1644 2022-06-06 23:14:00.713633 gen3-4.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1139 2022-06-06 23:16:27.049714 gen3-4.9.4/setup.py
+-rw-r--r--   0        0        0     1259 2022-06-06 23:16:27.049998 gen3-4.9.4/PKG-INFO
```

### Comparing `gen3-4.9.3/LICENSE` & `gen3-4.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/auth.py` & `gen3-4.9.4/gen3/auth.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/cli/__main__.py` & `gen3-4.9.4/gen3/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/cli/auth.py` & `gen3-4.9.4/gen3/cli/auth.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/cli/configure.py` & `gen3-4.9.4/gen3/cli/configure.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/cli/discovery.py` & `gen3-4.9.4/gen3/cli/discovery.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/cli/drs_pull.py` & `gen3-4.9.4/gen3/cli/drs_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import click
-from cdiserrors import get_logger
+from cdislogging import get_logger
 
 from gen3.tools.download.drs_download import (
     list_files_in_drs_manifest,
     list_drs_object,
     download_files_in_drs_manifest,
     download_drs_object,
     list_access_in_drs_manifest,
```

### Comparing `gen3-4.9.3/gen3/cli/objects.py` & `gen3-4.9.4/gen3/cli/objects.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/cli/pfb.py` & `gen3-4.9.4/gen3/cli/pfb.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/cli/wss.py` & `gen3-4.9.4/gen3/cli/wss.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/configure.py` & `gen3-4.9.4/gen3/configure.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/file.py` & `gen3-4.9.4/gen3/file.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/index.py` & `gen3-4.9.4/gen3/index.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/jobs.py` & `gen3-4.9.4/gen3/jobs.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/metadata.py` & `gen3-4.9.4/gen3/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -493,15 +493,14 @@
                     valid = False
             # generate package metadata
             package_metadata = self._get_package_metadata(
                 metadata,
                 indexd_doc.file_name,
                 indexd_doc.size,
                 indexd_doc.hashes,
-                indexd_doc.authz,
                 indexd_doc.urls,
                 package_contents,
             )
             to_submit.update(package_metadata)
         elif package_contents:
             logging.error(
                 f"ERROR: tried to set '{PACKAGE_CONTENTS_STANDARD_KEY}' for a non-package row. Ignoring '{PACKAGE_CONTENTS_STANDARD_KEY}'. Set '{RECORD_TYPE_STANDARD_KEY}' to 'package' to create packages."
@@ -510,64 +509,51 @@
 
         if not valid:
             raise Exception(f"Metadata is not valid: {metadata}")
 
         return to_submit
 
     def _get_package_metadata(
-        self, submitted_metadata, file_name, file_size, hashes, authz, urls, contents
+        self, submitted_metadata, file_name, file_size, hashes, urls, contents
     ):
         """
-        The MDS /objects API currently expects files that have not been
+        The MDS Objects API currently expects files that have not been
         uploaded yet. For files we only needs to index, not upload, create
         object records manually by generating the expected object fields.
         TODO: update the MDS objects API to not create upload URLs if the
         relevant data is provided.
         """
 
-        def _get_buckets_and_filename_from_urls(submitted_metadata, urls):
+        def _get_filename_from_urls(submitted_metadata, urls):
             file_name = ""
-            bucket_urls = []
             if not urls:
                 logging.warning(f"No URLs provided for: {submitted_metadata}")
             for url in urls:
                 _file_name = os.path.basename(url)
                 if not file_name:
                     file_name = _file_name
                 else:
                     if file_name != _file_name:
                         logging.warning(
                             f"Received multiple URLs with different file names; will use the first URL (file name '{file_name}'): {submitted_metadata}"
                         )
-                parsed = urlparse(url)
-                _bucket_url = f"{parsed.scheme}://{parsed.netloc}"
-                bucket_urls.append(_bucket_url)
-            return file_name, bucket_urls
-
-        file_name_from_url, bucket_urls = _get_buckets_and_filename_from_urls(
-            submitted_metadata, urls
-        )
+            return file_name
+
+        file_name_from_url = _get_filename_from_urls(submitted_metadata, urls)
         if not file_name:
             file_name = file_name_from_url
 
-        _, file_ext = os.path.splitext(file_name)
-        uploader = self._auth_provider._token_info.get("sub")
         now = str(datetime.utcnow())
         metadata = {
             "type": "package",
             "package": {
                 "version": "0.1",
                 "file_name": file_name,
                 "created_time": now,
                 "updated_time": now,
                 "size": file_size,
                 "hashes": hashes,
                 "contents": contents or None,
             },
-            "_resource_paths": authz,
-            "_uploader_id": uploader,
-            "_buckets": bucket_urls,
-            "_filename": file_name,
-            "_file_extension": file_ext,
             "_upload_status": "uploaded",
         }
         return metadata
```

### Comparing `gen3-4.9.3/gen3/object.py` & `gen3-4.9.4/gen3/object.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/query.py` & `gen3-4.9.4/gen3/query.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/submission.py` & `gen3-4.9.4/gen3/submission.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/bundle/ingest_manifest.py` & `gen3-4.9.4/gen3/tools/bundle/ingest_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/diff.py` & `gen3-4.9.4/gen3/tools/diff.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/download/drs_download.py` & `gen3-4.9.4/gen3/tools/download/drs_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from json import load as json_load, loads as json_loads, JSONDecodeError
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 import humanfriendly
 import requests
 import zipfile
-from cdiserrors import get_logger
+from cdislogging import get_logger
 from dataclasses_json import dataclass_json, LetterCase
 from dateutil import parser as date_parser
 from tqdm import tqdm
 from urllib.parse import urlparse
 
 from gen3.auth import Gen3Auth, Gen3AuthError, decode_token
 from gen3.auth import _handle_access_token_response
```

### Comparing `gen3-4.9.3/gen3/tools/download/drs_resolvers.py` & `gen3-4.9.4/gen3/tools/download/drs_resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional
 import requests
 import json
-from cdiserrors import get_logger
+from cdislogging import get_logger
 import os
 import inspect
 from datetime import datetime, timezone, timedelta
 from pathlib import Path
 
 # DRS Compact identifiers are resolved to hostnames using a set of resolvers
 # NOTE: that the policy is to minimize the requests to dataguids.org or other DRS
```

### Comparing `gen3-4.9.3/gen3/tools/indexing/download_manifest.py` & `gen3-4.9.4/gen3/tools/indexing/download_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/indexing/index_manifest.py` & `gen3-4.9.4/gen3/tools/indexing/index_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/indexing/manifest_columns.py` & `gen3-4.9.4/gen3/tools/indexing/manifest_columns.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/indexing/merge_manifests.py` & `gen3-4.9.4/gen3/tools/indexing/merge_manifests.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/indexing/validate_manifest_format.py` & `gen3-4.9.4/gen3/tools/indexing/validate_manifest_format.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/indexing/verify_manifest.py` & `gen3-4.9.4/gen3/tools/indexing/verify_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/merge.py` & `gen3-4.9.4/gen3/tools/merge.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/metadata/discovery.py` & `gen3-4.9.4/gen3/tools/metadata/discovery.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/metadata/ingest_manifest.py` & `gen3-4.9.4/gen3/tools/metadata/ingest_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/tools/metadata/verify_manifest.py` & `gen3-4.9.4/gen3/tools/metadata/verify_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/utils.py` & `gen3-4.9.4/gen3/utils.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/gen3/wss.py` & `gen3-4.9.4/gen3/wss.py`

 * *Files identical despite different names*

### Comparing `gen3-4.9.3/pyproject.toml` & `gen3-4.9.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gen3"
 homepage = "https://gen3.org/"
-version = "4.9.3"
+version = "4.9.4"
 description = "Gen3 CLI and Python SDK"
 authors = ["Center for Translational Data Science at the University of Chicago <support@datacommons.io>"]
 license = "Apache-2.0"
 packages = [
     { include = "gen3" },
 ]
 classifiers = [
```

### Comparing `gen3-4.9.3/setup.py` & `gen3-4.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'tqdm>=4.61.2']
 
 entry_points = \
 {'console_scripts': ['gen3 = gen3.cli.__main__:main']}
 
 setup_kwargs = {
     'name': 'gen3',
-    'version': '4.9.3',
+    'version': '4.9.4',
     'description': 'Gen3 CLI and Python SDK',
     'long_description': None,
     'author': 'Center for Translational Data Science at the University of Chicago',
     'author_email': 'support@datacommons.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gen3.org/',
```

### Comparing `gen3-4.9.3/PKG-INFO` & `gen3-4.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3
-Version: 4.9.3
+Version: 4.9.4
 Summary: Gen3 CLI and Python SDK
 Home-page: https://gen3.org/
 License: Apache-2.0
 Author: Center for Translational Data Science at the University of Chicago
 Author-email: support@datacommons.io
 Requires-Python: >=3.6,<3.11
 Classifier: Development Status :: 4 - Beta
```

