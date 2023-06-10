# Comparing `tmp/nonebot-plugin-pcrjjc-0.1.1.tar.gz` & `tmp/nonebot-plugin-pcrjjc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-pcrjjc-0.1.1.tar", last modified: Sat Jun 10 10:50:59 2023, max compression
+gzip compressed data, was "nonebot-plugin-pcrjjc-0.1.2.tar", last modified: Sat Jun 10 12:32:44 2023, max compression
```

## Comparing `nonebot-plugin-pcrjjc-0.1.1.tar` & `nonebot-plugin-pcrjjc-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 10:50:59.816019 nonebot-plugin-pcrjjc-0.1.1/
--rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2699 2023-06-10 10:50:59.759016 nonebot-plugin-pcrjjc-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-06-10 08:28:10.000000 nonebot-plugin-pcrjjc-0.1.1/README.md
--rw-rw-rw-   0        0        0     1597 2023-06-10 10:50:35.000000 nonebot-plugin-pcrjjc-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 10:50:59.817019 nonebot-plugin-pcrjjc-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 10:50:59.467423 nonebot-plugin-pcrjjc-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 10:50:59.471423 nonebot-plugin-pcrjjc-0.1.1/src/plugins/
-drwxrwxrwx   0        0        0        0 2023-06-10 10:50:59.707019 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/
--rw-rw-rw-   0        0        0    38805 2023-06-09 13:05:16.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/aiorequests.py
--rw-rw-rw-   0        0        0     6481 2023-06-09 05:09:18.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-rw-rw-   0        0        0      806 2023-06-10 04:58:52.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/config.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:50:59.724015 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/fonts/
--rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
--rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/pcrclient.py
--rw-rw-rw-   0        0        0     7610 2023-06-10 05:02:01.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/query.py
--rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/rsacr.py
--rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/text2img.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:50:59.521299 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/
--rw-rw-rw-   0        0        0     2699 2023-06-10 10:50:59.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2023-06-10 10:50:59.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 10:50:59.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-10 10:50:59.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-10 10:50:59.000000 nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 12:32:44.076891 nonebot-plugin-pcrjjc-0.1.2/
+-rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2699 2023-06-10 12:32:44.075889 nonebot-plugin-pcrjjc-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1835 2023-06-10 08:28:10.000000 nonebot-plugin-pcrjjc-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1597 2023-06-10 12:23:13.000000 nonebot-plugin-pcrjjc-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 12:32:44.076891 nonebot-plugin-pcrjjc-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 12:32:43.794500 nonebot-plugin-pcrjjc-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 12:32:43.816512 nonebot-plugin-pcrjjc-0.1.2/src/plugins/
+drwxrwxrwx   0        0        0        0 2023-06-10 12:32:43.940036 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/
+-rw-rw-rw-   0        0        0    38840 2023-06-10 12:27:03.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-rw-rw-   0        0        0     6481 2023-06-09 05:09:18.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-rw-rw-   0        0        0      806 2023-06-10 12:25:03.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/config.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:32:43.964040 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/fonts/
+-rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
+-rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-rw-rw-   0        0        0     7646 2023-06-10 12:26:23.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/query.py
+-rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/rsacr.py
+-rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/text2img.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:32:43.871808 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/
+-rw-rw-rw-   0        0        0     2699 2023-06-10 12:32:43.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2023-06-10 12:32:43.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 12:32:43.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-10 12:32:43.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-10 12:32:43.000000 nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-pcrjjc-0.1.1/LICENSE` & `nonebot-plugin-pcrjjc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/PKG-INFO` & `nonebot-plugin-pcrjjc-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.1
+Version: 0.1.2
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot-plugin-pcrjjc-0.1.1/README.md` & `nonebot-plugin-pcrjjc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/pyproject.toml` & `nonebot-plugin-pcrjjc-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
```

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/__init__.py` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,16 @@
 4）pcrjjc关闭排名上升
 '''
 
 # 数据库对象初始化
 # JJCH = JJCHistoryStorage()
 friend_list = []
 pcrid_list = []
-admin = int(config.superusers[0])
+if len(config.superusers) > 0:
+    admin = int(config.superusers[0])
 config = join(path, 'binds.json')
 root = {'arena_bind': {}}
 if exists(config):
     with open(config) as fp:
         root = load(fp)
 lck = Lock()
 lck_friend_list = Lock()
```

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/config.py` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/query.py` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 otto = config.otto
 ordd = 'x'
 validate = None
 validating = False
 ac_first = False
 client = None
 captcha_cnt = 0
-admin = int(config.superusers[0])
+if len(config.superusers) > 0:
+    admin = int(config.superusers[0])
 data_path = config.data_path
 path = join(str(Path()), data_path)
 ac_info = []
 binds_info = {}
 account_json_template = [
     {
         "account": "account1",
```

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc/text2img.py` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.1
+Version: 0.1.2
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot-plugin-pcrjjc-0.1.1/src/plugins/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot-plugin-pcrjjc-0.1.2/src/plugins/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

