# Comparing `tmp/nonebot_plugin_wol-1.0.3.tar.gz` & `tmp/nonebot_plugin_wol-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wol-1.0.3.tar", last modified: Sat Jun 10 01:42:13 2023, max compression
+gzip compressed data, was "nonebot_plugin_wol-1.0.4.tar", last modified: Sat Jun 10 02:03:37 2023, max compression
```

## Comparing `nonebot_plugin_wol-1.0.3.tar` & `nonebot_plugin_wol-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.682581 nonebot_plugin_wol-1.0.3/
--rw-rw-rw-   0        0        0    18429 2023-06-10 01:16:24.000000 nonebot_plugin_wol-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      675 2023-06-10 01:42:13.682581 nonebot_plugin_wol-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      114 2023-06-10 01:14:55.000000 nonebot_plugin_wol-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.676119 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/
--rw-rw-rw-   0        0        0     5675 2023-06-10 00:13:14.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/__init__.py
--rw-rw-rw-   0        0        0      175 2023-06-10 00:12:40.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/config.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.681528 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/img/
--rw-rw-rw-   0        0        0    21704 2023-06-10 00:15:22.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/img/help.png
-drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.681528 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/tools/
--rw-rw-rw-   0        0        0     2082 2023-06-10 00:12:40.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/tools/wol.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:42:13.680427 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/
--rw-rw-rw-   0        0        0      675 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-10 01:42:13.000000 nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      555 2023-06-10 01:42:02.000000 nonebot_plugin_wol-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 01:42:13.682581 nonebot_plugin_wol-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1139 2023-06-10 01:41:18.000000 nonebot_plugin_wol-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:37.228486 nonebot_plugin_wol-1.0.4/
+-rw-rw-rw-   0        0        0    18429 2023-06-10 01:16:24.000000 nonebot_plugin_wol-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-06-10 02:03:37.227482 nonebot_plugin_wol-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-06-10 01:14:55.000000 nonebot_plugin_wol-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:37.214448 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/
+-rw-rw-rw-   0        0        0     5802 2023-06-10 01:59:19.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-06-10 00:12:40.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/config.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:37.223547 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/img/
+-rw-rw-rw-   0        0        0    21704 2023-06-10 00:15:22.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/img/help.png
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:37.224909 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/tools/
+-rw-rw-rw-   0        0        0     2082 2023-06-10 00:12:40.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/tools/wol.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:37.223547 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-06-10 02:03:36.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-10 02:03:36.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 02:03:36.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-10 02:03:36.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-10 02:03:36.000000 nonebot_plugin_wol-1.0.4/nonebot_plugin_wol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2023-06-10 02:03:22.000000 nonebot_plugin_wol-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 02:03:37.228486 nonebot_plugin_wol-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-06-10 02:03:17.000000 nonebot_plugin_wol-1.0.4/setup.py
```

### Comparing `nonebot_plugin_wol-1.0.3/LICENSE` & `nonebot_plugin_wol-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wol-1.0.3/PKG-INFO` & `nonebot_plugin_wol-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_wol
-Version: 1.0.3
+Version: 1.0.4
 Summary: A WOL Nonebot plugin
 Home-page: https://github.com/twoonefour/nonebot_plugin_wol.git
 Author: TwoOnefour
 Author-email: TwoOnefour <lys214412@gmail.com>
 License: LICENSE
 Project-URL: Homepage, https://github.com/twoonefour/nonebot_plugin_wol
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/__init__.py` & `nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,18 @@
             await check_status.finish("在线")
 
 check_config = on_command("查看配置", aliases={"config"}, permission=SUPERUSER, priority=20)
 @check_config.handle()
 async def check_config_handler(event: Union[PrivateMessageEvent, GroupMessageEvent], args: Message = CommandArg()):
     if isinstance(event, PrivateMessageEvent):
         with open(f"{wol_path}/data/data.yaml", "r") as f:
-            await check_config.finish(f.read())
+            config_msg = f.read()
+            if config_msg.strip(" ") == "":
+                config_msg = "暂无配置"
+            await check_config.finish(config_msg)
 
 show_help = on_command("wolhelp", permission=SUPERUSER, priority=20)
 @show_help.handle()
 async def show_help_handler(event: Union[PrivateMessageEvent, GroupMessageEvent], args: Message = CommandArg()):
     if isinstance(event, PrivateMessageEvent):
         await check_config.finish("唤醒\n·/wol ip mac 为直接唤醒\n·/wol 名称\t使用配置名称唤醒\n\n添加配置\n·/wol添加 名称 ip mac\n\nping\n·/ping ip\n\n查看帮助\n·/wolhelp\n\n查看当前配置名称\n·/config")
```

### Comparing `nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/img/help.png` & `nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/img/help.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wol-1.0.3/nonebot_plugin_wol/tools/wol.py` & `nonebot_plugin_wol-1.0.4/nonebot_plugin_wol/tools/wol.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wol-1.0.3/nonebot_plugin_wol.egg-info/PKG-INFO` & `nonebot_plugin_wol-1.0.4/nonebot_plugin_wol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-wol
-Version: 1.0.3
+Version: 1.0.4
 Summary: A WOL Nonebot plugin
 Home-page: https://github.com/twoonefour/nonebot_plugin_wol.git
 Author: TwoOnefour
 Author-email: TwoOnefour <lys214412@gmail.com>
 License: LICENSE
 Project-URL: Homepage, https://github.com/twoonefour/nonebot_plugin_wol
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot_plugin_wol-1.0.3/pyproject.toml` & `nonebot_plugin_wol-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot_plugin_wol"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="TwoOnefour", email="lys214412@gmail.com"},
 ]
 description = "A WOL Nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `nonebot_plugin_wol-1.0.3/setup.py` & `nonebot_plugin_wol-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 MAJOR =1
 MINOR =0
-PATCH =3
+PATCH =4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 fp = open('README.md',encoding="utf-8")
 setup(
     name="nonebot_plugin_wol",
     version=VERSION,
     author="TwoOnefour",
     author_email="lys214412@gmail.com",
```

