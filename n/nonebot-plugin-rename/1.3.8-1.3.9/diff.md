# Comparing `tmp/nonebot_plugin_rename-1.3.8.tar.gz` & `tmp/nonebot_plugin_rename-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.3.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.3.9.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.3.8.tar` & `nonebot_plugin_rename-1.3.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1066 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/LICENSE
--rw-r--r--   0        0        0     5286 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/README.md
--rw-r--r--   0        0        0      549 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      293 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      903 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0     1020 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      450 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      607 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      893 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/starrail_time.py
--rw-r--r--   0        0        0      604 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      468 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0  1878036 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/fonts/draw.ttf
--rw-r--r--   0        0        0     8686 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      151 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      495 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      838 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1529 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      400 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      574 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/LICENSE
+-rw-r--r--   0        0        0     5286 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/README.md
+-rw-r--r--   0        0        0      550 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      535 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      903 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0     1020 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      450 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      607 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      892 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/starrail_time.py
+-rw-r--r--   0        0        0      604 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      697 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/year_time.py
+-rw-r--r--   0        0        0      468 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8709 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      264 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      912 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1529 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      400 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      683 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.9/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.3.8/LICENSE` & `nonebot_plugin_rename-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/README.md` & `nonebot_plugin_rename-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/__init__.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from nonebot.plugin import PluginMetadata
 
-from .main import *  # noqa
 from .config import env_config
+from .main import *  # noqa
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __plugin_meta__ = PluginMetadata(
     name="nonebot_plugin_rename",
     description="用于更改qq机器人的群名片，内置多种有趣名片",
     usage="查看本仓库readme",
     supported_adapters={"~onebot.v11"},
     type="application",
     config=env_config,
     homepage="https://github.com/forchannot/nonebot_plugin_rename",
     extra={
         "author": "forchannot",
         "version": __version__,
-    }
+    },
 )
```

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/genshin_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def genshin_version_time() -> str:
     # 原神版本号
     Versions = [36, 37, 38, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50]
     Index = 0
     # 获取持续时间
-    baseTime = datetime.strptime('2023-4-12 11:00:00', '%Y-%m-%d %H:%M:%S')
+    baseTime = datetime.strptime("2023-4-12 11:00:00", "%Y-%m-%d %H:%M:%S")
     nowTime = datetime.now()
     duringTime = (baseTime - nowTime).total_seconds() * 1000
     # 推算版本
     while duringTime <= 0:
         duringTime += 42 * 24 * 60 * 60 * 1000
         Index += 1
     # 计算版本号并取到小数点后一位
@@ -21,8 +21,8 @@
     leave1 = duringTime % (24 * 3600 * 1000)
     # 获取小时数并取整
     hours = int(leave1 / (3600 * 1000))
     leave2 = leave1 % (3600 * 1000)
     # 获取分钟数并取整
     minutes = int(leave2 / (60 * 1000))
     # 字符串处理
-    return f'离原神{Version}还有{days}天{hours}小时{minutes}分钟'
+    return f"离原神{Version}还有{days}天{hours}小时{minutes}分钟"
```

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/starrail_time.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/starrail_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,7 @@
     leave1 = duringTime % (24 * 3600 * 1000)
     # 获取小时数并取整
     hours = int(leave1 / (3600 * 1000))
     leave2 = leave1 % (3600 * 1000)
     # 获取分钟数并取整
     minutes = int(leave2 / (60 * 1000))
     return f"离崩铁{Version:.1f}还有{days}天{hours}小时{minutes}分钟"
-
```

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/fonts/draw.ttf` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/fonts/draw.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,15 @@
     PrivateMessageEvent,
 )
 from nonebot.drivers import Driver
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from .config import env_config
-from .utils import (
-    card_list,
-    choice_card,
-    generate_card_image,
-    read_yaml,
-    write_yaml,
-)
+from .utils import card_list, choice_card, generate_card_image, read_yaml, write_yaml
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler  # noqa
 
 driver: Driver = get_driver()
 hour, minute = env_config.set_group_card_hour, env_config.set_group_card_minute
 if driver.config.nickname:
@@ -116,15 +110,15 @@
     group_data = read_yaml(yml_file / "group_card.yaml") or {}
     if not group_data:
         return
     for bot_id, bot_case in bots.items():
         if group_info := group_data.get(bot_id, {}):
             tasks.extend(await set_card(group_info, bot_id, bot_case))
     results = await asyncio.gather(*tasks, return_exceptions=True)
-    for group_info, result in zip(group_data.values(), results):
+    for group_info, result in zip(group_data.values(), results):  # noqa: B905
         group_id = next(iter(group_info))
         if isinstance(result, Exception):
             logger.warning(f"群{group_id}名片更改失败，错误信息：{result}")
             set_wrong.append(group_id)
     if is_handle:
         return set_wrong
 
@@ -148,15 +142,17 @@
     else:
         result = "当前没有设置群名片哦,请先发送<设置群名片 序号>命令进行设置吧"
     await view_card.finish(message=MessageSegment.text(result) + img)
 
 
 # on_command "立即更改群名片"
 @set_card_now.handle()
-async def _(bot: Bot, event: GroupMessageEvent, arg: Message = CommandArg()):
+async def _(
+    bot: Bot, event: GroupMessageEvent, arg: Message = CommandArg()
+):  # noqa: B008
     card_number = arg.extract_plain_text().strip()
     if not card_number:
         await set_card_now.finish("请输入序号或序号输入错误")
     elif card_number not in map(str, range(1, len(card_list) + 1)):
         await set_card_now.finish("没有这种类型的群名片哦，可以发送[查看群名片列表]命令查看吧")
     card_names = await choice_card(card_number)
     if env_config.use_nickname_front:
@@ -192,15 +188,15 @@
     set_wrong = []
     group_data = read_yaml(yml_file / "group_card.yaml") or {}
     group_info = group_data.get(bot.self_id, {})
     if not group_info:
         await set_all_group_card.finish("没有设置过任何群名片哦")
     tasks = await set_card(group_info, bot.self_id, bot)
     results = await asyncio.gather(*tasks, return_exceptions=True)
-    for group_info, result in zip(group_data.values(), results):
+    for group_info, result in zip(group_data.values(), results):  # noqa: B905
         group_id = next(iter(group_info))
         if isinstance(result, Exception):
             logger.warning(f"群{group_id}名片更改失败，错误信息：{result}")
             set_wrong.append(group_id)
     msg = f"群名片设置成功,设置失败的群有\n{' '.join(set_wrong)}" if set_wrong else "所有群名片设置成功"
     await set_all_group_card.finish(msg)
```

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/card_name.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,16 @@
     get_msg,
     get_one_speak,
     gk,
     hot,
     now_time,
     old_time,
     system_status,
-    starrail_version_time
+    starrail_version_time,
+    next_year_time,
 )
 
 card_list = {
     "1": ("原神版本剩余时间", genshin_version_time),
     "2": ("北京时间(小时)", now_time),
     "3": ("当前时间(古代计时制)", old_time),
     "4": ("B站热搜", hot),
@@ -22,8 +23,9 @@
     "8": ("知乎热搜", hot),
     "9": ("今日头条热搜", hot),
     "10": ("每日一言", get_one_speak),
     "11": ("距离高考剩余时间", gk),
     "12": ("bot系统运行状态", system_status),
     "13": ("bot收发消息统计", get_msg),
     "14": ("崩铁版本剩余时间", starrail_version_time),
+    "15": ("距离下一年时间", next_year_time),
 }
```

### Comparing `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.8/PKG-INFO` & `nonebot_plugin_rename-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.3.8
+Version: 1.3.9
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.9 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
```

