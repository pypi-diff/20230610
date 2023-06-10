# Comparing `tmp/nonebot_plugin_learning_chat-0.2.2.tar.gz` & `tmp/nonebot_plugin_learning_chat-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_learning_chat-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_learning_chat-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_learning_chat-0.2.2.tar` & `nonebot_plugin_learning_chat-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    34523 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/LICENSE
--rw-r--r--   0        0        0     8329 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/README.md
--rw-r--r--   0        0        0     3494 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/__init__.py
--rw-r--r--   0        0        0     4168 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/config.py
--rw-r--r--   0        0        0     6587 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/genshin_word.txt
--rw-r--r--   0        0        0    28458 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/handler.py
--rw-r--r--   0        0        0     4780 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/models.py
--rw-r--r--   0        0        0    14386 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/web_api.py
--rw-r--r--   0        0        0    27832 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/web_page.py
--rw-r--r--   0        0        0      705 2023-02-21 15:14:30.312839 nonebot_plugin_learning_chat-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     9372 1970-01-01 00:00:00.000000 nonebot_plugin_learning_chat-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7613 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/README.md
+-rw-r--r--   0        0        0     3594 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/__init__.py
+-rw-r--r--   0        0        0     4484 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/config.py
+-rw-r--r--   0        0        0     6587 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/genshin_word.txt
+-rw-r--r--   0        0        0    30556 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/handler.py
+-rw-r--r--   0        0        0     4831 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/models.py
+-rw-r--r--   0        0        0    14892 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_api.py
+-rw-r--r--   0        0        0    26485 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_page.py
+-rw-r--r--   0        0        0      734 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8660 1970-01-01 00:00:00.000000 nonebot_plugin_learning_chat-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/LICENSE` & `nonebot_plugin_learning_chat-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_learning_chat-0.2.2/README.md` & `nonebot_plugin_learning_chat-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,52 +30,19 @@
 
 本插件还配备了一个`Web UI`后台管理供Bot主人修改配置，支持**分群**配置。
 
 本插件仅适用于`OneBot V11`适配器和**群聊**。
 
 ## 💿 安装
 
-<details>
-<summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
-    nb plugin install nonebot-plugin-learning-chat
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-learning-chat
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-learning-chat
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-learning-chat
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-learning-chat
-</details>
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
-
-    nonebot.load_plugin('nonebot_plugin_learning_chat')
-
-</details>
+```shell
+nb plugin install nonebot-plugin-learning-chat
+```
 
 ## ☀️ 指令
 不同于其它的命令式插件，本插件只有2个命令用于在群聊里管理Bot。
 
 |   指令    |             示例              |                         作用                          |
 |:-------:|:---------------------------:|:---------------------------------------------------:|
 | 开启\关闭学习 | @bot 开启学习\学说话\快学\关闭学习\别学\闭嘴 |                开启或关闭该群的学习能力(需艾特机器人)                 |
```

#### html2text {}

```diff
@@ -4,24 +4,17 @@
                         â¨_ [license] [pypi] [python]
 ## ð ä»ç»
 ä¸ä¸ªè½å¤è®©Botæ ¹æ®ç¾¤åçè§å¾æ§åè¨ï¼èªå¨éæ©åå²è¯­å½æèè¡¨æåè¿è¡åå¤çå­¦ä¹ æä»¶ã
 å®è£å®æ¬æä»¶åå¹¶ä¸ä¼é©¬ä¸æææï¼éè¦ç»Botä¸æ®µæ¶é´ç§¯ç´¯ç¾¤èè®°å½ã
 å­¦å°ä¸å®ç¨åº¦åï¼æä»¶å°±ä¼åæè¯å çï¼~~æç¾¤åä»¬çå¥æªåè¨åè¡¨æåééæ¢è¿æ¥~~ã
 æ¬æä»¶è¿éå¤äºä¸ä¸ª`Web
 UI`åå°ç®¡çä¾Botä¸»äººä¿®æ¹éç½®ï¼æ¯æ**åç¾¤**éç½®ã
-æ¬æä»¶ä»éç¨äº`OneBot V11`ééå¨å**ç¾¤è**ã ## ð¿ å®è£
-ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-learning-chat
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-learning-chat   pdm pdm add nonebot-plugin-
-learning-chat   poetry poetry add nonebot-plugin-learning-chat   conda conda
-install nonebot-plugin-learning-chat  æå¼ nonebot2 é¡¹ç®ç `bot.py`
-æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin('nonebot_plugin_learning_chat')  ##
-âï¸ æä»¤
+æ¬æä»¶ä»éç¨äº`OneBot V11`ééå¨å**ç¾¤è**ã ## ð¿ å®è£ å¨
+nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
+```shell nb plugin install nonebot-plugin-learning-chat ``` ## âï¸ æä»¤
 ä¸åäºå¶å®çå½ä»¤å¼æä»¶ï¼æ¬æä»¶åªæ2ä¸ªå½ä»¤ç¨äºå¨ç¾¤èéç®¡çBotã
 | æä»¤ | ç¤ºä¾ | ä½ç¨ | |:-------:|:---------------------------:|:--------
 -------------------------------------------:| | å¼å¯\å³é­å­¦ä¹  | @bot
 å¼å¯å­¦ä¹ \å­¦è¯´è¯\å¿«å­¦\å³é­å­¦ä¹ \å«å­¦\é­å´ |
 å¼å¯æå³é­è¯¥ç¾¤çå­¦ä¹ è½å(éè¾ç¹æºå¨äºº) | | ç¦ç¨åå¤ |
 @bot ä¸å¯ä»¥\è¾¾å©\ä¸è½è¯´è¿ |
 å°æå¥å·²å­¦ä¼çåå¤ç»ç¦ç¨æï¼ä»¥åä¸ä¼åè¯´è¿å¥è¯ï¼éè¦æç®¡çåæéèè¾ç¹æºå¨äººå¹¶**åå¤**æºå¨äººçåè¨
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/config.py` & `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,83 +2,87 @@
 from pathlib import Path
 
 from pydantic import BaseModel, Field
 
 from nonebot import get_driver, logger
 from ruamel import yaml
 
-CONFIG_PATH = Path() / 'data' / 'learning_chat' / 'learning_chat.yml'
+CONFIG_PATH = Path() / "data" / "learning_chat" / "learning_chat.yml"
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 driver = get_driver()
 try:
     SUPERUSERS: List[int] = [int(s) for s in driver.config.superusers]
 except Exception:
     SUPERUSERS = []
-    logger.warning('请在.env.prod文件中中配置超级用户SUPERUSERS')
+    logger.warning("请在.env.prod文件中中配置超级用户SUPERUSERS")
 
 try:
     NICKNAME: str = list(driver.config.nickname)[0]
 except Exception:
-    NICKNAME = 'bot'
+    NICKNAME = "bot"
 
 COMMAND_START = driver.config.command_start.copy()
-if '' in COMMAND_START:
-    COMMAND_START.remove('')
+if "" in COMMAND_START:
+    COMMAND_START.remove("")
 
 
 class ChatGroupConfig(BaseModel):
-    enable: bool = Field(True, alias='群聊学习开关')
-    ban_words: List[str] = Field([], alias='屏蔽词')
-    ban_users: List[int] = Field([], alias='屏蔽用户')
-    answer_threshold: int = Field(4, alias='回复阈值')
-    answer_threshold_weights: List[int] = Field([10, 30, 60], alias='回复阈值权重')
-    repeat_threshold: int = Field(3, alias='复读阈值')
-    break_probability: float = Field(0.25, alias='打断复读概率')
-    speak_enable: bool = Field(True, alias='主动发言开关')
-    speak_threshold: int = Field(5, alias='主动发言阈值')
-    speak_min_interval: int = Field(300, alias='主动发言最小间隔')
-    speak_continuously_probability: float = Field(0.5, alias='连续主动发言概率')
-    speak_continuously_max_len: int = Field(3, alias='最大连续主动发言句数')
-    speak_poke_probability: float = Field(0.5, alias='主动发言附带戳一戳概率')
+    enable: bool = Field(default=True, alias="群聊学习开关")
+    ban_words: List[str] = Field(default_factory=list, alias="屏蔽词")
+    ban_users: List[int] = Field(default_factory=list, alias="屏蔽用户")
+    answer_threshold: int = Field(default=4, alias="回复阈值")
+    answer_threshold_weights: List[int] = Field(default=[10, 30, 60], alias="回复阈值权重")
+    repeat_threshold: int = Field(default=3, alias="复读阈值")
+    break_probability: float = Field(default=0.25, alias="打断复读概率")
+    speak_enable: bool = Field(default=True, alias="主动发言开关")
+    speak_threshold: int = Field(default=5, alias="主动发言阈值")
+    speak_min_interval: int = Field(default=300, alias="主动发言最小间隔")
+    speak_continuously_probability: float = Field(default=0.5, alias="连续主动发言概率")
+    speak_continuously_max_len: int = Field(default=3, alias="最大连续主动发言句数")
+    speak_poke_probability: float = Field(default=0.5, alias="主动发言附带戳一戳概率")
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
 
 
 class ChatConfig(BaseModel):
-    total_enable: bool = Field(True, alias='群聊学习总开关')
-    enable_web: bool = Field(True, alias='启用后台管理')
-    web_username: str = Field('chat', alias='后台管理用户名')
-    web_password: str = Field('admin', alias='后台管理密码')
-    web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
-                                alias='后台管理token密钥')
-    ban_words: List[str] = Field([], alias='全局屏蔽词')
-    ban_users: List[int] = Field([], alias='全局屏蔽用户')
-    KEYWORDS_SIZE: int = Field(3, alias='单句关键词分词数量')
-    cross_group_threshold: int = Field(3, alias='跨群回复阈值')
-    learn_max_count: int = Field(6, alias='最高学习次数')
-    dictionary: List[str] = Field([], alias='自定义词典')
-    group_config: Dict[int, ChatGroupConfig] = Field({}, alias='分群配置')
+    total_enable: bool = Field(default=True, alias="群聊学习总开关")
+    enable_web: bool = Field(default=True, alias="启用后台管理")
+    web_username: str = Field(default="chat", alias="后台管理用户名")
+    web_password: str = Field(default="admin", alias="后台管理密码")
+    web_secret_key: str = Field(
+        default="49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0",
+        alias="后台管理token密钥",
+    )
+    ban_words: List[str] = Field(default_factory=list, alias="全局屏蔽词")
+    ban_users: List[int] = Field(default_factory=list, alias="全局屏蔽用户")
+    KEYWORDS_SIZE: int = Field(default=3, alias="单句关键词分词数量")
+    cross_group_threshold: int = Field(default=3, alias="跨群回复阈值")
+    learn_max_count: int = Field(default=6, alias="最高学习次数")
+    dictionary: List[str] = Field(default_factory=list, alias="自定义词典")
+    group_config: Dict[int, ChatGroupConfig] = Field(default_factory=dict, alias="分群配置")
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
 
 
 class ChatConfigManager:
-
     def __init__(self):
         self.file_path = CONFIG_PATH
         if self.file_path.exists():
             self.config = ChatConfig.parse_obj(
-                yaml.load(self.file_path.read_text(encoding='utf-8'), Loader=yaml.Loader))
+                yaml.load(
+                    self.file_path.read_text(encoding="utf-8"), Loader=yaml.Loader
+                )
+            )
         else:
             self.config = ChatConfig()
         self.save()
 
     def get_group_config(self, group_id: int) -> ChatGroupConfig:
         if group_id not in self.config.group_config:
             self.config.group_config[group_id] = ChatGroupConfig()
@@ -86,25 +90,26 @@
         return self.config.group_config[group_id]
 
     @property
     def config_list(self) -> List[str]:
         return list(self.config.dict(by_alias=True).keys())
 
     def save(self):
-        with self.file_path.open('w', encoding='utf-8') as f:
+        with self.file_path.open("w", encoding="utf-8") as f:
             yaml.dump(
                 self.config.dict(by_alias=True),
                 f,
                 indent=2,
                 Dumper=yaml.RoundTripDumper,
-                allow_unicode=True)
+                allow_unicode=True,
+            )
 
 
 config_manager = ChatConfigManager()
 
 
 def log_debug(command: str, info: str):
-    logger.opt(colors=True).debug(f'<u><y>[{command}]</y></u>{info}')
+    logger.opt(colors=True).debug(f"<u><y>[{command}]</y></u>{info}")
 
 
 def log_info(command: str, info: str):
-    logger.opt(colors=True).info(f'<u><y>[{command}]</y></u>{info}')
+    logger.opt(colors=True).info(f"<u><y>[{command}]</y></u>{info}")
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/genshin_word.txt` & `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/genshin_word.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/handler.py` & `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,25 +11,43 @@
     import jieba.analyse as jieba_analyse
 from typing import List, Union, Optional, Tuple
 from enum import IntEnum, auto
 from nonebot import get_bot
 from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, ActionFailed
 from tortoise.functions import Count
 from .models import ChatBlackList, ChatContext, ChatAnswer, ChatMessage
-from .config import config_manager, SUPERUSERS, NICKNAME, COMMAND_START, log_info, log_debug
+from .config import (
+    config_manager,
+    SUPERUSERS,
+    NICKNAME,
+    COMMAND_START,
+    log_info,
+    log_debug,
+)
 
 chat_config = config_manager.config
 
-NO_PERMISSION_WORDS = [f'{NICKNAME}就喜欢说这个，哼！', f'你管得着{NICKNAME}吗！']
-ENABLE_WORDS = [f'{NICKNAME}会尝试学你们说怪话！', f'好的呢，让{NICKNAME}学学你们的说话方式~']
-DISABLE_WORDS = [f'好好好，{NICKNAME}不学说话就是了！', f'果面呐噻，{NICKNAME}以后不学了...']
-SORRY_WORDS = [f'{NICKNAME}知道错了...达咩!', f'{NICKNAME}不会再这么说了...', f'果面呐噻,{NICKNAME}说错话了...']
-DOUBT_WORDS = [f'{NICKNAME}有说什么奇怪的话吗？']
-BREAK_REPEAT_WORDS = ['打断复读', '打断！']
-ALL_WORDS = NO_PERMISSION_WORDS + SORRY_WORDS + DOUBT_WORDS + ENABLE_WORDS + DISABLE_WORDS + BREAK_REPEAT_WORDS
+NO_PERMISSION_WORDS = [f"{NICKNAME}就喜欢说这个，哼！", f"你管得着{NICKNAME}吗！"]
+ENABLE_WORDS = [f"{NICKNAME}会尝试学你们说怪话！", f"好的呢，让{NICKNAME}学学你们的说话方式~"]
+DISABLE_WORDS = [f"好好好，{NICKNAME}不学说话就是了！", f"果面呐噻，{NICKNAME}以后不学了..."]
+SORRY_WORDS = [
+    f"{NICKNAME}知道错了...达咩!",
+    f"{NICKNAME}不会再这么说了...",
+    f"果面呐噻,{NICKNAME}说错话了...",
+]
+DOUBT_WORDS = [f"{NICKNAME}有说什么奇怪的话吗？"]
+BREAK_REPEAT_WORDS = ["打断复读", "打断！"]
+ALL_WORDS = (
+    NO_PERMISSION_WORDS
+    + SORRY_WORDS
+    + DOUBT_WORDS
+    + ENABLE_WORDS
+    + DISABLE_WORDS
+    + BREAK_REPEAT_WORDS
+)
 
 
 class Result(IntEnum):
     Learn = auto()
     Pass = auto()
     Repeat = auto()
     Ban = auto()
@@ -41,265 +59,330 @@
     def __init__(self, event: GroupMessageEvent):
         if event.reply:
             self.reply = event.reply
             self.data = ChatMessage(
                 group_id=event.group_id,
                 user_id=event.user_id,
                 message_id=event.message_id,
-                message=re.sub(r'(\[CQ:at,qq=.+])|(\[CQ:reply,id=.+])', '',
-                               re.sub(r'(,subType=\d+,url=.+])', r']', event.raw_message)).strip(),
+                message=re.sub(
+                    r"(\[CQ:at,qq=.+])|(\[CQ:reply,id=.+])",
+                    "",
+                    re.sub(r"(,subType=\d+,url=.+])", r"]", event.raw_message),
+                ).strip(),
                 raw_message=event.raw_message,
                 plain_text=event.get_plaintext(),
-                time=event.time
+                time=event.time,
             )
         else:
             self.data = ChatMessage(
                 group_id=event.group_id,
                 user_id=event.user_id,
                 message_id=event.message_id,
-                message=re.sub(r'(\[CQ:at,qq=.+])', '',
-                               re.sub(r'(,subType=\d+,url=.+])', r']', event.raw_message)).strip(),
+                message=re.sub(
+                    r"(\[CQ:at,qq=.+])",
+                    "",
+                    re.sub(r"(,subType=\d+,url=.+])", r"]", event.raw_message),
+                ).strip(),
                 raw_message=event.raw_message,
                 plain_text=event.get_plaintext(),
-                time=event.time
+                time=event.time,
             )
             self.reply = None
         self.bot_id = event.self_id
         self.to_me = event.to_me or NICKNAME in self.data.message
-        self.role = 'superuser' if event.user_id in SUPERUSERS else event.sender.role
+        self.role = "superuser" if event.user_id in SUPERUSERS else event.sender.role
         self.config = config_manager.get_group_config(self.data.group_id)
         self.ban_users = set(chat_config.ban_users + self.config.ban_users)
         self.ban_words = set(chat_config.ban_words + self.config.ban_words)
 
     async def _learn(self) -> Result:
-        if self.to_me and any(
-                w in self.data.message for w in {'学说话', '快学', '开启学习'}):
+        if self.to_me and any(w in self.data.message for w in {"学说话", "快学", "开启学习"}):
             return Result.SetEnable
-        elif self.to_me and any(
-                w in self.data.message for w in {'闭嘴', '别学', '关闭学习'}):
+        elif self.to_me and any(w in self.data.message for w in {"闭嘴", "别学", "关闭学习"}):
             return Result.SetDisable
         elif not chat_config.total_enable or not self.config.enable:
-            log_debug('群聊学习', f'➤该群<m>{self.data.group_id}</m>未开启群聊学习，跳过')
+            log_debug("群聊学习", f"➤该群<m>{self.data.group_id}</m>未开启群聊学习，跳过")
             # 如果未开启群聊学习，跳过
             return Result.Pass
         elif COMMAND_START and self.data.message.startswith(tuple(COMMAND_START)):
             # 以命令前缀开头的消息，跳过
-            log_debug('群聊学习', '➤该消息以命令前缀开头，跳过')
+            log_debug("群聊学习", "➤该消息以命令前缀开头，跳过")
             return Result.Pass
         elif self.data.user_id in self.ban_users:
             # 发言人在屏蔽列表中，跳过
-            log_debug('群聊学习', f'➤发言人<m>{self.data.user_id}</m>在屏蔽列表中，跳过')
+            log_debug("群聊学习", f"➤发言人<m>{self.data.user_id}</m>在屏蔽列表中，跳过")
             return Result.Pass
-        elif self.to_me and any(w in self.data.message for w in {'不可以', '达咩', '不能说这'}):
+        elif self.to_me and any(w in self.data.message for w in {"不可以", "达咩", "不能说这"}):
             # 如果是对某句话进行禁言
             return Result.Ban
         elif not await self._check_allow(self.data):
             # 本消息不合法，跳过
-            log_debug('群聊学习', '➤消息未通过校验，跳过')
+            log_debug("群聊学习", "➤消息未通过校验，跳过")
             return Result.Pass
         elif self.reply:
             # 如果是回复消息
-            if not (message := await ChatMessage.filter(message_id=self.reply.message_id).first()):
+            if not (
+                message := await ChatMessage.filter(
+                    message_id=self.reply.message_id
+                ).first()
+            ):
                 # 回复的消息在数据库中有记录
-                log_debug('群聊学习', '➤回复的消息不在数据库中，跳过')
+                log_debug("群聊学习", "➤回复的消息不在数据库中，跳过")
                 return Result.Pass
             if message.user_id in self.ban_users:
                 # 且回复的人不在屏蔽列表中
-                log_debug('群聊学习', '➤回复的人在屏蔽列表中，跳过')
+                log_debug("群聊学习", "➤回复的人在屏蔽列表中，跳过")
                 return Result.Pass
             if not await self._check_allow(message):
                 # 且回复的内容通过校验
-                log_debug('群聊学习', '➤回复的消息未通过校验，跳过')
+                log_debug("群聊学习", "➤回复的消息未通过校验，跳过")
                 return Result.Pass
             # 则将该回复作为该消息的答案
             await self._set_answer(message)
             return Result.Learn
-        elif messages := await ChatMessage.filter(group_id=self.data.group_id, time__gte=self.data.time - 3600).limit(
-                5):
+        elif messages := await ChatMessage.filter(
+            group_id=self.data.group_id, time__gte=self.data.time - 3600
+        ).limit(5):
             # 获取本群一个小时内的最后5条消息
             if messages[0].message == self.data.message:
                 # 判断是否为复读中
-                log_debug('群聊学习', '➤复读中，跳过')
+                log_debug("群聊学习", "➤复读中，跳过")
                 return Result.Repeat
             for message in messages:
                 # 如果5条内有相关信息，就作为该消息的答案
-                if message.user_id not in self.ban_users and set(self.data.keyword_list) & set(
-                        message.keyword_list) and self.data.keyword_list != message.keyword_list and await self._check_allow(
-                    message):
+                if (
+                    message.user_id not in self.ban_users
+                    and set(self.data.keyword_list) & set(message.keyword_list)
+                    and self.data.keyword_list != message.keyword_list
+                    and await self._check_allow(message)
+                ):
                     await self._set_answer(message)
                     return Result.Learn
             # 如果没有相关信息
-            if messages[0].user_id in self.ban_users or not await self._check_allow(messages[0]):
+            if messages[0].user_id in self.ban_users or not await self._check_allow(
+                messages[0]
+            ):
                 # 且最后一条消息的发送者不在屏蔽列表中并通过校验
-                log_debug('群聊学习', '➤最后一条消息未通过校验，跳过')
+                log_debug("群聊学习", "➤最后一条消息未通过校验，跳过")
                 return Result.Pass
             # 则作为最后一条消息的答案
             await self._set_answer(messages[0])
             return Result.Learn
         else:
             # 不符合任何情况，跳过
             return Result.Pass
 
     async def answer(self) -> Optional[List[Union[MessageSegment, str]]]:
         """获取这句话的回复"""
         result = await self._learn()
         await self.data.save()
         if result == Result.Ban:
             # 禁用某句话
-            if self.role not in {'superuser', 'admin', 'owner'}:
+            if self.role not in {"superuser", "admin", "owner"}:
                 # 检查权限
                 return [random.choice(NO_PERMISSION_WORDS)]
             if self.reply:
                 ban_result = await self._ban(message_id=self.reply.message_id)
             else:
                 ban_result = await self._ban()
             if ban_result:
                 return [random.choice(SORRY_WORDS)]
             else:
                 return [random.choice(DOUBT_WORDS)]
         elif result in [Result.SetEnable, Result.SetDisable]:
             # 检查权限
-            if self.role not in {'superuser', 'admin', 'owner'}:
+            if self.role not in {"superuser", "admin", "owner"}:
                 return [random.choice(NO_PERMISSION_WORDS)]
             self.config.update(enable=(result == Result.SetEnable))
             config_manager.config.group_config[self.data.group_id] = self.config
             config_manager.save()
-            log_info('群聊学习',
-                     f'群<m>{self.data.group_id}</m>{"开启" if result == Result.SetEnable else "关闭"}学习功能')
-            return [random.choice(ENABLE_WORDS if result == Result.SetEnable else DISABLE_WORDS)]
+            log_info(
+                "群聊学习",
+                f'群<m>{self.data.group_id}</m>{"开启" if result == Result.SetEnable else "关闭"}学习功能',
+            )
+            return [
+                random.choice(
+                    ENABLE_WORDS if result == Result.SetEnable else DISABLE_WORDS
+                )
+            ]
         elif result == Result.Pass:
             # 跳过
             return None
         elif result == Result.Repeat:
-            if await ChatMessage.filter(group_id=self.data.group_id,
-                                        time__gte=self.data.time - 3600).limit(
-                self.config.repeat_threshold + 5).filter(
-                user_id=self.bot_id, message=self.data.message).exists():
+            if (
+                await ChatMessage.filter(
+                    group_id=self.data.group_id, time__gte=self.data.time - 3600
+                )
+                .limit(self.config.repeat_threshold + 5)
+                .filter(user_id=self.bot_id, message=self.data.message)
+                .exists()
+            ):
                 # 如果在阈值+5条消息内，bot已经回复过这句话，则跳过
-                log_debug('群聊学习', '➤➤已经复读过了，跳过')
+                log_debug("群聊学习", "➤➤已经复读过了，跳过")
                 return None
-            if not (messages := await ChatMessage.filter(
-                    group_id=self.data.group_id,
-                    time__gte=self.data.time - 3600).limit(self.config.repeat_threshold)):
+            if not (
+                messages := await ChatMessage.filter(
+                    group_id=self.data.group_id, time__gte=self.data.time - 3600
+                ).limit(self.config.repeat_threshold)
+            ):
                 return None
             # 如果达到阈值，且不是全都为同一个人在说，则进行复读
-            if len(messages) >= self.config.repeat_threshold and all(
-                    message.message == self.data.message
-                    for message in messages) and any(message.user_id != self.data.user_id
-                                                     for message in messages):
+            if (
+                len(messages) >= self.config.repeat_threshold
+                and all(message.message == self.data.message for message in messages)
+                and any(message.user_id != self.data.user_id for message in messages)
+            ):
                 if random.random() < self.config.break_probability:
-                    log_debug('群聊学习', '➤➤达到复读阈值，打断复读！')
+                    log_debug("群聊学习", "➤➤达到复读阈值，打断复读！")
                     return [random.choice(BREAK_REPEAT_WORDS)]
                 else:
-                    log_debug('群聊学习', f'➤➤达到复读阈值，复读<m>{messages[0].message}</m>')
+                    log_debug("群聊学习", f"➤➤达到复读阈值，复读<m>{messages[0].message}</m>")
                     return [self.data.message]
             return None
         else:
             # 回复
             if self.data.is_plain_text and len(self.data.plain_text) <= 1:
-                log_debug('群聊学习', '➤➤消息过短，不回复')
+                log_debug("群聊学习", "➤➤消息过短，不回复")
                 return None
-            if not (context := await ChatContext.filter(keywords=self.data.keywords).first()):
-                log_debug('群聊学习', '➤➤尚未有已学习的回复，不回复')
+            if not (
+                context := await ChatContext.filter(keywords=self.data.keywords).first()
+            ):
+                log_debug("群聊学习", "➤➤尚未有已学习的回复，不回复")
                 return None
 
             # 获取回复阈值
             if not self.to_me:
                 answer_choices = list(
-                    range(self.config.answer_threshold - len(self.config.answer_threshold_weights) + 1,
-                          self.config.answer_threshold + 1))
-
-                answer_count_threshold = random.choices(answer_choices, weights=self.config.answer_threshold_weights)[0]
+                    range(
+                        self.config.answer_threshold
+                        - len(self.config.answer_threshold_weights)
+                        + 1,
+                        self.config.answer_threshold + 1,
+                    )
+                )
+
+                answer_count_threshold = random.choices(
+                    answer_choices, weights=self.config.answer_threshold_weights
+                )[0]
 
                 if len(self.data.keyword_list) == chat_config.KEYWORDS_SIZE:
                     answer_count_threshold -= 1
                 cross_group_threshold = chat_config.cross_group_threshold
             else:
                 answer_count_threshold = 1
                 cross_group_threshold = 1
-            log_debug('群聊学习',
-                      f'➤➤本次回复阈值为<m>{answer_count_threshold}</m>，跨群阈值为<m>{cross_group_threshold}</m>')
+            log_debug(
+                "群聊学习",
+                f"➤➤本次回复阈值为<m>{answer_count_threshold}</m>，跨群阈值为<m>{cross_group_threshold}</m>",
+            )
             # 获取满足跨群条件的回复
-            answers_cross = await ChatAnswer.filter(context=context, count__gte=answer_count_threshold,
-                                                    keywords__in=await ChatAnswer.annotate(
-                                                        cross=Count('keywords')).group_by('keywords').filter(
-                                                        cross__gte=cross_group_threshold).values_list('keywords',
-                                                                                                      flat=True))
+            answers_cross = await ChatAnswer.filter(
+                context=context,
+                count__gte=answer_count_threshold,
+                keywords__in=await ChatAnswer.annotate(cross=Count("keywords"))
+                .group_by("keywords")
+                .filter(cross__gte=cross_group_threshold)
+                .values_list("keywords", flat=True),
+            )
 
-            answer_same_group = await ChatAnswer.filter(context=context, count__gte=answer_count_threshold,
-                                                        group_id=self.data.group_id)
+            answer_same_group = await ChatAnswer.filter(
+                context=context,
+                count__gte=answer_count_threshold,
+                group_id=self.data.group_id,
+            )
 
             candidate_answers: List[Optional[ChatAnswer]] = []
             # 检查候选回复是否在屏蔽列表中
             for answer in set(answers_cross) | set(answer_same_group):
                 if not await self._check_allow(answer):
                     continue
                 # if answer_count_threshold > 0:
                 #     answer.count -= answer_count_threshold - 1
                 candidate_answers.append(answer)
             if not candidate_answers:
-                log_debug('群聊学习', '➤➤没有符合条件的候选回复')
+                log_debug("群聊学习", "➤➤没有符合条件的候选回复")
                 return None
 
             # 从候选回复中进行选择
             sum_count = sum(answer.count for answer in candidate_answers)
-            per_list = [answer.count / sum_count * (1 - 1 / answer.count) for answer in candidate_answers]
+            per_list = [
+                answer.count / sum_count * (1 - 1 / answer.count)
+                for answer in candidate_answers
+            ]
 
             per_list.append(1 - sum(per_list))
             answer_dict = tuple(zip(candidate_answers, per_list))
-            log_debug('群聊学习',
-                      f'➤➤候选回复有<m>{"|".join([f"""{a.keywords}({round(p, 3)})""" for a, p in answer_dict])}|不回复({round(per_list[-1], 3)})</m>')
+            log_debug(
+                "群聊学习",
+                f'➤➤候选回复有<m>{"|".join([f"""{a.keywords}({round(p, 3)})""" for a, p in answer_dict])}|不回复({round(per_list[-1], 3)})</m>',
+            )
 
-            if (result := random.choices(candidate_answers + [None], weights=per_list)[0]) is None:
-                log_debug('群聊学习', '➤➤但不进行回复')
+            if (
+                result := random.choices(candidate_answers + [None], weights=per_list)[
+                    0
+                ]
+            ) is None:
+                log_debug("群聊学习", "➤➤但不进行回复")
                 return None
             result_message = random.choice(result.messages)
-            log_debug('群聊学习', f'➤➤将回复<m>{result_message}</m>')
+            log_debug("群聊学习", f"➤➤将回复<m>{result_message}</m>")
             await asyncio.sleep(random.random() + 0.5)
             return [result_message]
 
     async def _ban(self, message_id: Optional[int] = None) -> bool:
         """屏蔽消息"""
         bot = get_bot()
         if message_id:
-            if not (message := await ChatMessage.filter(message_id=message_id).first()) or message.message in ALL_WORDS:
+            if (
+                not (message := await ChatMessage.filter(message_id=message_id).first())
+                or message.message in ALL_WORDS
+            ):
                 return False
             keywords = message.keywords
             try:
                 await bot.delete_msg(message_id=message_id)
             except ActionFailed:
-                log_info('群聊学习', f'待禁用消息<m>{message_id}</m>尝试撤回<r>失败</r>')
-        elif (last_reply := await ChatMessage.filter(group_id=self.data.group_id, user_id=self.bot_id).first()) and (
-                last_reply.message not in ALL_WORDS):
+                log_info("群聊学习", f"待禁用消息<m>{message_id}</m>尝试撤回<r>失败</r>")
+        elif (
+            last_reply := await ChatMessage.filter(
+                group_id=self.data.group_id, user_id=self.bot_id
+            ).first()
+        ) and (last_reply.message not in ALL_WORDS):
             # 没有指定消息ID，则屏蔽最后一条回复
             keywords = last_reply.keywords
             try:
                 await bot.delete_msg(message_id=last_reply.message_id)
             except ActionFailed:
-                log_info('群聊学习', f'待禁用消息<m>{last_reply.message_id}</m>尝试撤回<r>失败</r>')
+                log_info("群聊学习", f"待禁用消息<m>{last_reply.message_id}</m>尝试撤回<r>失败</r>")
         else:
             return False
         if ban_word := await ChatBlackList.filter(keywords=keywords).first():
             # 如果已有屏蔽记录
             if self.data.group_id not in ban_word.ban_group_id:
                 # 如果不在屏蔽群列表中，则添加
                 ban_word.ban_group_id.append(self.data.group_id)
             if len(ban_word.ban_group_id) >= 2:
                 # 如果有超过2个群都屏蔽了该条消息，则全局屏蔽
                 ban_word.global_ban = True
-                log_info('群聊学习', f'学习词<m>{keywords}</m>将被全局禁用')
+                log_info("群聊学习", f"学习词<m>{keywords}</m>将被全局禁用")
                 await ChatAnswer.filter(keywords=keywords).delete()
             else:
-                log_info('群聊学习', f'群<m>{self.data.group_id}</m>禁用了学习词<m>{keywords}</m>')
-                await ChatAnswer.filter(keywords=keywords, group_id=self.data.group_id).delete()
+                log_info("群聊学习", f"群<m>{self.data.group_id}</m>禁用了学习词<m>{keywords}</m>")
+                await ChatAnswer.filter(
+                    keywords=keywords, group_id=self.data.group_id
+                ).delete()
         else:
             # 没有屏蔽记录，则新建
-            log_info('群聊学习', f'群<m>{self.data.group_id}</m>禁用了学习词<m>{keywords}</m>')
-            ban_word = ChatBlackList(keywords=keywords, ban_group_id=[self.data.group_id])
-            await ChatAnswer.filter(keywords=keywords, group_id=self.data.group_id).delete()
+            log_info("群聊学习", f"群<m>{self.data.group_id}</m>禁用了学习词<m>{keywords}</m>")
+            ban_word = ChatBlackList(
+                keywords=keywords, ban_group_id=[self.data.group_id]
+            )
+            await ChatAnswer.filter(
+                keywords=keywords, group_id=self.data.group_id
+            ).delete()
         await ChatContext.filter(keywords=keywords).delete()
         await ban_word.save()
         return True
 
     @staticmethod
     async def add_ban(data: Union[ChatMessage, ChatContext, ChatAnswer]):
         if ban_word := await ChatBlackList.filter(keywords=data.keywords).first():
@@ -307,201 +390,291 @@
             if isinstance(data, ChatMessage):
                 if data.group_id not in ban_word.ban_group_id:
                     # 如果不在屏蔽群列表中，则添加
                     ban_word.ban_group_id.append(data.group_id)
                 if len(ban_word.ban_group_id) >= 2:
                     # 如果有超过2个群都屏蔽了该条消息，则全局屏蔽
                     ban_word.global_ban = True
-                    log_info('群聊学习', f'学习词<m>{data.keywords}</m>将被全局禁用')
+                    log_info("群聊学习", f"学习词<m>{data.keywords}</m>将被全局禁用")
                     await ChatAnswer.filter(keywords=data.keywords).delete()
                 else:
-                    log_info('群聊学习', f'群<m>{data.group_id}</m>禁用了学习词<m>{data.keywords}</m>')
-                    await ChatAnswer.filter(keywords=data.keywords, group_id=data.group_id).delete()
+                    log_info(
+                        "群聊学习", f"群<m>{data.group_id}</m>禁用了学习词<m>{data.keywords}</m>"
+                    )
+                    await ChatAnswer.filter(
+                        keywords=data.keywords, group_id=data.group_id
+                    ).delete()
             else:
                 ban_word.global_ban = True
-                log_info('群聊学习', f'学习词<m>{data.keywords}</m>将被全局禁用')
+                log_info("群聊学习", f"学习词<m>{data.keywords}</m>将被全局禁用")
                 await ChatAnswer.filter(keywords=data.keywords).delete()
         else:
             # 没有屏蔽记录，则新建
             if isinstance(data, ChatMessage):
-                log_info('群聊学习', f'群<m>{data.group_id}</m>禁用了学习词<m>{data.keywords}</m>')
-                ban_word = ChatBlackList(keywords=data.keywords, ban_group_id=[data.group_id])
-                await ChatAnswer.filter(keywords=data.keywords, group_id=data.group_id).delete()
+                log_info("群聊学习", f"群<m>{data.group_id}</m>禁用了学习词<m>{data.keywords}</m>")
+                ban_word = ChatBlackList(
+                    keywords=data.keywords, ban_group_id=[data.group_id]
+                )
+                await ChatAnswer.filter(
+                    keywords=data.keywords, group_id=data.group_id
+                ).delete()
             else:
-                log_info('群聊学习', f'学习词<m>{data.keywords}</m>将被全局禁用')
+                log_info("群聊学习", f"学习词<m>{data.keywords}</m>将被全局禁用")
                 ban_word = ChatBlackList(keywords=data.keywords, global_ban=True)
                 await ChatAnswer.filter(keywords=data.keywords).delete()
         await ChatContext.filter(keywords=data.keywords).delete()
         await ban_word.save()
 
     @staticmethod
-    async def speak(self_id: int) -> Optional[Tuple[int, List[Union[str, MessageSegment]]]]:
+    async def speak(
+        self_id: int,
+    ) -> Optional[Tuple[int, List[Union[str, MessageSegment]]]]:
         # 主动发言
         cur_time = int(time.time())
         today_time = time.mktime(datetime.date.today().timetuple())
         # 获取两小时内消息超过10条的群列表
-        groups = await ChatMessage.filter(time__gte=today_time).annotate(count=Count('id')).group_by('group_id'). \
-            filter(count__gte=10).values_list('group_id', flat=True)
+        groups = (
+            await ChatMessage.filter(time__gte=today_time)
+            .annotate(count=Count("id"))
+            .group_by("group_id")
+            .filter(count__gte=10)
+            .values_list("group_id", flat=True)
+        )
         if not groups:
             return None
         total_messages = {}
         # 获取这些群的两小时内的所有消息
         for group_id in groups:
-            if messages := await ChatMessage.filter(group_id=group_id, time__gte=today_time):
+            if messages := await ChatMessage.filter(
+                group_id=group_id, time__gte=today_time
+            ):
                 total_messages[group_id] = messages
         if not total_messages:
             return None
 
         # 根据消息平均间隔来对群进行排序
-        def group_popularity_cmp(left_group: Tuple[int, List[ChatMessage]],
-                                 right_group: Tuple[int, List[ChatMessage]]):
+        def group_popularity_cmp(
+            left_group: Tuple[int, List[ChatMessage]],
+            right_group: Tuple[int, List[ChatMessage]],
+        ):
             def cmp(a, b):
                 return (a > b) - (a < b)
 
             left_group_id, left_messages = left_group
             right_group_id, right_messages = right_group
             left_duration = left_messages[0].time - left_messages[-1].time
             right_duration = right_messages[0].time - right_messages[-1].time
-            return cmp(len(left_messages) / left_duration, len(right_messages) / right_duration)
+            return cmp(
+                len(left_messages) / left_duration, len(right_messages) / right_duration
+            )
 
-        popularity: List[Tuple[int, List[ChatMessage]]] = sorted(total_messages.items(),
-                                                                 key=cmp_to_key(group_popularity_cmp), reverse=True)
-        log_debug('群聊学习', f'主动发言：群热度排行<m>{">>".join([str(g[0]) for g in popularity])}</m>')
+        popularity: List[Tuple[int, List[ChatMessage]]] = sorted(
+            total_messages.items(), key=cmp_to_key(group_popularity_cmp), reverse=True
+        )
+        log_debug(
+            "群聊学习", f'主动发言：群热度排行<m>{">>".join([str(g[0]) for g in popularity])}</m>'
+        )
         for group_id, messages in popularity:
             if len(messages) < 30:
-                log_debug('群聊学习', f'主动发言：群<m>{group_id}</m>消息小于30条，不发言')
+                log_debug("群聊学习", f"主动发言：群<m>{group_id}</m>消息小于30条，不发言")
                 continue
 
             config = config_manager.get_group_config(group_id)
             ban_words = set(
-                chat_config.ban_words + config.ban_words + ['[CQ:xml', '[CQ:json', '[CQ:at', '[CQ:video', '[CQ:record',
-                                                            '[CQ:share'])
+                chat_config.ban_words
+                + config.ban_words
+                + [
+                    "[CQ:xml",
+                    "[CQ:json",
+                    "[CQ:at",
+                    "[CQ:video",
+                    "[CQ:record",
+                    "[CQ:share",
+                ]
+            )
 
             # 是否开启了主动发言
             if not config.speak_enable or not config.enable:
-                log_debug('群聊学习', f'主动发言：群<m>{group_id}</m>未开启，不发言')
+                log_debug("群聊学习", f"主动发言：群<m>{group_id}</m>未开启，不发言")
                 continue
 
             # 如果最后一条消息是自己发的，则不主动发言
-            if last_reply := await ChatMessage.filter(group_id=group_id, user_id=self_id).first():
+            if last_reply := await ChatMessage.filter(
+                group_id=group_id, user_id=self_id
+            ).first():
                 if last_reply.time >= messages[0].time:
-                    log_debug('群聊学习',
-                              f'主动发言：群<m>{group_id}</m>最后一条消息是{NICKNAME}发的{last_reply.message}，不发言')
+                    log_debug(
+                        "群聊学习",
+                        f"主动发言：群<m>{group_id}</m>最后一条消息是{NICKNAME}发的{last_reply.message}，不发言",
+                    )
                     continue
                 elif cur_time - last_reply.time < config.speak_min_interval:
-                    log_debug('群聊学习', f'主动发言：群<m>{group_id}</m>上次主动发言时间小于主动发言最小间隔，不发言')
+                    log_debug("群聊学习", f"主动发言：群<m>{group_id}</m>上次主动发言时间小于主动发言最小间隔，不发言")
                     continue
 
             # 该群每多少秒发一条消息
             avg_interval = (messages[0].time - messages[-1].time) / len(messages)
             # 如果该群已沉默的时间小于阈值，则不主动发言
             silent_time = cur_time - messages[0].time
             threshold = avg_interval * config.speak_threshold
             if silent_time < threshold:
-                log_debug('群聊学习',
-                          f'主动发言：群<m>{group_id}</m>已沉默时间({silent_time})小于阈值({int(threshold)})，不发言')
+                log_debug(
+                    "群聊学习",
+                    f"主动发言：群<m>{group_id}</m>已沉默时间({silent_time})小于阈值({int(threshold)})，不发言",
+                )
                 continue
 
-            if contexts := await ChatContext.filter(count__gte=config.answer_threshold).all():
+            if contexts := await ChatContext.filter(
+                count__gte=config.answer_threshold
+            ).all():
                 speak_list = []
                 # context = random.choices(contexts, weights=[context.count for context in contexts])[0]
                 # contexts.sort(key=lambda x: x.count, reverse=True)
                 random.shuffle(contexts)
                 for context in contexts:
-                    if (not speak_list or random.random() < config.speak_continuously_probability) and len(
-                            speak_list) < config.speak_continuously_max_len:
-                        if answers := await ChatAnswer.filter(context=context,
-                                                              group_id=group_id,
-                                                              count__gte=config.answer_threshold):
-                            answer = random.choices(answers,
-                                                    weights=[
-                                                        answer.count + 1 if answer.time >= today_time else answer.count
-                                                        for answer in answers])[0]
+                    if (
+                        not speak_list
+                        or random.random() < config.speak_continuously_probability
+                    ) and len(speak_list) < config.speak_continuously_max_len:
+                        if answers := await ChatAnswer.filter(
+                            context=context,
+                            group_id=group_id,
+                            count__gte=config.answer_threshold,
+                        ):
+                            answer = random.choices(
+                                answers,
+                                weights=[
+                                    answer.count + 1
+                                    if answer.time >= today_time
+                                    else answer.count
+                                    for answer in answers
+                                ],
+                            )[0]
                             message = random.choice(answer.messages)
                             if len(message) < 2:
                                 continue
-                            if message.startswith('&#91;') and message.endswith('&#93;'):
+                            if message.startswith("&#91;") and message.endswith(
+                                "&#93;"
+                            ):
                                 continue
                             if any(word in message for word in ban_words):
                                 continue
                             speak_list.append(message)
                             follow_answer = answer
-                            while random.random() < config.speak_continuously_probability and len(
-                                    speak_list) < config.speak_continuously_max_len:
-                                if (follow_context := await ChatContext.filter(
-                                        keywords=follow_answer.keywords).first()) and (
-                                        follow_answers := await ChatAnswer.filter(
-                                            group_id=group_id,
-                                            context=follow_context,
-                                            count__gte=config.answer_threshold)):
-                                    follow_answer = random.choices(follow_answers,
-                                                                   weights=[
-                                                                       a.count + 1 if a.time >= today_time else a.count
-                                                                       for a in follow_answers])[0]
+                            while (
+                                random.random() < config.speak_continuously_probability
+                                and len(speak_list) < config.speak_continuously_max_len
+                            ):
+                                if (
+                                    follow_context := await ChatContext.filter(
+                                        keywords=follow_answer.keywords
+                                    ).first()
+                                ) and (
+                                    follow_answers := await ChatAnswer.filter(
+                                        group_id=group_id,
+                                        context=follow_context,
+                                        count__gte=config.answer_threshold,
+                                    )
+                                ):
+                                    follow_answer = random.choices(
+                                        follow_answers,
+                                        weights=[
+                                            a.count + 1
+                                            if a.time >= today_time
+                                            else a.count
+                                            for a in follow_answers
+                                        ],
+                                    )[0]
                                     message = random.choice(follow_answer.messages)
                                     if len(message) < 2:
                                         continue
-                                    if message.startswith('&#91;') and message.endswith('&#93;'):
+                                    if message.startswith("&#91;") and message.endswith(
+                                        "&#93;"
+                                    ):
                                         continue
                                     if all(word not in message for word in ban_words):
                                         speak_list.append(message)
                                 else:
                                     break
                     else:
                         break
                 if speak_list:
                     if random.random() < config.speak_poke_probability:
-                        last_speak_users = {message.user_id for message in messages[:5] if message.user_id != self_id}
+                        last_speak_users = {
+                            message.user_id
+                            for message in messages[:5]
+                            if message.user_id != self_id
+                        }
                         select_user = random.choice(list(last_speak_users))
-                        speak_list.append(MessageSegment('poke', {'qq': select_user}))
+                        speak_list.append(MessageSegment("poke", {"qq": select_user}))
                     return group_id, speak_list
                 else:
-                    log_debug('群聊学习', f'主动发言：群<m>{group_id}</m>没有找到符合条件的发言，不发言')
-            log_debug('群聊学习', '主动发言：没有符合条件的群，不主动发言')
+                    log_debug("群聊学习", f"主动发言：群<m>{group_id}</m>没有找到符合条件的发言，不发言")
+            log_debug("群聊学习", "主动发言：没有符合条件的群，不主动发言")
             return None
 
     async def _set_answer(self, message: ChatMessage):
         if context := await ChatContext.filter(keywords=message.keywords).first():
             if context.count < chat_config.learn_max_count:
                 context.count += 1
             context.time = self.data.time
-            if answer := await ChatAnswer.filter(keywords=self.data.keywords,
-                                                 group_id=self.data.group_id,
-                                                 context=context).first():
+            if answer := await ChatAnswer.filter(
+                keywords=self.data.keywords,
+                group_id=self.data.group_id,
+                context=context,
+            ).first():
                 if answer.count < chat_config.learn_max_count:
                     answer.count += 1
                 answer.time = self.data.time
                 if self.data.message not in answer.messages:
                     answer.messages.append(self.data.message)
             else:
-                answer = ChatAnswer(keywords=self.data.keywords,
-                                    group_id=self.data.group_id,
-                                    time=self.data.time,
-                                    context=context,
-                                    messages=[self.data.message])
+                answer = ChatAnswer(
+                    keywords=self.data.keywords,
+                    group_id=self.data.group_id,
+                    time=self.data.time,
+                    context=context,
+                    messages=[self.data.message],
+                )
             await answer.save()
             await context.save()
         else:
-            context = await ChatContext.create(keywords=message.keywords,
-                                               time=self.data.time)
-            answer = await ChatAnswer.create(keywords=self.data.keywords,
-                                             group_id=self.data.group_id,
-                                             time=self.data.time,
-                                             context=context,
-                                             messages=[self.data.message])
-        log_debug('群聊学习', f'➤将被学习为<m>{message.message}</m>的回答，已学次数为<m>{answer.count}</m>')
+            context = await ChatContext.create(
+                keywords=message.keywords, time=self.data.time
+            )
+            answer = await ChatAnswer.create(
+                keywords=self.data.keywords,
+                group_id=self.data.group_id,
+                time=self.data.time,
+                context=context,
+                messages=[self.data.message],
+            )
+        log_debug(
+            "群聊学习", f"➤将被学习为<m>{message.message}</m>的回答，已学次数为<m>{answer.count}</m>"
+        )
 
     async def _check_allow(self, message: Union[ChatMessage, ChatAnswer]) -> bool:
-        raw_message = message.message if isinstance(message, ChatMessage) else message.messages[0]
+        raw_message = (
+            message.message if isinstance(message, ChatMessage) else message.messages[0]
+        )
         # if len(raw_message) < 2:
         #     return False
-        if any(i in raw_message for i in
-               {'[CQ:xml', '[CQ:json', '[CQ:at', '[CQ:video', '[CQ:record', '[CQ:share'}):
+        if any(
+            i in raw_message
+            for i in {
+                "[CQ:xml",
+                "[CQ:json",
+                "[CQ:at",
+                "[CQ:video",
+                "[CQ:record",
+                "[CQ:share",
+            }
+        ):
             return False
         if any(i in raw_message for i in self.ban_words):
             return False
-        if raw_message.startswith('&#91;') and raw_message.endswith('&#93;'):
+        if raw_message.startswith("&#91;") and raw_message.endswith("&#93;"):
             return False
         if ban_word := await ChatBlackList.filter(keywords=message.keywords).first():
             if ban_word.global_ban or message.group_id in ban_word.ban_group_id:
                 return False
         return True
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/models.py` & `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     await self._init_connections()
 
 
 ConnectionHandler._init = _init
 
 config = config_manager.config
 
-DATABASE_PATH = Path() / 'data' / 'learning_chat' / 'learning_chat.db'
+DATABASE_PATH = Path() / "data" / "learning_chat" / "learning_chat.db"
 DATABASE_PATH.parent.mkdir(parents=True, exist_ok=True)
 JSON_DUMPS = functools.partial(json.dumps, ensure_ascii=False)
 jieba.setLogLevel(jieba.logging.INFO)
-jieba.load_userdict(str(Path(__file__).parent / 'genshin_word.txt'))  # 加载原神词典
+jieba.load_userdict(str(Path(__file__).parent / "genshin_word.txt"))  # 加载原神词典
 jieba.load_userdict(config.dictionary)  # 加载用户自定义的词典
 
 
 class ChatMessage(Model):
     id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
     """自增主键"""
     group_id: int = fields.IntField()
@@ -58,54 +58,56 @@
     """原始消息"""
     plain_text: str = fields.TextField()
     """纯文本消息"""
     time: int = fields.IntField()
     """时间戳"""
 
     class Meta:
-        table = 'message'
-        indexes = ('group_id', 'time')
-        ordering = ['-time']
+        table = "message"
+        indexes = ("group_id", "time")
+        ordering = ["-time"]
 
     @cached_property
     def is_plain_text(self) -> bool:
         """是否纯文本"""
-        return '[CQ:' not in self.message
+        return "[CQ:" not in self.message
 
     @cached_property
     def keyword_list(self) -> List[str]:
         """获取纯文本部分的关键词列表"""
         if not self.is_plain_text and not len(self.plain_text):
             return []
         return jieba_analyse.extract_tags(self.plain_text, topK=config.KEYWORDS_SIZE)
 
     @cached_property
     def keywords(self) -> str:
         """获取纯文本部分的关键词结果"""
         if not self.is_plain_text and not len(self.plain_text):
             return self.message
-        return self.message if len(self.keyword_list) < 2 else ' '.join(self.keyword_list)
+        return (
+            self.message if len(self.keyword_list) < 2 else " ".join(self.keyword_list)
+        )
 
 
 class ChatContext(Model):
     id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
     """自增主键"""
     keywords: str = fields.TextField()
     """关键词"""
     time: int = fields.IntField()
     """时间戳"""
     count: int = fields.IntField(default=1)
     """次数"""
-    answers: fields.ReverseRelation['ChatAnswer']
+    answers: fields.ReverseRelation["ChatAnswer"]
     """答案"""
 
     class Meta:
-        table = 'context'
-        indexes = ('keywords', 'time')
-        ordering = ['-time']
+        table = "context"
+        indexes = ("keywords", "time")
+        ordering = ["-time"]
 
 
 class ChatAnswer(Model):
     id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
     """自增主键"""
     keywords: str = fields.TextField()
     """关键词"""
@@ -115,45 +117,48 @@
     """次数"""
     time: int = fields.IntField()
     """时间戳"""
     messages: List[str] = fields.JSONField(encoder=JSON_DUMPS, default=list)
     """消息列表"""
 
     context: fields.ForeignKeyNullableRelation[ChatContext] = fields.ForeignKeyField(
-        'models.ChatContext', related_name='answers', null=True)
+        "models.ChatContext", related_name="answers", null=True
+    )
 
     class Meta:
-        table = 'answer'
-        indexes = ('keywords', 'time')
-        ordering = ['-time']
+        table = "answer"
+        indexes = ("keywords", "time")
+        ordering = ["-time"]
 
 
 class ChatBlackList(Model):
     id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
     """自增主键"""
     keywords: str = fields.TextField()
     """关键词"""
     global_ban: bool = fields.BooleanField(default=False)
     """是否全局禁用"""
     ban_group_id: List[int] = fields.JSONField(default=list)
     """禁用的群id"""
 
     class Meta:
-        table = 'blacklist'
-        indexes = ('keywords',)
+        table = "blacklist"
+        indexes = ("keywords",)
 
 
 @driver.on_startup
 async def startup():
     try:
-        await Tortoise.init(db_url=f'sqlite://{DATABASE_PATH}', modules={'models': [__name__]})
+        await Tortoise.init(
+            db_url=f"sqlite://{DATABASE_PATH}", modules={"models": [__name__]}
+        )
         await Tortoise.generate_schemas()
-        log_info('群聊学习', '数据库连接<g>成功</g>')
+        log_info("群聊学习", "数据库连接<g>成功</g>")
     except Exception as e:
-        log_info('群聊学习', f'数据库连接<r>失败，{e}</r>')
+        log_info("群聊学习", f"数据库连接<r>失败，{e}</r>")
         raise e
 
 
 @driver.on_shutdown
 async def shutdown():
     await Tortoise.close_connections()
-    log_info('群聊学习', '数据库断开连接<g>成功</g>')
+    log_info("群聊学习", "数据库断开连接<g>成功</g>")
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/web_api.py` & `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,41 +14,46 @@
     import jieba
 
 from .handler import LearningChat
 from .models import ChatMessage, ChatContext, ChatAnswer, ChatBlackList
 from .config import config_manager, driver
 from .web_page import login_page, admin_app
 
-requestAdaptor = '''
+requestAdaptor = """
 requestAdaptor(api) {
     api.headers["token"] = localStorage.getItem("token");
     return api;
 },
-'''
-responseAdaptor = '''
+"""
+responseAdaptor = """
 responseAdaptor(api, payload, query, request, response) {
     if (response.data.detail == '登录验证失败或已失效，请重新登录') {
         window.location.href = '/learning_chat/login'
         window.localStorage.clear()
         window.sessionStorage.clear()
         window.alert('登录验证失败或已失效，请重新登录')
     }
     return payload
 },
-'''
+"""
 
 
 def authentication():
     def inner(token: Optional[str] = Header(...)):
         try:
-            payload = jwt.decode(token, config_manager.config.web_secret_key, algorithms='HS256')
-            if not (username := payload.get('username')) or username != config_manager.config.web_username:
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+            payload = jwt.decode(
+                token, config_manager.config.web_secret_key, algorithms="HS256"
+            )
+            if (
+                not (username := payload.get("username"))
+                or username != config_manager.config.web_username
+            ):
+                raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
         except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+            raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
 
     return Depends(inner)
 
 
 class UserModel(BaseModel):
     username: str
     password: str
@@ -56,280 +61,363 @@
 
 @driver.on_startup
 async def init_web():
     if not config_manager.config.enable_web:
         return
     app: FastAPI = get_app()
 
-    @app.post('/learning_chat/api/login', response_class=JSONResponse)
+    @app.post("/learning_chat/api/login", response_class=JSONResponse)
     async def login(user: UserModel):
-        if user.username != config_manager.config.web_username or user.password != config_manager.config.web_password:
-            return {
-                'status': -100,
-                'msg':    '登录失败，请确认用户ID和密码无误'
-            }
-        token = jwt.encode({'username': user.username,
-                            'exp':      datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
-                                minutes=30)}, config_manager.config.web_secret_key, algorithm='HS256')
-        return {
-            'status': 0,
-            'msg':    '登录成功',
-            'data':   {
-                'token': token
-            }
-        }
+        if (
+            user.username != config_manager.config.web_username
+            or user.password != config_manager.config.web_password
+        ):
+            return {"status": -100, "msg": "登录失败，请确认用户ID和密码无误"}
+        token = jwt.encode(
+            {
+                "username": user.username,
+                "exp": datetime.datetime.now(datetime.timezone.utc)
+                + datetime.timedelta(minutes=30),
+            },
+            config_manager.config.web_secret_key,
+            algorithm="HS256",
+        )
+        return {"status": 0, "msg": "登录成功", "data": {"token": token}}
 
-    @app.get('/learning_chat/api/get_group_list', response_class=JSONResponse, dependencies=[authentication()])
+    @app.get(
+        "/learning_chat/api/get_group_list",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def get_group_list_api():
         try:
             group_list = await get_bot().get_group_list()
-            group_list = [{'label': f'{group["group_name"]}({group["group_id"]})', 'value': group['group_id']} for group
-                          in group_list]
-            return {
-                'status': 0,
-                'msg':    'ok',
-                'data':   {
-                    'group_list': group_list
+            group_list = [
+                {
+                    "label": f'{group["group_name"]}({group["group_id"]})',
+                    "value": group["group_id"],
                 }
-            }
+                for group in group_list
+            ]
+            return {"status": 0, "msg": "ok", "data": {"group_list": group_list}}
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
-            }
+            return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
 
-    @app.get('/learning_chat/api/chat_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    @app.get(
+        "/learning_chat/api/chat_global_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def get_chat_global_config():
         try:
             bot = get_bot()
             groups = await bot.get_group_list()
             member_list = []
             for group in groups:
-                members = await bot.get_group_member_list(group_id=group['group_id'])
+                members = await bot.get_group_member_list(group_id=group["group_id"])
                 member_list.extend(
-                    [{'label': f'{member["nickname"] or member["card"]}({member["user_id"]})',
-                      'value': member['user_id']}
-                     for
-                     member in members])
-            config = config_manager.config.dict(exclude={'group_config'})
-            config['member_list'] = member_list
+                    [
+                        {
+                            "label": f'{member["nickname"] or member["card"]}({member["user_id"]})',
+                            "value": member["user_id"],
+                        }
+                        for member in members
+                    ]
+                )
+            config = config_manager.config.dict(exclude={"group_config"})
+            config["member_list"] = member_list
             return config
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
-            }
+            return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
 
-    @app.post('/learning_chat/api/chat_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    @app.post(
+        "/learning_chat/api/chat_global_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def post_chat_global_config(data: dict):
         config_manager.config.update(**data)
         config_manager.save()
-        await ChatContext.filter(count__gt=config_manager.config.learn_max_count).update(
-            count=config_manager.config.learn_max_count)
+        await ChatContext.filter(
+            count__gt=config_manager.config.learn_max_count
+        ).update(count=config_manager.config.learn_max_count)
         await ChatAnswer.filter(count__gt=config_manager.config.learn_max_count).update(
-            count=config_manager.config.learn_max_count)
+            count=config_manager.config.learn_max_count
+        )
         jieba.load_userdict(config_manager.config.dictionary)
-        return {
-            'status': 0,
-            'msg':    '保存成功'
-        }
+        return {"status": 0, "msg": "保存成功"}
 
-    @app.get('/learning_chat/api/chat_group_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_chat_global_config(group_id: int):
+    @app.get(
+        "/learning_chat/api/chat_group_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def get_chat_group_config(group_id: int):
         try:
             members = await get_bot().get_group_member_list(group_id=group_id)
             member_list = [
-                {'label': f'{member["nickname"] or member["card"]}({member["user_id"]})', 'value': member['user_id']}
-                for member in members]
+                {
+                    "label": f'{member["nickname"] or member["card"]}({member["user_id"]})',
+                    "value": member["user_id"],
+                }
+                for member in members
+            ]
             config = config_manager.get_group_config(group_id).dict()
-            config['break_probability'] = config['break_probability'] * 100
-            config['speak_continuously_probability'] = config['speak_continuously_probability'] * 100
-            config['speak_poke_probability'] = config['speak_poke_probability'] * 100
-            config['member_list'] = member_list
+            config["break_probability"] = config["break_probability"] * 100
+            config["speak_continuously_probability"] = (
+                config["speak_continuously_probability"] * 100
+            )
+            config["speak_poke_probability"] = config["speak_poke_probability"] * 100
+            config["member_list"] = member_list
             return config
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
-            }
-
-    @app.post('/learning_chat/api/chat_group_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def post_chat_global_config(group_id: Union[int, str], data: dict):
-        if not data['answer_threshold_weights']:
-            return {
-                'status': 400,
-                'msg':    '回复阈值权重不能为空，必须至少有一个数值'
-            }
-        data['break_probability'] = data['break_probability'] / 100
-        data['speak_continuously_probability'] = data['speak_continuously_probability'] / 100
-        data['speak_poke_probability'] = data['speak_poke_probability'] / 100
+            return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+
+    @app.post(
+        "/learning_chat/api/chat_group_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def post_chat_group_config(group_id: Union[int, str], data: dict):
+        if not data["answer_threshold_weights"]:
+            return {"status": 400, "msg": "回复阈值权重不能为空，必须至少有一个数值"}
+        data["break_probability"] = data["break_probability"] / 100
+        data["speak_continuously_probability"] = (
+            data["speak_continuously_probability"] / 100
+        )
+        data["speak_poke_probability"] = data["speak_poke_probability"] / 100
         groups = (
-            [{'group_id': group_id}]
-            if group_id != 'all'
+            [{"group_id": group_id}]
+            if group_id != "all"
             else await get_bot().get_group_list()
         )
         for group in groups:
-            config = config_manager.get_group_config(group['group_id'])
+            config = config_manager.get_group_config(int(group["group_id"]))
             config.update(**data)
-            config_manager.config.group_config[group['group_id']] = config
+            config_manager.config.group_config[int(group["group_id"])] = config
         config_manager.save()
-        return {
-            'status': 0,
-            'msg':    '保存成功'
-        }
+        return {"status": 0, "msg": "保存成功"}
 
-    @app.get('/learning_chat/api/get_chat_messages', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_chat_messages(page: int = 1,
-                                perPage: int = 10,
-                                orderBy: str = 'time',
-                                orderDir: str = 'desc',
-                                group_id: Optional[str] = None,
-                                user_id: Optional[str] = None,
-                                message: Optional[str] = None):
-        orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
-        filter_args = {f'{k}__contains': v for k, v in
-                       {'group_id': group_id, 'user_id': user_id, 'raw_message': message}.items() if v}
+    @app.get(
+        "/learning_chat/api/get_chat_messages",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def get_chat_messages(
+        page: int = 1,
+        perPage: int = 10,
+        orderBy: str = "time",
+        orderDir: str = "desc",
+        group_id: Optional[str] = None,
+        user_id: Optional[str] = None,
+        message: Optional[str] = None,
+    ):
+        orderBy = (
+            (orderBy or "time")
+            if (orderDir or "desc") == "asc"
+            else f'-{orderBy or "time"}'
+        )
+        filter_args = {
+            f"{k}__contains": v
+            for k, v in {
+                "group_id": group_id,
+                "user_id": user_id,
+                "raw_message": message,
+            }.items()
+            if v
+        }
         return {
-            'status': 0,
-            'msg':    'ok',
-            'data':   {
-                'items': await ChatMessage.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
-                    perPage).values(),
-                'total': await ChatMessage.filter(**filter_args).count()
-            }
+            "status": 0,
+            "msg": "ok",
+            "data": {
+                "items": await ChatMessage.filter(**filter_args)
+                .order_by(orderBy)
+                .offset((page - 1) * perPage)
+                .limit(perPage)
+                .values(),
+                "total": await ChatMessage.filter(**filter_args).count(),
+            },
         }
 
-    @app.get('/learning_chat/api/get_chat_contexts', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_chat_context(page: int = 1, perPage: int = 10, orderBy: str = 'time', orderDir: str = 'desc',
-                               keywords: Optional[str] = None):
-        orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
-        filter_arg = {'keywords__contains': keywords} if keywords else {}
+    @app.get(
+        "/learning_chat/api/get_chat_contexts",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def get_chat_context(
+        page: int = 1,
+        perPage: int = 10,
+        orderBy: str = "time",
+        orderDir: str = "desc",
+        keywords: Optional[str] = None,
+    ):
+        orderBy = (
+            (orderBy or "time")
+            if (orderDir or "desc") == "asc"
+            else f'-{orderBy or "time"}'
+        )
+        filter_arg = {"keywords__contains": keywords} if keywords else {}
         return {
-            'status': 0,
-            'msg':    'ok',
-            'data':   {
-                'items': await ChatContext.filter(**filter_arg).order_by(orderBy).offset((page - 1) * perPage).limit(
-                    perPage).values(),
-                'total': await ChatContext.filter(**filter_arg).count()
-            }
+            "status": 0,
+            "msg": "ok",
+            "data": {
+                "items": await ChatContext.filter(**filter_arg)
+                .order_by(orderBy)
+                .offset((page - 1) * perPage)
+                .limit(perPage)
+                .values(),
+                "total": await ChatContext.filter(**filter_arg).count(),
+            },
         }
 
-    @app.get('/learning_chat/api/get_chat_answers', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_chat_answers(context_id: Optional[int] = None, page: int = 1, perPage: int = 10,
-                               orderBy: str = 'count',
-                               orderDir: str = 'desc', keywords: Optional[str] = None):
-        filter_arg = {'context_id': context_id} if context_id else {}
+    @app.get(
+        "/learning_chat/api/get_chat_answers",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def get_chat_answers(
+        context_id: Optional[int] = None,
+        page: int = 1,
+        perPage: int = 10,
+        orderBy: str = "count",
+        orderDir: str = "desc",
+        keywords: Optional[str] = None,
+    ):
+        filter_arg = {"context_id": context_id} if context_id else {}
         if keywords:
-            filter_arg['keywords__contains'] = keywords  # type: ignore
-        orderBy = (orderBy or 'count') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "count"}'
+            filter_arg["keywords__contains"] = keywords  # type: ignore
+        orderBy = (
+            (orderBy or "count")
+            if (orderDir or "desc") == "asc"
+            else f'-{orderBy or "count"}'
+        )
         return {
-            'status': 0,
-            'msg':    'ok',
-            'data':   {
-                'items': list(
-                    map(lambda x: x.update({'messages': [{'msg': m} for m in x['messages']]}) or x,
-                        await ChatAnswer.filter(**filter_arg).order_by(orderBy).offset((page - 1) * perPage).limit(
-                            perPage).values())),
-                'total': await ChatAnswer.filter(**filter_arg).count()
-            }
+            "status": 0,
+            "msg": "ok",
+            "data": {
+                "items": list(
+                    map(
+                        lambda x: x.update(
+                            {"messages": [{"msg": m} for m in x["messages"]]}
+                        )
+                        or x,
+                        await ChatAnswer.filter(**filter_arg)
+                        .order_by(orderBy)
+                        .offset((page - 1) * perPage)
+                        .limit(perPage)
+                        .values(),
+                    )
+                ),
+                "total": await ChatAnswer.filter(**filter_arg).count(),
+            },
         }
 
-    @app.get('/learning_chat/api/get_chat_blacklist', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_chat_blacklist(page: int = 1, perPage: int = 10, keywords: Optional[str] = None,
-                                 bans: Optional[str] = None):
-        filter_arg = {'keywords__contains': keywords} if keywords else {}
-        items = await ChatBlackList.filter(**filter_arg).offset((page - 1) * perPage).limit(perPage).values()
+    @app.get(
+        "/learning_chat/api/get_chat_blacklist",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def get_chat_blacklist(
+        page: int = 1,
+        perPage: int = 10,
+        keywords: Optional[str] = None,
+        bans: Optional[str] = None,
+    ):
+        filter_arg = {"keywords__contains": keywords} if keywords else {}
+        items = (
+            await ChatBlackList.filter(**filter_arg)
+            .offset((page - 1) * perPage)
+            .limit(perPage)
+            .values()
+        )
         for item in items:
-            item['bans'] = '全局禁用' if item['global_ban'] else str(item['ban_group_id'][0])
+            item["bans"] = (
+                "全局禁用" if item["global_ban"] else str(item["ban_group_id"][0])
+            )
         if bans:
-            items = list(filter(lambda x: bans in x['bans'], items))
+            items = list(filter(lambda x: bans in x["bans"], items))
         return {
-            'status': 0,
-            'msg':    'ok',
-            'data':   {
-                'items': items,
-                'total': await ChatBlackList.filter(**filter_arg).count()
-            }
+            "status": 0,
+            "msg": "ok",
+            "data": {
+                "items": items,
+                "total": await ChatBlackList.filter(**filter_arg).count(),
+            },
         }
 
-    @app.delete('/learning_chat/api/delete_chat', response_class=JSONResponse, dependencies=[authentication()])
+    @app.delete(
+        "/learning_chat/api/delete_chat",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def delete_chat(id: int, type: str):
         try:
-            if type == 'message':
+            if type == "message":
                 await ChatMessage.filter(id=id).delete()
-            elif type == 'context':
+            elif type == "context":
                 c = await ChatContext.get(id=id)
                 await ChatAnswer.filter(context=c).delete()
                 await c.delete()
-            elif type == 'answer':
+            elif type == "answer":
                 await ChatAnswer.filter(id=id).delete()
-            elif type == 'blacklist':
+            elif type == "blacklist":
                 await ChatBlackList.filter(id=id).delete()
-            return {
-                'status': 0,
-                'msg':    '删除成功'
-            }
+            return {"status": 0, "msg": "删除成功"}
         except Exception as e:
-            return {
-                'status': 500,
-                'msg':    f'删除失败，{e}'
-            }
+            return {"status": 500, "msg": f"删除失败，{e}"}
 
-    @app.put('/learning_chat/api/ban_chat', response_class=JSONResponse, dependencies=[authentication()])
+    @app.put(
+        "/learning_chat/api/ban_chat",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def ban_chat(id: int, type: str):
         try:
-            if type == 'message':
+            if type == "message":
                 data = await ChatMessage.get(id=id)
-            elif type == 'context':
+            elif type == "context":
                 data = await ChatContext.get(id=id)
             else:
                 data = await ChatAnswer.get(id=id)
             await LearningChat.add_ban(data)
-            return {
-                'status': 0,
-                'msg':    '禁用成功'
-            }
+            return {"status": 0, "msg": "禁用成功"}
         except Exception as e:
-            return {
-                'status': 500,
-                'msg':    f'禁用失败: {e}'
-            }
+            return {"status": 500, "msg": f"禁用失败: {e}"}
 
-    @app.put('/learning_chat/api/delete_all', response_class=JSONResponse, dependencies=[authentication()])
+    @app.put(
+        "/learning_chat/api/delete_all",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def delete_all(type: str, id: Optional[int] = None):
         try:
-            if type == 'answer':
+            if type == "answer":
                 if id:
                     await ChatAnswer.filter(context_id=id).delete()
                 else:
                     await ChatAnswer.all().delete()
-            elif type == 'blacklist':
+            elif type == "blacklist":
                 await ChatBlackList.all().delete()
-            elif type == 'context':
+            elif type == "context":
                 await ChatContext.all().delete()
-            elif type == 'message':
+            elif type == "message":
                 await ChatMessage.all().delete()
-            return {
-                'status': 0,
-                'msg':    '操作成功'
-            }
+            return {"status": 0, "msg": "操作成功"}
         except Exception as e:
-            return {
-                'status': 500,
-                'msg':    f'操作失败，{e}'
-            }
+            return {"status": 500, "msg": f"操作失败，{e}"}
 
-    @app.get('/learning_chat', response_class=RedirectResponse)
+    @app.get("/learning_chat", response_class=RedirectResponse)
     async def redirect_page():
-        return RedirectResponse('/learning_chat/login')
+        return RedirectResponse("/learning_chat/login")
 
-    @app.get('/learning_chat/login', response_class=HTMLResponse)
+    @app.get("/learning_chat/login", response_class=HTMLResponse)
     async def login_page_app():
-        return login_page.render(site_title='登录 | Learning-Chat 后台管理',
-                                 theme='ang')
+        return login_page.render(site_title="登录 | Learning-Chat 后台管理", theme="ang")
 
-    @app.get('/learning_chat/admin', response_class=HTMLResponse)
+    @app.get("/learning_chat/admin", response_class=HTMLResponse)
     async def admin_page_app():
-        return admin_app.render(site_title='Learning-Chat 后台管理',
-                                theme='ang',
-                                requestAdaptor=requestAdaptor,
-                                responseAdaptor=responseAdaptor)
+        return admin_app.render(
+            site_title="Learning-Chat 后台管理",
+            theme="ang",
+            requestAdaptor=requestAdaptor,
+            responseAdaptor=responseAdaptor,
+        )
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/nonebot_plugin_learning_chat/web_page.py` & `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_page.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,352 +1,733 @@
 from amis import ColumnList, AmisList, ActionType, TableCRUD, TableColumn
 from amis import Dialog, PageSchema, Switch, InputNumber, InputTag, Action, App
-from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper
+from amis import (
+    Form,
+    InputText,
+    InputPassword,
+    DisplayModeEnum,
+    Horizontal,
+    Remark,
+    Html,
+    Page,
+    AmisAPI,
+    Wrapper,
+)
 from amis import LevelEnum, Select, InputArray, Alert, Tpl, Flex
 
 from .config import NICKNAME
 
-logo = Html(html='''
+logo = Html(
+    html="""
 <p align="center">
     <a href="https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat/">
         <img src="http://static.cherishmoon.fun/LittlePaimon/readme/logo.png"
          width="256" height="256" alt="Learning-Chat">
     </a>
 </p>
 <h1 align="center">Nonebot-Plugin-Learning-Chat 控制台</h1>
 <div align="center">
     <a href="https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat/" target="_blank">
     Github仓库</a>
 </div>
 <br>
 <br>
-''')
+"""
+)
 login_api = AmisAPI(
-    url='/learning_chat/api/login',
-    method='post',
-    adaptor='''
+    url="/learning_chat/api/login",
+    method="post",
+    adaptor="""
         if (payload.status == 0) {
             localStorage.setItem("token", payload.data.token);
         }
         return payload;
-    '''
+    """,
 )
 
-login_form = Form(api=login_api, title='', body=[
-    InputText(name='username', label='用户名',
-              labelRemark=Remark(shape='circle', content='后台管理用户名，默认为chat')),
-    InputPassword(name='password', label='密码',
-                  labelRemark=Remark(shape='circle', content='后台管理密码，默认为admin')),
-], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5), redirect='/learning_chat/admin')
-body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
-login_page = Page(title='', body=[logo, body])
+login_form = Form(
+    api=login_api,
+    title="",
+    body=[
+        InputText(
+            name="username",
+            label="用户名",
+            labelRemark=Remark(shape="circle", content="后台管理用户名，默认为chat"),
+        ),
+        InputPassword(
+            name="password",
+            label="密码",
+            labelRemark=Remark(shape="circle", content="后台管理密码，默认为admin"),
+        ),
+    ],
+    mode=DisplayModeEnum.horizontal,
+    horizontal=Horizontal(left=3, right=9, offset=5),
+    redirect="/learning_chat/admin",
+)
+body = Wrapper(className="w-2/5 mx-auto my-0 m:w-full", body=login_form)
+login_page = Page(title="", body=[logo, body])
 
 global_config_form = Form(
-    title='全局配置',
-    name='global_config',
-    initApi='/learning_chat/api/chat_global_config',
-    api='post:/learning_chat/api/chat_global_config',
+    title="全局配置",
+    name="global_config",
+    initApi="/learning_chat/api/chat_global_config",
+    api="post:/learning_chat/api/chat_global_config",
+    interval=None,
     body=[
-        Switch(label='群聊学习总开关', name='total_enable', value='${total_enable}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle',
-                                  content='关闭后，全局都将不会再学习和回复(但是仍会对收到的消息进行记录)。')),
-        Switch(label='后台管理总开关', name='enable_web', value='${enable_web}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle',
-                                  content='是否开启本后台管理，若关闭，则无法再访问本页面。')),
-        InputText(label='后台管理用户名', name='web_username', value='${web_username}',
-                  labelRemark=Remark(shape='circle',
-                                     content='登录本后台管理所需要的用户名。')),
-        InputPassword(label='后台管理密码', name='web_password', value='${web_password}',
-                      labelRemark=Remark(shape='circle',
-                                         content='登录本后台管理所需要的密码。')),
-        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于本后台管理加密验证token的密钥。')),
-        InputNumber(label='单句关键词数量', name='KEYWORDS_SIZE', value='${KEYWORDS_SIZE}', visibleOn='${total_enable}',
-                    min=2,
-                    labelRemark=Remark(shape='circle',
-                                       content='单句语句标签数量，影响对一句话的主题词提取效果，建议保持默认为3。')),
-        InputNumber(label='跨群回复阈值', name='cross_group_threshold', value='${cross_group_threshold}',
-                    visibleOn='${total_enable}', min=1,
-                    labelRemark=Remark(shape='circle',
-                                       content='当学习到的一种回复在N个群都有，那么这个回复就会变为全局回复。')),
-        InputNumber(label='最高学习次数', name='learn_max_count', value='${learn_max_count}',
-                    visibleOn='${total_enable}', min=2, labelRemark=Remark(shape='circle',
-                                                                           content='学习的回复最高能累计到的次数，值越高，这个回复就会学习得越深，越容易进行回复，如果不想每次都大概率固定回复某一句话，可以将该值设低点。')),
-        InputTag(label='全局屏蔽词', name='ban_words', value='${ban_words}', enableBatchAdd=True,
-                 placeholder='添加全局屏蔽词', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='全局屏蔽词，含有这些词的消息不会学习和回复，默认已屏蔽at、分享、语音、和视频等消息。(回车进行添加)')),
-        InputTag(label='全局屏蔽用户', name='ban_users', value='${ban_users}',
-                 enableBatchAdd=True,
-                 placeholder='添加全局屏蔽用户', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='全局屏蔽用户，和这些用户有关的消息不会学习和回复。(回车进行添加)')),
-        InputTag(label='自定义词典', name='dictionary', value='${dictionary}',
-                 enableBatchAdd=True,
-                 placeholder='添加自定义词语', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='添加自定义词语，让分词能够识别未收录的词汇，提高学习的准确性。你可以添加特殊名词，这样学习时就会将该词看作一个整体，目前词典中已默认添加部分原神相关词汇。(回车进行添加)')),
+        Switch(
+            label="群聊学习总开关",
+            name="total_enable",
+            value="${total_enable}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(
+                shape="circle", content="关闭后，全局都将不会再学习和回复(但是仍会对收到的消息进行记录)。"
+            ),
+        ),
+        Switch(
+            label="后台管理总开关",
+            name="enable_web",
+            value="${enable_web}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(shape="circle", content="是否开启本后台管理，若关闭，则无法再访问本页面。"),
+        ),
+        InputText(
+            label="后台管理用户名",
+            name="web_username",
+            value="${web_username}",
+            labelRemark=Remark(shape="circle", content="登录本后台管理所需要的用户名。"),
+        ),
+        InputPassword(
+            label="后台管理密码",
+            name="web_password",
+            value="${web_password}",
+            labelRemark=Remark(shape="circle", content="登录本后台管理所需要的密码。"),
+        ),
+        InputText(
+            label="后台管理token密钥",
+            name="web_secret_key",
+            value="${web_secret_key}",
+            labelRemark=Remark(shape="circle", content="用于本后台管理加密验证token的密钥。"),
+        ),
+        InputNumber(
+            label="单句关键词数量",
+            name="KEYWORDS_SIZE",
+            value="${KEYWORDS_SIZE}",
+            visibleOn="${total_enable}",
+            min=2,
+            labelRemark=Remark(
+                shape="circle", content="单句语句标签数量，影响对一句话的主题词提取效果，建议保持默认为3。"
+            ),
+        ),
+        InputNumber(
+            label="跨群回复阈值",
+            name="cross_group_threshold",
+            value="${cross_group_threshold}",
+            visibleOn="${total_enable}",
+            min=1,
+            labelRemark=Remark(
+                shape="circle", content="当学习到的一种回复在N个群都有，那么这个回复就会变为全局回复。"
+            ),
+        ),
+        InputNumber(
+            label="最高学习次数",
+            name="learn_max_count",
+            value="${learn_max_count}",
+            visibleOn="${total_enable}",
+            min=2,
+            labelRemark=Remark(
+                shape="circle",
+                content="学习的回复最高能累计到的次数，值越高，这个回复就会学习得越深，越容易进行回复，如果不想每次都大概率固定回复某一句话，可以将该值设低点。",
+            ),
+        ),
+        InputTag(
+            label="全局屏蔽词",
+            name="ban_words",
+            value="${ban_words}",
+            enableBatchAdd=True,
+            placeholder="添加全局屏蔽词",
+            visibleOn="${total_enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(
+                shape="circle",
+                content="全局屏蔽词，含有这些词的消息不会学习和回复，默认已屏蔽at、分享、语音、和视频等消息。(回车进行添加)",
+            ),
+        ),
+        InputTag(
+            label="全局屏蔽用户",
+            name="ban_users",
+            value="${ban_users}",
+            enableBatchAdd=True,
+            placeholder="添加全局屏蔽用户",
+            visibleOn="${total_enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(
+                shape="circle", content="全局屏蔽用户，和这些用户有关的消息不会学习和回复。(回车进行添加)"
+            ),
+        ),
+        InputTag(
+            label="自定义词典",
+            name="dictionary",
+            value="${dictionary}",
+            enableBatchAdd=True,
+            placeholder="添加自定义词语",
+            visibleOn="${total_enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(
+                shape="circle",
+                content="添加自定义词语，让分词能够识别未收录的词汇，提高学习的准确性。你可以添加特殊名词，这样学习时就会将该词看作一个整体，目前词典中已默认添加部分原神相关词汇。(回车进行添加)",
+            ),
+        ),
+    ],
+    actions=[
+        Action(label="保存", level=LevelEnum.success, type="submit"),
+        Action(label="重置", level=LevelEnum.warning, type="reset"),
     ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
-group_select = Select(label='分群配置', name='group_id', source='${group_list}',
-                      placeholder='选择群')
+group_select = Select(
+    label="分群配置", name="group_id", source="${group_list}", placeholder="选择群"
+)
 group_config_form = Form(
-    title='分群配置',
-    visibleOn='group_id != null',
-    initApi='/learning_chat/api/chat_group_config?group_id=${group_id}',
-    api='post:/learning_chat/api/chat_group_config?group_id=${group_id}',
+    title="分群配置",
+    visibleOn="group_id != null",
+    initApi="/learning_chat/api/chat_group_config?group_id=${group_id}",
+    api="post:/learning_chat/api/chat_group_config?group_id=${group_id}",
+    interval=None,
     body=[
-        Switch(label='群聊学习开关', name='enable', value='${enable}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle', content='针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。')),
-        InputNumber(label='回复阈值', name='answer_threshold', value='${answer_threshold}', visibleOn='${enable}',
-                    min=2,
-                    labelRemark=Remark(shape='circle', content='可以理解为学习成功所需要的次数，值越低学得越快。')),
-        InputArray(label='回复阈值权重', name='answer_threshold_weights', value='${answer_threshold_weights}',
-                   items=InputNumber(min=1, max=100, value=25, suffix='%'), inline=True, visibleOn='${enable}',
-                   labelRemark=Remark(shape='circle',
-                                      content='影响回复阈值的计算方式，以默认的回复阈值4、权重[10, 30, 60]为例，在计算阈值时，60%概率为4，30%概率为3，10%概率为2。')),
-        InputNumber(label='复读阈值', name='repeat_threshold', value='${repeat_threshold}', visibleOn='${enable}',
-                    min=2,
-                    labelRemark=Remark(shape='circle',
-                                       content=f'跟随复读所需要的阈值，有N个人复读后，{NICKNAME}就会跟着复读。')),
-        InputNumber(label='打断复读概率', name='break_probability', value='${break_probability}',
-                    min=0, max=100, suffix='%', visibleOn='${AND(enable, speak_enable)}',
-                    labelRemark=Remark(shape='circle', content='达到复读阈值时，打断复读而不是跟随复读的概率。')),
-        InputTag(label='屏蔽词', name='ban_words', value='${ban_words}', enableBatchAdd=True,
-                 placeholder='添加屏蔽词', visibleOn='${enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle', content='含有这些词的消息不会学习和回复。(回车进行添加)')),
-        InputTag(label='屏蔽用户', source='${member_list}', name='ban_users', value='${ban_users}', enableBatchAdd=True,
-                 placeholder='添加屏蔽用户', visibleOn='${enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle', content='和该群中这些用户有关的消息不会学习和回复。(回车进行添加)')),
-        Switch(label='主动发言开关', name='speak_enable', value='${speak_enable}', visibleOn='${enable}',
-               labelRemark=Remark(shape='circle',
-                                  content=f'是否允许{NICKNAME}在该群主动发言，主动发言是指每隔一段时间挑选一个热度较高的群，主动发一些学习过的内容。')),
-        InputNumber(label='主动发言阈值', name='speak_threshold', value='${speak_threshold}',
-                    visibleOn='${AND(enable, speak_enable)}', min=0,
-                    labelRemark=Remark(shape='circle', content='值越低，主动发言的可能性越高。')),
-        InputNumber(label='主动发言最小间隔', name='speak_min_interval', value='${speak_min_interval}', min=0,
-                    visibleOn='${AND(enable, speak_enable)}', suffix='秒',
-                    labelRemark=Remark(shape='circle', content='进行主动发言的最小时间间隔。')),
-        InputNumber(label='连续主动发言概率', name='speak_continuously_probability',
-                    value='${speak_continuously_probability}', min=0, max=100, suffix='%',
-                    visibleOn='${AND(enable, speak_enable)}',
-                    labelRemark=Remark(shape='circle', content='触发主动发言时，连续进行发言的概率。')),
-        InputNumber(label='最大连续主动发言句数', name='speak_continuously_max_len',
-                    value='${speak_continuously_max_len}', visibleOn='${AND(enable, speak_enable)}', min=1,
-                    labelRemark=Remark(shape='circle', content='连续主动发言的最大句数。')),
-        InputNumber(label='主动发言附带戳一戳概率', name='speak_poke_probability', value='${speak_poke_probability}',
-                    min=0, max=100, suffix='%', visibleOn='${AND(enable, speak_enable)}',
-                    labelRemark=Remark(shape='circle',
-                                       content='主动发言时附带戳一戳的概率，会在最近5个发言者中随机选一个戳。')),
-    ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             ActionType.Ajax(
-                 label='保存至所有群',
-                 level=LevelEnum.primary,
-                 confirmText='确认将当前配置保存至所有群？',
-                 api='post:/learning_chat/api/chat_group_config?group_id=all'
-             ),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
+        Switch(
+            label="群聊学习开关",
+            name="enable",
+            value="${enable}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(shape="circle", content="针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。"),
+        ),
+        InputNumber(
+            label="回复阈值",
+            name="answer_threshold",
+            value="${answer_threshold}",
+            visibleOn="${enable}",
+            min=2,
+            labelRemark=Remark(shape="circle", content="可以理解为学习成功所需要的次数，值越低学得越快。"),
+        ),
+        InputArray(
+            label="回复阈值权重",
+            name="answer_threshold_weights",
+            value="${answer_threshold_weights}",
+            items=InputNumber(min=1, max=100, value=25, suffix="%"),
+            inline=True,
+            visibleOn="${enable}",
+            labelRemark=Remark(
+                shape="circle",
+                content="影响回复阈值的计算方式，以默认的回复阈值4、权重[10, 30, 60]为例，在计算阈值时，60%概率为4，30%概率为3，10%概率为2。",
+            ),
+        ),
+        InputNumber(
+            label="复读阈值",
+            name="repeat_threshold",
+            value="${repeat_threshold}",
+            visibleOn="${enable}",
+            min=2,
+            labelRemark=Remark(
+                shape="circle", content=f"跟随复读所需要的阈值，有N个人复读后，{NICKNAME}就会跟着复读。"
+            ),
+        ),
+        InputNumber(
+            label="打断复读概率",
+            name="break_probability",
+            value="${break_probability}",
+            min=0,
+            max=100,
+            suffix="%",
+            visibleOn="${AND(enable, speak_enable)}",
+            labelRemark=Remark(shape="circle", content="达到复读阈值时，打断复读而不是跟随复读的概率。"),
+        ),
+        InputTag(
+            label="屏蔽词",
+            name="ban_words",
+            value="${ban_words}",
+            enableBatchAdd=True,
+            placeholder="添加屏蔽词",
+            visibleOn="${enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(shape="circle", content="含有这些词的消息不会学习和回复。(回车进行添加)"),
+        ),
+        InputTag(
+            label="屏蔽用户",
+            source="${member_list}",
+            name="ban_users",
+            value="${ban_users}",
+            enableBatchAdd=True,
+            placeholder="添加屏蔽用户",
+            visibleOn="${enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(shape="circle", content="和该群中这些用户有关的消息不会学习和回复。(回车进行添加)"),
+        ),
+        Switch(
+            label="主动发言开关",
+            name="speak_enable",
+            value="${speak_enable}",
+            visibleOn="${enable}",
+            labelRemark=Remark(
+                shape="circle",
+                content=f"是否允许{NICKNAME}在该群主动发言，主动发言是指每隔一段时间挑选一个热度较高的群，主动发一些学习过的内容。",
+            ),
+        ),
+        InputNumber(
+            label="主动发言阈值",
+            name="speak_threshold",
+            value="${speak_threshold}",
+            visibleOn="${AND(enable, speak_enable)}",
+            min=0,
+            labelRemark=Remark(shape="circle", content="值越低，主动发言的可能性越高。"),
+        ),
+        InputNumber(
+            label="主动发言最小间隔",
+            name="speak_min_interval",
+            value="${speak_min_interval}",
+            min=0,
+            visibleOn="${AND(enable, speak_enable)}",
+            suffix="秒",
+            labelRemark=Remark(shape="circle", content="进行主动发言的最小时间间隔。"),
+        ),
+        InputNumber(
+            label="连续主动发言概率",
+            name="speak_continuously_probability",
+            value="${speak_continuously_probability}",
+            min=0,
+            max=100,
+            suffix="%",
+            visibleOn="${AND(enable, speak_enable)}",
+            labelRemark=Remark(shape="circle", content="触发主动发言时，连续进行发言的概率。"),
+        ),
+        InputNumber(
+            label="最大连续主动发言句数",
+            name="speak_continuously_max_len",
+            value="${speak_continuously_max_len}",
+            visibleOn="${AND(enable, speak_enable)}",
+            min=1,
+            labelRemark=Remark(shape="circle", content="连续主动发言的最大句数。"),
+        ),
+        InputNumber(
+            label="主动发言附带戳一戳概率",
+            name="speak_poke_probability",
+            value="${speak_poke_probability}",
+            min=0,
+            max=100,
+            suffix="%",
+            visibleOn="${AND(enable, speak_enable)}",
+            labelRemark=Remark(
+                shape="circle", content="主动发言时附带戳一戳的概率，会在最近5个发言者中随机选一个戳。"
+            ),
+        ),
+    ],
+    actions=[
+        Action(label="保存", level=LevelEnum.success, type="submit"),
+        ActionType.Ajax(
+            label="保存至所有群",
+            level=LevelEnum.primary,
+            confirmText="确认将当前配置保存至所有群？",
+            api="post:/learning_chat/api/chat_group_config?group_id=all",
+        ),
+        Action(label="重置", level=LevelEnum.warning, type="reset"),
+    ],
 )
 
-blacklist_table = TableCRUD(mode='table',
-                            title='',
-                            syncLocation=False,
-                            api='/learning_chat/api/get_chat_blacklist',
-                            interval=15000,
-                            headerToolbar=[ActionType.Ajax(label='取消所有禁用',
-                                                           level=LevelEnum.warning,
-                                                           confirmText='确定要取消所有禁用吗？',
-                                                           api='put:/learning_chat/api/delete_all?type=blacklist')],
-                            itemActions=[ActionType.Ajax(tooltip='取消禁用',
-                                                         icon='fa fa-check-circle-o text-info',
-                                                         confirmText='取消该被禁用的内容/关键词，但是仍然需要重新学习哦！',
-                                                         api='delete:/learning_chat/api/delete_chat?type=blacklist&id=${id}')
-                                         ],
-                            footable=True,
-                            columns=[TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='内容/关键词',
-                                                 name='keywords',
-                                                 searchable=True, popOver={'mode':      'dialog', 'title': '全文',
-                                                                           'className': 'break-all',
-                                                                           'body':      {'type': 'tpl',
-                                                                                         'tpl':  '${keywords}'}}),
-                                     TableColumn(label='已禁用的群', name='bans', searchable=True),
-                                     ])
-message_table = TableCRUD(mode='table',
-                          title='',
-                          syncLocation=False,
-                          api='/learning_chat/api/get_chat_messages',
-                          interval=12000,
-                          headerToolbar=[ActionType.Ajax(label='删除所有聊天记录',
-                                                         level=LevelEnum.warning,
-                                                         confirmText='确定要删除所有聊天记录吗？',
-                                                         api='put:/learning_chat/api/delete_all?type=message')],
-                          itemActions=[ActionType.Ajax(tooltip='禁用',
-                                                       icon='fa fa-ban text-danger',
-                                                       confirmText='禁用该聊天记录相关的学习内容和回复',
-                                                       api='put:/learning_chat/api/ban_chat?type=message&id=${id}'),
-                                       ActionType.Ajax(tooltip='删除',
-                                                       icon='fa fa-times text-danger',
-                                                       confirmText='删除该条聊天记录',
-                                                       api='delete:/learning_chat/api/delete_chat?type=message&id=${id}')
-                                       ],
-                          footable=True,
-                          columns=[TableColumn(label='消息ID', name='message_id'),
-                                   TableColumn(label='群ID', name='group_id', searchable=True),
-                                   TableColumn(label='用户ID', name='user_id', searchable=True),
-                                   TableColumn(type='tpl', tpl='${raw_message|truncate:20}', label='消息',
-                                               name='message',
-                                               searchable=True, popOver={'mode':      'dialog', 'title': '消息全文',
-                                                                         'className': 'break-all',
-                                                                         'body':      {'type': 'tpl',
-                                                                                       'tpl':  '${raw_message}'}}),
-                                   TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='时间',
-                                               name='time', sortable=True)
-                                   ])
+blacklist_table = TableCRUD(
+    mode="table",
+    title="",
+    syncLocation=False,
+    api="/learning_chat/api/get_chat_blacklist",
+    interval=15000,
+    headerToolbar=[
+        ActionType.Ajax(
+            label="取消所有禁用",
+            level=LevelEnum.warning,
+            confirmText="确定要取消所有禁用吗？",
+            api="put:/learning_chat/api/delete_all?type=blacklist",
+        )
+    ],
+    itemActions=[
+        ActionType.Ajax(
+            tooltip="取消禁用",
+            icon="fa fa-check-circle-o text-info",
+            confirmText="取消该被禁用的内容/关键词，但是仍然需要重新学习哦！",
+            api="delete:/learning_chat/api/delete_chat?type=blacklist&id=${id}",
+        )
+    ],
+    footable=True,
+    columns=[
+        TableColumn(
+            type="tpl",
+            tpl="${keywords|truncate:20}",
+            label="内容/关键词",
+            name="keywords",
+            searchable=True,
+            popOver={
+                "mode": "dialog",
+                "title": "全文",
+                "className": "break-all",
+                "body": {"type": "tpl", "tpl": "${keywords}"},
+            },
+        ),
+        TableColumn(label="已禁用的群", name="bans", searchable=True),
+    ],
+)
+message_table = TableCRUD(
+    mode="table",
+    title="",
+    syncLocation=False,
+    api="/learning_chat/api/get_chat_messages",
+    interval=12000,
+    headerToolbar=[
+        ActionType.Ajax(
+            label="删除所有聊天记录",
+            level=LevelEnum.warning,
+            confirmText="确定要删除所有聊天记录吗？",
+            api="put:/learning_chat/api/delete_all?type=message",
+        )
+    ],
+    itemActions=[
+        ActionType.Ajax(
+            tooltip="禁用",
+            icon="fa fa-ban text-danger",
+            confirmText="禁用该聊天记录相关的学习内容和回复",
+            api="put:/learning_chat/api/ban_chat?type=message&id=${id}",
+        ),
+        ActionType.Ajax(
+            tooltip="删除",
+            icon="fa fa-times text-danger",
+            confirmText="删除该条聊天记录",
+            api="delete:/learning_chat/api/delete_chat?type=message&id=${id}",
+        ),
+    ],
+    footable=True,
+    columns=[
+        TableColumn(label="消息ID", name="message_id"),
+        TableColumn(label="群ID", name="group_id", searchable=True),
+        TableColumn(label="用户ID", name="user_id", searchable=True),
+        TableColumn(
+            type="tpl",
+            tpl="${raw_message|truncate:20}",
+            label="消息",
+            name="message",
+            searchable=True,
+            popOver={
+                "mode": "dialog",
+                "title": "消息全文",
+                "className": "break-all",
+                "body": {"type": "tpl", "tpl": "${raw_message}"},
+            },
+        ),
+        TableColumn(
+            type="tpl",
+            tpl="${time|date:YYYY-MM-DD HH\\:mm\\:ss}",
+            label="时间",
+            name="time",
+            sortable=True,
+        ),
+    ],
+)
 answer_table = TableCRUD(
-    mode='table',
+    mode="table",
     syncLocation=False,
     footable=True,
-    api='/learning_chat/api/get_chat_answers',
+    api="/learning_chat/api/get_chat_answers",
     interval=12000,
-    headerToolbar=[ActionType.Ajax(label='删除所有已学习的回复',
-                                   level=LevelEnum.warning,
-                                   confirmText='确定要删除所有已学习的回复吗？',
-                                   api='put:/learning_chat/api/delete_all?type=answer')],
-    itemActions=[ActionType.Ajax(tooltip='禁用',
-                                 icon='fa fa-ban text-danger',
-                                 confirmText='禁用并删除该已学回复',
-                                 api='put:/learning_chat/api/ban_chat?type=answer&id=${id}'),
-                 ActionType.Ajax(tooltip='删除',
-                                 icon='fa fa-times text-danger',
-                                 confirmText='仅删除该已学回复，不会禁用，所以依然能继续学',
-                                 api='delete:/learning_chat/api/delete_chat?type=answer&id=${id}')],
-    columns=[TableColumn(label='ID', name='id', visible=False),
-             TableColumn(label='群ID', name='group_id', searchable=True),
-             TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='内容/关键词', name='keywords',
-                         searchable=True, popOver={'mode': 'dialog', 'title': '内容全文', 'className': 'break-all',
-                                                   'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
-             TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='最后学习时间', name='time',
-                         sortable=True),
-             TableColumn(label='次数', name='count', sortable=True),
-             ColumnList(label='完整消息', name='messages', breakpoint='*', source='${messages}',
-                        listItem=AmisList.Item(body={'name': 'msg'}))
-             ])
+    headerToolbar=[
+        ActionType.Ajax(
+            label="删除所有已学习的回复",
+            level=LevelEnum.warning,
+            confirmText="确定要删除所有已学习的回复吗？",
+            api="put:/learning_chat/api/delete_all?type=answer",
+        )
+    ],
+    itemActions=[
+        ActionType.Ajax(
+            tooltip="禁用",
+            icon="fa fa-ban text-danger",
+            confirmText="禁用并删除该已学回复",
+            api="put:/learning_chat/api/ban_chat?type=answer&id=${id}",
+        ),
+        ActionType.Ajax(
+            tooltip="删除",
+            icon="fa fa-times text-danger",
+            confirmText="仅删除该已学回复，不会禁用，所以依然能继续学",
+            api="delete:/learning_chat/api/delete_chat?type=answer&id=${id}",
+        ),
+    ],
+    columns=[
+        TableColumn(label="ID", name="id", visible=False),
+        TableColumn(label="群ID", name="group_id", searchable=True),
+        TableColumn(
+            type="tpl",
+            tpl="${keywords|truncate:20}",
+            label="内容/关键词",
+            name="keywords",
+            searchable=True,
+            popOver={
+                "mode": "dialog",
+                "title": "内容全文",
+                "className": "break-all",
+                "body": {"type": "tpl", "tpl": "${keywords}"},
+            },
+        ),
+        TableColumn(
+            type="tpl",
+            tpl="${time|date:YYYY-MM-DD HH\\:mm\\:ss}",
+            label="最后学习时间",
+            name="time",
+            sortable=True,
+        ),
+        TableColumn(label="次数", name="count", sortable=True),
+        ColumnList(
+            label="完整消息",
+            name="messages",
+            breakpoint="*",
+            source="${messages}",
+            listItem=AmisList.Item(body=[AmisList.Item.ListBodyField(name="msg")]),
+        ),
+    ],
+)
 answer_table_on_context = TableCRUD(
-    mode='table',
+    mode="table",
     syncLocation=False,
     footable=True,
-    api='/learning_chat/api/get_chat_answers?context_id=${id}&page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}',
+    api="/learning_chat/api/get_chat_answers?context_id=${id}&page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}",
+    interval=12000,
+    headerToolbar=[
+        ActionType.Ajax(
+            label="删除该内容所有回复",
+            level=LevelEnum.warning,
+            confirmText="确定要删除该条内容已学习的回复吗？",
+            api="put:/learning_chat/api/delete_all?type=answer&id=${id}",
+        )
+    ],
+    itemActions=[
+        ActionType.Ajax(
+            tooltip="禁用",
+            icon="fa fa-ban text-danger",
+            confirmText="禁用并删除该已学回复",
+            api="put:/learning_chat/api/ban_chat?type=answer&id=${id}",
+        ),
+        ActionType.Ajax(
+            tooltip="删除",
+            icon="fa fa-times text-danger",
+            confirmText="仅删除该已学回复，但不禁用，依然能继续学",
+            api="delete:/learning_chat/api/delete_chat?type=answer&id=${id}",
+        ),
+    ],
+    columns=[
+        TableColumn(label="ID", name="id", visible=False),
+        TableColumn(label="群ID", name="group_id"),
+        TableColumn(
+            type="tpl",
+            tpl="${keywords|truncate:20}",
+            label="内容/关键词",
+            name="keywords",
+            searchable=True,
+            popOver={
+                "mode": "dialog",
+                "title": "内容全文",
+                "className": "break-all",
+                "body": {"type": "tpl", "tpl": "${keywords}"},
+            },
+        ),
+        TableColumn(
+            type="tpl",
+            tpl="${time|date:YYYY-MM-DD HH\\:mm\\:ss}",
+            label="最后学习时间",
+            name="time",
+            sortable=True,
+        ),
+        TableColumn(label="次数", name="count", sortable=True),
+        ColumnList(
+            label="完整消息",
+            name="messages",
+            breakpoint="*",
+            source="${messages}",
+            listItem=AmisList.Item(body=[AmisList.Item.ListBodyField(name="msg")]),
+        ),
+    ],
+)
+context_table = TableCRUD(
+    mode="table",
+    title="",
+    syncLocation=False,
+    api="/learning_chat/api/get_chat_contexts",
     interval=12000,
-    headerToolbar=[ActionType.Ajax(label='删除该内容所有回复',
-                                   level=LevelEnum.warning,
-                                   confirmText='确定要删除该条内容已学习的回复吗？',
-                                   api='put:/learning_chat/api/delete_all?type=answer&id=${id}')],
-    itemActions=[ActionType.Ajax(tooltip='禁用',
-                                 icon='fa fa-ban text-danger',
-                                 confirmText='禁用并删除该已学回复',
-                                 api='put:/learning_chat/api/ban_chat?type=answer&id=${id}'),
-                 ActionType.Ajax(tooltip='删除',
-                                 icon='fa fa-times text-danger',
-                                 confirmText='仅删除该已学回复，但不禁用，依然能继续学',
-                                 api='delete:/learning_chat/api/delete_chat?type=answer&id=${id}')],
-    columns=[TableColumn(label='ID', name='id', visible=False),
-             TableColumn(label='群ID', name='group_id'),
-             TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='内容/关键词', name='keywords',
-                         searchable=True, popOver={'mode': 'dialog', 'title': '内容全文', 'className': 'break-all',
-                                                   'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
-             TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='最后学习时间', name='time',
-                         sortable=True),
-             TableColumn(label='次数', name='count', sortable=True),
-             ColumnList(label='完整消息', name='messages', breakpoint='*', source='${messages}',
-                        listItem=AmisList.Item(body={'name': 'msg'}))
-             ])
-context_table = TableCRUD(mode='table',
-                          title='',
-                          syncLocation=False,
-                          api='/learning_chat/api/get_chat_contexts',
-                          interval=12000,
-                          headerToolbar=[ActionType.Ajax(label='删除所有学习内容',
-                                                         level=LevelEnum.warning,
-                                                         confirmText='确定要删除所有已学习的内容吗？',
-                                                         api='put:/learning_chat/api/delete_all?type=context')],
-                          itemActions=[ActionType.Dialog(tooltip='回复列表',
-                                                         icon='fa fa-book text-info',
-                                                         dialog=Dialog(title='回复列表',
-                                                                       size='lg',
-                                                                       body=answer_table_on_context)),
-                                       ActionType.Ajax(tooltip='禁用',
-                                                       icon='fa fa-ban text-danger',
-                                                       confirmText='禁用并删除该学习的内容及其所有回复',
-                                                       api='put:/learning_chat/api/ban_chat?type=context&id=${id}'),
-                                       ActionType.Ajax(tooltip='删除',
-                                                       icon='fa fa-times text-danger',
-                                                       confirmText='仅删除该学习的内容及其所有回复，但不禁用，依然能继续学',
-                                                       api='delete:/learning_chat/api/delete_chat?type=context&id=${id}')
-                                       ],
-                          footable=True,
-                          columns=[TableColumn(label='ID', name='id', visible=False),
-                                   TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='内容/关键词',
-                                               name='keywords', searchable=True,
-                                               popOver={'mode': 'dialog', 'title': '内容全文', 'className': 'break-all',
-                                                        'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
-                                   TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-                                               label='最后学习时间', name='time', sortable=True),
-                                   TableColumn(label='已学次数', name='count', sortable=True),
-                                   ])
+    headerToolbar=[
+        ActionType.Ajax(
+            label="删除所有学习内容",
+            level=LevelEnum.warning,
+            confirmText="确定要删除所有已学习的内容吗？",
+            api="put:/learning_chat/api/delete_all?type=context",
+        )
+    ],
+    itemActions=[
+        ActionType.Dialog(
+            tooltip="回复列表",
+            icon="fa fa-book text-info",
+            dialog=Dialog(title="回复列表", size="lg", body=answer_table_on_context),
+        ),
+        ActionType.Ajax(
+            tooltip="禁用",
+            icon="fa fa-ban text-danger",
+            confirmText="禁用并删除该学习的内容及其所有回复",
+            api="put:/learning_chat/api/ban_chat?type=context&id=${id}",
+        ),
+        ActionType.Ajax(
+            tooltip="删除",
+            icon="fa fa-times text-danger",
+            confirmText="仅删除该学习的内容及其所有回复，但不禁用，依然能继续学",
+            api="delete:/learning_chat/api/delete_chat?type=context&id=${id}",
+        ),
+    ],
+    footable=True,
+    columns=[
+        TableColumn(label="ID", name="id", visible=False),
+        TableColumn(
+            type="tpl",
+            tpl="${keywords|truncate:20}",
+            label="内容/关键词",
+            name="keywords",
+            searchable=True,
+            popOver={
+                "mode": "dialog",
+                "title": "内容全文",
+                "className": "break-all",
+                "body": {"type": "tpl", "tpl": "${keywords}"},
+            },
+        ),
+        TableColumn(
+            type="tpl",
+            tpl="${time|date:YYYY-MM-DD HH\\:mm\\:ss}",
+            label="最后学习时间",
+            name="time",
+            sortable=True,
+        ),
+        TableColumn(label="已学次数", name="count", sortable=True),
+    ],
+)
 
-message_page = PageSchema(url='/messages', icon='fa fa-comments', label='群聊消息',
-                          schema=Page(title='群聊消息', body=[
-                              Alert(level=LevelEnum.info,
-                                    className='white-space-pre-wrap',
-                                    body=(f'此数据库记录了{NICKNAME}收到的聊天记录。\n'
-                                          '· 点击"禁用"可以将某条聊天记录进行禁用，这样其相关的学习就会列入禁用列表。\n'
-                                          '· 点击"删除"可以删除某条记录，但不会影响它的学习。\n'
-                                          f'· 可以通过搜索{NICKNAME}的QQ号，来查看它的回复记录。')),
-                              message_table]))
-context_page = PageSchema(url='/contexts', icon='fa fa-comment', label='学习内容',
-                          schema=Page(title='内容',
-                                      body=[Alert(level=LevelEnum.info,
-                                                  className='white-space-pre-wrap',
-                                                  body=(f'此数据库记录了{NICKNAME}所学习的内容。\n'
-                                                        '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
-                                                        '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
-                                                        '· 点击"删除"可以删除该学习，让它重新开始学习这句话。')),
-                                            context_table]))
-answer_page = PageSchema(url='/answers', icon='fa fa-commenting-o', label='内容回复',
-                         schema=Page(title='回复',
-                                     body=[Alert(level=LevelEnum.info,
-                                                 className='white-space-pre-wrap',
-                                                 body=(
-                                                     f'此数据库记录了{NICKNAME}已学习到的所有回复，但看不到这些回复属于哪些内容，推荐到"学习内容"表进行操作。\n'
-                                                     '· 点击"禁用"可以将该回复进行禁用，以后不会再学。\n'
-                                                     '· 点击"删除"可以删除该回复，让它重新开始学习。')),
-                                           answer_table]))
-blacklist_page = PageSchema(url='/blacklist', icon='fa fa-ban', label='禁用列表',
-                            schema=Page(title='禁用列表',
-                                        body=[Alert(level=LevelEnum.info,
-                                                    className='white-space-pre-wrap',
-                                                    body=f'此数据库记录了{NICKNAME}被禁用的内容/关键词。\n'
-                                                         '· 可以取消禁用，使其能够重新继续学习。\n'
-                                                         '· 不能在此添加禁用，只能在群中回复[不可以]或者在<配置>中添加屏蔽词来达到禁用效果。'),
-                                              blacklist_table]))
-database_page = PageSchema(label='数据库', icon='fa fa-database',
-                           children=[message_page, context_page, answer_page, blacklist_page])
-config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='配置',
-                         schema=Page(title='配置', initApi='/learning_chat/api/get_group_list',
-                                     body=[global_config_form, group_select, group_config_form]))
-chat_page = PageSchema(label='群聊学习', icon='fa fa-wechat (alias)', children=[config_page, database_page])
+message_page = PageSchema(
+    url="/messages",
+    icon="fa fa-comments",
+    label="群聊消息",
+    schema=Page(
+        title="群聊消息",
+        body=[
+            Alert(
+                level=LevelEnum.info,
+                className="white-space-pre-wrap",
+                body=(
+                    f"此数据库记录了{NICKNAME}收到的聊天记录。\n"
+                    '· 点击"禁用"可以将某条聊天记录进行禁用，这样其相关的学习就会列入禁用列表。\n'
+                    '· 点击"删除"可以删除某条记录，但不会影响它的学习。\n'
+                    f"· 可以通过搜索{NICKNAME}的QQ号，来查看它的回复记录。"
+                ),
+            ),
+            message_table,
+        ],
+    ),
+)
+context_page = PageSchema(
+    url="/contexts",
+    icon="fa fa-comment",
+    label="学习内容",
+    schema=Page(
+        title="内容",
+        body=[
+            Alert(
+                level=LevelEnum.info,
+                className="white-space-pre-wrap",
+                body=(
+                    f"此数据库记录了{NICKNAME}所学习的内容。\n"
+                    '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
+                    '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
+                    '· 点击"删除"可以删除该学习，让它重新开始学习这句话。'
+                ),
+            ),
+            context_table,
+        ],
+    ),
+)
+answer_page = PageSchema(
+    url="/answers",
+    icon="fa fa-commenting-o",
+    label="内容回复",
+    schema=Page(
+        title="回复",
+        body=[
+            Alert(
+                level=LevelEnum.info,
+                className="white-space-pre-wrap",
+                body=(
+                    f'此数据库记录了{NICKNAME}已学习到的所有回复，但看不到这些回复属于哪些内容，推荐到"学习内容"表进行操作。\n'
+                    '· 点击"禁用"可以将该回复进行禁用，以后不会再学。\n'
+                    '· 点击"删除"可以删除该回复，让它重新开始学习。'
+                ),
+            ),
+            answer_table,
+        ],
+    ),
+)
+blacklist_page = PageSchema(
+    url="/blacklist",
+    icon="fa fa-ban",
+    label="禁用列表",
+    schema=Page(
+        title="禁用列表",
+        body=[
+            Alert(
+                level=LevelEnum.info,
+                className="white-space-pre-wrap",
+                body=f"此数据库记录了{NICKNAME}被禁用的内容/关键词。\n"
+                "· 可以取消禁用，使其能够重新继续学习。\n"
+                "· 不能在此添加禁用，只能在群中回复[不可以]或者在<配置>中添加屏蔽词来达到禁用效果。",
+            ),
+            blacklist_table,
+        ],
+    ),
+)
+database_page = PageSchema(
+    label="数据库",
+    icon="fa fa-database",
+    children=[message_page, context_page, answer_page, blacklist_page],
+)
+config_page = PageSchema(
+    url="/configs",
+    isDefaultPage=True,
+    icon="fa fa-wrench",
+    label="配置",
+    schema=Page(
+        title="配置",
+        initApi="/learning_chat/api/get_group_list",
+        interval=60000,
+        body=[global_config_form, group_select, group_config_form],
+    ),
+)
+chat_page = PageSchema(
+    label="群聊学习", icon="fa fa-wechat (alias)", children=[config_page, database_page]
+)
 
-github_logo = Tpl(className='w-full',
-                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>')
-header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
+github_logo = Tpl(
+    className="w-full",
+    tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>',
+)
+header = Flex(
+    className="w-full", justify="flex-end", alignItems="flex-end", items=[github_logo]
+)
 
-admin_app = App(brandName='Learning-Chat',
-                logo='http://static.cherishmoon.fun/LittlePaimon/readme/logo.png',
-                header=header,
-                pages=[{
-                    'children': [config_page, database_page]
-                }],
-                footer='<div class="p-2 text-center bg-blue-100">Copyright © 2021 - 2022 <a href="https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat" target="_blank" class="link-secondary">Learning-Chat</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>')
+admin_app = App(
+    brandName="Learning-Chat",
+    logo="http://static.cherishmoon.fun/LittlePaimon/readme/logo.png",
+    header=header,
+    pages=[{"children": [config_page, database_page]}],
+    footer='<div class="p-2 text-center bg-blue-100">Copyright © 2021 - 2022 <a href="https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat" target="_blank" class="link-secondary">Learning-Chat</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>',
+)
```

#### html2text {}

```diff
@@ -1,271 +1,276 @@
 from amis import ColumnList, AmisList, ActionType, TableCRUD, TableColumn from
 amis import Dialog, PageSchema, Switch, InputNumber, InputTag, Action, App from
-amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal,
-Remark, Html, Page, AmisAPI, Wrapper from amis import LevelEnum, Select,
-InputArray, Alert, Tpl, Flex from .config import NICKNAME logo = Html(html='''
+amis import ( Form, InputText, InputPassword, DisplayModeEnum, Horizontal,
+Remark, Html, Page, AmisAPI, Wrapper, ) from amis import LevelEnum, Select,
+InputArray, Alert, Tpl, Flex from .config import NICKNAME logo = Html( html="""
                                 [Learning-Chat]
              ****** Nonebot-Plugin-Learning-Chat æ§å¶å° ******
                                  Githubä»åº
 
 
-''') login_api = AmisAPI( url='/learning_chat/api/login', method='post',
-adaptor=''' if (payload.status == 0) { localStorage.setItem("token",
-payload.data.token); } return payload; ''' ) login_form = Form(api=login_api,
-title='', body=[ InputText(name='username', label='ç¨æ·å',
-labelRemark=Remark(shape='circle',
-content='åå°ç®¡çç¨æ·åï¼é»è®¤ä¸ºchat')), InputPassword
-(name='password', label='å¯ç ', labelRemark=Remark(shape='circle',
-content='åå°ç®¡çå¯ç ï¼é»è®¤ä¸ºadmin')), ],
+""" ) login_api = AmisAPI( url="/learning_chat/api/login", method="post",
+adaptor=""" if (payload.status == 0) { localStorage.setItem("token",
+payload.data.token); } return payload; """, ) login_form = Form( api=login_api,
+title="", body=[ InputText( name="username", label="ç¨æ·å",
+labelRemark=Remark(shape="circle",
+content="åå°ç®¡çç¨æ·åï¼é»è®¤ä¸ºchat"), ), InputPassword
+( name="password", label="å¯ç ", labelRemark=Remark(shape="circle",
+content="åå°ç®¡çå¯ç ï¼é»è®¤ä¸ºadmin"), ), ],
 mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9,
-offset=5), redirect='/learning_chat/admin') body = Wrapper(className='w-2/5 mx-
-auto my-0 m:w-full', body=login_form) login_page = Page(title='', body=[logo,
-body]) global_config_form = Form( title='å¨å±éç½®', name='global_config',
-initApi='/learning_chat/api/chat_global_config', api='post:/learning_chat/api/
-chat_global_config', body=[ Switch(label='ç¾¤èå­¦ä¹ æ»å¼å³',
-name='total_enable', value='${total_enable}', onText='å¼å¯',
-offText='å³é­', labelRemark=Remark(shape='circle',
-content='å³é­åï¼å¨å±é½å°ä¸ä¼åå­¦ä¹ ååå¤
-(ä½æ¯ä»ä¼å¯¹æ¶å°çæ¶æ¯è¿è¡è®°å½)ã')), Switch
-(label='åå°ç®¡çæ»å¼å³', name='enable_web', value='${enable_web}',
-onText='å¼å¯', offText='å³é­', labelRemark=Remark(shape='circle',
-content='æ¯å¦å¼å¯æ¬åå°ç®¡çï¼è¥å³é­ï¼åæ æ³åè®¿é®æ¬é¡µé¢ã')),
-InputText(label='åå°ç®¡çç¨æ·å', name='web_username', value='$
-{web_username}', labelRemark=Remark(shape='circle',
-content='ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã')), InputPassword
-(label='åå°ç®¡çå¯ç ', name='web_password', value='${web_password}',
-labelRemark=Remark(shape='circle',
-content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
-(label='åå°ç®¡çtokenå¯é¥', name='web_secret_key', value='$
-{web_secret_key}', labelRemark=Remark(shape='circle',
-content='ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã')), InputNumber
-(label='åå¥å³é®è¯æ°é', name='KEYWORDS_SIZE', value='${KEYWORDS_SIZE}',
-visibleOn='${total_enable}', min=2, labelRemark=Remark(shape='circle',
-content='åå¥è¯­å¥æ ç­¾æ°éï¼å½±åå¯¹ä¸å¥è¯çä¸»é¢è¯æåææï¼å»ºè®®ä¿æé»è®¤ä¸º3ã')),
-InputNumber(label='è·¨ç¾¤åå¤éå¼', name='cross_group_threshold', value='$
-{cross_group_threshold}', visibleOn='${total_enable}', min=1,
-labelRemark=Remark(shape='circle',
-content='å½å­¦ä¹ å°çä¸ç§åå¤å¨Nä¸ªç¾¤é½æï¼é£ä¹è¿ä¸ªåå¤å°±ä¼åä¸ºå¨å±åå¤ã')),
-InputNumber(label='æé«å­¦ä¹ æ¬¡æ°', name='learn_max_count', value='$
-{learn_max_count}', visibleOn='${total_enable}', min=2, labelRemark=Remark
-(shape='circle',
-content='å­¦ä¹ çåå¤æé«è½ç´¯è®¡å°çæ¬¡æ°ï¼å¼è¶é«ï¼è¿ä¸ªåå¤å°±ä¼å­¦ä¹ å¾è¶æ·±ï¼è¶å®¹æè¿è¡åå¤ï¼å¦æä¸æ³æ¯æ¬¡é½å¤§æ¦çåºå®åå¤æä¸å¥è¯ï¼å¯ä»¥å°è¯¥å¼è®¾ä½ç¹ã')),
-InputTag(label='å¨å±å±è½è¯', name='ban_words', value='${ban_words}',
-enableBatchAdd=True, placeholder='æ·»å å¨å±å±è½è¯', visibleOn='$
-{total_enable}', joinValues=False, extractValue=True, labelRemark=Remark
-(shape='circle',
-content='å¨å±å±è½è¯ï¼å«æè¿äºè¯çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ï¼é»è®¤å·²å±è½atãåäº«ãè¯­é³ãåè§é¢ç­æ¶æ¯ã
-(åè½¦è¿è¡æ·»å )')), InputTag(label='å¨å±å±è½ç¨æ·', name='ban_users',
-value='${ban_users}', enableBatchAdd=True,
-placeholder='æ·»å å¨å±å±è½ç¨æ·', visibleOn='${total_enable}',
-joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
-content='å¨å±å±è½ç¨æ·ï¼åè¿äºç¨æ·æå³çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ã
-(åè½¦è¿è¡æ·»å )')), InputTag(label='èªå®ä¹è¯å¸', name='dictionary',
-value='${dictionary}', enableBatchAdd=True,
-placeholder='æ·»å èªå®ä¹è¯è¯­', visibleOn='${total_enable}',
-joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
-content='æ·»å èªå®ä¹è¯è¯­ï¼è®©åè¯è½å¤è¯å«æªæ¶å½çè¯æ±ï¼æé«å­¦ä¹ çåç¡®æ§ãä½ å¯ä»¥æ·»å ç¹æ®åè¯ï¼è¿æ ·å­¦ä¹ æ¶å°±ä¼å°è¯¥è¯çä½ä¸ä¸ªæ´ä½ï¼ç®åè¯å¸ä¸­å·²é»è®¤æ·»å é¨ååç¥ç¸å³è¯æ±ã
-(åè½¦è¿è¡æ·»å )')), ], actions=[Action(label='ä¿å­',
-level=LevelEnum.success, type='submit'), Action(label='éç½®',
-level=LevelEnum.warning, type='reset')] ) group_select = Select
-(label='åç¾¤éç½®', name='group_id', source='${group_list}',
-placeholder='éæ©ç¾¤') group_config_form = Form( title='åç¾¤éç½®',
-visibleOn='group_id != null', initApi='/learning_chat/api/
-chat_group_config?group_id=${group_id}', api='post:/learning_chat/api/
-chat_group_config?group_id=${group_id}', body=[ Switch
-(label='ç¾¤èå­¦ä¹ å¼å³', name='enable', value='${enable}', onText='å¼å¯',
-offText='å³é­', labelRemark=Remark(shape='circle',
-content='éå¯¹è¯¥ç¾¤çç¾¤èå­¦ä¹ å¼å³ï¼å³é­åï¼ä»è¯¥ç¾¤ä¸ä¼å­¦ä¹ ååå¤ã')),
-InputNumber(label='åå¤éå¼', name='answer_threshold', value='$
-{answer_threshold}', visibleOn='${enable}', min=2, labelRemark=Remark
-(shape='circle',
-content='å¯ä»¥çè§£ä¸ºå­¦ä¹ æåæéè¦çæ¬¡æ°ï¼å¼è¶ä½å­¦å¾è¶å¿«ã')),
-InputArray(label='åå¤éå¼æé', name='answer_threshold_weights',
-value='${answer_threshold_weights}', items=InputNumber(min=1, max=100,
-value=25, suffix='%'), inline=True, visibleOn='${enable}', labelRemark=Remark
-(shape='circle',
-content='å½±ååå¤éå¼çè®¡ç®æ¹å¼ï¼ä»¥é»è®¤çåå¤éå¼4ãæé
+offset=5), redirect="/learning_chat/admin", ) body = Wrapper(className="w-2/
+5 mx-auto my-0 m:w-full", body=login_form) login_page = Page(title="", body=
+[logo, body]) global_config_form = Form( title="å¨å±éç½®",
+name="global_config", initApi="/learning_chat/api/chat_global_config",
+api="post:/learning_chat/api/chat_global_config", interval=None, body=[ Switch
+( label="ç¾¤èå­¦ä¹ æ»å¼å³", name="total_enable", value="${total_enable}",
+onText="å¼å¯", offText="å³é­", labelRemark=Remark( shape="circle",
+content="å³é­åï¼å¨å±é½å°ä¸ä¼åå­¦ä¹ ååå¤
+(ä½æ¯ä»ä¼å¯¹æ¶å°çæ¶æ¯è¿è¡è®°å½)ã" ), ), Switch
+( label="åå°ç®¡çæ»å¼å³", name="enable_web", value="${enable_web}",
+onText="å¼å¯", offText="å³é­", labelRemark=Remark(shape="circle",
+content="æ¯å¦å¼å¯æ¬åå°ç®¡çï¼è¥å³é­ï¼åæ æ³åè®¿é®æ¬é¡µé¢ã"),
+), InputText( label="åå°ç®¡çç¨æ·å", name="web_username", value="$
+{web_username}", labelRemark=Remark(shape="circle",
+content="ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã"), ), InputPassword
+( label="åå°ç®¡çå¯ç ", name="web_password", value="${web_password}",
+labelRemark=Remark(shape="circle",
+content="ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã"), ), InputText
+( label="åå°ç®¡çtokenå¯é¥", name="web_secret_key", value="$
+{web_secret_key}", labelRemark=Remark(shape="circle",
+content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã"), ), InputNumber
+( label="åå¥å³é®è¯æ°é", name="KEYWORDS_SIZE", value="$
+{KEYWORDS_SIZE}", visibleOn="${total_enable}", min=2, labelRemark=Remark
+( shape="circle",
+content="åå¥è¯­å¥æ ç­¾æ°éï¼å½±åå¯¹ä¸å¥è¯çä¸»é¢è¯æåææï¼å»ºè®®ä¿æé»è®¤ä¸º3ã"
+), ), InputNumber( label="è·¨ç¾¤åå¤éå¼", name="cross_group_threshold",
+value="${cross_group_threshold}", visibleOn="${total_enable}", min=1,
+labelRemark=Remark( shape="circle",
+content="å½å­¦ä¹ å°çä¸ç§åå¤å¨Nä¸ªç¾¤é½æï¼é£ä¹è¿ä¸ªåå¤å°±ä¼åä¸ºå¨å±åå¤ã"
+), ), InputNumber( label="æé«å­¦ä¹ æ¬¡æ°", name="learn_max_count", value="$
+{learn_max_count}", visibleOn="${total_enable}", min=2, labelRemark=Remark
+( shape="circle",
+content="å­¦ä¹ çåå¤æé«è½ç´¯è®¡å°çæ¬¡æ°ï¼å¼è¶é«ï¼è¿ä¸ªåå¤å°±ä¼å­¦ä¹ å¾è¶æ·±ï¼è¶å®¹æè¿è¡åå¤ï¼å¦æä¸æ³æ¯æ¬¡é½å¤§æ¦çåºå®åå¤æä¸å¥è¯ï¼å¯ä»¥å°è¯¥å¼è®¾ä½ç¹ã",
+), ), InputTag( label="å¨å±å±è½è¯", name="ban_words", value="$
+{ban_words}", enableBatchAdd=True, placeholder="æ·»å å¨å±å±è½è¯",
+visibleOn="${total_enable}", joinValues=False, extractValue=True,
+labelRemark=Remark( shape="circle",
+content="å¨å±å±è½è¯ï¼å«æè¿äºè¯çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ï¼é»è®¤å·²å±è½atãåäº«ãè¯­é³ãåè§é¢ç­æ¶æ¯ã
+(åè½¦è¿è¡æ·»å )", ), ), InputTag( label="å¨å±å±è½ç¨æ·",
+name="ban_users", value="${ban_users}", enableBatchAdd=True,
+placeholder="æ·»å å¨å±å±è½ç¨æ·", visibleOn="${total_enable}",
+joinValues=False, extractValue=True, labelRemark=Remark( shape="circle",
+content="å¨å±å±è½ç¨æ·ï¼åè¿äºç¨æ·æå³çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ã
+(åè½¦è¿è¡æ·»å )" ), ), InputTag( label="èªå®ä¹è¯å¸",
+name="dictionary", value="${dictionary}", enableBatchAdd=True,
+placeholder="æ·»å èªå®ä¹è¯è¯­", visibleOn="${total_enable}",
+joinValues=False, extractValue=True, labelRemark=Remark( shape="circle",
+content="æ·»å èªå®ä¹è¯è¯­ï¼è®©åè¯è½å¤è¯å«æªæ¶å½çè¯æ±ï¼æé«å­¦ä¹ çåç¡®æ§ãä½ å¯ä»¥æ·»å ç¹æ®åè¯ï¼è¿æ ·å­¦ä¹ æ¶å°±ä¼å°è¯¥è¯çä½ä¸ä¸ªæ´ä½ï¼ç®åè¯å¸ä¸­å·²é»è®¤æ·»å é¨ååç¥ç¸å³è¯æ±ã
+(åè½¦è¿è¡æ·»å )", ), ), ], actions=[ Action(label="ä¿å­",
+level=LevelEnum.success, type="submit"), Action(label="éç½®",
+level=LevelEnum.warning, type="reset"), ], ) group_select = Select
+( label="åç¾¤éç½®", name="group_id", source="${group_list}",
+placeholder="éæ©ç¾¤" ) group_config_form = Form( title="åç¾¤éç½®",
+visibleOn="group_id != null", initApi="/learning_chat/api/
+chat_group_config?group_id=${group_id}", api="post:/learning_chat/api/
+chat_group_config?group_id=${group_id}", interval=None, body=[ Switch
+( label="ç¾¤èå­¦ä¹ å¼å³", name="enable", value="${enable}",
+onText="å¼å¯", offText="å³é­", labelRemark=Remark(shape="circle",
+content="éå¯¹è¯¥ç¾¤çç¾¤èå­¦ä¹ å¼å³ï¼å³é­åï¼ä»è¯¥ç¾¤ä¸ä¼å­¦ä¹ ååå¤ã"),
+), InputNumber( label="åå¤éå¼", name="answer_threshold", value="$
+{answer_threshold}", visibleOn="${enable}", min=2, labelRemark=Remark
+(shape="circle",
+content="å¯ä»¥çè§£ä¸ºå­¦ä¹ æåæéè¦çæ¬¡æ°ï¼å¼è¶ä½å­¦å¾è¶å¿«ã"),
+), InputArray( label="åå¤éå¼æé", name="answer_threshold_weights",
+value="${answer_threshold_weights}", items=InputNumber(min=1, max=100,
+value=25, suffix="%"), inline=True, visibleOn="${enable}", labelRemark=Remark
+( shape="circle",
+content="å½±ååå¤éå¼çè®¡ç®æ¹å¼ï¼ä»¥é»è®¤çåå¤éå¼4ãæé
 [10, 30,
-60]ä¸ºä¾ï¼å¨è®¡ç®éå¼æ¶ï¼60%æ¦çä¸º4ï¼30%æ¦çä¸º3ï¼10%æ¦çä¸º2ã')),
-InputNumber(label='å¤è¯»éå¼', name='repeat_threshold', value='$
-{repeat_threshold}', visibleOn='${enable}', min=2, labelRemark=Remark
-(shape='circle',
-content=f'è·éå¤è¯»æéè¦çéå¼ï¼æNä¸ªäººå¤è¯»åï¼
-{NICKNAME}å°±ä¼è·çå¤è¯»ã')), InputNumber(label='ææ­å¤è¯»æ¦ç',
-name='break_probability', value='${break_probability}', min=0, max=100,
-suffix='%', visibleOn='${AND(enable, speak_enable)}', labelRemark=Remark
-(shape='circle',
-content='è¾¾å°å¤è¯»éå¼æ¶ï¼ææ­å¤è¯»èä¸æ¯è·éå¤è¯»çæ¦çã')),
-InputTag(label='å±è½è¯', name='ban_words', value='${ban_words}',
-enableBatchAdd=True, placeholder='æ·»å å±è½è¯', visibleOn='${enable}',
-joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
-content='å«æè¿äºè¯çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ã
-(åè½¦è¿è¡æ·»å )')), InputTag(label='å±è½ç¨æ·', source='$
-{member_list}', name='ban_users', value='${ban_users}', enableBatchAdd=True,
-placeholder='æ·»å å±è½ç¨æ·', visibleOn='${enable}', joinValues=False,
-extractValue=True, labelRemark=Remark(shape='circle',
-content='åè¯¥ç¾¤ä¸­è¿äºç¨æ·æå³çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ã
-(åè½¦è¿è¡æ·»å )')), Switch(label='ä¸»å¨åè¨å¼å³',
-name='speak_enable', value='${speak_enable}', visibleOn='${enable}',
-labelRemark=Remark(shape='circle', content=f'æ¯å¦åè®¸
-{NICKNAME}å¨è¯¥ç¾¤ä¸»å¨åè¨ï¼ä¸»å¨åè¨æ¯ææ¯éä¸æ®µæ¶é´æéä¸ä¸ªç­åº¦è¾é«çç¾¤ï¼ä¸»å¨åä¸äºå­¦ä¹ è¿çåå®¹ã')),
-InputNumber(label='ä¸»å¨åè¨éå¼', name='speak_threshold', value='$
-{speak_threshold}', visibleOn='${AND(enable, speak_enable)}', min=0,
-labelRemark=Remark(shape='circle',
-content='å¼è¶ä½ï¼ä¸»å¨åè¨çå¯è½æ§è¶é«ã')), InputNumber
-(label='ä¸»å¨åè¨æå°é´é', name='speak_min_interval', value='$
-{speak_min_interval}', min=0, visibleOn='${AND(enable, speak_enable)}',
-suffix='ç§', labelRemark=Remark(shape='circle',
-content='è¿è¡ä¸»å¨åè¨çæå°æ¶é´é´éã')), InputNumber
-(label='è¿ç»­ä¸»å¨åè¨æ¦ç', name='speak_continuously_probability',
-value='${speak_continuously_probability}', min=0, max=100, suffix='%',
-visibleOn='${AND(enable, speak_enable)}', labelRemark=Remark(shape='circle',
-content='è§¦åä¸»å¨åè¨æ¶ï¼è¿ç»­è¿è¡åè¨çæ¦çã')), InputNumber
-(label='æå¤§è¿ç»­ä¸»å¨åè¨å¥æ°', name='speak_continuously_max_len',
-value='${speak_continuously_max_len}', visibleOn='${AND(enable,
-speak_enable)}', min=1, labelRemark=Remark(shape='circle',
-content='è¿ç»­ä¸»å¨åè¨çæå¤§å¥æ°ã')), InputNumber
-(label='ä¸»å¨åè¨éå¸¦æ³ä¸æ³æ¦ç', name='speak_poke_probability',
-value='${speak_poke_probability}', min=0, max=100, suffix='%', visibleOn='${AND
-(enable, speak_enable)}', labelRemark=Remark(shape='circle',
-content='ä¸»å¨åè¨æ¶éå¸¦æ³ä¸æ³çæ¦çï¼ä¼å¨æè¿5ä¸ªåè¨èä¸­éæºéä¸ä¸ªæ³ã')),
-], actions=[Action(label='ä¿å­', level=LevelEnum.success, type='submit'),
-ActionType.Ajax( label='ä¿å­è³ææç¾¤', level=LevelEnum.primary,
-confirmText='ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼', api='post:/
-learning_chat/api/chat_group_config?group_id=all' ), Action(label='éç½®',
-level=LevelEnum.warning, type='reset')] ) blacklist_table = TableCRUD
-(mode='table', title='', syncLocation=False, api='/learning_chat/api/
-get_chat_blacklist', interval=15000, headerToolbar=[ActionType.Ajax
-(label='åæ¶ææç¦ç¨', level=LevelEnum.warning,
-confirmText='ç¡®å®è¦åæ¶ææç¦ç¨åï¼', api='put:/learning_chat/api/
-delete_all?type=blacklist')], itemActions=[ActionType.Ajax
-(tooltip='åæ¶ç¦ç¨', icon='fa fa-check-circle-o text-info',
-confirmText='åæ¶è¯¥è¢«ç¦ç¨çåå®¹/
-å³é®è¯ï¼ä½æ¯ä»ç¶éè¦éæ°å­¦ä¹ å¦ï¼', api='delete:/learning_chat/
-api/delete_chat?type=blacklist&id=${id}') ], footable=True, columns=
-[TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='åå®¹/
-å³é®è¯', name='keywords', searchable=True, popOver={'mode': 'dialog',
-'title': 'å¨æ', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
-{keywords}'}}), TableColumn(label='å·²ç¦ç¨çç¾¤', name='bans',
-searchable=True), ]) message_table = TableCRUD(mode='table', title='',
-syncLocation=False, api='/learning_chat/api/get_chat_messages', interval=12000,
-headerToolbar=[ActionType.Ajax(label='å é¤ææèå¤©è®°å½',
-level=LevelEnum.warning, confirmText='ç¡®å®è¦å é¤ææèå¤©è®°å½åï¼',
-api='put:/learning_chat/api/delete_all?type=message')], itemActions=
-[ActionType.Ajax(tooltip='ç¦ç¨', icon='fa fa-ban text-danger',
-confirmText='ç¦ç¨è¯¥èå¤©è®°å½ç¸å³çå­¦ä¹ åå®¹ååå¤', api='put:/
-learning_chat/api/ban_chat?type=message&id=${id}'), ActionType.Ajax
-(tooltip='å é¤', icon='fa fa-times text-danger',
-confirmText='å é¤è¯¥æ¡èå¤©è®°å½', api='delete:/learning_chat/api/
-delete_chat?type=message&id=${id}') ], footable=True, columns=[TableColumn
-(label='æ¶æ¯ID', name='message_id'), TableColumn(label='ç¾¤ID',
-name='group_id', searchable=True), TableColumn(label='ç¨æ·ID',
-name='user_id', searchable=True), TableColumn(type='tpl', tpl='$
-{raw_message|truncate:20}', label='æ¶æ¯', name='message', searchable=True,
-popOver={'mode': 'dialog', 'title': 'æ¶æ¯å¨æ', 'className': 'break-all',
-'body': {'type': 'tpl', 'tpl': '${raw_message}'}}), TableColumn(type='tpl',
-tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='æ¶é´', name='time',
-sortable=True) ]) answer_table = TableCRUD( mode='table', syncLocation=False,
-footable=True, api='/learning_chat/api/get_chat_answers', interval=12000,
-headerToolbar=[ActionType.Ajax(label='å é¤ææå·²å­¦ä¹ çåå¤',
-level=LevelEnum.warning,
-confirmText='ç¡®å®è¦å é¤ææå·²å­¦ä¹ çåå¤åï¼', api='put:/
-learning_chat/api/delete_all?type=answer')], itemActions=[ActionType.Ajax
-(tooltip='ç¦ç¨', icon='fa fa-ban text-danger',
-confirmText='ç¦ç¨å¹¶å é¤è¯¥å·²å­¦åå¤', api='put:/learning_chat/api/
-ban_chat?type=answer&id=${id}'), ActionType.Ajax(tooltip='å é¤', icon='fa fa-
-times text-danger',
-confirmText='ä»å é¤è¯¥å·²å­¦åå¤ï¼ä¸ä¼ç¦ç¨ï¼æä»¥ä¾ç¶è½ç»§ç»­å­¦',
-api='delete:/learning_chat/api/delete_chat?type=answer&id=${id}')], columns=
-[TableColumn(label='ID', name='id', visible=False), TableColumn(label='ç¾¤ID',
-name='group_id', searchable=True), TableColumn(type='tpl', tpl='$
-{keywords|truncate:20}', label='åå®¹/å³é®è¯', name='keywords',
-searchable=True, popOver={'mode': 'dialog', 'title': 'åå®¹å¨æ',
-'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
-TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-label='æåå­¦ä¹ æ¶é´', name='time', sortable=True), TableColumn
-(label='æ¬¡æ°', name='count', sortable=True), ColumnList(label='å®æ´æ¶æ¯',
-name='messages', breakpoint='*', source='${messages}', listItem=AmisList.Item
-(body={'name': 'msg'})) ]) answer_table_on_context = TableCRUD( mode='table',
-syncLocation=False, footable=True, api='/learning_chat/api/
-get_chat_answers?context_id=${id}&page=${page}&perPage=${perPage}&orderBy=$
-{orderBy}&orderDir=${orderDir}', interval=12000, headerToolbar=[ActionType.Ajax
-(label='å é¤è¯¥åå®¹ææåå¤', level=LevelEnum.warning,
-confirmText='ç¡®å®è¦å é¤è¯¥æ¡åå®¹å·²å­¦ä¹ çåå¤åï¼', api='put:/
-learning_chat/api/delete_all?type=answer&id=${id}')], itemActions=
-[ActionType.Ajax(tooltip='ç¦ç¨', icon='fa fa-ban text-danger',
-confirmText='ç¦ç¨å¹¶å é¤è¯¥å·²å­¦åå¤', api='put:/learning_chat/api/
-ban_chat?type=answer&id=${id}'), ActionType.Ajax(tooltip='å é¤', icon='fa fa-
-times text-danger',
-confirmText='ä»å é¤è¯¥å·²å­¦åå¤ï¼ä½ä¸ç¦ç¨ï¼ä¾ç¶è½ç»§ç»­å­¦',
-api='delete:/learning_chat/api/delete_chat?type=answer&id=${id}')], columns=
-[TableColumn(label='ID', name='id', visible=False), TableColumn(label='ç¾¤ID',
-name='group_id'), TableColumn(type='tpl', tpl='${keywords|truncate:20}',
-label='åå®¹/å³é®è¯', name='keywords', searchable=True, popOver={'mode':
-'dialog', 'title': 'åå®¹å¨æ', 'className': 'break-all', 'body': {'type':
-'tpl', 'tpl': '${keywords}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-
-MM-DD HH\\:mm\\:ss}', label='æåå­¦ä¹ æ¶é´', name='time', sortable=True),
-TableColumn(label='æ¬¡æ°', name='count', sortable=True), ColumnList
-(label='å®æ´æ¶æ¯', name='messages', breakpoint='*', source='${messages}',
-listItem=AmisList.Item(body={'name': 'msg'})) ]) context_table = TableCRUD
-(mode='table', title='', syncLocation=False, api='/learning_chat/api/
-get_chat_contexts', interval=12000, headerToolbar=[ActionType.Ajax
-(label='å é¤ææå­¦ä¹ åå®¹', level=LevelEnum.warning,
-confirmText='ç¡®å®è¦å é¤ææå·²å­¦ä¹ çåå®¹åï¼', api='put:/
-learning_chat/api/delete_all?type=context')], itemActions=[ActionType.Dialog
-(tooltip='åå¤åè¡¨', icon='fa fa-book text-info', dialog=Dialog
-(title='åå¤åè¡¨', size='lg', body=answer_table_on_context)),
-ActionType.Ajax(tooltip='ç¦ç¨', icon='fa fa-ban text-danger',
-confirmText='ç¦ç¨å¹¶å é¤è¯¥å­¦ä¹ çåå®¹åå¶ææåå¤', api='put:/
-learning_chat/api/ban_chat?type=context&id=${id}'), ActionType.Ajax
-(tooltip='å é¤', icon='fa fa-times text-danger',
-confirmText='ä»å é¤è¯¥å­¦ä¹ çåå®¹åå¶ææåå¤ï¼ä½ä¸ç¦ç¨ï¼ä¾ç¶è½ç»§ç»­å­¦',
-api='delete:/learning_chat/api/delete_chat?type=context&id=${id}') ],
-footable=True, columns=[TableColumn(label='ID', name='id', visible=False),
-TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='åå®¹/
-å³é®è¯', name='keywords', searchable=True, popOver={'mode': 'dialog',
-'title': 'åå®¹å¨æ', 'className': 'break-all', 'body': {'type': 'tpl',
-'tpl': '${keywords}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD
-HH\\:mm\\:ss}', label='æåå­¦ä¹ æ¶é´', name='time', sortable=True),
-TableColumn(label='å·²å­¦æ¬¡æ°', name='count', sortable=True), ]) message_page
-= PageSchema(url='/messages', icon='fa fa-comments', label='ç¾¤èæ¶æ¯',
-schema=Page(title='ç¾¤èæ¶æ¯', body=[ Alert(level=LevelEnum.info,
-className='white-space-pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
-{NICKNAME}æ¶å°çèå¤©è®°å½ã\n' 'Â·
+60]ä¸ºä¾ï¼å¨è®¡ç®éå¼æ¶ï¼60%æ¦çä¸º4ï¼30%æ¦çä¸º3ï¼10%æ¦çä¸º2ã",
+), ), InputNumber( label="å¤è¯»éå¼", name="repeat_threshold", value="$
+{repeat_threshold}", visibleOn="${enable}", min=2, labelRemark=Remark
+( shape="circle",
+content=f"è·éå¤è¯»æéè¦çéå¼ï¼æNä¸ªäººå¤è¯»åï¼
+{NICKNAME}å°±ä¼è·çå¤è¯»ã" ), ), InputNumber( label="ææ­å¤è¯»æ¦ç",
+name="break_probability", value="${break_probability}", min=0, max=100,
+suffix="%", visibleOn="${AND(enable, speak_enable)}", labelRemark=Remark
+(shape="circle",
+content="è¾¾å°å¤è¯»éå¼æ¶ï¼ææ­å¤è¯»èä¸æ¯è·éå¤è¯»çæ¦çã"),
+), InputTag( label="å±è½è¯", name="ban_words", value="${ban_words}",
+enableBatchAdd=True, placeholder="æ·»å å±è½è¯", visibleOn="${enable}",
+joinValues=False, extractValue=True, labelRemark=Remark(shape="circle",
+content="å«æè¿äºè¯çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ã
+(åè½¦è¿è¡æ·»å )"), ), InputTag( label="å±è½ç¨æ·", source="$
+{member_list}", name="ban_users", value="${ban_users}", enableBatchAdd=True,
+placeholder="æ·»å å±è½ç¨æ·", visibleOn="${enable}", joinValues=False,
+extractValue=True, labelRemark=Remark(shape="circle",
+content="åè¯¥ç¾¤ä¸­è¿äºç¨æ·æå³çæ¶æ¯ä¸ä¼å­¦ä¹ ååå¤ã
+(åè½¦è¿è¡æ·»å )"), ), Switch( label="ä¸»å¨åè¨å¼å³",
+name="speak_enable", value="${speak_enable}", visibleOn="${enable}",
+labelRemark=Remark( shape="circle", content=f"æ¯å¦åè®¸
+{NICKNAME}å¨è¯¥ç¾¤ä¸»å¨åè¨ï¼ä¸»å¨åè¨æ¯ææ¯éä¸æ®µæ¶é´æéä¸ä¸ªç­åº¦è¾é«çç¾¤ï¼ä¸»å¨åä¸äºå­¦ä¹ è¿çåå®¹ã",
+), ), InputNumber( label="ä¸»å¨åè¨éå¼", name="speak_threshold", value="$
+{speak_threshold}", visibleOn="${AND(enable, speak_enable)}", min=0,
+labelRemark=Remark(shape="circle",
+content="å¼è¶ä½ï¼ä¸»å¨åè¨çå¯è½æ§è¶é«ã"), ), InputNumber
+( label="ä¸»å¨åè¨æå°é´é", name="speak_min_interval", value="$
+{speak_min_interval}", min=0, visibleOn="${AND(enable, speak_enable)}",
+suffix="ç§", labelRemark=Remark(shape="circle",
+content="è¿è¡ä¸»å¨åè¨çæå°æ¶é´é´éã"), ), InputNumber
+( label="è¿ç»­ä¸»å¨åè¨æ¦ç", name="speak_continuously_probability",
+value="${speak_continuously_probability}", min=0, max=100, suffix="%",
+visibleOn="${AND(enable, speak_enable)}", labelRemark=Remark(shape="circle",
+content="è§¦åä¸»å¨åè¨æ¶ï¼è¿ç»­è¿è¡åè¨çæ¦çã"), ),
+InputNumber( label="æå¤§è¿ç»­ä¸»å¨åè¨å¥æ°",
+name="speak_continuously_max_len", value="${speak_continuously_max_len}",
+visibleOn="${AND(enable, speak_enable)}", min=1, labelRemark=Remark
+(shape="circle", content="è¿ç»­ä¸»å¨åè¨çæå¤§å¥æ°ã"), ),
+InputNumber( label="ä¸»å¨åè¨éå¸¦æ³ä¸æ³æ¦ç",
+name="speak_poke_probability", value="${speak_poke_probability}", min=0,
+max=100, suffix="%", visibleOn="${AND(enable, speak_enable)}",
+labelRemark=Remark( shape="circle",
+content="ä¸»å¨åè¨æ¶éå¸¦æ³ä¸æ³çæ¦çï¼ä¼å¨æè¿5ä¸ªåè¨èä¸­éæºéä¸ä¸ªæ³ã"
+), ), ], actions=[ Action(label="ä¿å­", level=LevelEnum.success,
+type="submit"), ActionType.Ajax( label="ä¿å­è³ææç¾¤",
+level=LevelEnum.primary,
+confirmText="ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼", api="post:/
+learning_chat/api/chat_group_config?group_id=all", ), Action(label="éç½®",
+level=LevelEnum.warning, type="reset"), ], ) blacklist_table = TableCRUD
+( mode="table", title="", syncLocation=False, api="/learning_chat/api/
+get_chat_blacklist", interval=15000, headerToolbar=[ ActionType.Ajax
+( label="åæ¶ææç¦ç¨", level=LevelEnum.warning,
+confirmText="ç¡®å®è¦åæ¶ææç¦ç¨åï¼", api="put:/learning_chat/api/
+delete_all?type=blacklist", ) ], itemActions=[ ActionType.Ajax
+( tooltip="åæ¶ç¦ç¨", icon="fa fa-check-circle-o text-info",
+confirmText="åæ¶è¯¥è¢«ç¦ç¨çåå®¹/
+å³é®è¯ï¼ä½æ¯ä»ç¶éè¦éæ°å­¦ä¹ å¦ï¼", api="delete:/learning_chat/
+api/delete_chat?type=blacklist&id=${id}", ) ], footable=True, columns=
+[ TableColumn( type="tpl", tpl="${keywords|truncate:20}", label="åå®¹/
+å³é®è¯", name="keywords", searchable=True, popOver={ "mode": "dialog",
+"title": "å¨æ", "className": "break-all", "body": {"type": "tpl", "tpl": "$
+{keywords}"}, }, ), TableColumn(label="å·²ç¦ç¨çç¾¤", name="bans",
+searchable=True), ], ) message_table = TableCRUD( mode="table", title="",
+syncLocation=False, api="/learning_chat/api/get_chat_messages", interval=12000,
+headerToolbar=[ ActionType.Ajax( label="å é¤ææèå¤©è®°å½",
+level=LevelEnum.warning, confirmText="ç¡®å®è¦å é¤ææèå¤©è®°å½åï¼",
+api="put:/learning_chat/api/delete_all?type=message", ) ], itemActions=
+[ ActionType.Ajax( tooltip="ç¦ç¨", icon="fa fa-ban text-danger",
+confirmText="ç¦ç¨è¯¥èå¤©è®°å½ç¸å³çå­¦ä¹ åå®¹ååå¤", api="put:/
+learning_chat/api/ban_chat?type=message&id=${id}", ), ActionType.Ajax
+( tooltip="å é¤", icon="fa fa-times text-danger",
+confirmText="å é¤è¯¥æ¡èå¤©è®°å½", api="delete:/learning_chat/api/
+delete_chat?type=message&id=${id}", ), ], footable=True, columns=[ TableColumn
+(label="æ¶æ¯ID", name="message_id"), TableColumn(label="ç¾¤ID",
+name="group_id", searchable=True), TableColumn(label="ç¨æ·ID",
+name="user_id", searchable=True), TableColumn( type="tpl", tpl="$
+{raw_message|truncate:20}", label="æ¶æ¯", name="message", searchable=True,
+popOver={ "mode": "dialog", "title": "æ¶æ¯å¨æ", "className": "break-all",
+"body": {"type": "tpl", "tpl": "${raw_message}"}, }, ), TableColumn
+( type="tpl", tpl="${time|date:YYYY-MM-DD HH\\:mm\\:ss}", label="æ¶é´",
+name="time", sortable=True, ), ], ) answer_table = TableCRUD( mode="table",
+syncLocation=False, footable=True, api="/learning_chat/api/get_chat_answers",
+interval=12000, headerToolbar=[ ActionType.Ajax
+( label="å é¤ææå·²å­¦ä¹ çåå¤", level=LevelEnum.warning,
+confirmText="ç¡®å®è¦å é¤ææå·²å­¦ä¹ çåå¤åï¼", api="put:/
+learning_chat/api/delete_all?type=answer", ) ], itemActions=[ ActionType.Ajax
+( tooltip="ç¦ç¨", icon="fa fa-ban text-danger",
+confirmText="ç¦ç¨å¹¶å é¤è¯¥å·²å­¦åå¤", api="put:/learning_chat/api/
+ban_chat?type=answer&id=${id}", ), ActionType.Ajax( tooltip="å é¤", icon="fa
+fa-times text-danger",
+confirmText="ä»å é¤è¯¥å·²å­¦åå¤ï¼ä¸ä¼ç¦ç¨ï¼æä»¥ä¾ç¶è½ç»§ç»­å­¦",
+api="delete:/learning_chat/api/delete_chat?type=answer&id=${id}", ), ],
+columns=[ TableColumn(label="ID", name="id", visible=False), TableColumn
+(label="ç¾¤ID", name="group_id", searchable=True), TableColumn( type="tpl",
+tpl="${keywords|truncate:20}", label="åå®¹/å³é®è¯", name="keywords",
+searchable=True, popOver={ "mode": "dialog", "title": "åå®¹å¨æ",
+"className": "break-all", "body": {"type": "tpl", "tpl": "${keywords}"}, }, ),
+TableColumn( type="tpl", tpl="${time|date:YYYY-MM-DD HH\\:mm\\:ss}",
+label="æåå­¦ä¹ æ¶é´", name="time", sortable=True, ), TableColumn
+(label="æ¬¡æ°", name="count", sortable=True), ColumnList
+( label="å®æ´æ¶æ¯", name="messages", breakpoint="*", source="${messages}",
+listItem=AmisList.Item(body=[AmisList.Item.ListBodyField(name="msg")]), ), ], )
+answer_table_on_context = TableCRUD( mode="table", syncLocation=False,
+footable=True, api="/learning_chat/api/get_chat_answers?context_id=${id}&page=$
+{page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}",
+interval=12000, headerToolbar=[ ActionType.Ajax
+( label="å é¤è¯¥åå®¹ææåå¤", level=LevelEnum.warning,
+confirmText="ç¡®å®è¦å é¤è¯¥æ¡åå®¹å·²å­¦ä¹ çåå¤åï¼", api="put:/
+learning_chat/api/delete_all?type=answer&id=${id}", ) ], itemActions=
+[ ActionType.Ajax( tooltip="ç¦ç¨", icon="fa fa-ban text-danger",
+confirmText="ç¦ç¨å¹¶å é¤è¯¥å·²å­¦åå¤", api="put:/learning_chat/api/
+ban_chat?type=answer&id=${id}", ), ActionType.Ajax( tooltip="å é¤", icon="fa
+fa-times text-danger",
+confirmText="ä»å é¤è¯¥å·²å­¦åå¤ï¼ä½ä¸ç¦ç¨ï¼ä¾ç¶è½ç»§ç»­å­¦",
+api="delete:/learning_chat/api/delete_chat?type=answer&id=${id}", ), ],
+columns=[ TableColumn(label="ID", name="id", visible=False), TableColumn
+(label="ç¾¤ID", name="group_id"), TableColumn( type="tpl", tpl="$
+{keywords|truncate:20}", label="åå®¹/å³é®è¯", name="keywords",
+searchable=True, popOver={ "mode": "dialog", "title": "åå®¹å¨æ",
+"className": "break-all", "body": {"type": "tpl", "tpl": "${keywords}"}, }, ),
+TableColumn( type="tpl", tpl="${time|date:YYYY-MM-DD HH\\:mm\\:ss}",
+label="æåå­¦ä¹ æ¶é´", name="time", sortable=True, ), TableColumn
+(label="æ¬¡æ°", name="count", sortable=True), ColumnList
+( label="å®æ´æ¶æ¯", name="messages", breakpoint="*", source="${messages}",
+listItem=AmisList.Item(body=[AmisList.Item.ListBodyField(name="msg")]), ), ], )
+context_table = TableCRUD( mode="table", title="", syncLocation=False, api="/
+learning_chat/api/get_chat_contexts", interval=12000, headerToolbar=
+[ ActionType.Ajax( label="å é¤ææå­¦ä¹ åå®¹", level=LevelEnum.warning,
+confirmText="ç¡®å®è¦å é¤ææå·²å­¦ä¹ çåå®¹åï¼", api="put:/
+learning_chat/api/delete_all?type=context", ) ], itemActions=
+[ ActionType.Dialog( tooltip="åå¤åè¡¨", icon="fa fa-book text-info",
+dialog=Dialog(title="åå¤åè¡¨", size="lg", body=answer_table_on_context),
+), ActionType.Ajax( tooltip="ç¦ç¨", icon="fa fa-ban text-danger",
+confirmText="ç¦ç¨å¹¶å é¤è¯¥å­¦ä¹ çåå®¹åå¶ææåå¤", api="put:/
+learning_chat/api/ban_chat?type=context&id=${id}", ), ActionType.Ajax
+( tooltip="å é¤", icon="fa fa-times text-danger",
+confirmText="ä»å é¤è¯¥å­¦ä¹ çåå®¹åå¶ææåå¤ï¼ä½ä¸ç¦ç¨ï¼ä¾ç¶è½ç»§ç»­å­¦",
+api="delete:/learning_chat/api/delete_chat?type=context&id=${id}", ), ],
+footable=True, columns=[ TableColumn(label="ID", name="id", visible=False),
+TableColumn( type="tpl", tpl="${keywords|truncate:20}", label="åå®¹/
+å³é®è¯", name="keywords", searchable=True, popOver={ "mode": "dialog",
+"title": "åå®¹å¨æ", "className": "break-all", "body": {"type": "tpl",
+"tpl": "${keywords}"}, }, ), TableColumn( type="tpl", tpl="${time|date:YYYY-MM-
+DD HH\\:mm\\:ss}", label="æåå­¦ä¹ æ¶é´", name="time", sortable=True, ),
+TableColumn(label="å·²å­¦æ¬¡æ°", name="count", sortable=True), ], )
+message_page = PageSchema( url="/messages", icon="fa fa-comments",
+label="ç¾¤èæ¶æ¯", schema=Page( title="ç¾¤èæ¶æ¯", body=[ Alert
+( level=LevelEnum.info, className="white-space-pre-wrap", body=
+( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æ¶å°çèå¤©è®°å½ã\n" 'Â·
 ç¹å»"ç¦ç¨"å¯ä»¥å°ææ¡èå¤©è®°å½è¿è¡ç¦ç¨ï¼è¿æ ·å¶ç¸å³çå­¦ä¹ å°±ä¼åå¥ç¦ç¨åè¡¨ã\n'
 'Â· ç¹å»"å é¤"å¯ä»¥å é¤ææ¡è®°å½ï¼ä½ä¸ä¼å½±åå®çå­¦ä¹ ã\n'
-f'Â· å¯ä»¥éè¿æç´¢{NICKNAME}çQQå·ï¼æ¥æ¥çå®çåå¤è®°å½ã')),
-message_table])) context_page = PageSchema(url='/contexts', icon='fa fa-
-comment', label='å­¦ä¹ åå®¹', schema=Page(title='åå®¹', body=[Alert
-(level=LevelEnum.info, className='white-space-pre-wrap', body=
-(f'æ­¤æ°æ®åºè®°å½äº{NICKNAME}æå­¦ä¹ çåå®¹ã\n' 'Â·
+f"Â· å¯ä»¥éè¿æç´¢{NICKNAME}çQQå·ï¼æ¥æ¥çå®çåå¤è®°å½ã" ),
+), message_table, ], ), ) context_page = PageSchema( url="/contexts", icon="fa
+fa-comment", label="å­¦ä¹ åå®¹", schema=Page( title="åå®¹", body=[ Alert
+( level=LevelEnum.info, className="white-space-pre-wrap", body=
+( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æå­¦ä¹ çåå®¹ã\n" 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n' 'Â·
-ç¹å»"å é¤"å¯ä»¥å é¤è¯¥å­¦ä¹ ï¼è®©å®éæ°å¼å§å­¦ä¹ è¿å¥è¯ã')),
-context_table])) answer_page = PageSchema(url='/answers', icon='fa fa-
-commenting-o', label='åå®¹åå¤', schema=Page(title='åå¤', body=[Alert
-(level=LevelEnum.info, className='white-space-pre-wrap', body=
+ç¹å»"å é¤"å¯ä»¥å é¤è¯¥å­¦ä¹ ï¼è®©å®éæ°å¼å§å­¦ä¹ è¿å¥è¯ã' ),
+), context_table, ], ), ) answer_page = PageSchema( url="/answers", icon="fa
+fa-commenting-o", label="åå®¹åå¤", schema=Page( title="åå¤", body=
+[ Alert( level=LevelEnum.info, className="white-space-pre-wrap", body=
 ( f'æ­¤æ°æ®åºè®°å½äº
 {NICKNAME}å·²å­¦ä¹ å°çææåå¤ï¼ä½çä¸å°è¿äºåå¤å±äºåªäºåå®¹ï¼æ¨èå°"å­¦ä¹ åå®¹"è¡¨è¿è¡æä½ã\n'
 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥åå¤è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n' 'Â·
-ç¹å»"å é¤"å¯ä»¥å é¤è¯¥åå¤ï¼è®©å®éæ°å¼å§å­¦ä¹ ã')),
-answer_table])) blacklist_page = PageSchema(url='/blacklist', icon='fa fa-ban',
-label='ç¦ç¨åè¡¨', schema=Page(title='ç¦ç¨åè¡¨', body=[Alert
-(level=LevelEnum.info, className='white-space-pre-wrap',
-body=f'æ­¤æ°æ®åºè®°å½äº{NICKNAME}è¢«ç¦ç¨çåå®¹/å³é®è¯ã\n' 'Â·
-å¯ä»¥åæ¶ç¦ç¨ï¼ä½¿å¶è½å¤éæ°ç»§ç»­å­¦ä¹ ã\n' 'Â·
+ç¹å»"å é¤"å¯ä»¥å é¤è¯¥åå¤ï¼è®©å®éæ°å¼å§å­¦ä¹ ã' ), ),
+answer_table, ], ), ) blacklist_page = PageSchema( url="/blacklist", icon="fa
+fa-ban", label="ç¦ç¨åè¡¨", schema=Page( title="ç¦ç¨åè¡¨", body=[ Alert
+( level=LevelEnum.info, className="white-space-pre-wrap",
+body=f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}è¢«ç¦ç¨çåå®¹/å³é®è¯ã\n" "Â·
+å¯ä»¥åæ¶ç¦ç¨ï¼ä½¿å¶è½å¤éæ°ç»§ç»­å­¦ä¹ ã\n" "Â·
 ä¸è½å¨æ­¤æ·»å ç¦ç¨ï¼åªè½å¨ç¾¤ä¸­åå¤
-[ä¸å¯ä»¥]æèå¨<éç½®>ä¸­æ·»å å±è½è¯æ¥è¾¾å°ç¦ç¨ææã'),
-blacklist_table])) database_page = PageSchema(label='æ°æ®åº', icon='fa fa-
-database', children=[message_page, context_page, answer_page, blacklist_page])
-config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-
-wrench', label='éç½®', schema=Page(title='éç½®', initApi='/learning_chat/
-api/get_group_list', body=[global_config_form, group_select,
-group_config_form])) chat_page = PageSchema(label='ç¾¤èå­¦ä¹ ', icon='fa fa-
-wechat (alias)', children=[config_page, database_page]) github_logo = Tpl
-(className='w-full', tpl='
-') header = Flex(className='w-full', justify='flex-end', alignItems='flex-end',
-items=[github_logo]) admin_app = App(brandName='Learning-Chat', logo='http://
-static.cherishmoon.fun/LittlePaimon/readme/logo.png', header=header, pages=[
-{ 'children': [config_page, database_page] }], footer='
+[ä¸å¯ä»¥]æèå¨<éç½®>ä¸­æ·»å å±è½è¯æ¥è¾¾å°ç¦ç¨ææã", ),
+blacklist_table, ], ), ) database_page = PageSchema( label="æ°æ®åº",
+icon="fa fa-database", children=[message_page, context_page, answer_page,
+blacklist_page], ) config_page = PageSchema( url="/configs",
+isDefaultPage=True, icon="fa fa-wrench", label="éç½®", schema=Page
+( title="éç½®", initApi="/learning_chat/api/get_group_list", interval=60000,
+body=[global_config_form, group_select, group_config_form], ), ) chat_page =
+PageSchema( label="ç¾¤èå­¦ä¹ ", icon="fa fa-wechat (alias)", children=
+[config_page, database_page] ) github_logo = Tpl( className="w-full", tpl='
+', ) header = Flex( className="w-full", justify="flex-end", alignItems="flex-
+end", items=[github_logo] ) admin_app = App( brandName="Learning-Chat",
+logo="http://static.cherishmoon.fun/LittlePaimon/readme/logo.png",
+header=header, pages=[{"children": [config_page, database_page]}], footer='
 Copyright Â© 2021 - 2022 Learning-Chat Xamis_v2.2.0
-')
+', )
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/pyproject.toml` & `nonebot_plugin_learning_chat-0.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "nonebot_plugin_learning_chat"
-version = "0.2.2"
+version = "0.2.3"
 description = "Nonebot2 plugin to learn what your group members say."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 keywords = ["nonebot2"]
 homepage = "https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat"
 readme = "README.md"
 license = "AGPL"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.0.0-rc.2"
+nonebot2 = {version = "^2.0.0", extras = ["fastapi"]}
 nonebot-adapter-onebot = "^2.1"
 nonebot-plugin-apscheduler = "^0.2.0"
 tortoise-orm = "^0.19.2"
 jieba = "^0.42.1"
 "ruamel.yaml" = "^0.17.21"
 amis-python = "^1.0.6"
 python-jose = "^3.3.0"
```

### Comparing `nonebot_plugin_learning_chat-0.2.2/PKG-INFO` & `nonebot_plugin_learning_chat-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-learning-chat
-Version: 0.2.2
+Version: 0.2.3
 Summary: Nonebot2 plugin to learn what your group members say.
 Home-page: https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat
 License: AGPL
 Keywords: nonebot2
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1,<3.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: tortoise-orm (>=0.19.2,<0.20.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
@@ -56,52 +56,19 @@
 
 本插件还配备了一个`Web UI`后台管理供Bot主人修改配置，支持**分群**配置。
 
 本插件仅适用于`OneBot V11`适配器和**群聊**。
 
 ## 💿 安装
 
-<details>
-<summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
-    nb plugin install nonebot-plugin-learning-chat
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-learning-chat
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-learning-chat
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-learning-chat
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-learning-chat
-</details>
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
-
-    nonebot.load_plugin('nonebot_plugin_learning_chat')
-
-</details>
+```shell
+nb plugin install nonebot-plugin-learning-chat
+```
 
 ## ☀️ 指令
 不同于其它的命令式插件，本插件只有2个命令用于在群聊里管理Bot。
 
 |   指令    |             示例              |                         作用                          |
 |:-------:|:---------------------------:|:---------------------------------------------------:|
 | 开启\关闭学习 | @bot 开启学习\学说话\快学\关闭学习\别学\闭嘴 |                开启或关闭该群的学习能力(需艾特机器人)                 |
```

#### html2text {}

```diff
@@ -1,41 +1,34 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-learning-chat Version: 0.2.2
+Metadata-Version: 2.1 Name: nonebot-plugin-learning-chat Version: 0.2.3
 Summary: Nonebot2 plugin to learn what your group members say. Home-page:
 https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat License: AGPL
 Keywords: nonebot2 Author: CMHopeSunshine Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.1,<3.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0) Requires-Dist: python-jose
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Requires-Dist: python-jose
 (>=3.3.0,<4.0.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist:
 tortoise-orm (>=0.19.2,<0.20.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-learning-chat _â¨ è®©Botå­¦ä¹ ç¾¤åçåè¨åè¡¨æå!
                         â¨_ [license] [pypi] [python]
 ## ð ä»ç»
 ä¸ä¸ªè½å¤è®©Botæ ¹æ®ç¾¤åçè§å¾æ§åè¨ï¼èªå¨éæ©åå²è¯­å½æèè¡¨æåè¿è¡åå¤çå­¦ä¹ æä»¶ã
 å®è£å®æ¬æä»¶åå¹¶ä¸ä¼é©¬ä¸æææï¼éè¦ç»Botä¸æ®µæ¶é´ç§¯ç´¯ç¾¤èè®°å½ã
 å­¦å°ä¸å®ç¨åº¦åï¼æä»¶å°±ä¼åæè¯å çï¼~~æç¾¤åä»¬çå¥æªåè¨åè¡¨æåééæ¢è¿æ¥~~ã
 æ¬æä»¶è¿éå¤äºä¸ä¸ª`Web
 UI`åå°ç®¡çä¾Botä¸»äººä¿®æ¹éç½®ï¼æ¯æ**åç¾¤**éç½®ã
-æ¬æä»¶ä»éç¨äº`OneBot V11`ééå¨å**ç¾¤è**ã ## ð¿ å®è£
-ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-learning-chat
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-learning-chat   pdm pdm add nonebot-plugin-
-learning-chat   poetry poetry add nonebot-plugin-learning-chat   conda conda
-install nonebot-plugin-learning-chat  æå¼ nonebot2 é¡¹ç®ç `bot.py`
-æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin('nonebot_plugin_learning_chat')  ##
-âï¸ æä»¤
+æ¬æä»¶ä»éç¨äº`OneBot V11`ééå¨å**ç¾¤è**ã ## ð¿ å®è£ å¨
+nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
+```shell nb plugin install nonebot-plugin-learning-chat ``` ## âï¸ æä»¤
 ä¸åäºå¶å®çå½ä»¤å¼æä»¶ï¼æ¬æä»¶åªæ2ä¸ªå½ä»¤ç¨äºå¨ç¾¤èéç®¡çBotã
 | æä»¤ | ç¤ºä¾ | ä½ç¨ | |:-------:|:---------------------------:|:--------
 -------------------------------------------:| | å¼å¯\å³é­å­¦ä¹  | @bot
 å¼å¯å­¦ä¹ \å­¦è¯´è¯\å¿«å­¦\å³é­å­¦ä¹ \å«å­¦\é­å´ |
 å¼å¯æå³é­è¯¥ç¾¤çå­¦ä¹ è½å(éè¾ç¹æºå¨äºº) | | ç¦ç¨åå¤ |
 @bot ä¸å¯ä»¥\è¾¾å©\ä¸è½è¯´è¿ |
 å°æå¥å·²å­¦ä¼çåå¤ç»ç¦ç¨æï¼ä»¥åä¸ä¼åè¯´è¿å¥è¯ï¼éè¦æç®¡çåæéèè¾ç¹æºå¨äººå¹¶**åå¤**æºå¨äººçåè¨
```

