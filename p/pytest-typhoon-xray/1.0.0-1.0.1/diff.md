# Comparing `tmp/pytest-typhoon-xray-1.0.0.tar.gz` & `tmp/pytest-typhoon-xray-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-typhoon-xray-1.0.0.tar", last modified: Fri Jun  9 18:04:20 2023, max compression
+gzip compressed data, was "pytest-typhoon-xray-1.0.1.tar", last modified: Sat Jun 10 07:41:46 2023, max compression
```

## Comparing `pytest-typhoon-xray-1.0.0.tar` & `pytest-typhoon-xray-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-09 18:04:20.560589 pytest-typhoon-xray-1.0.0/
--rw-r--r--   0 branko     (501) staff       (20)     1068 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/LICENSE
--rw-r--r--   0 branko     (501) staff       (20)       97 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/MANIFEST.in
--rw-r--r--   0 branko     (501) staff       (20)     6895 2023-06-09 18:04:20.560483 pytest-typhoon-xray-1.0.0/PKG-INFO
--rw-r--r--   0 branko     (501) staff       (20)     5842 2022-02-14 12:03:51.000000 pytest-typhoon-xray-1.0.0/README.rst
-drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-09 18:04:20.559083 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/
--rw-r--r--   0 branko     (501) staff       (20)     6895 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/PKG-INFO
--rw-r--r--   0 branko     (501) staff       (20)      418 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/SOURCES.txt
--rw-r--r--   0 branko     (501) staff       (20)        1 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/dependency_links.txt
--rw-r--r--   0 branko     (501) staff       (20)       35 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/entry_points.txt
--rw-r--r--   0 branko     (501) staff       (20)       55 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/requires.txt
--rw-r--r--   0 branko     (501) staff       (20)        7 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/top_level.txt
--rw-r--r--   0 branko     (501) staff       (20)       38 2023-06-09 18:04:20.560625 pytest-typhoon-xray-1.0.0/setup.cfg
--rw-r--r--   0 branko     (501) staff       (20)     1607 2023-06-09 18:02:10.000000 pytest-typhoon-xray-1.0.0/setup.py
-drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-09 18:04:20.560154 pytest-typhoon-xray-1.0.0/tytest/
--rw-r--r--   0 branko     (501) staff       (20)        0 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/tytest/__init__.py
--rw-r--r--   0 branko     (501) staff       (20)      654 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/tytest/exceptions.py
--rw-r--r--   0 branko     (501) staff       (20)     6059 2022-06-23 09:21:58.000000 pytest-typhoon-xray-1.0.0/tytest/plugin.py
--rw-r--r--   0 branko     (501) staff       (20)      476 2022-02-14 11:39:31.000000 pytest-typhoon-xray-1.0.0/tytest/runtime_settings.py
--rw-r--r--   0 branko     (501) staff       (20)     1229 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/tytest/utils.py
--rw-r--r--   0 branko     (501) staff       (20)     3306 2023-06-09 18:00:12.000000 pytest-typhoon-xray-1.0.0/tytest/xray_api.py
+drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-10 07:41:46.292762 pytest-typhoon-xray-1.0.1/
+-rw-r--r--   0 branko     (501) staff       (20)     1068 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.1/LICENSE
+-rw-r--r--   0 branko     (501) staff       (20)       97 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.1/MANIFEST.in
+-rw-r--r--   0 branko     (501) staff       (20)     6895 2023-06-10 07:41:46.292647 pytest-typhoon-xray-1.0.1/PKG-INFO
+-rw-r--r--   0 branko     (501) staff       (20)     5842 2022-02-14 12:03:51.000000 pytest-typhoon-xray-1.0.1/README.rst
+drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-10 07:41:46.291206 pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/
+-rw-r--r--   0 branko     (501) staff       (20)     6895 2023-06-10 07:41:46.000000 pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/PKG-INFO
+-rw-r--r--   0 branko     (501) staff       (20)      418 2023-06-10 07:41:46.000000 pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 branko     (501) staff       (20)        1 2023-06-10 07:41:46.000000 pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 branko     (501) staff       (20)       35 2023-06-10 07:41:46.000000 pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/entry_points.txt
+-rw-r--r--   0 branko     (501) staff       (20)       55 2023-06-10 07:41:46.000000 pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/requires.txt
+-rw-r--r--   0 branko     (501) staff       (20)        7 2023-06-10 07:41:46.000000 pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/top_level.txt
+-rw-r--r--   0 branko     (501) staff       (20)       38 2023-06-10 07:41:46.292799 pytest-typhoon-xray-1.0.1/setup.cfg
+-rw-r--r--   0 branko     (501) staff       (20)     1607 2023-06-10 07:41:29.000000 pytest-typhoon-xray-1.0.1/setup.py
+drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-10 07:41:46.292455 pytest-typhoon-xray-1.0.1/tytest/
+-rw-r--r--   0 branko     (501) staff       (20)        0 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.1/tytest/__init__.py
+-rw-r--r--   0 branko     (501) staff       (20)      654 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.1/tytest/exceptions.py
+-rw-r--r--   0 branko     (501) staff       (20)     6059 2022-06-23 09:21:58.000000 pytest-typhoon-xray-1.0.1/tytest/plugin.py
+-rw-r--r--   0 branko     (501) staff       (20)      476 2022-02-14 11:39:31.000000 pytest-typhoon-xray-1.0.1/tytest/runtime_settings.py
+-rw-r--r--   0 branko     (501) staff       (20)     1229 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.1/tytest/utils.py
+-rw-r--r--   0 branko     (501) staff       (20)     3251 2023-06-10 07:39:11.000000 pytest-typhoon-xray-1.0.1/tytest/xray_api.py
```

### Comparing `pytest-typhoon-xray-1.0.0/LICENSE` & `pytest-typhoon-xray-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-1.0.0/PKG-INFO` & `pytest-typhoon-xray-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-typhoon-xray
-Version: 1.0.0
+Version: 1.0.1
 Summary: Typhoon HIL plugin for pytest
 Home-page: https://github.com/typhoon-hil/pytest-typhoon-xray
 Author: Branko Milosavljevic
 Author-email: branko@typhoon-hil.com
 Maintainer: Branko Milosavljevic
 Maintainer-email: branko@typhoon-hil.com
 License: MIT
```

### Comparing `pytest-typhoon-xray-1.0.0/README.rst` & `pytest-typhoon-xray-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/PKG-INFO` & `pytest-typhoon-xray-1.0.1/pytest_typhoon_xray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-typhoon-xray
-Version: 1.0.0
+Version: 1.0.1
 Summary: Typhoon HIL plugin for pytest
 Home-page: https://github.com/typhoon-hil/pytest-typhoon-xray
 Author: Branko Milosavljevic
 Author-email: branko@typhoon-hil.com
 Maintainer: Branko Milosavljevic
 Maintainer-email: branko@typhoon-hil.com
 License: MIT
```

### Comparing `pytest-typhoon-xray-1.0.0/setup.py` & `pytest-typhoon-xray-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-typhoon-xray',
-    version='1.0.0',
+    version='1.0.1',
     author='Branko Milosavljevic',
     author_email='branko@typhoon-hil.com',
     maintainer='Branko Milosavljevic',
     maintainer_email='branko@typhoon-hil.com',
     license='MIT',
     url='https://github.com/typhoon-hil/pytest-typhoon-xray',
     description='Typhoon HIL plugin for pytest',
```

### Comparing `pytest-typhoon-xray-1.0.0/tytest/exceptions.py` & `pytest-typhoon-xray-1.0.1/tytest/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-1.0.0/tytest/plugin.py` & `pytest-typhoon-xray-1.0.1/tytest/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-1.0.0/tytest/utils.py` & `pytest-typhoon-xray-1.0.1/tytest/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-1.0.0/tytest/xray_api.py` & `pytest-typhoon-xray-1.0.1/tytest/xray_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,35 +47,32 @@
         output = r.json()
         return output
     except JSONDecodeError as e:
         return None
 
 
 def add_remote_link(issue_id, remote_link, title,
-                    icon_url='https://qameta.io/allure-report/img/reportlogo.svg'):
+                    icon_url='https://images.opencollective.com/allure-report/a3f97da/logo/256.png'):
     req = {
         'object': {
             'url': remote_link,
             'title': title,
             'icon': {
                 'url16x16': icon_url,
                 'title': 'Report details'
             }
         }
     }
     if not Settings.XRAY_SERVER and not Settings.XRAY_PLAN_KEY:
         return None
     if Settings.XRAY_SERVER:
-        headers = {
-            'Authorization': f'Bearer {Settings.JIRA_TOKEN}',
-            'Content-type': 'application/json'
-        }
+        basic = HTTPBasicAuth(Settings.JIRA_USER, Settings.JIRA_TOKEN)
         r = requests.post(
             f'{Settings.JIRA_HOST}/rest/api/2/issue/{issue_id}/remotelink',
-            headers=headers, json=req)
+            auth=basic, json=req)
     else:
         r = requests.post(
             f'{Settings.JIRA_HOST}/rest/api/2/issue/{issue_id}/remotelink',
             auth=Settings.JIRA_AUTH, json=req)
     OK_CODES = range(200, 205)
     if r.status_code not in OK_CODES and not Settings.XRAY_FAIL_SILENTLY:
         raise JiraError
```

