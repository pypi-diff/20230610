# Comparing `tmp/synmax_api_python_client-0.0b8-py3-none-any.whl.zip` & `tmp/synmax_api_python_client-0.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6087 bytes, number of entries: 13
+Zip file size: 6204 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-25 10:28 synmax/__init__.py
 -rw-rw-rw-  2.0 fat       90 b- defN 22-Jun-26 04:17 synmax/common/__init__.py
--rw-rw-rw-  2.0 fat     3753 b- defN 22-Jun-30 23:45 synmax/common/api_client.py
+-rw-rw-rw-  2.0 fat     3819 b- defN 22-Jul-13 10:46 synmax/common/api_client.py
 -rw-rw-rw-  2.0 fat      330 b- defN 22-Jun-29 19:33 synmax/common/model.py
 -rw-rw-rw-  2.0 fat       60 b- defN 22-Jun-25 12:00 synmax/hyperion/__init__.py
 -rw-rw-rw-  2.0 fat     2361 b- defN 22-Jun-29 19:45 synmax/hyperion/hyperion_client.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-25 10:34 synmax/theia/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-25 11:38 test/__init__.py
--rw-rw-rw-  2.0 fat      523 b- defN 22-Jun-29 19:57 test/hyperion_test.py
--rw-rw-rw-  2.0 fat     3204 b- defN 22-Jun-30 23:45 synmax_api_python_client-0.0b8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jun-30 23:45 synmax_api_python_client-0.0b8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 22-Jun-30 23:45 synmax_api_python_client-0.0b8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1078 b- defN 22-Jun-30 23:45 synmax_api_python_client-0.0b8.dist-info/RECORD
-13 files, 11503 bytes uncompressed, 4257 bytes compressed:  63.0%
+-rw-rw-rw-  2.0 fat     1175 b- defN 22-Jul-11 18:54 test/hyperion_test.py
+-rw-rw-rw-  2.0 fat     3204 b- defN 22-Jul-13 10:48 synmax_api_python_client-0.0b9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Jul-13 10:48 synmax_api_python_client-0.0b9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 22-Jul-13 10:48 synmax_api_python_client-0.0b9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1079 b- defN 22-Jul-13 10:48 synmax_api_python_client-0.0b9.dist-info/RECORD
+13 files, 12222 bytes uncompressed, 4374 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/hyperion_test.py
 Comment: 
 
-Filename: synmax_api_python_client-0.0b8.dist-info/METADATA
+Filename: synmax_api_python_client-0.0b9.dist-info/METADATA
 Comment: 
 
-Filename: synmax_api_python_client-0.0b8.dist-info/WHEEL
+Filename: synmax_api_python_client-0.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: synmax_api_python_client-0.0b8.dist-info/top_level.txt
+Filename: synmax_api_python_client-0.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: synmax_api_python_client-0.0b8.dist-info/RECORD
+Filename: synmax_api_python_client-0.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synmax/common/api_client.py

```diff
@@ -5,14 +5,16 @@
 import requests
 from tqdm import tqdm
 
 from synmax.common.model import PayloadModelBase
 
 LOGGER = logging.getLogger(__name__)
 
+_api_timeout = 300
+
 
 class ApiClient:
     def __init__(self, access_token):
         self.access_key = access_token
         self.session = requests.Session()
         # update headers
         self.session.headers.update(self.headers)
@@ -51,15 +53,15 @@
             in the query string for the :class:`Request`.
         :param return_json:
         :param \*\*kwargs: Optional arguments that ``request`` takes.
         :return: :class:`Response <Response>` object
         :rtype: requests.Response
         """
         LOGGER.info(url)
-        response = self.session.get(url, params=params, **kwargs)
+        response = self.session.get(url, params=params, timeout=_api_timeout, **kwargs)
         json_result = self._return_response(response, return_json)
         df = pandas.DataFrame(json_result['data'])
         return df
 
     def post(self, url, payload: PayloadModelBase = None, return_json=False, **kwargs) -> pandas.DataFrame:
         r"""Sends a POST request.
 
@@ -76,15 +78,15 @@
 
         data_list: List[Dict] = []
         total_count = 1
 
         with tqdm(desc=F"Querying API {url} pages", total=total_count, dynamic_ncols=True, miniters=0) as progress_bar:
             while True:
                 progress_bar.refresh()
-                response = self.session.post(url, data=payload.payload(), **kwargs)
+                response = self.session.post(url, data=payload.payload(), timeout=_api_timeout, **kwargs)
                 json_result = self._return_response(response, return_json)
                 pagination = json_result['pagination']
                 data_list.extend(json_result['data'])
                 progress_bar.update()
 
                 if not payload.fetch_all or pagination['total_count'] <= pagination['start'] + pagination['page_size']:
                     break
```

## test/hyperion_test.py

```diff
@@ -15,14 +15,34 @@
 def well_completion():
     payload = ApiPayload(start_date='2021-01-1', end_date='2022-06-25', state_code='TX')
 
     result_df = client.wells()
     print(result_df.count())
 
 
+def test_ducs_by_operator():
+    payload = ApiPayload(start_date='2021-01-01', end_date='2021-12-31')
+
+    result_df = client.ducs_by_operator(payload)
+    print(result_df.count())
+
+
+def test_production_by_county_and_operator():
+    payload = ApiPayload(start_date='2018-01-01', end_date='2018-12-31')
+    result_df = client.production_by_county_and_operator(payload)
+    print(result_df.count())
+
+
+def test_production_by_well():
+    payload = ApiPayload(start_date='2016-01-01', end_date='2016-12-31')
+    result_df = client.production_by_well(payload)
+    print(result_df.count())
+
+
 def main():
     # fetch_region()
-    well_completion()
+    # well_completion()
+    test_production_by_county_and_operator()
 
 
 if __name__ == '__main__':
     main()
```

## Comparing `synmax_api_python_client-0.0b8.dist-info/METADATA` & `synmax_api_python_client-0.0b9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synmax-api-python-client
-Version: 0.0b8
+Version: 0.0b9
 Summary: Synmax API client
 Home-page: https://github.com/SynMaxDev/synmax-api-python-client.git
 Author: Eric Anderson and Deepa Aswathaiah
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `synmax_api_python_client-0.0b8.dist-info/RECORD` & `synmax_api_python_client-0.0b9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 synmax/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 synmax/common/__init__.py,sha256=KIMT-JysXOyBM6ytUjm-omlHeWc8l5pm_CFvktACSl0,90
-synmax/common/api_client.py,sha256=v5CMj4cjndT1E6q6HW2moTJbwKC5WIR5PFfjOQCRt7w,3753
+synmax/common/api_client.py,sha256=39HeXAOHRQtNjdtc1dwNFsDmkpGj6cFF36MXkWl-zE8,3819
 synmax/common/model.py,sha256=UYPHnII-HgHbI7Q-B48rU7ZOu40q-LWmF4Od8J2suCQ,330
 synmax/hyperion/__init__.py,sha256=MCWhYXHyQDrcCJXi2qolp8Dn7qP-1sUX2axlReRAJE8,60
 synmax/hyperion/hyperion_client.py,sha256=kHpbr33TWx2t3eH1N1rtJzkMkpIia_V7sZOe3zfyRUE,2361
 synmax/theia/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test/hyperion_test.py,sha256=zbmqe7UvJ3_lIB164MvyoyFmQIZmLh8VTMhdePudXfM,523
-synmax_api_python_client-0.0b8.dist-info/METADATA,sha256=h-YSMy6M663DcSv8NKl0ejGNhkVCSm1RtrStDd4vZ4I,3204
-synmax_api_python_client-0.0b8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-synmax_api_python_client-0.0b8.dist-info/top_level.txt,sha256=ZuSgW0z_OuhlSQYBWIcFIw2-K0v_RlDWa6_oP_wq2qI,12
-synmax_api_python_client-0.0b8.dist-info/RECORD,,
+test/hyperion_test.py,sha256=nbKbxcDL1L1aypmXuwMI9CEuI1OfZsj2U1L5m64RjVM,1175
+synmax_api_python_client-0.0b9.dist-info/METADATA,sha256=m50COcvRRg-yKfbqNAXJcSefS0o1QCkcfsKE1AA0vZA,3204
+synmax_api_python_client-0.0b9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+synmax_api_python_client-0.0b9.dist-info/top_level.txt,sha256=ZuSgW0z_OuhlSQYBWIcFIw2-K0v_RlDWa6_oP_wq2qI,12
+synmax_api_python_client-0.0b9.dist-info/RECORD,,
```

