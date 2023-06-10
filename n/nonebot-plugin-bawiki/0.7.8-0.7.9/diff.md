# Comparing `tmp/nonebot_plugin_bawiki-0.7.8.tar.gz` & `tmp/nonebot_plugin_bawiki-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.7.8.tar", last modified: Sun Jun  4 17:32:28 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.7.9.tar", last modified: Wed Jun  7 14:22:00 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.7.8.tar` & `nonebot_plugin_bawiki-0.7.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1068 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/LICENSE
--rw-r--r--   0        0        0     7722 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/README.md
--rw-r--r--   0        0        0    14616 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0    22664 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__main__.py
--rw-r--r--   0        0        0     1881 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0     5812 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_bawiki.py
--rw-r--r--   0        0        0     8291 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_gamekee.py
--rw-r--r--   0        0        0    18827 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_schaledb.py
--rw-r--r--   0        0        0     7390 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0    21514 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-06-04 17:15:18.642142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gradient.png
--rw-r--r--   0        0        0      872 2023-06-04 17:15:18.642142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/resource.py
--rw-r--r--   0        0        0     3555 2023-06-04 17:15:18.642142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1379 2023-06-04 17:32:28.667012 nonebot_plugin_bawiki-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     9061 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/LICENSE
+-rw-r--r--   0        0        0     7936 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/README.md
+-rw-r--r--   0        0        0    14616 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0    23189 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/__main__.py
+-rw-r--r--   0        0        0     1814 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0     5812 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_bawiki.py
+-rw-r--r--   0        0        0     8291 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_gamekee.py
+-rw-r--r--   0        0        0    18827 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_schaledb.py
+-rw-r--r--   0        0        0     7390 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/gacha.py
+-rw-r--r--   0        0        0    21514 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gradient.png
+-rw-r--r--   0        0        0      872 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/resource.py
+-rw-r--r--   0        0        0     3555 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1379 2023-06-07 14:22:00.566046 nonebot_plugin_bawiki-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     9275 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.9/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.7.8/LICENSE` & `nonebot_plugin_bawiki-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/README.md` & `nonebot_plugin_bawiki-0.7.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,22 +100,23 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置
 
-|         配置项         | 必填 | 默认值 |                          说明                           |
-| :--------------------: | :--: | :----: | :-----------------------------------------------------: |
-|       `BA_PROXY`       |  否  | `None` | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
-|  `BA_GACHA_COOL_DOWN`  |  否  |  `0`   |               每群每人的抽卡冷却，单位秒                |
-|    `BA_GAMEKEE_URL`    |  否  |  ...   |                  GameKee 数据源的地址                   |
-|    `BA_SCHALE_URL`     |  否  |  ...   |                SchaleDB Json 数据的地址                 |
-| `BA_SCHALE_MIRROR_URL` |  否  |  ...   |                 SchaleDB 网页截图的地址                 |
-|   `BA_BAWIKI_DB_URL`   |  否  |  ...   |                   bawiki-data 的地址                    |
+|         配置项         | 必填 | 默认值  |                          说明                           |
+| :--------------------: | :--: | :-----: | :-----------------------------------------------------: |
+|       `BA_PROXY`       |  否  | `None`  | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
+|  `BA_GACHA_COOL_DOWN`  |  否  |   `0`   |               每群每人的抽卡冷却，单位秒                |
+|  `BA_VOICE_USE_CARD`   |  否  | `False` |           是否使用自定义音乐卡片发送角色语音            |
+|    `BA_GAMEKEE_URL`    |  否  |   ...   |                  GameKee 数据源的地址                   |
+|    `BA_SCHALE_URL`     |  否  |   ...   |                SchaleDB Json 数据的地址                 |
+| `BA_SCHALE_MIRROR_URL` |  否  |   ...   |                 SchaleDB 网页截图的地址                 |
+|   `BA_BAWIKI_DB_URL`   |  否  |   ...   |                   bawiki-data 的地址                    |
 
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
@@ -150,14 +151,22 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.7.9
+
+- 添加配置项 `BA_VOICE_USE_CARD`
+
+### 0.7.8
+
+- 🎉 NoneBot 2.0 🚀
+
 ### 0.7.7
 
 - 修复 bug
 
 ### 0.7.6
 
 - 修复卡池为空不会提示的 bug
```

#### html2text {}

```diff
@@ -16,39 +16,42 @@
 pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
 nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
 conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :----: | :--------------
----------------------------------------: | | `BA_PROXY` | å¦ | `None` | è®¿é®
-`SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :-----: | :-------------
+----------------------------------------: | | `BA_PROXY` | å¦ | `None` |
+è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
 `BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
-`BA_GAMEKEE_URL` | å¦ | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` |
-å¦ | ... | SchaleDB Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ |
-... | SchaleDB ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... |
-bawiki-data çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
+`BA_VOICE_USE_CARD` | å¦ | `False` |
+æ¯å¦ä½¿ç¨èªå®ä¹é³ä¹å¡çåéè§è²è¯­é³ | | `BA_GAMEKEE_URL` | å¦
+| ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` | å¦ | ... | SchaleDB
+Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
+ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
+çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-PicMenu](https:
+//github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
 ä¼èªå¨å¸®ä½ æ PicMenu
 çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
 å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹è¯·ç [\_\_init\_\_.py](https://
 github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/
 __init__.py) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/
 lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)
 é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
 æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5
-- æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
+0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ### 0.7.8 - ð NoneBot 2.0 ð
+### 0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ###
+0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
 ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
 æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
```

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import Cfg as Cfg  # noqa: E402
 
-__version__ = "0.7.8"
+__version__ = "0.7.9"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage="感谢各位 sensei 使用本插件！装载 PicMenu 插件即可查看插件详细菜单哦\n祝玩得愉快～",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki",
     type="application",
     config=Cfg,
-    supported_adapters=["~onebot.v11"],
+    supported_adapters={"~onebot.v11"},
     extra={"License": "MIT", "Author": "student_2333"},
 )
 
 extra_pic_menu = {
     "menu_template": "default",
     "menu_data": [
         {
```

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__main__.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     schale_to_gamekee,
 )
 from .data_gamekee import (
     GameKeeVoice,
     game_kee_calender,
     game_kee_get_page,
     game_kee_get_stu_cid_li,
+    game_kee_get_stu_li,
     game_kee_get_voice,
     game_kee_grab_l2d,
     game_kee_page_url,
 )
 from .data_schaledb import (
     draw_fav_li,
     find_current_event,
@@ -535,48 +536,64 @@
 
     arg = arg.split()
     arg_len = len(arg)
     name = " ".join(arg[:-1]) if arg_len > 1 else arg[0]
     v_type = arg[-1].strip().lower() if arg_len > 1 else None
 
     try:
-        ret = await game_kee_get_stu_cid_li()
+        ret = await game_kee_get_stu_li()
     except:
         logger.exception("获取学生列表出错")
         await matcher.finish("获取学生列表出错，请检查后台输出")
 
     if not ret:
         await matcher.finish("没有获取到学生列表数据")
 
     try:
         org_stu_name = await recover_stu_alia(name, True)
         stu_name = await schale_to_gamekee(org_stu_name)
     except:
         logger.exception("还原学生别名失败")
         await matcher.finish("还原学生别名失败，请检查后台输出")
 
-    if not (sid := ret.get(stu_name)):
+    if not (stu_info := ret.get(stu_name)):
         await matcher.finish("未找到该学生")
 
-    voices = await game_kee_get_voice(sid)
+    voices = await game_kee_get_voice(stu_info["content_id"])
     if v_type:
         voices = [x for x in voices if v_type in x.title.lower()]
     if not voices:
         await matcher.finish("没找到符合要求的语音捏")
 
     v: GameKeeVoice = random.choice(voices)
-    v_data = await async_req(v.url, raw=True)
 
     im = [f"学生 {org_stu_name} 语音 {v.title}\n-=-=-=-=-=-=-=-"]
     if v.jp:
         im.append(v.jp)
     if v.cn:
         im.append(v.cn)
     await matcher.send("\n".join(im))
-    await matcher.send(MessageSegment.record(v_data))
+    if config.ba_voice_use_card:
+        await matcher.send(
+            MessageSegment(
+                "music",
+                {
+                    "type": "custom",
+                    "subtype": "163",
+                    "url": v.url,
+                    "voice": v.url,
+                    "title": v.title,
+                    "content": org_stu_name,
+                    "image": f'http:{stu_info["icon"]}',
+                },
+            ),
+        )
+    else:
+        v_data = await async_req(v.url, raw=True)
+        await matcher.send(MessageSegment.record(v_data))
 
 
 def get_1st_pool(data: dict) -> Optional[GachaPool]:
     if not data:
         return None
 
     pool_data = data["current_pools"]
```

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 from pil_utils.fonts import get_proper_font
 from pydantic import BaseModel, validator
 
 
 class Cfg(BaseModel):
     ba_proxy: Optional[str] = None
     ba_gacha_cool_down: int = 0
+    ba_voice_use_card: bool = False
 
-    ba_gamekee_url = "https://ba.gamekee.com/"
-    ba_schale_url = "https://schale.lgc.cyberczy.xyz/"
-    ba_schale_mirror_url = "https://schale.lgc.cyberczy.xyz/"
-    ba_bawiki_db_url = "https://bawiki.lgc.cyberczy.xyz/"
-
-    @validator("ba_gamekee_url", allow_reuse=True)  # type: ignore
-    @validator("ba_schale_url", allow_reuse=True)  # type: ignore
-    @validator("ba_schale_mirror_url", allow_reuse=True)  # type: ignore
-    @validator("ba_bawiki_db_url", allow_reuse=True)  # type: ignore
+    ba_gamekee_url: str = "https://ba.gamekee.com/"
+    ba_schale_url: str = "https://schale.lgc.cyberczy.xyz/"
+    ba_schale_mirror_url: str = "https://schale.lgc.cyberczy.xyz/"
+    ba_bawiki_db_url: str = "https://bawiki.lgc.cyberczy.xyz/"
+
+    @validator(
+        "ba_gamekee_url",
+        "ba_schale_url",
+        "ba_schale_mirror_url",
+        "ba_bawiki_db_url",
+    )
     def _(cls, val: str):  # noqa: N805
         if not ((val.startswith(("https://", "http://"))) and val.endswith("/")):
             raise ValueError('自定义的 URL 请以 "http(s)://" 开头，以 "/" 结尾')
+        return val
 
 
 config = Cfg.parse_obj(get_driver().config.dict())
 
 
 # 给 PicMenu 用户上个默认字体
 def set_pic_menu_font():
```

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_bawiki.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_gamekee.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_schaledb.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_schaledb.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/calender_banner.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_new.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_star.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gradient.png` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/resource.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.8/pyproject.toml` & `nonebot_plugin_bawiki-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.7.8"
+version = "0.7.9"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.3",
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_bawiki-0.7.8/PKG-INFO` & `nonebot_plugin_bawiki-0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.7.8
+Version: 0.7.9
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -132,22 +132,23 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置
 
-|         配置项         | 必填 | 默认值 |                          说明                           |
-| :--------------------: | :--: | :----: | :-----------------------------------------------------: |
-|       `BA_PROXY`       |  否  | `None` | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
-|  `BA_GACHA_COOL_DOWN`  |  否  |  `0`   |               每群每人的抽卡冷却，单位秒                |
-|    `BA_GAMEKEE_URL`    |  否  |  ...   |                  GameKee 数据源的地址                   |
-|    `BA_SCHALE_URL`     |  否  |  ...   |                SchaleDB Json 数据的地址                 |
-| `BA_SCHALE_MIRROR_URL` |  否  |  ...   |                 SchaleDB 网页截图的地址                 |
-|   `BA_BAWIKI_DB_URL`   |  否  |  ...   |                   bawiki-data 的地址                    |
+|         配置项         | 必填 | 默认值  |                          说明                           |
+| :--------------------: | :--: | :-----: | :-----------------------------------------------------: |
+|       `BA_PROXY`       |  否  | `None`  | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
+|  `BA_GACHA_COOL_DOWN`  |  否  |   `0`   |               每群每人的抽卡冷却，单位秒                |
+|  `BA_VOICE_USE_CARD`   |  否  | `False` |           是否使用自定义音乐卡片发送角色语音            |
+|    `BA_GAMEKEE_URL`    |  否  |   ...   |                  GameKee 数据源的地址                   |
+|    `BA_SCHALE_URL`     |  否  |   ...   |                SchaleDB Json 数据的地址                 |
+| `BA_SCHALE_MIRROR_URL` |  否  |   ...   |                 SchaleDB 网页截图的地址                 |
+|   `BA_BAWIKI_DB_URL`   |  否  |   ...   |                   bawiki-data 的地址                    |
 
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
@@ -182,14 +183,22 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.7.9
+
+- 添加配置项 `BA_VOICE_USE_CARD`
+
+### 0.7.8
+
+- 🎉 NoneBot 2.0 🚀
+
 ### 0.7.7
 
 - 修复 bug
 
 ### 0.7.6
 
 - 修复卡池为空不会提示的 bug
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.8 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.9 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -35,39 +35,42 @@
 pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
 nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
 conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :----: | :--------------
----------------------------------------: | | `BA_PROXY` | å¦ | `None` | è®¿é®
-`SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :-----: | :-------------
+----------------------------------------: | | `BA_PROXY` | å¦ | `None` |
+è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
 `BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
-`BA_GAMEKEE_URL` | å¦ | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` |
-å¦ | ... | SchaleDB Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ |
-... | SchaleDB ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... |
-bawiki-data çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
+`BA_VOICE_USE_CARD` | å¦ | `False` |
+æ¯å¦ä½¿ç¨èªå®ä¹é³ä¹å¡çåéè§è²è¯­é³ | | `BA_GAMEKEE_URL` | å¦
+| ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` | å¦ | ... | SchaleDB
+Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
+ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
+çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-PicMenu](https:
+//github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
 ä¼èªå¨å¸®ä½ æ PicMenu
 çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
 å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹è¯·ç [\_\_init\_\_.py](https://
 github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/
 __init__.py) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/
 lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)
 é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
 æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5
-- æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
+0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ### 0.7.8 - ð NoneBot 2.0 ð
+### 0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ###
+0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
 ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
 æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
```

