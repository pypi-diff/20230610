# Comparing `tmp/liteclashproman-0.1.3.tar.gz` & `tmp/liteclashproman-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteclashproman-0.1.3.tar", last modified: Tue Jun  6 17:50:24 2023, max compression
+gzip compressed data, was "liteclashproman-0.1.4.tar", last modified: Sat Jun 10 05:08:44 2023, max compression
```

## Comparing `liteclashproman-0.1.3.tar` & `liteclashproman-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LICENSE
--rw-r--r--   0        0        0     1177 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/__init__.py
--rw-r--r--   0        0        0     3565 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/config.py
--rw-r--r--   0        0        0     1782 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/log.py
--rw-r--r--   0        0        0     1936 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/main.py
--rw-r--r--   0        0        0     2008 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/proxy.py
--rw-r--r--   0        0        0      379 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/proxygroup.py
--rw-r--r--   0        0        0      166 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/ruleprovider.py
--rw-r--r--   0        0        0     3637 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/static/config.exp.yaml
--rw-r--r--   0        0        0     3508 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/static/template/blacklist.yaml
--rw-r--r--   0        0        0     2607 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/static/template/whitelist.yaml
--rw-r--r--   0        0        0     2226 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/base64.py
--rw-r--r--   0        0        0      774 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/clash.py
--rw-r--r--   0        0        0     1224 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/jms.py
--rw-r--r--   0        0        0     1789 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/utils.py
--rw-r--r--   0        0        0     3222 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/README.md
--rw-r--r--   0        0        0      595 2023-06-06 17:50:24.673786 liteclashproman-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 liteclashproman-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1177 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/__init__.py
+-rw-r--r--   0        0        0     3565 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/config.py
+-rw-r--r--   0        0        0     1782 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/log.py
+-rw-r--r--   0        0        0     1936 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/main.py
+-rw-r--r--   0        0        0     2008 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/proxy.py
+-rw-r--r--   0        0        0      379 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/proxygroup.py
+-rw-r--r--   0        0        0      166 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/ruleprovider.py
+-rw-r--r--   0        0        0     3637 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/static/config.exp.yaml
+-rw-r--r--   0        0        0     3508 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/static/template/blacklist.yaml
+-rw-r--r--   0        0        0     2607 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/static/template/whitelist.yaml
+-rw-r--r--   0        0        0     2226 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/base64.py
+-rw-r--r--   0        0        0      774 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/clash.py
+-rw-r--r--   0        0        0     1530 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/jms.py
+-rw-r--r--   0        0        0     1789 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/utils.py
+-rw-r--r--   0        0        0     3222 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/README.md
+-rw-r--r--   0        0        0      595 2023-06-10 05:08:44.387228 liteclashproman-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 liteclashproman-0.1.4/PKG-INFO
```

### Comparing `liteclashproman-0.1.3/LICENSE` & `liteclashproman-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/__init__.py` & `liteclashproman-0.1.4/LiteClashProMan/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/config.py` & `liteclashproman-0.1.4/LiteClashProMan/config.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/log.py` & `liteclashproman-0.1.4/LiteClashProMan/log.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/main.py` & `liteclashproman-0.1.4/LiteClashProMan/main.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/model/clash/__init__.py` & `liteclashproman-0.1.4/LiteClashProMan/model/clash/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/model/clash/proxy.py` & `liteclashproman-0.1.4/LiteClashProMan/model/clash/proxy.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/static/config.exp.yaml` & `liteclashproman-0.1.4/LiteClashProMan/static/config.exp.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/static/template/blacklist.yaml` & `liteclashproman-0.1.4/LiteClashProMan/static/template/blacklist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/static/template/whitelist.yaml` & `liteclashproman-0.1.4/LiteClashProMan/static/template/whitelist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/subscribe/__init__.py` & `liteclashproman-0.1.4/LiteClashProMan/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/subscribe/base64.py` & `liteclashproman-0.1.4/LiteClashProMan/subscribe/base64.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/subscribe/clash.py` & `liteclashproman-0.1.4/LiteClashProMan/subscribe/clash.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/LiteClashProMan/subscribe/jms.py` & `liteclashproman-0.1.4/LiteClashProMan/subscribe/jms.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,30 +7,39 @@
 
 from ..model.clash import SS, Vmess
 from ..utils import Download
 from .base64 import ss, vmess
 
 
 async def counter(url, tz: Optional[str] = None):
+    tz = timezone(tz) if tz else None
     info = json.loads(await Download.content(url))
     download_ = info["bw_counter_b"]
     total = info["monthly_bw_limit_b"]
-    timenow = datetime.now()
-    if timenow.month == 12:
-        month = 1
-        year = timenow.year + 1
+    expire_time = datetime.now(tz)
+
+    if expire_time.day >= info["bw_reset_day_of_month"]:
+        # If today's date passes reset_day_of_month
+        # the next month should be taken
+        if expire_time.month == 12:
+            year = expire_time.year + 1
+            month = expire_time.month = 1
+        else:
+            year = expire_time.year
+            month = expire_time.month + 1
     else:
-        month = timenow.month + 1
-        year = timenow.year
+        year = expire_time.year
+        month = expire_time.month
+
     expire = int(
         datetime(
             year=year,
             month=month,
             day=info["bw_reset_day_of_month"],
-            tzinfo=timezone(tz) if tz else None,
+            tzinfo=tz,
         ).timestamp()
     )
 
     return f"upload=0; download={download_}; total={total}; expire={expire}"
 
 
 async def get(url: str) -> List[Union[SS, Vmess]]:
```

### Comparing `liteclashproman-0.1.3/LiteClashProMan/utils.py` & `liteclashproman-0.1.4/LiteClashProMan/utils.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/README.md` & `liteclashproman-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.3/pyproject.toml` & `liteclashproman-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LiteClashProMan"
-version = "0.1.3"
+version = "0.1.4"
 description = "生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。"
 authors = [
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "pyyaml>=6.0",
     "fastapi[all]>=0.96.0",
```

### Comparing `liteclashproman-0.1.3/PKG-INFO` & `liteclashproman-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteclashproman
-Version: 0.1.3
+Version: 0.1.4
 Summary: 生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。
 Author-Email: Well404 <well_404@outlook.com>
 License: APGL-3.0
 Requires-Python: >=3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fastapi[all]>=0.96.0
 Requires-Dist: httpx>=0.24.1
```

