# Comparing `tmp/nonebot_plugin_picmcstat-0.3.2.tar.gz` & `tmp/nonebot_plugin_picmcstat-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_picmcstat-0.3.2.tar", last modified: Sun Jun  4 17:17:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_picmcstat-0.3.3.tar", last modified: Sat Jun 10 13:13:10 2023, max compression
```

## Comparing `nonebot_plugin_picmcstat-0.3.2.tar` & `nonebot_plugin_picmcstat-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/LICENSE
--rw-r--r--   0        0        0     5998 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/README.md
--rw-r--r--   0        0        0      541 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/__init__.py
--rw-r--r--   0        0        0     1572 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/__main__.py
--rw-r--r--   0        0        0      452 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/config.py
--rw-r--r--   0        0        0     1480 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/const.py
--rw-r--r--   0        0        0     7748 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/draw.py
--rw-r--r--   0        0        0      399 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res.py
--rw-r--r--   0        0        0    12656 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/default.png
--rw-r--r--   0        0        0      335 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/dirt.png
--rw-r--r--   0        0        0      556 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/grass_side_carried.png
--rw-r--r--   0        0        0     4078 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/util.py
--rw-r--r--   0        0        0      675 2023-06-04 17:17:16.354115 nonebot_plugin_picmcstat-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6612 1970-01-01 00:00:00.000000 nonebot_plugin_picmcstat-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6308 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/README.md
+-rw-r--r--   0        0        0      541 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/__init__.py
+-rw-r--r--   0        0        0     1544 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/__main__.py
+-rw-r--r--   0        0        0      475 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/config.py
+-rw-r--r--   0        0        0     1480 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/const.py
+-rw-r--r--   0        0        0    10116 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/draw.py
+-rw-r--r--   0        0        0      399 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/res.py
+-rw-r--r--   0        0        0    12656 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/res/default.png
+-rw-r--r--   0        0        0      335 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/res/dirt.png
+-rw-r--r--   0        0        0      556 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/res/grass_side_carried.png
+-rw-r--r--   0        0        0     3364 2023-06-10 13:12:55.810627 nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/util.py
+-rw-r--r--   0        0        0      675 2023-06-10 13:13:10.690761 nonebot_plugin_picmcstat-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6922 1970-01-01 00:00:00.000000 nonebot_plugin_picmcstat-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_picmcstat-0.3.2/LICENSE` & `nonebot_plugin_picmcstat-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picmcstat-0.3.2/README.md` & `nonebot_plugin_picmcstat-0.3.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -115,18 +115,22 @@
 如果不行，请尝试右键字体文件点击 `为所有用户安装`  
 如果还是不行，请尝试修改插件字体配置
 
 ## ⚙️ 配置
 
 ### `MCSTAT_FONT` - 使用的字体名称 / 路径
 
-默认：`unifont-15.0.01.ttf`
+默认：`unifont`
 
 请按需自行更改
 
+### `MCSTAT_SHOW_ADDR` - 是否在生成的图片中显示服务器地址
+
+默认：`False`
+
 ### `MCSTAT_SHORTCUTS` - 快捷指令列表
 
 这个配置项能够帮助你简化一些查询指令
 
 此配置项的类型是一个列表，里面的元素需要为一个特定结构的字典  
 这个字典需要有三个元素
 
@@ -172,14 +176,27 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.3
+
+- 修复特殊情况下玩家列表排版错误的问题
+- 添加显示服务器地址的配置项 (`MCSTAT_SHOW_ADDR`)
+
+### 0.3.2
+
+- 🎉 NoneBot 2.0 🚀
+
+### 0.3.1
+
+- 修复文本内含有 `§k` 时报错的问题
+
 ### 0.3.0
 
 - 弃用 `nonebot-plugin-imageutils`，换用 `pil-utils`
 - 支持了更多字体样式
 - 支持自定义字体
 
 ### 0.2.7
```

#### html2text {}

```diff
@@ -21,16 +21,18 @@
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_picmcstat" ] ```  ### å­ä½ å­ä½æä»¶è¯·èªè¡å»èªè¡å»
 [è¿é](http://ftp.gnu.org/gnu/unifont/unifont-15.0.01/unifont-15.0.01.ttf)
 ä¸è½½ å°å­ä½æä»¶ç´æ¥å®è£å¨ç³»ç»ä¸­å³å¯
 å¦æä¸è¡ï¼è¯·å°è¯å³é®å­ä½æä»¶ç¹å» `ä¸ºææç¨æ·å®è£`
 å¦æè¿æ¯ä¸è¡ï¼è¯·å°è¯ä¿®æ¹æä»¶å­ä½éç½® ## âï¸ éç½® ###
-`MCSTAT_FONT` - ä½¿ç¨çå­ä½åç§° / è·¯å¾ é»è®¤ï¼`unifont-15.0.01.ttf`
-è¯·æéèªè¡æ´æ¹ ### `MCSTAT_SHORTCUTS` - å¿«æ·æä»¤åè¡¨
+`MCSTAT_FONT` - ä½¿ç¨çå­ä½åç§° / è·¯å¾ é»è®¤ï¼`unifont`
+è¯·æéèªè¡æ´æ¹ ### `MCSTAT_SHOW_ADDR` -
+æ¯å¦å¨çæçå¾çä¸­æ¾ç¤ºæå¡å¨å°å é»è®¤ï¼`False` ###
+`MCSTAT_SHORTCUTS` - å¿«æ·æä»¤åè¡¨
 è¿ä¸ªéç½®é¡¹è½å¤å¸®å©ä½ ç®åä¸äºæ¥è¯¢æä»¤
 æ­¤éç½®é¡¹çç±»åæ¯ä¸ä¸ªåè¡¨ï¼éé¢çåç´ éè¦ä¸ºä¸ä¸ªç¹å®ç»æçå­å¸
 è¿ä¸ªå­å¸éè¦æä¸ä¸ªåç´  - `regex` -
 ç¨äºå¹éæä»¤çæ­£åï¼ä¾å¦ `^æ¥æ$` ï¼æ³¨æï¼nb2 ä»¥ JSON
 æ ¼å¼è§£æéç½®é¡¹ï¼æä»¥å½ä½ è¦å¨æ­£åè¡¨è¾¾å¼éè¡¨ç¤º`\`æ¶ï¼ä½ éè¦å°å¶è½¬ä¹ä¸º`\\`ï¼
 - `host` - è¦æ¥è¯¢çæå¡å¨å°åï¼æ ¼å¼ä¸º `[:ç«¯å£]`ï¼ ä¾å¦
 `hypixel.net` æ `example.com:1919` - `type` -
@@ -45,19 +47,23 @@
 ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [pil-utils](https://github.com/MeetWq/pil-utils)
 è¶å¥½ç¨ç Pillow è¾å©åºï¼wq ä½¬æ¯å ï¼å¿«å»ç¨ awa ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.0 - å¼ç¨ `nonebot-plugin-
-imageutils`ï¼æ¢ç¨ `pil-utils` - æ¯æäºæ´å¤å­ä½æ ·å¼ -
-æ¯æèªå®ä¹å­ä½ ### 0.2.7 - ä¿®å¤ `shortcut` ç `whitelist`
-çå¥æªè¡¨ç° ### 0.2.6 - ä¿®å¤ `shortcut` ä¸­æ²¡æ `whitelist`
-é¡¹ä¼æ¥éçé®é¢ ### 0.2.5 - `shortcut` å å¥ `whitelist`
-é¡¹éç½®è§¦åç¾¤ç½åå ### 0.2.4 - ä¿®å¤ç©å®¶åè¡¨åºä¸çå¤ä½ç©ºè¡
-### 0.2.3 - ä¿®å¤ JE æå¡å¨ Motd ä¸­ç²ä½æå¤æ¾ç¤ºä¸ºèè²ç bug ###
-0.2.2 - ä¿®å¤ motd ååççç©ºå»ä¸å¹²åçé®é¢ -
-ä¼åç©å®¶åè¡¨æ¾ç¤ºææ ### 0.2.1 - ä¿®å¤å½æå¤§äººæ°ä¸º 0
-æ¶åºéçé®é¢ ### 0.2.0 - å å¥å¿«æ·æä»¤ï¼è¯¦è§éç½®é¡¹ -
-ä¿®å¤æäº JE ææ æ³æ­£ç¡®æ¾ç¤º Motd çé®é¢ - ### 0.1.1 - å°æ¥ JE
-ææ¶ç `æ¸¸æå»¶è¿` å­æ · æ¹ä¸º `æµè¯å»¶è¿`
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.3 -
+ä¿®å¤ç¹æ®æåµä¸ç©å®¶åè¡¨æçéè¯¯çé®é¢ -
+æ·»å æ¾ç¤ºæå¡å¨å°åçéç½®é¡¹ (`MCSTAT_SHOW_ADDR`) ### 0.3.2 - ð
+NoneBot 2.0 ð ### 0.3.1 - ä¿®å¤ææ¬åå«æ `Â§k` æ¶æ¥éçé®é¢ ###
+0.3.0 - å¼ç¨ `nonebot-plugin-imageutils`ï¼æ¢ç¨ `pil-utils` -
+æ¯æäºæ´å¤å­ä½æ ·å¼ - æ¯æèªå®ä¹å­ä½ ### 0.2.7 - ä¿®å¤
+`shortcut` ç `whitelist` çå¥æªè¡¨ç° ### 0.2.6 - ä¿®å¤ `shortcut`
+ä¸­æ²¡æ `whitelist` é¡¹ä¼æ¥éçé®é¢ ### 0.2.5 - `shortcut` å å¥
+`whitelist` é¡¹éç½®è§¦åç¾¤ç½åå ### 0.2.4 -
+ä¿®å¤ç©å®¶åè¡¨åºä¸çå¤ä½ç©ºè¡ ### 0.2.3 - ä¿®å¤ JE æå¡å¨ Motd
+ä¸­ç²ä½æå¤æ¾ç¤ºä¸ºèè²ç bug ### 0.2.2 - ä¿®å¤ motd
+ååççç©ºå»ä¸å¹²åçé®é¢ - ä¼åç©å®¶åè¡¨æ¾ç¤ºææ ### 0.2.1
+- ä¿®å¤å½æå¤§äººæ°ä¸º 0 æ¶åºéçé®é¢ ### 0.2.0 -
+å å¥å¿«æ·æä»¤ï¼è¯¦è§éç½®é¡¹ - ä¿®å¤æäº JE ææ æ³æ­£ç¡®æ¾ç¤º
+Motd çé®é¢ - ### 0.1.1 - å°æ¥ JE ææ¶ç `æ¸¸æå»¶è¿` å­æ · æ¹ä¸º
+`æµè¯å»¶è¿`
```

### Comparing `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/__init__.py` & `nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from nonebot.plugin import PluginMetadata
 
 from . import __main__ as __main__
 from .config import ConfigClass
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 __plugin_meta__ = PluginMetadata(
     name="PicMCStat",
     description="将一个 Minecraft 服务器的 MOTD 信息绘制为一张图片",
     usage="使用 motd 指令查看使用帮助",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-picmcstat",
     type="application",
     config=ConfigClass,
-    supported_adapters=["~onebot.v11"],
+    supported_adapters={"~onebot.v11"},
     extra={"License": "MIT", "Author": "student_2333"},
 )
```

### Comparing `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/__main__.py` & `nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from typing import Awaitable, Callable, NoReturn
 
 from nonebot import on_command, on_regex
 from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageEvent
-from nonebot.internal.adapter import Message
 from nonebot.matcher import Matcher
-from nonebot.params import CommandArg
+from nonebot.params import RawCommand
 
 from .config import ShortcutType, config
 from .draw import ServerType, draw
 
+BE_SVR_PREFIX = ["pe", "be"]
+
+
 motd_handler = on_command("motd", aliases={"!motd", "！motd"})
 
 
 @motd_handler.handle()
-async def _(matcher: Matcher, msg_arg: Message = CommandArg()):
-    arg: str = msg_arg.extract_plain_text()
+async def _(matcher: Matcher, event: MessageEvent, cmd: str = RawCommand()):
+    arg = event.get_plaintext().lstrip().replace(cmd, "", 1)
 
     svr_type: ServerType = "je"
-    be_svr_prefix = ["pe", "be"]
-    for p in be_svr_prefix:
-        if arg.startswith(p):
-            arg = arg.replace(p, "", 1)
-            svr_type = "be"
-            break
+    if p := next((p for p in BE_SVR_PREFIX if arg.startswith(p)), None):
+        arg = arg.replace(p, "", 1)
+        svr_type = "be"
 
     arg = arg.strip()
     await matcher.finish(await draw(arg, svr_type))
 
 
 def get_shortcut_handler(
     host: str,
```

### Comparing `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/const.py` & `nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/const.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/draw.py` & `nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/draw.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import socket
 from asyncio.exceptions import TimeoutError
 from io import BytesIO
-from typing import Optional, Union
+from itertools import zip_longest
+from typing import List, Optional, Union
 
 from mcstatus import BedrockServer, JavaServer
 from mcstatus.bedrock_status import BedrockStatusResponse
 from mcstatus.pinger import PingResponse
 from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot.log import logger
@@ -14,15 +15,14 @@
 from pil_utils import BuildImage, Text2Image
 
 from .config import config
 from .const import CODE_COLOR, GAME_MODE_MAP, STROKE_COLOR, ServerType
 from .res import DEFAULT_ICON_RES, DIRT_RES, GRASS_RES
 from .util import (
     format_code_to_bbcode,
-    format_list,
     get_latency_color,
     json_to_format_code,
     strip_lines,
 )
 
 MARGIN = 32
 MIN_WIDTH = 512
@@ -48,23 +48,47 @@
     for hi in range(0, height, size):
         for wi in range(0, width, size):
             bg.paste(DIRT_RES if hi else GRASS_RES, (wi, hi))
 
     return bg
 
 
+def merge_extra(extra: List[Union[Text2Image, BuildImage]]) -> BuildImage:
+    spacing = 2
+
+    bg = BuildImage.new(
+        "RGBA",
+        (
+            max(x.width for x in extra),
+            sum(x.height for x in extra) + spacing * (len(extra) - 1),
+        ),
+    )
+
+    y_offset = 0
+    for img in extra:
+        if isinstance(img, Text2Image):
+            img.draw_on_image(bg.image, (0, y_offset))
+        else:
+            bg.paste(img, (0, y_offset), alpha=True)
+        y_offset += img.height + spacing
+
+    return bg
+
+
 def build_img(
     header1: str,
     header2: str,
-    extra: Optional[Text2Image] = None,
     icon: Optional[BuildImage] = None,
+    extras: Optional[List[Union[Text2Image, BuildImage]]] = None,
 ) -> BytesIO:
     if not icon:
         icon = DEFAULT_ICON_RES
 
+    extra = merge_extra(extras) if extras else None
+
     header_text_color = CODE_COLOR["f"]
     header_stroke_color = STROKE_COLOR["f"]
 
     header_height = 128
     half_header_height = int(header_height / 2)
 
     bg_width = extra.width + MARGIN * 2 if extra else MIN_WIDTH
@@ -111,17 +135,18 @@
         max_fontsize=TITLE_FONT_SIZE,
         fontname=config.mcstat_font,
         stroke_ratio=STROKE_RATIO,
         stroke_fill=header_stroke_color,
     )
 
     if extra:
-        extra.draw_on_image(
-            bg.image,
+        bg.paste(
+            extra,
             (MARGIN, int(header_height + MARGIN + MARGIN / 2)),
+            alpha=True,
         )
 
     return bg.convert("RGB").save("PNG")
 
 
 def format_extra(extra: str) -> Text2Image:
     return Text2Image.from_bbcode_text(
@@ -131,65 +156,114 @@
         fontname=config.mcstat_font,
         stroke_ratio=STROKE_RATIO,
         stroke_fill=STROKE_COLOR["f"],
         spacing=EXTRA_SPACING,
     )
 
 
+def format_list(title: str, sample: List[str]) -> Optional[BuildImage]:
+    text_img = [format_extra(x) for x in sample if x]
+    if not text_img:
+        return None
+
+    title_img = format_extra(title)
+
+    text_img_l = text_img[::2]
+    text_img_r = text_img[1::2]
+    max_width_l = max([x.width for x in text_img_l]) if text_img_l else 0
+    max_width_r = max([x.width for x in text_img_r]) if text_img_r else 0
+    height_l = sum([x.height for x in text_img_l])
+    height_r = sum([x.height for x in text_img_r])
+
+    spacing_width = format_extra("  ").width
+
+    img_height = max(height_l, height_r)
+    img_width = title_img.width + max_width_l
+    if max_width_r:
+        img_width += spacing_width + max_width_r
+
+    img = BuildImage.new("RGBA", (img_width, img_height), (255, 255, 255, 0))
+    title_img.draw_on_image(img.image, (0, 0))
+
+    y_offset = 0
+    for lt, rt in zip_longest(text_img_l, text_img_r):
+        if lt:
+            lt.draw_on_image(img.image, (title_img.width, y_offset))
+        if rt:
+            rt.draw_on_image(
+                img.image,
+                (title_img.width + max_width_l + spacing_width, y_offset),
+            )
+        y_offset += max(lt.height if lt else 0, rt.height if rt else 0)
+
+    return img
+
+
 def draw_help(svr_type: ServerType) -> BytesIO:
     cmd_prefix_li = list(get_driver().config.command_start)
     prefix = cmd_prefix_li[0] if cmd_prefix_li else ""
 
     extra_txt = f"查询Java版服务器: {prefix}motd <服务器IP>\n查询基岩版服务器: {prefix}motdpe <服务器IP>"
-    return build_img(get_header_by_svr_type(svr_type), "使用帮助", format_extra(extra_txt))
+    return build_img(
+        get_header_by_svr_type(svr_type),
+        "使用帮助",
+        extras=[format_extra(extra_txt)],
+    )
 
 
-def draw_java(res: PingResponse) -> BytesIO:
-    icon = None
-    if res.favicon:
-        icon = BuildImage.open(BytesIO(base64.b64decode(res.favicon.split(",")[-1])))
+def draw_java(res: PingResponse, addr: str) -> BytesIO:
+    icon = (
+        BuildImage.open(BytesIO(base64.b64decode(res.favicon.split(",")[-1])))
+        if res.favicon
+        else None
+    )
 
+    addr_txt = f"§7测试地址: §f{addr}\n" if config.mcstat_show_addr else ""
     players_online = res.players.online
     players_max = res.players.max
     online_percent = (
         "{:.2f}".format(players_online / players_max * 100) if players_max else "?.??"
     )
     motd = strip_lines(json_to_format_code(res.raw["description"]))
 
-    player_li = ""
-    if res.players.sample:
-        sample = [x.name for x in res.players.sample]
-        player_li = f"\n§7玩家列表: §f{format_list(sample)}"
+    player_li = [x.name for x in res.players.sample] if res.players.sample else []
 
     mod_client = ""
     mod_total = ""
-    mod_list = ""
+    mod_list = []
     if mod_info := res.raw.get("modinfo"):
         if tmp := mod_info.get("type"):
             mod_client = f"§7Mod端类型: §f{tmp}\n"
 
         if tmp := mod_info.get("modList"):
             mod_total = f"§7Mod总数: §f{len(tmp)}\n"
-            mod_list = f"§7Mod列表: §f{format_list(tmp)}\n"
+            mod_list = tmp
 
     extra_txt = (
         f"{motd}§r\n"
+        f"{addr_txt}"
         f"§7服务端名: §f{res.version.name}\n"
         f"{mod_client}"
         f"§7协议版本: §f{res.version.protocol}\n"
         f"§7当前人数: §f{players_online}/{players_max} ({online_percent}%)\n"
         f"{mod_total}"
         f"§7测试延迟: §{get_latency_color(res.latency)}{res.latency:.2f}ms"
-        f"{player_li}"
-        f"{mod_list}"
     )
-    return build_img(JE_HEADER, SUCCESS_TITLE, format_extra(extra_txt), icon)
 
+    extras: List[Union[Text2Image, BuildImage]] = [format_extra(extra_txt)]
+    if mod_list and (li := format_list("§7Mod列表: ", mod_list)):
+        extras.append(li)
+    if player_li and (li := format_list("§7玩家列表: ", player_li)):
+        extras.append(li)
+
+    return build_img(JE_HEADER, SUCCESS_TITLE, icon=icon, extras=extras)
 
-def draw_bedrock(res: BedrockStatusResponse) -> BytesIO:
+
+def draw_bedrock(res: BedrockStatusResponse, addr: str) -> BytesIO:
+    addr_txt = f"§7测试地址: §f{addr}\n" if config.mcstat_show_addr else ""
     map_name = f"§7存档名称: §f{res.map}§r\n" if res.map else ""
     game_mode = (
         f"§7游戏模式: §f{GAME_MODE_MAP.get(res.gamemode, res.gamemode)}\n"
         if res.gamemode
         else ""
     )
     online_percent = (
@@ -197,22 +271,23 @@
         if res.players_max
         else "?.??"
     )
     motd = strip_lines(res.motd)
 
     extra_txt = (
         f"{motd}§r\n"
+        f"{addr_txt}"
         f"§7协议版本: §f{res.version.protocol}\n"
         f"§7游戏版本: §f{res.version.version}\n"
         f"§7在线人数: §f{res.players_online}/{res.players_max} ({online_percent}%)\n"
         f"{map_name}"
         f"{game_mode}"
         f"§7测试延迟: §{get_latency_color(res.latency)}{res.latency:.2f}ms"
     )
-    return build_img(BE_HEADER, SUCCESS_TITLE, format_extra(extra_txt))
+    return build_img(BE_HEADER, SUCCESS_TITLE, extras=[format_extra(extra_txt)])
 
 
 def draw_error(e: Exception, svr_type: ServerType) -> BytesIO:
     extra = ""
     if isinstance(e, TimeoutError):
         reason = "请求超时"
     elif isinstance(e, socket.gaierror):
@@ -220,32 +295,36 @@
         extra = str(e)
     else:
         reason = "出错了！"
         extra = repr(e)
 
     extra_img = format_extra(extra).wrap(MIN_WIDTH - MARGIN * 2) if extra else None
 
-    return build_img(get_header_by_svr_type(svr_type), reason, extra_img)
+    return build_img(
+        get_header_by_svr_type(svr_type),
+        reason,
+        extras=[extra_img] if extra_img else None,
+    )
 
 
 async def draw(ip: str, svr_type: ServerType) -> Union[MessageSegment, str]:
     if svr_type not in ("je", "be"):
         raise ValueError("Server type must be `je` or `be`")  # noqa: TRY003
 
     try:
         if not ip:
             return MessageSegment.image(draw_help(svr_type))
 
         if svr_type == "je":
             return MessageSegment.image(
-                draw_java(await (await JavaServer.async_lookup(ip)).async_status()),
+                draw_java(await (await JavaServer.async_lookup(ip)).async_status(), ip),
             )
 
         return MessageSegment.image(
-            draw_bedrock(await BedrockServer.lookup(ip).async_status()),
+            draw_bedrock(await BedrockServer.lookup(ip).async_status(), ip),
         )
     except Exception as e:
         logger.exception("获取服务器状态/画服务器状态图出错")
         try:
             return MessageSegment.image(draw_error(e, svr_type))
         except:
             logger.exception("画异常状态图失败")
```

### Comparing `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/default.png` & `nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/res/default.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/grass_side_carried.png` & `nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/res/grass_side_carried.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/util.py` & `nonebot_plugin_picmcstat-0.3.3/nonebot_plugin_picmcstat/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,44 +86,14 @@
         parsed.append(txt)
 
     parsed.extend(color_tails)
     parsed.extend(format_tails)
     return "".join(parsed)
 
 
-def format_list(
-    sample: List[str],
-    items_per_line=2,
-    line_start_spaces=10,
-    list_gap=2,
-) -> str:
-    sample = [x for x in sample if x]
-    if not sample:
-        return ""
-
-    max_width = max([len(replace_format_code(x)) for x in sample]) + list_gap
-
-    line_added = 0
-    tmp = []
-    for name in sample:
-        if line_added < items_per_line:
-            code_len = len(name) - len(replace_format_code(name))
-            name = name.ljust(max_width + code_len)
-
-        tmp.append(name)
-        line_added += 1
-
-        if line_added >= items_per_line:
-            tmp.append("\n")
-            tmp.append(" " * line_start_spaces)
-            line_added = 0
-
-    return "".join(tmp).strip()
-
-
 def get_format_code_by_dict(json: "RawResponseDescriptionWhenDict") -> list:
     codes = []
     if color := json.get("color"):
         codes.append(f"§{STRING_CODE[color]}")
 
     for k in ["bold", "italic", "underlined", "strikethrough", "obfuscated"]:
         if json.get(k):
```

### Comparing `nonebot_plugin_picmcstat-0.3.2/pyproject.toml` & `nonebot_plugin_picmcstat-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-picmcstat"
-version = "0.3.2"
+version = "0.3.3"
 description = "A NoneBot2 plugin generates a pic from a Minecraft server's MOTD"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "mcstatus<11.0.0,>=10.0.1",
     "nonebot2<3.0.0,>=2.0.0",
```

### Comparing `nonebot_plugin_picmcstat-0.3.2/PKG-INFO` & `nonebot_plugin_picmcstat-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-picmcstat
-Version: 0.3.2
+Version: 0.3.3
 Summary: A NoneBot2 plugin generates a pic from a Minecraft server's MOTD
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picmcstat
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-picmcstat
 Requires-Python: <4.0,>=3.8
 Requires-Dist: mcstatus<11.0.0,>=10.0.1
@@ -131,18 +131,22 @@
 如果不行，请尝试右键字体文件点击 `为所有用户安装`  
 如果还是不行，请尝试修改插件字体配置
 
 ## ⚙️ 配置
 
 ### `MCSTAT_FONT` - 使用的字体名称 / 路径
 
-默认：`unifont-15.0.01.ttf`
+默认：`unifont`
 
 请按需自行更改
 
+### `MCSTAT_SHOW_ADDR` - 是否在生成的图片中显示服务器地址
+
+默认：`False`
+
 ### `MCSTAT_SHORTCUTS` - 快捷指令列表
 
 这个配置项能够帮助你简化一些查询指令
 
 此配置项的类型是一个列表，里面的元素需要为一个特定结构的字典  
 这个字典需要有三个元素
 
@@ -188,14 +192,27 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.3
+
+- 修复特殊情况下玩家列表排版错误的问题
+- 添加显示服务器地址的配置项 (`MCSTAT_SHOW_ADDR`)
+
+### 0.3.2
+
+- 🎉 NoneBot 2.0 🚀
+
+### 0.3.1
+
+- 修复文本内含有 `§k` 时报错的问题
+
 ### 0.3.0
 
 - 弃用 `nonebot-plugin-imageutils`，换用 `pil-utils`
 - 支持了更多字体样式
 - 支持自定义字体
 
 ### 0.2.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-picmcstat Version: 0.3.2 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-picmcstat Version: 0.3.3 Summary: A
 NoneBot2 plugin generates a pic from a Minecraft server's MOTD Home-page:
 https://github.com/lgc-NB2Dev/nonebot-plugin-picmcstat Author-Email:
 student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-picmcstat Requires-Python: <4.0,>=3.8 Requires-Dist:
 mcstatus<11.0.0,>=10.0.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0 Requires-Dist:
 nonebot-adapter-onebot<3.0.0,>=2.2.0 Requires-Dist: pydantic<2.0.0,>=1.10.4
@@ -30,16 +30,18 @@
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_picmcstat" ] ```  ### å­ä½ å­ä½æä»¶è¯·èªè¡å»èªè¡å»
 [è¿é](http://ftp.gnu.org/gnu/unifont/unifont-15.0.01/unifont-15.0.01.ttf)
 ä¸è½½ å°å­ä½æä»¶ç´æ¥å®è£å¨ç³»ç»ä¸­å³å¯
 å¦æä¸è¡ï¼è¯·å°è¯å³é®å­ä½æä»¶ç¹å» `ä¸ºææç¨æ·å®è£`
 å¦æè¿æ¯ä¸è¡ï¼è¯·å°è¯ä¿®æ¹æä»¶å­ä½éç½® ## âï¸ éç½® ###
-`MCSTAT_FONT` - ä½¿ç¨çå­ä½åç§° / è·¯å¾ é»è®¤ï¼`unifont-15.0.01.ttf`
-è¯·æéèªè¡æ´æ¹ ### `MCSTAT_SHORTCUTS` - å¿«æ·æä»¤åè¡¨
+`MCSTAT_FONT` - ä½¿ç¨çå­ä½åç§° / è·¯å¾ é»è®¤ï¼`unifont`
+è¯·æéèªè¡æ´æ¹ ### `MCSTAT_SHOW_ADDR` -
+æ¯å¦å¨çæçå¾çä¸­æ¾ç¤ºæå¡å¨å°å é»è®¤ï¼`False` ###
+`MCSTAT_SHORTCUTS` - å¿«æ·æä»¤åè¡¨
 è¿ä¸ªéç½®é¡¹è½å¤å¸®å©ä½ ç®åä¸äºæ¥è¯¢æä»¤
 æ­¤éç½®é¡¹çç±»åæ¯ä¸ä¸ªåè¡¨ï¼éé¢çåç´ éè¦ä¸ºä¸ä¸ªç¹å®ç»æçå­å¸
 è¿ä¸ªå­å¸éè¦æä¸ä¸ªåç´  - `regex` -
 ç¨äºå¹éæä»¤çæ­£åï¼ä¾å¦ `^æ¥æ$` ï¼æ³¨æï¼nb2 ä»¥ JSON
 æ ¼å¼è§£æéç½®é¡¹ï¼æä»¥å½ä½ è¦å¨æ­£åè¡¨è¾¾å¼éè¡¨ç¤º`\`æ¶ï¼ä½ éè¦å°å¶è½¬ä¹ä¸º`\\`ï¼
 - `host` - è¦æ¥è¯¢çæå¡å¨å°åï¼æ ¼å¼ä¸º `[:ç«¯å£]`ï¼ ä¾å¦
 `hypixel.net` æ `example.com:1919` - `type` -
@@ -54,19 +56,23 @@
 ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [pil-utils](https://github.com/MeetWq/pil-utils)
 è¶å¥½ç¨ç Pillow è¾å©åºï¼wq ä½¬æ¯å ï¼å¿«å»ç¨ awa ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.0 - å¼ç¨ `nonebot-plugin-
-imageutils`ï¼æ¢ç¨ `pil-utils` - æ¯æäºæ´å¤å­ä½æ ·å¼ -
-æ¯æèªå®ä¹å­ä½ ### 0.2.7 - ä¿®å¤ `shortcut` ç `whitelist`
-çå¥æªè¡¨ç° ### 0.2.6 - ä¿®å¤ `shortcut` ä¸­æ²¡æ `whitelist`
-é¡¹ä¼æ¥éçé®é¢ ### 0.2.5 - `shortcut` å å¥ `whitelist`
-é¡¹éç½®è§¦åç¾¤ç½åå ### 0.2.4 - ä¿®å¤ç©å®¶åè¡¨åºä¸çå¤ä½ç©ºè¡
-### 0.2.3 - ä¿®å¤ JE æå¡å¨ Motd ä¸­ç²ä½æå¤æ¾ç¤ºä¸ºèè²ç bug ###
-0.2.2 - ä¿®å¤ motd ååççç©ºå»ä¸å¹²åçé®é¢ -
-ä¼åç©å®¶åè¡¨æ¾ç¤ºææ ### 0.2.1 - ä¿®å¤å½æå¤§äººæ°ä¸º 0
-æ¶åºéçé®é¢ ### 0.2.0 - å å¥å¿«æ·æä»¤ï¼è¯¦è§éç½®é¡¹ -
-ä¿®å¤æäº JE ææ æ³æ­£ç¡®æ¾ç¤º Motd çé®é¢ - ### 0.1.1 - å°æ¥ JE
-ææ¶ç `æ¸¸æå»¶è¿` å­æ · æ¹ä¸º `æµè¯å»¶è¿`
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.3 -
+ä¿®å¤ç¹æ®æåµä¸ç©å®¶åè¡¨æçéè¯¯çé®é¢ -
+æ·»å æ¾ç¤ºæå¡å¨å°åçéç½®é¡¹ (`MCSTAT_SHOW_ADDR`) ### 0.3.2 - ð
+NoneBot 2.0 ð ### 0.3.1 - ä¿®å¤ææ¬åå«æ `Â§k` æ¶æ¥éçé®é¢ ###
+0.3.0 - å¼ç¨ `nonebot-plugin-imageutils`ï¼æ¢ç¨ `pil-utils` -
+æ¯æäºæ´å¤å­ä½æ ·å¼ - æ¯æèªå®ä¹å­ä½ ### 0.2.7 - ä¿®å¤
+`shortcut` ç `whitelist` çå¥æªè¡¨ç° ### 0.2.6 - ä¿®å¤ `shortcut`
+ä¸­æ²¡æ `whitelist` é¡¹ä¼æ¥éçé®é¢ ### 0.2.5 - `shortcut` å å¥
+`whitelist` é¡¹éç½®è§¦åç¾¤ç½åå ### 0.2.4 -
+ä¿®å¤ç©å®¶åè¡¨åºä¸çå¤ä½ç©ºè¡ ### 0.2.3 - ä¿®å¤ JE æå¡å¨ Motd
+ä¸­ç²ä½æå¤æ¾ç¤ºä¸ºèè²ç bug ### 0.2.2 - ä¿®å¤ motd
+ååççç©ºå»ä¸å¹²åçé®é¢ - ä¼åç©å®¶åè¡¨æ¾ç¤ºææ ### 0.2.1
+- ä¿®å¤å½æå¤§äººæ°ä¸º 0 æ¶åºéçé®é¢ ### 0.2.0 -
+å å¥å¿«æ·æä»¤ï¼è¯¦è§éç½®é¡¹ - ä¿®å¤æäº JE ææ æ³æ­£ç¡®æ¾ç¤º
+Motd çé®é¢ - ### 0.1.1 - å°æ¥ JE ææ¶ç `æ¸¸æå»¶è¿` å­æ · æ¹ä¸º
+`æµè¯å»¶è¿`
```

