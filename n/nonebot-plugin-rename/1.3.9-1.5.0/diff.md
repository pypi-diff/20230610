# Comparing `tmp/nonebot_plugin_rename-1.3.9.tar.gz` & `tmp/nonebot_plugin_rename-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.3.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.5.0.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.3.9.tar` & `nonebot_plugin_rename-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/LICENSE
--rw-r--r--   0        0        0     5286 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/README.md
--rw-r--r--   0        0        0      550 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      535 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      903 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0     1020 2023-06-10 10:53:20.215589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      450 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      607 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      892 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/starrail_time.py
--rw-r--r--   0        0        0      604 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      697 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/year_time.py
--rw-r--r--   0        0        0      468 2023-06-10 10:53:20.219589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0  1878036 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/fonts/draw.ttf
--rw-r--r--   0        0        0     8709 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      264 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      495 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      912 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1529 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      400 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      683 2023-06-10 10:53:20.235589 nonebot_plugin_rename-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5656 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/README.md
+-rw-r--r--   0        0        0      550 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0     1584 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/exam_time.py
+-rw-r--r--   0        0        0      689 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      450 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0     1500 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/mhy_time.py
+-rw-r--r--   0        0        0      607 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      604 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      697 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/year_time.py
+-rw-r--r--   0        0        0      534 2023-06-10 13:13:00.702340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8723 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      264 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      964 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1528 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      400 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      700 2023-06-10 13:13:00.722340 nonebot_plugin_rename-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6561 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.3.9/LICENSE` & `nonebot_plugin_rename-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.9/README.md` & `nonebot_plugin_rename-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-rename.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-yellow.svg" alt="python">
 
 </div>
 
 <!-- TOC -->
-* [nonebot-plugin-rename](#nonebot-plugin-rename)
-  * [📖简介](#简介)
-  * [🔐许可](#许可)
-  * [💿 安装方法](#-安装方法)
-  * [🏷️插件命令](#插件命令)
-  * [⚙️插件配置项](#插件配置项)
-  * [🎉目前已实现的群名片功能](#目前已实现的群名片功能)
-  * [🧐PR需知](#pr需知)
-  * [🔥鸣谢](#鸣谢)
+- [nonebot-plugin-rename](#nonebot-plugin-rename)
+  - [📖简介](#简介)
+  - [🔐许可](#许可)
+  - [💿 安装方法](#-安装方法)
+  - [🏷️插件命令](#️插件命令)
+  - [⚙️插件配置项](#️插件配置项)
+  - [🎉目前已实现的群名片功能](#目前已实现的群名片功能)
+  - [🧐PR需知](#pr需知)
+  - [🔥鸣谢](#鸣谢)
 <!-- TOC -->
 
 ## 📖简介
 
 通过定时任务更改bot(s)所在群自己的群名片
 
 ## 🔐许可
@@ -84,16 +84,22 @@
 |-------------------------------|-----------------------------|------|
 | set_group_card_hour           | 间隔时间(小时)                    | int  |
 | set_group_card_minute         | 间隔时间(分钟)                    | int  |
 | use_nickname_front            | 是否在群名片前加上bot名称              | bool |
 | self_name                     | 自定义前缀(需开启上一个配置)             | str  |
 | is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
  | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
+ | zk_time | 设置当地中考时间 | tuple |
 
-**请注意不要将两个间隔时间都设为0!!!!!!**
+**如果要使用中考剩余时间，由于每个地方中考时间并不统一，请务必填写`zk_time`配置项，否则获取的时间并不是你们当地的中考时间节点（开始和结束时间），参考配置如下**
+```dotenv
+zk_time=("06-12 09:00:00", "06-14 11:00:00")
+```
+
+**请注意不要将`set_group_card_hour`和`set_group_card_minute`都设为0**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
 <summary>一图流</summary>
 <img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230517/2b2b6734352a6ef94ff64cf1b7d8922d.5rr8s2fnai80.webp" alt="help">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                          # nonebot-plugin-rename _â¨
 éè¿å®æ¶ä»»å¡æ´æ¹botæå¨ç¾¤èªå·±çç¾¤åç,åç½®äºå ç§å¸¸è§çç¾¤åçå¹¶ä¸åæ­¥æ¯æäºå¤bot,æ¬¢è¿**pr**æ°çç¾¤åç!
                         â¨_ [license] [pypi] [python]
- * [nonebot-plugin-rename](#nonebot-plugin-rename) * [ðç®ä»](#ç®ä») *
-[ðè®¸å¯](#è®¸å¯) * [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) *
-[ð·ï¸æä»¶å½ä»¤](#æä»¶å½ä»¤) * [âï¸æä»¶éç½®é¡¹]
-(#æä»¶éç½®é¡¹) * [ðç®åå·²å®ç°çç¾¤åçåè½]
-(#ç®åå·²å®ç°çç¾¤åçåè½) * [ð§PRéç¥](#préç¥) * [ð¥é¸£è°¢]
+ - [nonebot-plugin-rename](#nonebot-plugin-rename) - [ðç®ä»](#ç®ä») -
+[ðè®¸å¯](#è®¸å¯) - [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) -
+[ð·ï¸æä»¶å½ä»¤](#ï¸æä»¶å½ä»¤) - [âï¸æä»¶éç½®é¡¹]
+(#ï¸æä»¶éç½®é¡¹) - [ðç®åå·²å®ç°çç¾¤åçåè½]
+(#ç®åå·²å®ç°çç¾¤åçåè½) - [ð§PRéç¥](#préç¥) - [ð¥é¸£è°¢]
 (#é¸£è°¢)  ## ðç®ä» éè¿å®æ¶ä»»å¡æ´æ¹bot
 (s)æå¨ç¾¤èªå·±çç¾¤åç ## ðè®¸å¯ [MIT](https://github.com/
 forchannot/nonebot-plugin-rename/blob/main/LICENSE) ## ð¿ å®è£æ¹æ³
 ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-rename   pip
 pip install nonebot-plugin-rename æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
@@ -28,16 +28,19 @@
 âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | |------------------------
 -------|-----------------------------|------| | set_group_card_hour |
 é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
 int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
 self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
 is_one_bot_set_all_group_card |
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
-| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool |
-**è¯·æ³¨æä¸è¦å°ä¸¤ä¸ªé´éæ¶é´é½è®¾ä¸º0!!!!!!**
+| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool | |
+zk_time | è®¾ç½®å½å°ä¸­èæ¶é´ | tuple |
+**å¦æè¦ä½¿ç¨ä¸­èå©ä½æ¶é´ï¼ç±äºæ¯ä¸ªå°æ¹ä¸­èæ¶é´å¹¶ä¸ç»ä¸ï¼è¯·å¡å¿å¡«å`zk_time`éç½®é¡¹ï¼å¦åè·åçæ¶é´å¹¶ä¸æ¯ä½ ä»¬å½å°çä¸­èæ¶é´èç¹ï¼å¼å§åç»ææ¶é´ï¼ï¼åèéç½®å¦ä¸**
+```dotenv zk_time=("06-12 09:00:00", "06-14 11:00:00") ```
+**è¯·æ³¨æä¸è¦å°`set_group_card_hour`å`set_group_card_minute`é½è®¾ä¸º0**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
 -- æéçæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
```

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/__init__.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot.plugin import PluginMetadata
 
 from .config import env_config
 from .main import *  # noqa
 
-__version__ = "1.3.9"
+__version__ = "1.5.0"
 __plugin_meta__ = PluginMetadata(
     name="nonebot_plugin_rename",
     description="用于更改qq机器人的群名片，内置多种有趣名片",
     usage="查看本仓库readme",
     supported_adapters={"~onebot.v11"},
     type="application",
     config=env_config,
```

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/card/year_time.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/card/year_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/fonts/draw.ttf` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/fonts/draw.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         result = "当前没有设置群名片哦,请先发送<设置群名片 序号>命令进行设置吧"
     await view_card.finish(message=MessageSegment.text(result) + img)
 
 
 # on_command "立即更改群名片"
 @set_card_now.handle()
 async def _(
-    bot: Bot, event: GroupMessageEvent, arg: Message = CommandArg()
+    bot: Bot, event: GroupMessageEvent, arg: Message = CommandArg()  # noqa: B008
 ):  # noqa: B008
     card_number = arg.extract_plain_text().strip()
     if not card_number:
         await set_card_now.finish("请输入序号或序号输入错误")
     elif card_number not in map(str, range(1, len(card_list) + 1)):
         await set_card_now.finish("没有这种类型的群名片哦，可以发送[查看群名片列表]命令查看吧")
     card_names = await choice_card(card_number)
```

### Comparing `nonebot_plugin_rename-1.3.9/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.5.0/nonebot_plugin_rename/utils/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from io import BytesIO
 from pathlib import Path
 
 from PIL import Image, ImageDraw, ImageFont
 
 from .card_name import card_list
 
-
 font_path = Path(__file__).parent.parent / "fonts" / "draw.ttf"
 
 
 def generate_card_image(
     font: Path = font_path,
     font_size: int = 20,
     title_left: str = "群名片序号",
```

### Comparing `nonebot_plugin_rename-1.3.9/PKG-INFO` & `nonebot_plugin_rename-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.3.9
+Version: 1.5.0
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -40,23 +40,23 @@
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-rename.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-yellow.svg" alt="python">
 
 </div>
 
 <!-- TOC -->
-* [nonebot-plugin-rename](#nonebot-plugin-rename)
-  * [📖简介](#简介)
-  * [🔐许可](#许可)
-  * [💿 安装方法](#-安装方法)
-  * [🏷️插件命令](#插件命令)
-  * [⚙️插件配置项](#插件配置项)
-  * [🎉目前已实现的群名片功能](#目前已实现的群名片功能)
-  * [🧐PR需知](#pr需知)
-  * [🔥鸣谢](#鸣谢)
+- [nonebot-plugin-rename](#nonebot-plugin-rename)
+  - [📖简介](#简介)
+  - [🔐许可](#许可)
+  - [💿 安装方法](#-安装方法)
+  - [🏷️插件命令](#️插件命令)
+  - [⚙️插件配置项](#️插件配置项)
+  - [🎉目前已实现的群名片功能](#目前已实现的群名片功能)
+  - [🧐PR需知](#pr需知)
+  - [🔥鸣谢](#鸣谢)
 <!-- TOC -->
 
 ## 📖简介
 
 通过定时任务更改bot(s)所在群自己的群名片
 
 ## 🔐许可
@@ -107,16 +107,22 @@
 |-------------------------------|-----------------------------|------|
 | set_group_card_hour           | 间隔时间(小时)                    | int  |
 | set_group_card_minute         | 间隔时间(分钟)                    | int  |
 | use_nickname_front            | 是否在群名片前加上bot名称              | bool |
 | self_name                     | 自定义前缀(需开启上一个配置)             | str  |
 | is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
  | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
+ | zk_time | 设置当地中考时间 | tuple |
 
-**请注意不要将两个间隔时间都设为0!!!!!!**
+**如果要使用中考剩余时间，由于每个地方中考时间并不统一，请务必填写`zk_time`配置项，否则获取的时间并不是你们当地的中考时间节点（开始和结束时间），参考配置如下**
+```dotenv
+zk_time=("06-12 09:00:00", "06-14 11:00:00")
+```
+
+**请注意不要将`set_group_card_hour`和`set_group_card_minute`都设为0**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
 <summary>一图流</summary>
 <img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230517/2b2b6734352a6ef94ff64cf1b7d8922d.5rr8s2fnai80.webp" alt="help">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.5.0 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
@@ -11,19 +11,19 @@
 Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist: psutil (>=5.9.5,<6.0.0) Requires-
 Dist: pyyaml (>=6.0,<7.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                          # nonebot-plugin-rename _â¨
 éè¿å®æ¶ä»»å¡æ´æ¹botæå¨ç¾¤èªå·±çç¾¤åç,åç½®äºå ç§å¸¸è§çç¾¤åçå¹¶ä¸åæ­¥æ¯æäºå¤bot,æ¬¢è¿**pr**æ°çç¾¤åç!
                         â¨_ [license] [pypi] [python]
- * [nonebot-plugin-rename](#nonebot-plugin-rename) * [ðç®ä»](#ç®ä») *
-[ðè®¸å¯](#è®¸å¯) * [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) *
-[ð·ï¸æä»¶å½ä»¤](#æä»¶å½ä»¤) * [âï¸æä»¶éç½®é¡¹]
-(#æä»¶éç½®é¡¹) * [ðç®åå·²å®ç°çç¾¤åçåè½]
-(#ç®åå·²å®ç°çç¾¤åçåè½) * [ð§PRéç¥](#préç¥) * [ð¥é¸£è°¢]
+ - [nonebot-plugin-rename](#nonebot-plugin-rename) - [ðç®ä»](#ç®ä») -
+[ðè®¸å¯](#è®¸å¯) - [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) -
+[ð·ï¸æä»¶å½ä»¤](#ï¸æä»¶å½ä»¤) - [âï¸æä»¶éç½®é¡¹]
+(#ï¸æä»¶éç½®é¡¹) - [ðç®åå·²å®ç°çç¾¤åçåè½]
+(#ç®åå·²å®ç°çç¾¤åçåè½) - [ð§PRéç¥](#préç¥) - [ð¥é¸£è°¢]
 (#é¸£è°¢)  ## ðç®ä» éè¿å®æ¶ä»»å¡æ´æ¹bot
 (s)æå¨ç¾¤èªå·±çç¾¤åç ## ðè®¸å¯ [MIT](https://github.com/
 forchannot/nonebot-plugin-rename/blob/main/LICENSE) ## ð¿ å®è£æ¹æ³
 ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-rename   pip
 pip install nonebot-plugin-rename æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
@@ -40,16 +40,19 @@
 âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | |------------------------
 -------|-----------------------------|------| | set_group_card_hour |
 é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
 int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
 self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
 is_one_bot_set_all_group_card |
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
-| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool |
-**è¯·æ³¨æä¸è¦å°ä¸¤ä¸ªé´éæ¶é´é½è®¾ä¸º0!!!!!!**
+| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool | |
+zk_time | è®¾ç½®å½å°ä¸­èæ¶é´ | tuple |
+**å¦æè¦ä½¿ç¨ä¸­èå©ä½æ¶é´ï¼ç±äºæ¯ä¸ªå°æ¹ä¸­èæ¶é´å¹¶ä¸ç»ä¸ï¼è¯·å¡å¿å¡«å`zk_time`éç½®é¡¹ï¼å¦åè·åçæ¶é´å¹¶ä¸æ¯ä½ ä»¬å½å°çä¸­èæ¶é´èç¹ï¼å¼å§åç»ææ¶é´ï¼ï¼åèéç½®å¦ä¸**
+```dotenv zk_time=("06-12 09:00:00", "06-14 11:00:00") ```
+**è¯·æ³¨æä¸è¦å°`set_group_card_hour`å`set_group_card_minute`é½è®¾ä¸º0**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
 -- æéçæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
```

