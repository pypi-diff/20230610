# Comparing `tmp/pwl-chat-python-1.4.5.tar.gz` & `tmp/pwl-chat-python-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.5.tar", last modified: Thu Jun  8 10:00:28 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.6.tar", last modified: Sat Jun 10 14:17:09 2023, max compression
```

## Comparing `pwl-chat-python-1.4.5.tar` & `pwl-chat-python-1.4.6.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.065382 pwl-chat-python-1.4.5/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2210 2023-06-08 10:00:28.064956 pwl-chat-python-1.4.5/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1611 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.055693 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2210 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-06-08 10:00:28.065520 pwl-chat-python-1.4.5/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.056207 pwl-chat-python-1.4.5/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.058008 pwl-chat-python-1.4.5/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1712 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.5/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.063104 pwl-chat-python-1.4.5/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2884 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1699 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     2159 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     2424 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1605 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     5311 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1217 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1324 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1463 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.064217 pwl-chat-python-1.4.5/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)     1044 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.420221 pwl-chat-python-1.4.6/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.6/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2246 2023-06-10 14:17:09.419762 pwl-chat-python-1.4.6/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1647 2023-06-10 14:02:37.000000 pwl-chat-python-1.4.6/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.401338 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2246 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      570 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       41 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-06-10 14:17:09.420365 pwl-chat-python-1.4.6/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3539 2023-06-10 14:02:37.000000 pwl-chat-python-1.4.6/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.401934 pwl-chat-python-1.4.6/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.407830 pwl-chat-python-1.4.6/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.6/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1833 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     2036 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1351 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/api/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.6/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.417298 pwl-chat-python-1.4.6/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2951 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1699 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.6/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     2164 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     5084 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1666 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     5469 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1217 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.6/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1326 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1395 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.418944 pwl-chat-python-1.4.6/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1675 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-06-10 14:02:37.000000 pwl-chat-python-1.4.6/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.5/LICENSE` & `pwl-chat-python-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.5/PKG-INFO` & `pwl-chat-python-1.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.5
+Version: 1.4.6
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -60,24 +60,25 @@
     - 自定义抢红包延时
     - 心跳红包防止踩坑
     - 心跳红包风险预测
     - ~~猜拳红包百分百胜率~~
 - 命令模式
   - 命令/聊天模式切换
     - (聊天模式也可以执行命令)
+  - 进入答题模式(前缀自动加上 鸽)
   - ⬆️ 社区快捷命令
     - 领取昨日活跃度奖励
     - 查看个人积分
     - 查看签到状态
     - 查看当前活跃度
     - 查看在线用户列表
     - 查询用户详细信息
     - 🈲️ 小黑屋功能
       - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
       - 将某人从小黑屋中放出
-    - 发红包(待开发)
+    - 发红包
 
 ## 效果
 
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.5/README.md` & `pwl-chat-python-1.4.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -42,24 +42,25 @@
     - 自定义抢红包延时
     - 心跳红包防止踩坑
     - 心跳红包风险预测
     - ~~猜拳红包百分百胜率~~
 - 命令模式
   - 命令/聊天模式切换
     - (聊天模式也可以执行命令)
+  - 进入答题模式(前缀自动加上 鸽)
   - ⬆️ 社区快捷命令
     - 领取昨日活跃度奖励
     - 查看个人积分
     - 查看签到状态
     - 查看当前活跃度
     - 查看在线用户列表
     - 查询用户详细信息
     - 🈲️ 小黑屋功能
       - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
       - 将某人从小黑屋中放出
-    - 发红包(待开发)
+    - 发红包
 
 ## 效果
 
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.5/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.6/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.5
+Version: 1.4.6
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -60,24 +60,25 @@
     - 自定义抢红包延时
     - 心跳红包防止踩坑
     - 心跳红包风险预测
     - ~~猜拳红包百分百胜率~~
 - 命令模式
   - 命令/聊天模式切换
     - (聊天模式也可以执行命令)
+  - 进入答题模式(前缀自动加上 鸽)
   - ⬆️ 社区快捷命令
     - 领取昨日活跃度奖励
     - 查看个人积分
     - 查看签到状态
     - 查看当前活跃度
     - 查看在线用户列表
     - 查询用户详细信息
     - 🈲️ 小黑屋功能
       - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
       - 将某人从小黑屋中放出
-    - 发红包(待开发)
+    - 发红包
 
 ## 效果
 
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.5/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.6/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pwl_chat_python.egg-info/entry_points.txt
 pwl_chat_python.egg-info/requires.txt
 pwl_chat_python.egg-info/top_level.txt
 src/main.py
 src/api/__api__.py
 src/api/__init__.py
 src/api/chatroom.py
+src/api/redpacket.py
 src/api/user.py
 src/core/__init__.py
 src/core/blacklist.py
 src/core/chatroom.py
 src/core/cli.py
 src/core/config.py
 src/core/redpacket.py
```

### Comparing `pwl-chat-python-1.4.5/setup.py` & `pwl-chat-python-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 EMAIL = 'gakkiyomi@gmail.com'
 AUTHOR = 'gakkiyomi'
 REQUIRES_PYTHON = '>=3.10.8'
 VERSION = __version__
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'requests', 'websocket-client', 'rel', 'click', 'schedule'
+    'requests', 'websocket-client', 'click', 'schedule'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

### Comparing `pwl-chat-python-1.4.5/src/api/__init__.py` & `pwl-chat-python-1.4.6/src/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 import requests
 import hashlib
 import json
 
 
 class FishPi(Base):
     def __init__(self):
+        self.ws_calls = []
         self.ws = None
         self.current_user = ''
         self.user = User()
         self.chatroom = ChatRoom()
         Base.__init__(self)
 
+    def add_listener(self, listener):
+        self.ws_calls.append(listener)
+
     def set_current_user(self, username):
         self.current_user = username
 
     def set_token(self, key):
         Base.set_token(self, key)
         self.user.set_token(key)
         self.chatroom.set_token(key)
@@ -46,7 +50,10 @@
         else:
             print(f"登陆失败: {rsp['msg']}")
             sys.exit(1)
 
     def get_yesterday_reward(self) -> dict:
         resp = requests.get(f'{HOST}/activity/yesterday-liveness-reward-api?apiKey={self.api_key}', headers={'User-Agent': UA})
         return json.loads(resp.text)
+
+
+API = FishPi()
```

### Comparing `pwl-chat-python-1.4.5/src/api/chatroom.py` & `pwl-chat-python-1.4.6/src/api/chatroom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import json
 import random
+from .redpacket import *
 from src.utils.utils import UA, HOST
 from src.utils.version import __version__
 from .__api__ import Base
 
 
 class ChatRoom(Base):
 
@@ -15,20 +16,26 @@
                             headers={'User-Agent': UA})
         return json.loads(resp.text)
 
     def send(self, message: str) -> dict | None:
         if self.api_key == '':
             return None
         params = {'apiKey': self.api_key, 'content': message,
-                  'client': f'Python/{__version__}'}
+                  'client': f'Python/客户端v{__version__}'}
         ret = requests.post(HOST + "/chat-room/send",
                             json=params, headers={'User-Agent': UA})
         ret_json = json.loads(ret.text)
         if ('code' in ret_json and ret_json['code'] == -1):
             print(ret_json['msg'])
+            
+
+    def send_redpacket(self, redpacket :RedPacket=RedPacket('最后的发', 128, 5,RedPacketType.RANDOM)):
+        content = f'[redpacket]{json.dumps(redpacket.__json__())}[/redpacket]'
+        print(content)
+        self.send(content)        
 
     def open_redpacket(self, red_packet_id) -> dict:
         params = {
             'apiKey': self.api_key,
             'oId': red_packet_id
         }
         resp = requests.post(HOST + "/chat-room/red-packet/open",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pwl-chat-python-1.4.5/src/api/user.py` & `pwl-chat-python-1.4.6/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.5/src/core/__init__.py` & `pwl-chat-python-1.4.6/src/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 
 from src.api import FishPi
-from .chatroom import init_soliloquize
-from .cli import init_sys_in
+from .chatroom import init_soliloquize, listener
 from .config import GLOBAL_CONFIG, RedPacketConfig, AuthConfig, ChatConfig
 import configparser
 import os
 
 
 def __init__(api: FishPi, file_path: str = None):
     if file_path is None:   
@@ -22,18 +21,21 @@
             GLOBAL_CONFIG.auth_config = __init_login_auth_config(config)
             GLOBAL_CONFIG.redpacket_config = __int_redpacket_config(config)
             GLOBAL_CONFIG.chat_config = __init_chat_config(config)
             GLOBAL_CONFIG.cfg_path = file_path
     except:
         print(f'{file_path}配置文件不合法')
         __init_default_config()
+    __init_message_listener(api)
     init_soliloquize(api)
-    init_sys_in(api)
 
 
+def __init_message_listener(api :FishPi):
+    api.add_listener(listener)
+
 def __init_default_config():
     print("加载默认配置文件")
     GLOBAL_CONFIG.auth_config = AuthConfig()
     GLOBAL_CONFIG.redpacket_config = RedPacketConfig()
     GLOBAL_CONFIG.chat_config = ChatConfig()
     GLOBAL_CONFIG.cfg_path = None
```

### Comparing `pwl-chat-python-1.4.5/src/core/blacklist.py` & `pwl-chat-python-1.4.6/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.5/src/core/chatroom.py` & `pwl-chat-python-1.4.6/src/core/chatroom.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 def soliloquize(api: FishPi) -> None:
     length = len(GLOBAL_CONFIG.chat_config.sentences)
     index = random.randint(0, length - 1)
     api.chatroom.send(GLOBAL_CONFIG.chat_config.sentences[index])
 
-
-def listener(api: FishPi, message) -> None:
+def listener(api: FishPi, message :dict) -> None:
     if message['type'] == 'msg':
         if message['content'].find("redPacket") != -1:
             rush_redpacket(api, message)
         else:
             time = message['time']
             user = message['userName']
             user_nick_name = message['userNickname']
```

### Comparing `pwl-chat-python-1.4.5/src/core/config.py` & `pwl-chat-python-1.4.6/src/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,23 @@
         self.username = username
         self.password = password
         self.mfa_code = mfa_code
 
 
 class ChatConfig(object):
     def __init__(self, blacklist=[], repeat_mode_switch=False, frequency=5, soliloquize_switch=False,
-                 soliloquize_frequency=20, sentences=[]):
+                 soliloquize_frequency=20, sentences=[], answerMode :bool=False):
         self.repeat_mode_switch = repeat_mode_switch
         self.frequency = frequency
         self.soliloquize_switch = soliloquize_switch
         self.soliloquize_frequency = soliloquize_frequency
         self.sentences = ['你们好！', '牵着我的手，闭着眼睛走你也不会迷路。',
                           '吃饭了没有?', '💗 爱你哟！'] + sentences
         self.blacklist = blacklist
+        self.answerMode = answerMode
 
 
 class Config(object):
     def __init__(self, auth: AuthConfig = None, redpacket: RedPacketConfig = None, chat: ChatConfig = None, cfg_path :str = None):
         self.auth_config = auth
         self.redpacket_config = redpacket
         self.chat_config = chat
```

### Comparing `pwl-chat-python-1.4.5/src/core/redpacket.py` & `pwl-chat-python-1.4.6/src/core/redpacket.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,18 @@
         api.chatroom.send(utils.RPS_LOSED)
     elif code == CODE.ZERO:
         api.chatroom.send(utils.RPS_ZERO)    
 
 
 def rush_redpacket(api: FishPi, redpacket):
     sender = redpacket['userName']
+    if sender == api.current_user:
+        print('\t\t\t\t\t\t[' + redpacket['time'] + ']')
+        print('\t\t\t\t\t\t发送了一个红包')
+        return
     if (GLOBAL_CONFIG.redpacket_config.red_packet_switch == False):
         print('红包助手: '+sender+'发送了一个红包 你错过了这个红包，请开启抢红包模式！')
         return
     sender = redpacket['userName']
     content = json.loads(redpacket['content'])
     if content['type'] == 'heartbeat':
         if GLOBAL_CONFIG.redpacket_config.heartbeat:
```

### Comparing `pwl-chat-python-1.4.5/src/core/user.py` & `pwl-chat-python-1.4.6/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.5/src/core/websocket.py` & `pwl-chat-python-1.4.6/src/core/websocket.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import json
 import ssl
-import rel
+import _thread
 import schedule
 import websocket
 
-from src.api import FishPi
-from .chatroom import listener
+from src.api import API,FishPi
 from .config import GLOBAL_CONFIG
 
-__api = FishPi()
+
 def on_message(ws, message):
-    json_body = json.loads(message)
-    listener(__api, json_body)
+    data = json.loads(message)
+    for call in API.ws_calls:
+        call(API, data)
 
 
 def on_error(ws, error):
     print(error)
 
 
 def on_close(ws, close_status_code, close_msg):
     print("已经离开聊天室,可以执行命令 #chatroom 重新进入聊天室")
 
 
 
 def on_open(ws):
-    print(f'欢迎{__api.current_user}进入聊天室!')
+    print(f'欢迎{API.current_user}进入聊天室!')
     if len(GLOBAL_CONFIG.chat_config.blacklist) > 0:
         print('小黑屋成员: ' + str(GLOBAL_CONFIG.chat_config.blacklist))
     if GLOBAL_CONFIG.chat_config.soliloquize_switch:
             schedule.run_pending()
 
 def chatroom_out(api: FishPi):
     api.ws.close()
     api.ws = None
+      
 
-def chatroom_in(api: FishPi) -> websocket.WebSocketApp:
-    global __api
-    __api = api
+def __chatroom_in(api :FishPi):
     websocket.enableTrace(False)
     ws = websocket.WebSocketApp("wss://fishpi.cn/chat-room-channel?apiKey=" + api.api_key,
                                 on_open=on_open,
                                 on_message=on_message,
                                 on_error=on_error,
                                 on_close=on_close)
-    ws.run_forever(dispatcher=rel, sslopt={"cert_reqs": ssl.CERT_NONE})
-    return ws
+    api.ws = ws
+    ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
+    
+def init_chatroom(api: FishPi):
+    _thread.start_new_thread(__chatroom_in, (api,))
```

### Comparing `pwl-chat-python-1.4.5/src/main.py` & `pwl-chat-python-1.4.6/src/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 # -*- coding: utf-8 -*-
 import click
 import rel
 from src.core import __init__
 from src.core.config import GLOBAL_CONFIG, AuthConfig
 from src.core.user import login
-from src.core.websocket import chatroom_in
+from src.core.cli import console_input
+from src.core.websocket import init_chatroom
 from src.utils.version import __version__
-from src.api import FishPi
+from src.api import API
 
 
 class CliConfig(object):
     def __init__(self, username: str = '', password: str = '', code: str = '', file_path: str = None):
         self.username = username
         self.password = password
         self.code = code
         self.file_path = file_path
 
 
 def run(config: CliConfig):
-    api = FishPi()
-    __init__(api, config.file_path)
+    __init__(API, config.file_path)
     if config.username is not None and config.password is not None:
         GLOBAL_CONFIG.auth_config = AuthConfig(
             config.username, config.password, config.code)
-    login(api)
-    rel.safe_read()
-    api.ws = chatroom_in(api)
-    pending()
-
-    
-def pending():
-    rel.signal(2, rel.abort)
-    rel.dispatch()
+    login(API)
+    init_chatroom(API)
+    console_input(API)
 
 @click.command()
 @click.version_option(__version__)
 @click.option("--username", "-u", type=click.STRING, help="摸鱼派用户名")
 @click.option("--password", "-p", type=click.STRING, help="密码")
 @click.option("--code", "-c", type=click.STRING, help="两步验证码")
 @click.option("--file_path", "-f", type=click.STRING, help="配置文件路径")
```

