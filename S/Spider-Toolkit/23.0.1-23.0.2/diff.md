# Comparing `tmp/Spider_Toolkit-23.0.1.tar.gz` & `tmp/Spider_Toolkit-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Spider_Toolkit-23.0.1.tar", last modified: Fri Jun  9 07:08:28 2023, max compression
+gzip compressed data, was "Spider_Toolkit-23.0.2.tar", last modified: Sat Jun 10 10:40:09 2023, max compression
```

## Comparing `Spider_Toolkit-23.0.1.tar` & `Spider_Toolkit-23.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 07:08:28.793575 Spider_Toolkit-23.0.1/
--rw-rw-rw-   0        0        0     1079 2023-06-09 06:25:44.000000 Spider_Toolkit-23.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2023-06-09 07:08:28.793575 Spider_Toolkit-23.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-09 05:31:00.000000 Spider_Toolkit-23.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 07:08:28.770569 Spider_Toolkit-23.0.1/Spider_Toolkit/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.1/Spider_Toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:08:28.790574 Spider_Toolkit-23.0.1/Spider_Toolkit/engine/
--rw-rw-rw-   0        0        0     2492 2023-06-09 03:36:08.000000 Spider_Toolkit-23.0.1/Spider_Toolkit/engine/Parameter_filtering_engine.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.1/Spider_Toolkit/engine/__init__.py
--rw-rw-rw-   0        0        0     3305 2023-06-09 07:08:07.000000 Spider_Toolkit-23.0.1/Spider_Toolkit/spidertools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:08:28.792589 Spider_Toolkit-23.0.1/Spider_Toolkit/tools/
--rw-rw-rw-   0        0        0     9993 2023-06-09 03:36:08.000000 Spider_Toolkit-23.0.1/Spider_Toolkit/tools/Download_byte.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.1/Spider_Toolkit/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:08:28.788575 Spider_Toolkit-23.0.1/Spider_Toolkit.egg-info/
--rw-rw-rw-   0        0        0      687 2023-06-09 07:08:28.000000 Spider_Toolkit-23.0.1/Spider_Toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-06-09 07:08:28.000000 Spider_Toolkit-23.0.1/Spider_Toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 07:08:28.000000 Spider_Toolkit-23.0.1/Spider_Toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 07:08:28.000000 Spider_Toolkit-23.0.1/Spider_Toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-09 07:08:28.000000 Spider_Toolkit-23.0.1/Spider_Toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-09 07:08:28.794575 Spider_Toolkit-23.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2097 2023-06-09 07:08:07.000000 Spider_Toolkit-23.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.487496 Spider_Toolkit-23.0.2/
+-rw-rw-rw-   0        0        0     1079 2023-06-09 06:25:44.000000 Spider_Toolkit-23.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      658 2023-06-10 10:40:09.487496 Spider_Toolkit-23.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-10 10:39:49.000000 Spider_Toolkit-23.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.453487 Spider_Toolkit-23.0.2/Spider_Toolkit/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.481493 Spider_Toolkit-23.0.2/Spider_Toolkit/engine/
+-rw-rw-rw-   0        0        0     9259 2023-06-10 10:39:49.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/engine/Parameter_filtering_engine.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/engine/__init__.py
+-rw-rw-rw-   0        0        0    12143 2023-06-10 10:19:44.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/spidertools.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.486495 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/
+-rw-rw-rw-   0        0        0    11626 2023-06-10 10:31:24.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Download_byte.py
+-rw-rw-rw-   0        0        0      314 2023-06-10 08:09:27.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Open_js.py
+-rw-rw-rw-   0        0        0     4200 2023-06-10 09:36:32.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Save.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.479494 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/
+-rw-rw-rw-   0        0        0      658 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-10 10:40:09.488497 Spider_Toolkit-23.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2114 2023-06-10 10:39:49.000000 Spider_Toolkit-23.0.2/setup.py
```

### Comparing `Spider_Toolkit-23.0.1/LICENSE.txt` & `Spider_Toolkit-23.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.1/PKG-INFO` & `Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: Spider_Toolkit
-Version: 23.0.1
+Name: Spider-Toolkit
+Version: 23.0.2
 Summary: 爬虫辅助模块
 Home-page: https://github.com/pypa/sampleproject
 Author: Uncle_Ming
 Author-email: 2462711716@qq.com
 Keywords: tools spider requests download
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 
-爬虫辅助模块0.0.1版本更新了byte下载器，如果未设置最大线程数，返回的为单线程对象
+爬虫辅助模块0.0.2版本更新了byte下载器function，保存器，js调用器
```

### Comparing `Spider_Toolkit-23.0.1/Spider_Toolkit/tools/Download_byte.py` & `Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Download_byte.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import time
 import requests
-import os
 import datetime
 from concurrent.futures import ThreadPoolExecutor, wait, ALL_COMPLETED
 from collections import deque
 
+
 class download_byte():
 
     def __init__(
             self,
             Max_Thread: int = 0,
             Max_Rerty: int = 3,
             Time_Sleep: [float, int] = 0,
@@ -20,16 +20,18 @@
             param: [dict[str, any], None] = None,
             data: [dict[str, any], None] = None,
             proxies: [dict[str, any], None] = None,
             verify: bool = True,
             path_: str = './',
             Name_Rules: str = 'default',
             titles: [list, None] = None,
+            type_: str = '',
             Save_Error_Log: bool = True,
             Show_Progress_Bar: bool = False,
+            Show_Error_Info: bool = True
     ):
         self.Max_Thread = Max_Thread
         self.Max_Rerty = Max_Rerty
         self.Time_Sleep = Time_Sleep
         self.Request_Timeout = Request_Timeout
         self.urls = urls
         self.headers = headers
@@ -39,110 +41,116 @@
         self.proxies = proxies
         self.verify = verify
         self.path_ = path_
         self.Name_Rules = Name_Rules
         self.titles = titles
         self.Save_Error_Log = Save_Error_Log
         self.Show_Progress_Bar = Show_Progress_Bar
+        self.Show_Error_Info = Show_Error_Info
         self.error_list = []
-        if self.path_[-1] != '/':
-            self.path_ += '/'
+        self.type_ = type_
         self.deque_ = deque(maxlen=len(self.urls) + 1)
         self.title_deque_ = None
         self.all_task_number = len(self.urls)
         for u in self.urls:
             self.deque_.append({'url': u, 'n': 0, 'log': ''})
-        if self.titles != 'title':
-            self.title_deque_ = deque(maxlen=len(self.urls) + 1)
-        else:
+        if self.Name_Rules == 'title':
             self.title_deque_ = deque(maxlen=len(self.titles) + 1)
             for t in self.titles:
                 self.title_deque_.append(t)
+        else:
+            print(self.titles)
+            self.title_deque_ = deque(maxlen=len(self.urls) + 1)
         self.urls = None
         self.titles = None
 
     def start(self):
 
         if self.Name_Rules.lower() == 'default':
             while bool(self.deque_):
                 url = self.deque_.popleft()
-                print(url)
-                if '?' in url['url']:
-                    title = url['url'].split('?')[0].split('/')[-1].split('.')[0]
-                    format = url['url'].split('?')[0].split('/')[-1].split('.')[1]
+                if self.type_ != '':
+                    if '?' in url['url']:
+                        title = url['url'].split('?')[0].split('/')[-1]
+                        type__ = self.type_
+                    else:
+                        title = url['url'].split('/')[-1]
+                        type__ = self.type_
                 else:
-                    title = url['url'].split('/')[-1].split('.')[0]
-                    format = url['url'].split('/')[-1].split('.')[1]
-                self.get_(url, title, format)
+                    if '?' in url['url']:
+                        title = url['url'].split('?')[0].split('/')[-1].split('.')[0]
+                        type__ = url['url'].split('?')[0].split('/')[-1].split('.')[1]
+                    else:
+                        title = url['url'].split('/')[-1].split('.')[0]
+                        type__ = url['url'].split('/')[-1].split('.')[1]
+                self.get_(url, title, type__)
                 if self.Show_Progress_Bar:
                     self.progress_bar(self.all_task_number - self.deque_.__len__(), self.all_task_number)
                 else:
                     pass
         else:
             while bool(self.deque_):
                 url = self.deque_.popleft()
-                if '?' in url['url']:
-                    title = self.titles[0]
-                    format = url['url'].split('?')[0].split('/')[-1].split('.')[1]
+                if self.type_ != '':
+                    title = self.title_deque_.popleft()
+                    type__ = self.type_
                 else:
-                    title = self.titles[0]
-                    format = url['url'].split('/')[-1].split('.')[1]
-                self.get_(url, title, format)
+                    if '?' in url['url']:
+                        title = self.title_deque_.popleft()
+                        type__ = url['url'].split('?')[0].split('/')[-1].split('.')[1]
+                    else:
+                        title = self.title_deque_.popleft()
+                        type__ = url['url'].split('/')[-1].split('.')[1]
+                self.get_(url, title, type__)
                 if self.Show_Progress_Bar:
                     self.progress_bar(self.all_task_number - self.deque_.__len__(), self.all_task_number)
                 else:
                     pass
 
-
-    def get_(self, url, name, type_):
+    def get_(self, url, name, type__):
         try:
             respones = requests.get(url=url['url'], headers=self.headers, cookies=self.cookie, proxies=self.proxies,
                                     verify=self.verify, params=self.param, data=self.data)
             if respones.status_code == 200:
-                self.save_(respones.content, name, type_)
+                self.save_(respones.content, name, type__)
             else:
                 raise Exception('响应码:{}，请求失败'.format(respones.status_code))
         except Exception as e:
             self.error_prompt(e, url, name)
         time.sleep(self.Time_Sleep)
 
     def error_prompt(self, e, url, name):
         if url['n'] < self.Max_Rerty:
-            print('当前url：{}\n出现异常：{}\n未超出指定重试次数({}/{})，将添加回对列\n'.format(url['url'], e, url['n'] + 1,
-                                                                        self.Max_Rerty))
+            if self.Show_Error_Info:
+                print('当前url：{}\n出现异常：{}\n未超出指定重试次数({}/{})，将添加回对列\n'.format(url['url'], e, url['n'] + 1,
+                                                                            self.Max_Rerty))
             self.deque_.append({'url': url['url'], 'n': url['n'] + 1, 'log': ''})
             self.title_deque_.append(name)
         else:
-            print('当前url：{}\n出现异常：{}\n超出指定重试次数({})，将写入错误列表\n'.format(url['url'], e,
-                                                                     self.Max_Rerty))
+            if self.Show_Error_Info:
+                print('当前url：{}\n出现异常：{}\n超出指定重试次数({})，将写入错误列表\n'.format(url['url'], e,
+                                                                         self.Max_Rerty))
             self.error_list.append({'url': url['url'], 'n': url['n'] + 1, 'log': e})
 
-    def save_(self, content_, name, type_):
-        if os.path.exists(self.path_):
-            pass
-        else:
-            os.makedirs(self.path_)
-        with open(self.path_ + name + '.' + type_, 'wb') as f:
+    def save_(self, content_, name, type__):
+        with open(self.path_ + name + '.' + type__, 'wb') as f:
             f.write(content_)
 
     def progress_bar(self, finish_tasks_number, all_task_number):
         percentage = round(finish_tasks_number / all_task_number * 100)
         print("\r下载进度: {}%: ".format(percentage), "▓" * (percentage // 2), end="")
         sys.stdout.flush()
 
     def save_log(self):
-        if os.path.exists(self.path_):
-            pass
-        else:
-            os.makedirs(self.path_)
         with open(self.path_ + datetime.datetime.now().strftime("%Y年%m月%d日_%H时%M分%S秒") + '_log.txt', 'w',
                   encoding='utf-8') as f:
             for i in self.error_list:
                 f.write(str(i) + '\n')
 
+
 class thread_download_byte(download_byte):
     def __init__(
             self,
             Max_Thread: int = 0,
             Max_Rerty: int = 3,
             Time_Sleep: [float, int] = 0,
             Request_Timeout: [float, int] = 10,
@@ -152,16 +160,18 @@
             param: [dict[str, any], None] = None,
             data: [dict[str, any], None] = None,
             proxies: [dict[str, any], None] = None,
             verify: bool = True,
             path_: str = './',
             Name_Rules: str = 'default',
             titles: [list, None] = None,
+            type_: str = '',
             Save_Error_Log: bool = True,
             Show_Progress_Bar: bool = False,
+            Show_Error_Info: bool = True
     ):
         super(thread_download_byte, self).__init__(
             Max_Thread=Max_Thread,
             Max_Rerty=Max_Rerty,
             Time_Sleep=Time_Sleep,
             Request_Timeout=Request_Timeout,
             urls=urls,
@@ -170,71 +180,108 @@
             param=param,
             data=data,
             proxies=proxies,
             verify=verify,
             path_=path_,
             Name_Rules=Name_Rules,
             titles=titles,
+            type_=type_,
             Save_Error_Log=Save_Error_Log,
-            Show_Progress_Bar=Show_Progress_Bar
+            Show_Progress_Bar=Show_Progress_Bar,
+            Show_Error_Info=Show_Error_Info
         )
         self.threadpool = ThreadPoolExecutor(max_workers=self.Max_Thread)
 
-    def start(self):
-        self.all_task = []
-        if self.Name_Rules.lower() == 'default':
-            while bool(self.deque_):
-                self.all_task = []
-                if self.deque_.__len__() >= self.Max_Thread:
-                    for i in range(self.Max_Thread):
-                        self.creat_default_thread()
-                    wait(self.all_task, return_when=ALL_COMPLETED, timeout=self.Request_Timeout)
-                else:
-                    for i in range(self.deque_.__len__()):
-                        self.creat_default_thread()
-                    wait(self.all_task, return_when=ALL_COMPLETED, timeout=self.Request_Timeout)
-                if self.Show_Progress_Bar:
-                    self.progress_bar(self.all_task_number - self.deque_.__len__(), self.all_task_number)
-                else:
-                    pass
 
-        else:
-            while bool(self.deque_):
-                self.all_task = []
-                if self.deque_.__len__() >= self.Max_Thread:
-                    for t in range(self.Max_Thread):
-                        self.creat_title_thread()
-                    wait(self.all_task, return_when=ALL_COMPLETED)
-                else:
-                    for t in range(self.deque_.__len__()):
-                        self.creat_title_thread()
-                    wait(self.all_task, return_when=ALL_COMPLETED)
-                if self.Show_Progress_Bar:
-                    self.progress_bar(self.all_task_number - self.deque_.__len__(), self.all_task_number)
-                else:
-                    pass
-        if self.Save_Error_Log and self.error_list != []:
-            self.save_log()
+def start(self):
+    self.all_task = []
+    if self.Name_Rules.lower() == 'default':
+        while bool(self.deque_):
+            self.all_task = []
+            if self.deque_.__len__() >= self.Max_Thread:
+                for i in range(self.Max_Thread):
+                    self.creat_default_thread()
+                wait(self.all_task, return_when=ALL_COMPLETED, timeout=self.Request_Timeout)
+            else:
+                for i in range(self.deque_.__len__()):
+                    self.creat_default_thread()
+                wait(self.all_task, return_when=ALL_COMPLETED, timeout=self.Request_Timeout)
+            if self.Show_Progress_Bar:
+                self.progress_bar(self.all_task_number - self.deque_.__len__(), self.all_task_number)
+            else:
+                pass
+
+    else:
+        while bool(self.deque_):
+            self.all_task = []
+            if self.deque_.__len__() >= self.Max_Thread:
+                for t in range(self.Max_Thread):
+                    self.creat_title_thread()
+                wait(self.all_task, return_when=ALL_COMPLETED)
+            else:
+                for t in range(self.deque_.__len__()):
+                    self.creat_title_thread()
+                wait(self.all_task, return_when=ALL_COMPLETED)
+            if self.Show_Progress_Bar:
+                self.progress_bar(self.all_task_number - self.deque_.__len__(), self.all_task_number)
+            else:
+                pass
+    if self.Save_Error_Log and self.error_list != []:
+        self.save_log()
 
-    def creat_default_thread(self):
-        url_ = self.deque_.popleft()
+
+def creat_default_thread(self):
+    url_ = self.deque_.popleft()
+    if self.type_ != '':
+        if '?' in url_['url']:
+            title = url_['url'].split('?')[0].split('/')[-1]
+            type__ = self.type_
+        else:
+            title = url_['url'].split('/')[-1]
+            type__ = self.type_
+    else:
         if '?' in url_['url']:
             title = url_['url'].split('?')[0].split('/')[-1].split('.')[0]
-            format = url_['url'].split('?')[0].split('/')[-1].split('.')[1]
+            type__ = url_['url'].split('?')[0].split('/')[-1].split('.')[1]
         else:
             title = url_['url'].split('/')[-1].split('.')[0]
-            format = url_['url'].split('/')[-1].split('.')[1]
-        args = [url_,
-                title,
-                format]
-        self.all_task.append(self.threadpool.submit(lambda p: self.get_(*p), args))
+            type__ = url_['url'].split('/')[-1].split('.')[1]
+    args = [url_,
+            title,
+            type__]
+    self.all_task.append(self.threadpool.submit(lambda p: self.get_(*p), args))
+
 
-    def creat_title_thread(self):
-        url_ = self.deque_.popleft()
+def creat_title_thread(self):
+    url_ = self.deque_.popleft()
+    if self.type_ != '':
+        type__ = self.type_
+    else:
         if '?' in url_['url']:
-            format = url_['url'].split('?')[0].split('/')[-1].split('.')[1]
+            type__ = url_['url'].split('?')[0].split('/')[-1].split('.')[1]
         else:
-            format = url_['url'].split('/')[-1].split('.')[1]
-        args = [url_,
-                str(self.title_deque_.popleft()),
-                format]
-        self.all_task.append(self.threadpool.submit(lambda p: self.get_(*p), args))
+            type__ = url_['url'].split('/')[-1].split('.')[1]
+    args = [url_,
+            str(self.title_deque_.popleft()),
+            type__]
+    self.all_task.append(self.threadpool.submit(lambda p: self.get_(*p), args))
+
+
+def donwload_byte_function(
+        url: str = None,
+        headers: [dict[str, any], None] = None,
+        cookie: [dict[str, any], None] = None,
+        param: [dict[str, any], None] = None,
+        data: [dict[str, any], None] = None,
+        proxies: [dict[str, any], None] = None,
+        verify: bool = True,
+        path_: str = './',
+        name: str = '',
+        type_: str = ''
+):
+    respones = requests.get(url=url, headers=headers, cookies=cookie, proxies=proxies,
+                            verify=verify, params=param, data=data)
+    if respones.status_code == 200:
+        with open(path_ + name + '.' + type_, 'wb') as f:
+            f.write(respones.content)
+    else:
+        raise Exception('响应码:{}，请求失败'.format(respones.status_code))
```

### Comparing `Spider_Toolkit-23.0.1/Spider_Toolkit.egg-info/PKG-INFO` & `Spider_Toolkit-23.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: Spider-Toolkit
-Version: 23.0.1
+Name: Spider_Toolkit
+Version: 23.0.2
 Summary: 爬虫辅助模块
 Home-page: https://github.com/pypa/sampleproject
 Author: Uncle_Ming
 Author-email: 2462711716@qq.com
 Keywords: tools spider requests download
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 
-爬虫辅助模块0.0.1版本更新了byte下载器，如果未设置最大线程数，返回的为单线程对象
+爬虫辅助模块0.0.2版本更新了byte下载器function，保存器，js调用器
```

### Comparing `Spider_Toolkit-23.0.1/setup.py` & `Spider_Toolkit-23.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     # 以下为必需参数
     name='Spider_Toolkit',  # 模块名
-    version='23.0.1',  # 当前版本
+    version='23.0.2',  # 当前版本
     description='爬虫辅助模块',  # 简短描述
     packages=find_packages(),  # 多文件模块写法 exclude=['contrib', 'docs', 'tests']
     # 以下均为可选参数
-    long_description="爬虫辅助模块0.0.1版本更新了byte下载器，如果未设置最大线程数，返回的为单线程对象",  # 长描述
+    long_description="爬虫辅助模块0.0.2版本更新了byte下载器function，保存器，js调用器",  # 长描述
     url='https://github.com/pypa/sampleproject',  # 主页链接
     author='Uncle_Ming',  # 作者名
     author_email='2462711716@qq.com',  # 作者邮箱
     classifiers=[
         'Development Status :: 1 - Planning',  # 当前开发进度等级（测试版，正式版等）
         'License :: OSI Approved :: MIT License',  # 模块的license
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='tools spider requests download',  # 模块的关键词，使用空格分割
-    install_requires=['requests'],  # 依赖模块
+    install_requires=['requests','pandas','execjs','pymysql','redis','pymongo'],  # 依赖模块
     # extras_require={  # 分组依赖模块，可使用pip install sampleproject[dev] 安装分组内的依赖
     #     'dev': ['check-manifest'],
     #     'test': ['coverage'],
     # },
     # package_data={  # 模块所需的额外文件
     #     'sample': ['package_data.dat'],
     # },
```

