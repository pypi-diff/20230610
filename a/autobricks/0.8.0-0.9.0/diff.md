# Comparing `tmp/autobricks-0.8.0.tar.gz` & `tmp/autobricks-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobricks-0.8.0.tar", last modified: Sun Jun  4 12:50:57 2023, max compression
+gzip compressed data, was "autobricks-0.9.0.tar", last modified: Sat Jun 10 18:24:22 2023, max compression
```

## Comparing `autobricks-0.8.0.tar` & `autobricks-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:50:57.102836 autobricks-0.8.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-06-04 12:50:57.102836 autobricks-0.8.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-06-04 12:50:35.000000 autobricks-0.8.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:50:57.102836 autobricks-0.8.0/autobricks/
--rw-r--r--   0 vsts      (1001) docker     (123)     8987 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/Cluster.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3545 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/Dbfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5787 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/Job.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1395 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/Library.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7619 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/SetupTools.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12859 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/Sql.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8297 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/Workspace.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/_common.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1266 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/_decode_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:50:57.102836 autobricks-0.8.0/autobricks/api_service/
--rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5017 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/_auth.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1440 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/_auth_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1686 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/_base_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2876 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4363 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/api_service.py
--rw-r--r--   0 vsts      (1001) docker     (123)      312 2023-06-04 12:50:35.000000 autobricks-0.8.0/autobricks/api_service/autobricks_logging.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:50:57.102836 autobricks-0.8.0/autobricks.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-06-04 12:50:57.000000 autobricks-0.8.0/autobricks.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-06-04 12:50:57.000000 autobricks-0.8.0/autobricks.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-04 12:50:57.000000 autobricks-0.8.0/autobricks.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-04 12:50:57.000000 autobricks-0.8.0/autobricks.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-06-04 12:50:57.000000 autobricks-0.8.0/autobricks.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-06-04 12:50:57.000000 autobricks-0.8.0/autobricks.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-04 12:50:57.102836 autobricks-0.8.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-06-04 12:50:35.000000 autobricks-0.8.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 18:24:22.523325 autobricks-0.9.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-06-10 18:24:22.519325 autobricks-0.9.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-06-10 18:23:59.000000 autobricks-0.9.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 18:24:22.519325 autobricks-0.9.0/autobricks/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8987 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/Cluster.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3545 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/Dbfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5753 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/Job.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1395 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/Library.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3630 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/Pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7619 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/SetupTools.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12859 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/Sql.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8297 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/Workspace.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/_common.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1266 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/_decode_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 18:24:22.519325 autobricks-0.9.0/autobricks/api_service/
+-rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5017 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/_auth.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1440 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/_auth_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2167 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/_base_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2876 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5195 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/api_service.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      312 2023-06-10 18:23:59.000000 autobricks-0.9.0/autobricks/api_service/autobricks_logging.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 18:24:22.519325 autobricks-0.9.0/autobricks.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-06-10 18:24:22.000000 autobricks-0.9.0/autobricks.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      746 2023-06-10 18:24:22.000000 autobricks-0.9.0/autobricks.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-10 18:24:22.000000 autobricks-0.9.0/autobricks.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-10 18:24:22.000000 autobricks-0.9.0/autobricks.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-06-10 18:24:22.000000 autobricks-0.9.0/autobricks.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-06-10 18:24:22.000000 autobricks-0.9.0/autobricks.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-10 18:24:22.523325 autobricks-0.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-06-10 18:23:59.000000 autobricks-0.9.0/setup.py
```

### Comparing `autobricks-0.8.0/PKG-INFO` & `autobricks-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.8.0
+Version: 0.9.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.8.0/README.md` & `autobricks-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/Cluster.py` & `autobricks-0.9.0/autobricks/Cluster.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/Dbfs.py` & `autobricks-0.9.0/autobricks/Dbfs.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/Job.py` & `autobricks-0.9.0/autobricks/Job.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,18 +194,15 @@
     except KeyError as e:
         raise Exception(f"Job definition doesn't have a {e}.")
 
     job_id = job_get_id(name)
 
     if job_id:
         _logger.info(f"updaing job {name} job_id={job_id}")
-        upd_job = {
-            "new_settings": job,
-            "job_id": job_id
-        }
+        upd_job = {"new_settings": job, "job_id": job_id}
         job_update(job=upd_job)
     else:
         _logger.info(f"creating new job {name}")
         job_create(job=job)
 
 
 def job_import_jobs(
```

### Comparing `autobricks-0.8.0/autobricks/Library.py` & `autobricks-0.9.0/autobricks/Library.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/SetupTools.py` & `autobricks-0.9.0/autobricks/SetupTools.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/Sql.py` & `autobricks-0.9.0/autobricks/Sql.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/Workspace.py` & `autobricks-0.9.0/autobricks/Workspace.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/_common.py` & `autobricks-0.9.0/autobricks/_common.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/_decode_utils.py` & `autobricks-0.9.0/autobricks/_decode_utils.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/api_service/_auth.py` & `autobricks-0.9.0/autobricks/api_service/_auth.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/api_service/_auth_factory.py` & `autobricks-0.9.0/autobricks/api_service/_auth_factory.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/api_service/_base_api.py` & `autobricks-0.9.0/autobricks/api_service/_base_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,37 @@
         msg = f"{e.response.status_code} error at {url} {e.response.text}"
         _logger.error(msg)
         raise e
 
     return response
 
 
+def base_api_put(
+    url: str, headers: dict, json: dict = None, data: dict = None, params=None
+):
+    response = requests.put(
+        url=url,
+        headers=headers,
+        json=json,
+        data=data,
+        verify=_ssl_verify,
+        params=params,
+    )
+
+    try:
+        response.raise_for_status()
+
+    except HTTPError as e:
+        msg = f"{e.response.status_code} error at {url} {e.response.text}"
+        _logger.error(msg)
+        raise e
+
+    return response
+
+
 def base_api_delete(
     url: str, headers: dict, json: dict = None, data: dict = None, params=None
 ):
     response = requests.delete(
         url=url,
         headers=headers,
         json=json,
```

### Comparing `autobricks-0.8.0/autobricks/api_service/_configuration.py` & `autobricks-0.9.0/autobricks/api_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/api_service/_exceptions.py` & `autobricks-0.9.0/autobricks/api_service/_exceptions.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.8.0/autobricks/api_service/api_service.py` & `autobricks-0.9.0/autobricks/api_service/api_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ._auth_factory import auth_factory, AuthenticationType
 from ._auth import Auth
 from ._base_api import (
     base_api_get as _base_api_get,
     base_api_post as _base_api_post,
     base_api_delete as _base_api_delete,
+    base_api_put as _base_api_put,
 )
 from . import autobricks_logging
 from ._exceptions import AutobricksConfigurationInvalid, AutobricksResponseJsonError
 from ._configuration import configuration
 import json
 
 _logger = autobricks_logging.get_logger(__name__)
@@ -64,28 +65,58 @@
         auth: Auth = auth_factory.get_auth(self.auth_type, _config)
 
         _logger.debug("Setting Authorisation Headers")
         self._headers = auth.get_headers()
         _header_json = json.dumps(self._headers, indent=4)
         _logger.debug(_header_json)
 
-    def api_get(
+    def api_put(
         self,
         api: str,
         function: str,
         data: dict = None,
         params=None,
         preview: bool = False,
         api_version=_API_VERSION,
     ):
         if preview:
             url = f"{self.host}/api/{api_version}/{_PREVIEW}/{api}/{function}"
         else:
             url = f"{self.host}/api/{api_version}/{api}/{function}"
 
+        response = _base_api_put(
+            url=url, headers=self._headers, json=data, params=params
+        )
+
+        try:
+            json = response.json()
+        except Exception:
+            ex = AutobricksResponseJsonError(url, "PUT", data, response.text)
+            _logger.error(ex.message)
+            raise ex
+
+        return json
+
+    def api_get(
+        self,
+        api: str,
+        function: str,
+        data: dict = None,
+        params=None,
+        preview: bool = False,
+        api_version=_API_VERSION,
+    ):
+        if preview:
+            url = f"{self.host}/api/{api_version}/{_PREVIEW}/{api}"
+        else:
+            url = f"{self.host}/api/{api_version}/{api}"
+
+        if function:
+            url = f"{url}/{function}"
+
         response = _base_api_get(
             url=url, headers=self._headers, json=data, params=params
         )
 
         try:
             json = response.json()
         except Exception:
@@ -127,17 +158,20 @@
         api: str,
         function: str,
         data: dict,
         preview: bool = False,
         api_version=_API_VERSION,
     ):
         if preview:
-            url = f"{self.host}/api/{api_version}/{_PREVIEW}/{api}/{function}"
+            url = f"{self.host}/api/{api_version}/{_PREVIEW}/{api}"
         else:
-            url = f"{self.host}/api/{api_version}/{api}/{function}"
+            url = f"{self.host}/api/{api_version}/{api}"
+
+        if function:
+            url = f"{url}/{function}"
 
         response = _base_api_post(url=url, headers=self._headers, json=data)
 
         try:
             json = response.json()
         except Exception:
             ex = AutobricksResponseJsonError(url, "POST", data, response.text)
```

### Comparing `autobricks-0.8.0/autobricks.egg-info/PKG-INFO` & `autobricks-0.9.0/autobricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.8.0
+Version: 0.9.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.8.0/autobricks.egg-info/SOURCES.txt` & `autobricks-0.9.0/autobricks.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 autobricks/Cluster.py
 autobricks/Dbfs.py
 autobricks/Job.py
 autobricks/Library.py
+autobricks/Pipeline.py
 autobricks/SetupTools.py
 autobricks/Sql.py
 autobricks/Workspace.py
 autobricks/_common.py
 autobricks/_decode_utils.py
 autobricks.egg-info/PKG-INFO
 autobricks.egg-info/SOURCES.txt
```

### Comparing `autobricks-0.8.0/setup.py` & `autobricks-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "PYPI.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="autobricks",
-    version="0.8.0",
+    version="0.9.0",
     description="Databricks Deployment Utils",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://autobricks.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/autobricks',
         'Documentation': 'https://autobricks.readthedocs.io/en/latest/'
```

