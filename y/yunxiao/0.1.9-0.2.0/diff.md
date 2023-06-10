# Comparing `tmp/yunxiao-0.1.9.tar.gz` & `tmp/yunxiao-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.1.9.tar", last modified: Sat Jun 10 02:56:51 2023, max compression
+gzip compressed data, was "yunxiao-0.2.0.tar", last modified: Sat Jun 10 06:17:16 2023, max compression
```

## Comparing `yunxiao-0.1.9.tar` & `yunxiao-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 02:56:51.312584 yunxiao-0.1.9/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.9/LICENSE
--rw-rw-rw-   0        0        0    14308 2023-06-10 02:56:51.312584 yunxiao-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.1.9/README.md
--rw-rw-rw-   0        0        0      882 2023-06-10 02:03:21.000000 yunxiao-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 02:56:51.312584 yunxiao-0.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 02:56:51.306036 yunxiao-0.1.9/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.9/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21350 2023-06-10 02:31:52.000000 yunxiao-0.1.9/yunxiao/app.py
--rw-rw-rw-   0        0        0    10138 2023-06-10 02:37:03.000000 yunxiao-0.1.9/yunxiao/web.py
--rw-rw-rw-   0        0        0     4077 2023-06-10 01:55:31.000000 yunxiao-0.1.9/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:56:51.311578 yunxiao-0.1.9/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    14308 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 06:17:16.407701 yunxiao-0.2.0/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    14308 2023-06-10 06:17:16.407701 yunxiao-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.2.0/README.md
+-rw-rw-rw-   0        0        0      905 2023-06-10 06:16:55.000000 yunxiao-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 06:17:16.407701 yunxiao-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 06:17:16.385879 yunxiao-0.2.0/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.0/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21418 2023-06-10 04:23:34.000000 yunxiao-0.2.0/yunxiao/app.py
+-rw-rw-rw-   0        0        0    10205 2023-06-10 06:16:21.000000 yunxiao-0.2.0/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-10 06:16:21.000000 yunxiao-0.2.0/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-10 06:17:16.406688 yunxiao-0.2.0/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    14308 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.1.9/LICENSE` & `yunxiao-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.9/PKG-INFO` & `yunxiao-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.9
+Version: 0.2.0
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.1.9/README.md` & `yunxiao-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.9/pyproject.toml` & `yunxiao-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.1.9"
+version = "0.2.0"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,8 +22,9 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.2.0" = "BUG修复"
 "0.1.9" = "更改鉴权方式，保存鉴权到系统环境变量。当因鉴权失效导致请求失败时，自动更新鉴权并重新发起请求。意图减少更新鉴权的次数。"
```

### Comparing `yunxiao-0.1.9/yunxiao/app.py` & `yunxiao-0.2.0/yunxiao/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import logging
-import os
 from .yunxiao import YunXiao, UsedTime
 import requests
 
 
 class App(YunXiao):
-    def __init__(self, userphone: str, password: str, campus: list = None):
+    def __init__(self, configfile: str = "yunxiao_config.ini", campus: list = None):
         """
         初始化，输入用户账号密码，以及要操作的校区。
-        :param userphone: 账号
-        :param password: 密码
         :param campus: 校区
         """
-        super().__init__(userphone, password)
+        super().__init__(configfile)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
 
         self.reportpath = "https://yunxiao.xiaogj.com/api/cs-report/report/"
         self.orderpath = "https://yunxiao.xiaogj.com/api/cs-edu/order"
@@ -25,30 +22,30 @@
 
     def request(self, **kwargs):
         response = requests.request(
             method=kwargs.get("method"),
             url=kwargs.get("url"),
             json=kwargs.get("json"),
             params=kwargs.get("params"),
-            headers={"x3-authentication": os.environ.get("YUNXIAO_OAUTH_TOKEN")}
+            headers={"x3-authentication": self.token}
         )
 
         if response.status_code != 200:
             logging.error("无法到连接云校服务器。")
             return "无法到连接云校服务器。"
 
         if response.json()["code"] == 401:
             logging.error(response.json()["msg"])
             self.renew_token()
             response = requests.request(
                 method=kwargs.get("method"),
                 url=kwargs.get("url"),
                 json=kwargs.get("json"),
                 params=kwargs.get("params"),
-                headers={"x3-authentication": os.environ.get("YUNXIAO_OAUTH_TOKEN")}
+                headers={"x3-authentication": self.token}
             )
 
         return response.json()
 
     def find_now_data_report(self):
         """
         [数据/当前数据]
@@ -684,7 +681,13 @@
                 "_t_": UsedTime.stamp,
                 "queryKey": querykey,
                 "campusIds": self.campus,
                 "statusList": [1],
                 "page": {"pageNum": 1, "pageSize": 1000}
             }
         )
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level="INFO")
+    app = App("18050019727", "jm123456", [])
+    app.find_student_course_fee(status=[1]).get("data").get("cardCourseTradedList")
```

### Comparing `yunxiao-0.1.9/yunxiao/web.py` & `yunxiao-0.2.0/yunxiao/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import logging
-import os
-
 import requests
-
 from .yunxiao import YunXiao, UsedTime
 
 
 class Web(YunXiao):
-    def __init__(self, userphone: str, password: str, campus: list = None):
-        super().__init__(userphone, password)
+    def __init__(self, configfile: str = "yunxiao_config.ini", campus: list = None):
+        """
+        初始化，输入用户账号密码，以及要操作的校区。
+        :param campus: 校区
+        """
+        super().__init__(configfile)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
+
         self.reportpath = "https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/"
         self.edupath = "https://yunxiao.xiaogj.com/api/cs-pc-edu/"
 
     def request(self, **kwargs):
         response = requests.request(
             method=kwargs.get("method"),
             url=kwargs.get("url"),
             json=kwargs.get("json"),
             params=kwargs.get("params"),
-            headers={"Cookie": os.environ.get("YUNXIAO_OAUTH_COOKIE")}
+            headers={"Cookie": self.cookie}
         )
 
         if response.status_code != 200:
             logging.error("无法到连接云校服务器。")
             return "无法到连接云校服务器。"
 
         if response.json()["code"] == 401:
             logging.error(response.json()["msg"])
-            self.renew_token()
+            self.renew_cookie()
             response = requests.request(
                 method=kwargs.get("method"),
                 url=kwargs.get("url"),
                 json=kwargs.get("json"),
                 params=kwargs.get("params"),
-                headers={"Cookie": os.environ.get("YUNXIAO_OAUTH_COOKIE")}
+                headers={"Cookie": self.cookie}
             )
 
         return response.json()
 
     def find_course_sign_charge(
             self,
             starttime: str = None,
```

### Comparing `yunxiao-0.1.9/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.0/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.9
+Version: 0.2.0
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

