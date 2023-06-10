# Comparing `tmp/prefai-0.0.3.tar.gz` & `tmp/prefai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefai-0.0.3.tar", last modified: Wed Jun  7 06:52:27 2023, max compression
+gzip compressed data, was "prefai-0.0.4.tar", last modified: Sat Jun 10 06:00:28 2023, max compression
```

## Comparing `prefai-0.0.3.tar` & `prefai-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.715684 prefai-0.0.3/
--rw-r--r--   0 bjaros     (501) staff       (20)     1079 2023-06-01 06:14:59.000000 prefai-0.0.3/LICENSE.txt
--rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-07 06:52:27.715519 prefai-0.0.3/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)     1238 2023-06-03 22:24:22.000000 prefai-0.0.3/README.md
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.714136 prefai-0.0.3/prefai/
--rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.3/prefai/__init__.py
--rw-r--r--   0 bjaros     (501) staff       (20)     5880 2023-06-07 06:48:49.000000 prefai-0.0.3/prefai/client.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.714983 prefai-0.0.3/prefai.egg-info/
--rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/SOURCES.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/dependency_links.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/top_level.txt
--rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-06-07 06:52:27.715734 prefai-0.0.3/setup.cfg
--rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-06-07 06:50:21.000000 prefai-0.0.3/setup.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.715122 prefai-0.0.3/tests/
--rw-r--r--   0 bjaros     (501) staff       (20)     3204 2023-06-03 22:24:22.000000 prefai-0.0.3/tests/test_client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.962169 prefai-0.0.4/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1079 2023-06-01 06:14:59.000000 prefai-0.0.4/LICENSE.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-10 06:00:28.962021 prefai-0.0.4/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)     1238 2023-06-03 22:24:22.000000 prefai-0.0.4/README.md
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.960837 prefai-0.0.4/prefai/
+-rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.4/prefai/__init__.py
+-rw-r--r--   0 bjaros     (501) staff       (20)     5863 2023-06-10 05:52:41.000000 prefai-0.0.4/prefai/client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.961549 prefai-0.0.4/prefai.egg-info/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/SOURCES.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/dependency_links.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/top_level.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-06-10 06:00:28.962214 prefai-0.0.4/setup.cfg
+-rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-06-10 05:13:24.000000 prefai-0.0.4/setup.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.961662 prefai-0.0.4/tests/
+-rw-r--r--   0 bjaros     (501) staff       (20)     3665 2023-06-09 23:46:47.000000 prefai-0.0.4/tests/test_client.py
```

### Comparing `prefai-0.0.3/LICENSE.txt` & `prefai-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prefai-0.0.3/PKG-INFO` & `prefai-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prefai-0.0.3/README.md` & `prefai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `prefai-0.0.3/prefai/client.py` & `prefai-0.0.4/prefai/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             response_content = response.content.decode()
             if response_content:
                 response_dict = json.loads(response_content)
                 if 'detail' in response_dict:
                     raise PrefaiError(f"Request failed: {http_err}. Reason: {response_dict['detail']}")
             raise PrefaiError(f"Request failed: {http_err}")
 
-    def retrieve_prompt(self,
+    def pref_prompt(self,
         user_action: str,
         context: Optional[str] = None,
         user_email: Optional[str] = None,
         user_id: Optional[str] = None,
         max_tokens: Optional[int] = 300,
         min_similarity: Optional[float] = None,
     ) -> Dict:
@@ -150,15 +150,15 @@
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
 
         try:
             response = requests.post(
-                f"{self._api_base_url}/v1/records/retrieve-prompt",
+                f"{self._api_base_url}/v1/prompt/new",
                 json={
                     "context": context,
                     "user_action": user_action,
                     "user_email": user_email,
                     "user_id": user_id,
                     "max_tokens": max_tokens,
                     "min_similarity": min_similarity,
```

### Comparing `prefai-0.0.3/prefai.egg-info/PKG-INFO` & `prefai-0.0.4/prefai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prefai-0.0.3/setup.py` & `prefai-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="prefai",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     author="Bobby Jaros",
     author_email="bobby@pref.ai",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="http://github.com/prefai/pythonclient",
```

### Comparing `prefai-0.0.3/tests/test_client.py` & `prefai-0.0.4/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,7 +96,21 @@
         user_action = "How do you say I love you in Spanish?",
         min_similarity = -1.0
     )
     assert res.get('success')
     assert res['records'][0]['user_action'].startswith('Is that a casual way to ask?')
     print(res['records'])
 
+def test_pref_prompt():
+    res = prefai_client.pref_prompt(
+        user_email = test_user_email,
+        context = "User: Hola.\nAI: Hola!",
+        user_action = "How do you say I love you in Spanish?",
+        min_similarity = -1.0
+    )
+    assert res.get('success')
+    return res
+    # assert res['records'][0]['user_action'].startswith('Is that a casual way to ask?')
+    # print(res['records'])
+
+if __name__ == "__main__":
+    res = test_pref_prompt()
```

