# Comparing `tmp/yaylib-0.1.0.tar.gz` & `tmp/yaylib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-0.1.0.tar", last modified: Sat Jun  3 15:00:12 2023, max compression
+gzip compressed data, was "yaylib-0.1.2.tar", last modified: Sat Jun 10 05:31:49 2023, max compression
```

## Comparing `yaylib-0.1.0.tar` & `yaylib-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 15:00:12.260525 yaylib-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-06-03 14:25:16.000000 yaylib-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     9636 2023-06-03 15:00:12.259520 yaylib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8662 2023-06-03 14:55:58.000000 yaylib-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 15:00:12.260525 yaylib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-06-03 14:56:39.000000 yaylib-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 15:00:12.219146 yaylib-0.1.0/yaylib/
--rw-rw-rw-   0        0        0      263 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 15:00:12.258372 yaylib-0.1.0/yaylib/api/
--rw-rw-rw-   0        0        0      356 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0     4850 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/api.py
--rw-rw-rw-   0        0        0     6491 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/call.py
--rw-rw-rw-   0        0        0     1325 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    11253 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    17175 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/group.py
--rw-rw-rw-   0        0        0     4392 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/login.py
--rw-rw-rw-   0        0        0     3698 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    26681 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/post.py
--rw-rw-rw-   0        0        0     2618 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/review.py
--rw-rw-rw-   0        0        0     3480 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    21116 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/api/user.py
--rw-rw-rw-   0        0        0    57872 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/client.py
--rw-rw-rw-   0        0        0     5792 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/config.py
--rw-rw-rw-   0        0        0      373 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/errors.py
--rw-rw-rw-   0        0        0    51011 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/models.py
--rw-rw-rw-   0        0        0    30967 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/responses.py
--rw-rw-rw-   0        0        0      832 2023-06-03 14:25:16.000000 yaylib-0.1.0/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 15:00:12.243253 yaylib-0.1.0/yaylib.egg-info/
--rw-rw-rw-   0        0        0     9636 2023-06-03 15:00:12.000000 yaylib-0.1.0/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-06-03 15:00:12.000000 yaylib-0.1.0/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 15:00:12.000000 yaylib-0.1.0/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-03 15:00:12.000000 yaylib-0.1.0/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 15:00:12.000000 yaylib-0.1.0/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.419185 yaylib-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-10 05:03:11.000000 yaylib-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     9580 2023-06-10 05:31:49.418185 yaylib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8723 2023-06-10 05:03:26.000000 yaylib-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 05:31:49.419185 yaylib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1484 2023-06-10 05:03:11.000000 yaylib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.372517 yaylib-0.1.2/tests/
+-rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_call.py
+-rw-rw-rw-   0        0        0      829 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_chat.py
+-rw-rw-rw-   0        0        0      231 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_group.py
+-rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_misc.py
+-rw-rw-rw-   0        0        0     2552 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_post.py
+-rw-rw-rw-   0        0        0      922 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_review.py
+-rw-rw-rw-   0        0        0      233 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_thread.py
+-rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.381663 yaylib-0.1.2/yaylib/
+-rw-rw-rw-   0        0        0      263 2023-06-05 07:27:36.000000 yaylib-0.1.2/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.415186 yaylib-0.1.2/yaylib/api/
+-rw-rw-rw-   0        0        0      356 2023-06-03 14:25:16.000000 yaylib-0.1.2/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0     5007 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     7358 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     1393 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    12641 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    19292 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     4720 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     5561 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    29245 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     3036 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     3968 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    22815 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    76106 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/client.py
+-rw-rw-rw-   0        0        0     5732 2023-06-10 05:31:25.000000 yaylib-0.1.2/yaylib/config.py
+-rw-rw-rw-   0        0        0      373 2023-06-03 14:25:16.000000 yaylib-0.1.2/yaylib/errors.py
+-rw-rw-rw-   0        0        0    50977 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/models.py
+-rw-rw-rw-   0        0        0    30969 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/responses.py
+-rw-rw-rw-   0        0        0     1079 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.395664 yaylib-0.1.2/yaylib.egg-info/
+-rw-rw-rw-   0        0        0     9580 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-0.1.0/LICENSE` & `yaylib-0.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 qvco, Konn
+Copyright (c) 2023 Qvco, Konn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `yaylib-0.1.0/PKG-INFO` & `yaylib-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 0.1.0
-Summary: This Python package provides an easy-to-use interface for accessing data from Yay!, a social networking platform. With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts. Compatible with Yay! version 3.16 and later. Please note that some API calls may be subject to rate limits or require authentication.
+Version: 0.1.2
+Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
-Author: qvco, Konn
+Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
-Maintainer: qvco, Konn
+Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
-Keywords: yay,yaylib,api,bot,library,wrapper
+Keywords: yay,yaylib,api,bot,library,wrapper,ボット,ライブラリ
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
@@ -36,15 +36,15 @@
     </a> -->
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
         このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
-        <a href="https://github.com/qvco/yaylib">
+        <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
             <strong>詳しい機能の詳細や使い方はこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
@@ -128,17 +128,17 @@
 メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 
-api.login_with_email(email="hello@example.com", password="abc123")
+api.login(email="メールアドレス", password="パスワード")
 
-api.create_post(text="Hi there.", color=2)
+api.create_post(text="初めての投稿！", color=2)
 ```
 
 より詳細な使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
@@ -154,25 +154,25 @@
             <th>Funktion (架空)</th>
             <th>香ばしいボット (架空)</th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/MindReaderAI.jpg" width="200px"></a>
+                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/Funktion.jpg" width="200px"></a>
+                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/香ばしいボット.jpg" width="200px"></a>
+                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
             </td>
         </tr>
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: yaylib Version: 0.1.0 Summary: This Python package
-provides an easy-to-use interface for accessing data from Yay!, a social
-networking platform. With this API Client, you can retrieve user profiles,
-posts, comments, and other content from Yay!, as well as perform common tasks
-like liking and commenting on posts. Compatible with Yay! version 3.16 and
-later. Please note that some API calls may be subject to rate limits or require
-authentication. Home-page: https://github.com/qvco/yaylib Download-URL: https:/
-/github.com/qvco/yaylib Author: qvco, Konn Author-email:
-nikola.desuga@gmail.com Maintainer: qvco, Konn Maintainer-email:
+Metadata-Version: 2.1 Name: yaylib Version: 0.1.2 Summary: This Python package
+provides an easy-to-use interface for accessing data from Yay! (https://
+yay.space/). With this API Client, you can retrieve user profiles, posts,
+comments, and other content from Yay!, as well as perform common tasks like
+liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
+Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
+nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
-yay,yaylib,api,bot,library,wrapper Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE
+yay,yaylib,api,bot,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
+Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
@@ -46,26 +44,27 @@
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```  ## ä½¿ç¨ä¾
 ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
-```python import yaylib api = yaylib.Client() api.login_with_email
-(email="hello@example.com", password="abc123") api.create_post(text="Hi
-there.", color=2) ``` ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã]
-(https://github.com/qvco/yaylib/blob/master/examples)
-ãåç§ãã¦ãã ããã
+```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+(text="åãã¦ã®æç¨¿ï¼", color=2) ```
+ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
+yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## yaylib ã§èªçããã­ããããã¡ yaylib
 ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader AI                                      Funktion (æ¶ç©º)                é¦ã°ããããã (æ¶ç©º)
-[https://github.com/qvco/yaylib/blob/main/assets/  [https://github.com/qvco/yaylib/blob/      [https://github.com/qvco/yaylib/blob/main/assets/bot-icons/
-           bot-icons/MindReaderAI.jpg]              main/assets/bot-icons/Funktion.jpg]                       é¦ã°ããããã.jpg]
-            éçºè: æ¯ã®å¯�         éçºè: ãºã                éçºè: ããã¶ãå¤©ç¶æ°´ã
+ [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
+      472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
+            éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
+                                                            éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
 ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
 ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ããï¼    ##
 åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
```

### Comparing `yaylib-0.1.0/README.md` & `yaylib-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     </a> -->
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
         このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
-        <a href="https://github.com/qvco/yaylib">
+        <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
             <strong>詳しい機能の詳細や使い方はこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
@@ -110,17 +110,17 @@
 メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 
-api.login_with_email(email="hello@example.com", password="abc123")
+api.login(email="メールアドレス", password="パスワード")
 
-api.create_post(text="Hi there.", color=2)
+api.create_post(text="初めての投稿！", color=2)
 ```
 
 より詳細な使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
@@ -136,25 +136,25 @@
             <th>Funktion (架空)</th>
             <th>香ばしいボット (架空)</th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/MindReaderAI.jpg" width="200px"></a>
+                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/Funktion.jpg" width="200px"></a>
+                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/香ばしいボット.jpg" width="200px"></a>
+                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
             </td>
         </tr>
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -32,26 +32,27 @@
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```  ## ä½¿ç¨ä¾
 ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
-```python import yaylib api = yaylib.Client() api.login_with_email
-(email="hello@example.com", password="abc123") api.create_post(text="Hi
-there.", color=2) ``` ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã]
-(https://github.com/qvco/yaylib/blob/master/examples)
-ãåç§ãã¦ãã ããã
+```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+(text="åãã¦ã®æç¨¿ï¼", color=2) ```
+ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
+yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## yaylib ã§èªçããã­ããããã¡ yaylib
 ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader AI                                      Funktion (æ¶ç©º)                é¦ã°ããããã (æ¶ç©º)
-[https://github.com/qvco/yaylib/blob/main/assets/  [https://github.com/qvco/yaylib/blob/      [https://github.com/qvco/yaylib/blob/main/assets/bot-icons/
-           bot-icons/MindReaderAI.jpg]              main/assets/bot-icons/Funktion.jpg]                       é¦ã°ããããã.jpg]
-            éçºè: æ¯ã®å¯�         éçºè: ãºã                éçºè: ããã¶ãå¤©ç¶æ°´ã
+ [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
+      472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
+            éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
+                                                            éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
 ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
 ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ããï¼    ##
 åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
```

### Comparing `yaylib-0.1.0/setup.py` & `yaylib-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from setuptools import setup, find_packages
 from yaylib import __version__
 
 name = "yaylib"
-author = "qvco, Konn"
+author = "Qvco, Konn"
 author_email = "nikola.desuga@gmail.com"
-description = "This Python package provides an easy-to-use interface for accessing data from Yay!, a social networking platform. With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts. Compatible with Yay! version 3.16 and later. Please note that some API calls may be subject to rate limits or require authentication."
+description = "This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts."
 long_description_content_type = "text/markdown"
 license = "MIT"
 url = "https://github.com/qvco/yaylib"
 
 keywords = [
     "yay",
     "yaylib",
     "api",
     "bot",
     "library",
-    "wrapper"
+    "wrapper",
+    "ボット",
+    "ライブラリ"
 ]
 
 install_requires = [
     "httpx>=0.17.1"
 ]
 
 classifiers = [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yaylib-0.1.0/yaylib/api/api.py` & `yaylib-0.1.2/yaylib/api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import os
 import logging
+
+from json import JSONDecodeError
 from typing import Optional, Dict, Any
 
 import httpx
 
 from ..config import *
 from ..errors import *
+from ..responses import LoginUserResponse
 from ..utils import *
 
 
 current_path = os.path.abspath(os.getcwd())
 
 
 class API:
 
     def __init__(
             self,
             access_token: str = None,
+            refresh_token: str = None,
             proxy: str = None,
             timeout=60,
             base_path=current_path,
             loglevel_stream=logging.INFO,
             host=Configs.YAY_PRODUCTION_HOST,
     ):
         self.yaylib_version = Configs.YAYLIB_VERSION
-        self.yay_version_message = Configs.YAY_VERSION_MESSAGE
         self.api_version = Configs.YAY_API_VERSION
-        self.api_version_key = Configs.YAY_API_VERSION_KEY
         self.api_key = Configs.YAY_API_KEY
-        self.access_token = access_token
-        self.login_data = None
+
+        self.login_data = LoginUserResponse({
+            "access_token": access_token,
+            "refresh_token": refresh_token,
+        })
 
         self.proxy = {}
         if proxy is not None:
             self.proxy["https"] = proxy
 
         self.timeout = timeout
         self.base_path = base_path
@@ -90,15 +95,19 @@
         self.logger.debug(
             "Received API response:\n\n"
             f"Status Code: {response.status_code}\n\n"
             f"Headers: {response.headers}\n\n"
             f"Response: {response.text}\n"
         )
         self._handle_response(response)
-        return response.json()
+
+        try:
+            return response.json()
+        except JSONDecodeError:
+            return response.text
 
     def _make_request(
             self, method: str, endpoint: str, params: dict = None,
             payload: dict = None, data_type=None, user_auth=True, headers=None
     ):
         response = self.request(
             method, endpoint, params, payload, user_auth, headers
```

### Comparing `yaylib-0.1.0/yaylib/api/call.py` & `yaylib-0.1.2/yaylib/api/call.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 from ..utils import *
 
 
 def bump_call(self, call_id: int, participant_limit: int = None):
     params = {}
     if participant_limit:
         params["participant_limit"] = participant_limit
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bump",
         params=params
     )
+    self.logger.info("Call bumped.")
+    return response
 
 
 def get_user_active_call(self, user_id: int) -> Post:
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V1}/active_call",
         params={"user_id": user_id}, data_type=PostResponse
     ).post
@@ -35,23 +37,19 @@
 def get_call(self, call_id: int) -> ConferenceCall:
     return self._make_request(
         "GET", endpoint=f"{Endpoints.CALLS_V1}/conferences/{call_id}",
         data_type=ConferenceCallResponse
     ).conference_call
 
 
-def get_call_invitable_users(self, call_id: int, **params) -> UsersByTimestampResponse:
+def get_call_invitable_users(self, call_id: int, from_timestamp: int = None) -> UsersByTimestampResponse:
     # @Nullable @Query("user[nickname]")
-    """
-
-    Parameters:
-    ---------------
-        - from_timestamp: int - (optional)
-
-    """
+    params = {}
+    if from_timestamp:
+        params["from_timestamp"] = from_timestamp
     return self._make_request(
         "GET", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/invitable",
         params=params, data_type=UsersByTimestampResponse
     )
 
 
 def get_call_status(self, opponent_id: int) -> CallStatusResponse:
@@ -60,47 +58,47 @@
         data_type=CallStatusResponse
     )
 
 
 def get_games(self, **params) -> GamesResponse:
     """
 
-    Parameters:
-    ---------------
+    Parameters
+    ----------
         - number: int - (optional)
         - ids: List[int] - (optional)
         - from_id: int - (optional)
 
     """
     return self._make_request(
         "GET", endpoint=f"{Endpoints.GAMES_V1}/apps",
         params=params, data_type=GamesResponse
     )
 
 
 def get_genres(self, **params) -> GenresResponse:
     """
 
-    Parameters:
-    ---------------
+    Parameters
+    ----------
         - number: int - (optional)
         - from: int - (optional)
 
     """
     return self._make_request(
         "GET", endpoint=f"{Endpoints.GENRES_V1}",
         params=params, data_type=GenresResponse
     )
 
 
 def get_group_calls(self, **params) -> PostsResponse:
     """
 
-    Parameters:
-    ---------------
+    Parameters
+    ----------
         - number: int - (optional)
         - group_category_id: int - (optional)
         - from_timestamp: int - (optional)
         - scope: str - (optional)
 
     """
     return self._make_request(
@@ -108,141 +106,163 @@
         params=params, data_type=PostsResponse
     )
 
 
 def invite_to_call_bulk(self, call_id: int, group_id: int = None):
     """
 
-    Parameters:
-    ---------------
+    Parameters
+    ----------
         - call_id: int - (required)
         - group_id: int - (optional)
 
     """
     params = {}
     if group_id:
         params["group_id"] = group_id
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bulk_invite",
         params=params
     )
+    self.logger.info("Invited to call bulk.")
+    return response
 
 
 def invite_users_to_call(self, call_id: int, user_ids: List[int]):
     """
 
-    Parameters:
-    ---------------
+    Parameters
+    ----------
         - call_id: int - (required)
         - user_ids: List[int] - (required)
 
     """
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/invite",
         payload={
             "call_id": call_id,
             "user_ids[]": user_ids
         }
     )
+    self.logger.info("Invitation sent.")
+    return response
 
 
 def invite_users_to_chat_call(
         self,
         chat_room_id: int,
         room_id: int,
         room_url: str
 ):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V2}/invite",
         payload={
             "chat_room_id": chat_room_id,
             "room_id": room_id,
             "room_url": room_url
         }
     )
+    self.logger.info("Invitation of chat call sent.")
+    return response
 
 
 def kick_and_ban_from_call(self, call_id: int, user_id: int):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/kick",
         payload={"user_id": user_id}
     )
+    self.logger.info("User has been banned from the call.")
+    return response
 
 
 def notify_anonymous_user_leave_agora_channel(self, conference_id: int, agora_uid: str):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.ANONYMOUS_CALLS_V1}/leave_agora_channel",
         payload={"conference_id": conference_id, "agora_uid": agora_uid}
     )
+    self.logger.info("Notified anonymous user left the call.")
+    return response
 
 
 def notify_user_leave_agora_channel(self, conference_id: int, user_id: int):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/leave_agora_channel",
         payload={"conference_id": conference_id, "user_id": user_id}
     )
+    self.logger.info(f"Notified user '{user_id}' left the call.")
+    return response
 
 
 def send_call_screenshot(
         self,
         screenshot_filename: str,
         conference_id: int
 ):
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.CALLS_V1}/screenshot",
         payload={
             "conference_id": conference_id,
             "screenshot_filename": screenshot_filename
         }
     )
+    self.logger.info("Call screenshot sent.")
+    return response
 
 
 def set_call(
         self,
         call_id: int,
         joinable_by: str,
         game_title: str = None,
         category_id: str = None
 ):
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.CALLS_V1}/{call_id}",
         payload={
             "joinable_by": joinable_by,
             "game_title": game_title,
             "category_id": category_id,
         }
     )
+    self.logger.info("Call set.")
+    return response
 
 
 def set_user_role(
         self,
         call_id: int,
         user_id: int,
         role: str
 ):
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/{user_id}",
         payload={"role": role}
     )
+    self.logger.info("User has been given a role.")
+    return response
 
 
 def start_call(
         self,
         conference_id: int,
         call_sid: str
 ) -> ConferenceCall:
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/start_conference_call",
         payload={"conference_id": conference_id, "call_sid": call_sid},
         data_type=ConferenceCallResponse
     ).conference_call
+    self.logger.info("Joined the call.")
+    return response
 
 
 def stop_call(
         self,
         conference_id: int,
         call_sid: str
 ):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/leave_conference_call",
         payload={"conference_id": conference_id, "call_sid": call_sid}
     )
+    self.logger.info("Left the call.")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/api/cassandra.py` & `yaylib-0.1.2/yaylib/api/cassandra.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,40 @@
 from ..responses import *
 from ..utils import *
 
 
 def get_user_activities(self, **params) -> ActivitiesResponse:
     """
 
-    Parameters:
-    ---------------
+    Parameters
+    ----------
         - important: bool - (required)
         - from_timestamp: int - (optional)
         - number: int - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{self.host}/api/user_activities",
+        "GET", endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/user_activities",
         params=params, data_type=ActivitiesResponse
     )
 
 
-def get_user_merged_activities(self, from_timestamp: int = None) -> ActivitiesResponse:
+def get_user_merged_activities(self, **params) -> ActivitiesResponse:
+    """
+    Parameters
+    ----------
+
+        - from_timestamp: int - (optional)
+        - number: int - (optional)
+
+    """
     self._check_authorization()
-    params = {}
-    if from_timestamp:
-        params["from_timestamp"] = from_timestamp
     return self._make_request(
-        "GET", endpoint=f"{self.host}/api/v2/user_activities",
+        "GET", endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/v2/user_activities",
         params=params, data_type=ActivitiesResponse
     )
 
 
 def received_notification(self, pid: str, type: str, opened_at: int = None):
     # TODO: opened_atはnullalbeか確認する
     self._check_authorization()
```

### Comparing `yaylib-0.1.0/yaylib/api/chat.py` & `yaylib-0.1.2/yaylib/api/chat.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,99 +4,111 @@
 from ..config import *
 from ..errors import *
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
-def accept_request(self, chat_room_ids: List[int]):
+def accept_chat_request(self, chat_room_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/accept_chat_request",
         payload={"chat_room_ids[]": chat_room_ids}
     )
+    self.logger.info("Chat request accepted.")
+    return response
 
 
 def check_unread_status(self, from_time: int) -> UnreadStatusResponse:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/accept_chat_request",
+        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/unread_status",
         params={"from_time": from_time},
         data_type=UnreadStatusResponse
     )
 
 
 def create_group_chat(
         self,
         name: str,
         with_user_ids: List[int],
         icon_filename: str = None,
         background_filename: str = None
 ) -> CreateChatRoomResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V3}/new",
         payload={
             "name": name,
             "with_user_ids[]": with_user_ids,
             "icon_filename": icon_filename,
             "background_filename": background_filename,
         },
         data_type=CreateChatRoomResponse
     )
+    self.logger.info(f"Group chat '{name}' created.")
+    return response
 
 
 def create_private_chat(
         self,
         with_user_id: int,
         matching_id: int = None,
         hima_chat: bool = False
 ) -> CreateChatRoomResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/new",
         payload={
             "with_user_id": with_user_id,
             "matching_id": matching_id,
             "hima_chat": hima_chat,
         },
         data_type=CreateChatRoomResponse
     )
+    self.logger.info(f"Private chatroom with '{with_user_id}' created.")
+    return response
 
 
 def delete_background(self, room_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{room_id}/background",
     )
+    self.logger.info("Background deleted.")
+    return response
 
 
 def delete_message(self, room_id: int, message_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/messages/{message_id}/delete",
     )
+    self.logger.info("Message deleted.")
+    return response
 
 
 def edit_chat_room(
         self,
         chat_room_id: int,
         name: str,
         icon_filename: str = None,
         background_filename: str = None
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{chat_room_id}/edit",
         payload={
             "name": name,
             "icon_filename": icon_filename,
             "background_filename": background_filename,
         }
     )
+    self.logger.info("Chatroom updated.")
+    return response
 
 
 def get_chatable_users(
         self,
         # @Body @Nullable SearchUsersRequest searchUsersRequest
         from_follow_id: int = None,
         from_timestamp: int = None,
@@ -204,75 +216,89 @@
         "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/total_chat_request",
         data_type=TotalChatRequestResponse
     ).total
 
 
 def hide_chat(self, chat_room_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.HIDDEN_V1}/chats",
         payload={"chat_room_id": chat_room_id},
     )
+    self.logger.info("Chatroom hidden.")
+    return response
 
 
 def invite_to_chat(self, chat_room_id: int, user_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/invite",
         payload={"with_user_ids[]": user_ids},
     )
+    self.logger.info("Chatroom invitation sent.")
+    return response
 
 
 def kick_users_from_chat(self, chat_room_id: int, user_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/kick",
         payload={"with_user_ids[]": user_ids},
     )
+    self.logger.info(f"Users have been kicked from the chatroom.")
+    return response
 
 
 def pin_chat(self, room_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/pinned"
     )
+    self.logger.info("Pinned chatroom.")
+    return response
 
 
 def read_attachment(
         self,
         room_id: int,
         attachment_msg_ids: List[int]
 ):
     # TODO: check if this works
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/attachments_read",
         payload={
             "attachment_msg_ids[]": attachment_msg_ids
         }
     )
+    self.logger.info("Attachment read.")
+    return response
 
 
 def read_message(self, chat_room_id: int, message_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/messages/{message_id}/read",
     )
+    self.logger.info("Message read.")
+    return response
 
 
 def read_video_message(
         self,
         room_id: int,
         video_msg_ids: List[int]
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/videos_read",
         payload={"video_msg_ids": video_msg_ids},
     )
+    self.logger.info("Video message read.")
+    return response
 
 
 def refresh_chat_rooms(self, from_time: int = None) -> ChatRoomsResponse:
     self._check_authorization()
     params = {}
     if from_time:
         params["from_time"] = from_time
@@ -280,52 +306,58 @@
         "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/update",
         params=params, data_type=ChatRoomsResponse
     )
 
 
 def remove_chat_rooms(self, chat_room_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/mass_destroy",
         payload={"chat_room_ids[]": chat_room_ids},
     )
+    self.logger.info("Chat rooms removed.")
+    return response
 
 
 def report_chat_room(
         self,
         chat_room_id: int,
         opponent_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V3}/{chat_room_id}/report",
         payload={
             "chat_room_id": chat_room_id,
             "opponent_id": opponent_id,
             "category_id": category_id,
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
         },
     )
+    self.logger.info("Chat room reported.")
+    return response
 
 
 def send_media_screenshot_notification(self, room_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/screen_captured"
     )
+    self.logger.info("Media screenshot notification sent.")
+    return response
 
 
 def send_message(
         self,
         chat_room_id: int,
         message_type: str,
         call_type: str = None,
@@ -333,45 +365,51 @@
         font_size: int = None,
         gif_image_id: int = None,
         attachment_file_name: str = None,
         sticker_pack_id: int = None,
         video_file_name: str = None
 ) -> MessageResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V3}/{chat_room_id}/messages/new",
         payload={
             "chat_room_id": chat_room_id,
             "message_type": message_type,
             "call_type": call_type,
             "text": text,
             "font_size": font_size,
             "gif_image_id": gif_image_id,
             "attachment_file_name": attachment_file_name,
             "sticker_pack_id": sticker_pack_id,
             "video_file_name": video_file_name,
         }, data_type=MessageResponse
     )
+    self.logger.info("Message sent.")
+    return response
 
 
 def set_notification_settings(
         self,
         chat_room_id: int,
         notification_chat: int
 ) -> Settings:
     # NotificationSettingResponse
     pass
 
 
 def unhide_chat(self, chat_room_ids: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.HIDDEN_V1}/chats",
         params={"chat_room_ids[]": chat_room_ids},
     )
+    self.logger.info("Chatroom unhidden.")
+    return response
 
 
 def unpin_chat(self, chat_room_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{chat_room_id}/pinned"
     )
+    self.logger.info("Chatroom unpinned.")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/api/group.py` & `yaylib-0.1.2/yaylib/api/group.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,46 +6,56 @@
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
 def accept_moderator_offer(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize"
     )
+    self.logger.info("Moderator offer accepted.")
+    return response
 
 
 def accept_ownership_offer(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer"
     )
+    self.logger.info("Ownership offer accepted.")
+    return response
 
 
 def accept_group_join_request(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/accept/{user_id}"
     )
+    self.logger.info("Accepted group join request.")
+    return response
 
 
 def add_related_groups(self, group_id: int, related_group_id: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
         params={"related_group_id[]": related_group_id}
     )
+    self.logger.info("Group added to the related groups")
+    return response
 
 
 def ban_group_user(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/ban/{user_id}"
     )
+    self.logger.info("User has been banned from the group.")
+    return response
 
 
 def check_unread_status(self, from_time: int = None) -> UnreadStatusResponse:
     self._check_authorization()
     params = {}
     if from_time:
         params["from_time"] = from_time
@@ -75,15 +85,15 @@
         sub_category_id: str = None,
         hide_from_game_eight: bool = None,
         allow_members_to_post_media: bool = None,
         allow_members_to_post_url: bool = None,
         guidelines: str = None,
 ) -> CreateGroupResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/new",
         payload={
             "topic": topic,
             "description": description,
             "secret": secret,
             "hide_reported_posts": hide_reported_posts,
             "hide_conference_call": hide_conference_call,
@@ -107,50 +117,62 @@
             "sub_category_id": sub_category_id,
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
         }, data_type=CreateGroupResponse
     )
+    self.logger.info("Group created.")
+    return response
 
 
 def create_pin_group(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.PINNED_V1}/groups",
         payload={"id": group_id}
     )
+    self.logger.info("Pinned post in the group.")
+    return response
 
 
 def decline_moderator_offer(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize"
     )
+    self.logger.info("Declined moderator offer.")
+    return response
 
 
 def decline_ownership_offer(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer"
     )
+    self.logger.info("Declined ownership offer.")
+    return response
 
 
 def decline_group_join_request(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/decline/{user_id}"
     )
+    self.logger.info("Declined group join request")
+    return response
 
 
 def delete_pin_group(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.PINNED_V1}/groups/{group_id}"
     )
+    self.logger.info("Unpinned group post.")
+    return response
 
 
 def get_banned_group_members(self, group_id: int, page: int = None) -> UsersResponse:
     self._check_authorization()
     params = {}
     if page:
         params["page"] = page
@@ -322,115 +344,135 @@
         "GET", endpoint=f"{Endpoints.GROUPS_V1}/user_group_list",
         params=params, data_type=GroupsResponse
     )
 
 
 def invite_users_to_group(self, group_id: int, user_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/invite",
         payload={"user_ids[]": user_ids}
     )
+    self.logger.info("Group invitation sent.")
+    return response
 
 
 def join_group(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/join",
     )
+    self.logger.info("Joined the group.")
+    return response
 
 
 def leave_group(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/leave",
     )
+    self.logger.info("Left the group.")
+    return response
 
 
 def post_gruop_social_shared(self, group_id: int, sns_name: str):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/social_shared",
         params={"sns_name": sns_name}
     )
+    self.logger.info("Group social shared posted.")
+    return response
 
 
 def remove_group_cover(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/remove_cover",
     )
+    self.logger.info("Group cover removed.")
+    return response
 
 
 def remove_moderator(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/fire/{user_id}",
     )
+    self.logger.info("Group moderator removed.")
+    return response
 
 
 def remove_related_groups(self, group_id: int, related_group_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
         params={"related_group_id[]": related_group_ids}
     )
+    self.logger.info("Related groups removed.")
+    return response
 
 
 def report_group(
         self,
         group_id: int,
         category_id: int,
         reason: str = None,
         opponent_id: int = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None,
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/report",
         payload={
             "category_id": category_id, "reason": reason,
             "opponent_id": opponent_id, "screenshot_filename": screenshot_filename, "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename
         }
     )
+    self.logger.info("Group reported.")
+    return response
 
 
 def send_moderator_offers(self, group_id: int, user_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/deputize/mass",
         payload={
             "user_ids[]": user_ids, "uuid": self.uuid,
             "api_key": self.api_key, "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
                 self.api_key, self.device_uuid,
                 int(datetime.now().timestamp())
             ),
         }
     )
+    self.logger.info("Group moderator offer sent.")
+    return response
 
 
 def send_ownership_offer(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/transfer",
         payload={
             "user_id": user_id, "uuid": self.uuid,
             "api_key": self.api_key, "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
                 self.api_key, self.device_uuid,
                 int(datetime.now().timestamp())
             ),
         }
     )
+    self.logger.info("Group ownership offer sent.")
+    return response
 
 
 def set_group_notification_settings(
         self,
         group_id: int,
         notification_group_post: int = None,
         notification_group_join: int = None,
@@ -438,32 +480,38 @@
         notification_group_message_tag_all: int = None,
 ) -> AdditionalSettingsResponse:
     pass
 
 
 def set_group_title(self, group_id: int, title: str):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/set_title",
         payload={"title": title}
     )
+    self.logger.info("Group title set.")
+    return response
 
 
 def take_over_group_ownership(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/take_over",
     )
+    self.logger.info(f"Took over the group ownership of {group_id}")
+    return response
 
 
 def unban_group_member(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/unban/{user_id}",
     )
+    self.logger.info("Group user has been unbanned.")
+    return response
 
 
 def update_group(
         self,
         group_id: int,
         topic: str,
         description: str = None,
@@ -483,15 +531,15 @@
         sub_category_id: str = None,
         hide_from_game_eight: bool = None,
         allow_members_to_post_media: bool = None,
         allow_members_to_post_url: bool = None,
         guidelines: str = None,
 ) -> GroupResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/update",
         payload={
             "topic": topic,
             "description": description,
             "secret": secret,
             "hide_reported_posts": hide_reported_posts,
             "hide_conference_call": hide_conference_call,
@@ -515,28 +563,36 @@
             ),
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
         }, data_type=GroupResponse
     )
+    self.logger.info("Group has been updated.")
+    return response
 
 
 def visit_group(self, group_id: int):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/visit",
     )
+    self.logger.info("Group visited.")
+    return response
 
 
 def withdraw_moderator_offer(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize/{user_id}/withdraw",
     )
+    self.logger.info("Group moderator offer withdrawn")
+    return response
 
 
 def withdraw_ownership_offer(self, group_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer/withdraw",
         payload={"user_id": user_id}
     )
+    self.logger.info("Group ownershipt offer withdrawn")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/api/login.py` & `yaylib-0.1.2/yaylib/api/login.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,38 +10,42 @@
 
 def change_email(
         self,
         email: str,
         password: str,
         email_grant_token: str = None
 ) -> LoginUpdateResponse:
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.USERS_V1}/change_email",
         payload={
             "api_key": self.api_key,
             "email": email,
             "password": password,
             "email_grant_token": email_grant_token
         }, data_type=LoginUpdateResponse
     )
+    self.logger.info("Email has been changed.")
+    return response
 
 
 def change_password(
         self,
         current_password: str,
         new_password: str
 ) -> LoginUpdateResponse:
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.USERS_V1}/change_email",
         payload={
             "api_key": self.api_key,
             "current_password": current_password,
             "password": new_password
         }, data_type=LoginUpdateResponse
     )
+    self.logger.info("Password has been changed.")
+    return response
 
 
 def connect_account_with_sns(self):
     pass
 
 
 def disconnect_account_with_sns(self):
@@ -62,15 +66,15 @@
             "email": email,
             "password": password,
             "refresh_token": refresh_token
         }, data_type=TokenResponse
     )
 
 
-def login_with_email(self, email: str, password: str) -> LoginUserResponse:
+def login(self, email: str, password: str) -> LoginUserResponse:
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V3}/login_with_email",
         payload={
             "api_key": self.api_key,
             "email": email,
             "password": password,
             "uuid": self.uuid
@@ -121,45 +125,51 @@
 def resend_confirm_email(self):
     return self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/resend_confirm_email"
     )
 
 
 def restore_user(self, user_id: int) -> LoginUserResponse:
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/restore",
         payload={
             "user_id": user_id,
             "api_key": self.api_key,
             "uuid": self.uuid,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
         }
     )
+    self.logger.info("User restored.")
+    return response
 
 
 def revoke_tokens(self):
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V1}/device_tokens"
     )
+    self.logger.info("Token revoked.")
+    return response
 
 
 def save_account_with_email(
         self,
         email: str,
         password: str = None,
         current_password: str = None,
         email_grant_token: str = None
 ) -> LoginUpdateResponse:
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V3}/login_update",
         payload={
             "api_key": self.api_key,
             "email": email,
             "password": password,
             "current_password": current_password,
             "email_grant_token": email_grant_token
         }, data_type=LoginUpdateResponse
     )
+    self.logger.info("Account has been save with email.")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/api/misc.py` & `yaylib-0.1.2/yaylib/api/review.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,127 +4,107 @@
 from ..config import *
 from ..errors import *
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
-def accept_policy_agreement(self, type: str):
-    return self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/policy_agreements/{type}"
-    )
-
-
-def generate_sns_thumbnail(self, **params):
-    """
-
-    Parameters:
-    ----------
-
-        - resource_type: str - (Required)
-        - resource_id: int - (Required)
-
-    """
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.SNS_THUMBNAIL_V1}/generate",
-        params=params
+def create_review(self, user_id: int, comment: str):
+    self._check_authorization()
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
+        "POST", endpoint=f"{Endpoints.USERS_V2}/reviews/{user_id}",
+        payload={
+            "comment": comment,
+            "uuid": self.uuid,
+            "api_key": self.api_key,
+            "timestamp": timestamp,
+            "signed_info": signed_info_calculating(
+                self.uuid, timestamp, shared_key=True
+            ),
+        },
     )
+    self.logger.info("Review created.")
+    return response
 
 
-def get_email_verification_presigned_url(self, email: str, locale: str, intent: str = None) -> str:
-    return self._make_request(
-        "POST", endpoint=f"{Endpoints.EMAIL_VERIFICATION_URL_V1}",
+def create_reviews(self, user_ids: List[int], comment: str):
+    self._check_authorization()
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
+        "POST", endpoint=f"{Endpoints.USERS_V1}/reviews",
         payload={
-            "device_uuid": self.device_uuid,
-            "email": email,
-            "locale": locale,
-            "intent": intent
-        }, data_type=EmailVerificationPresignedUrlResponse
-    ).url
+            "user_ids": user_ids,
+            "comment": comment,
+            "uuid": self.uuid,
+            "api_key": self.api_key,
+            "timestamp": timestamp,
+            "signed_info": signed_info_calculating(
+                self.uuid, timestamp, shared_key=True
+            ),
+        },
+    )
+    self.logger.info("Reviews created.")
+    return response
 
 
-def get_file_upload_presigned_urls(self, file_names: List[str]) -> List[PresignedUrl]:
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.BUCKETS_V1}/presigned_urls",
-        params={"file_names[]": file_names}, data_type=PresignedUrlsResponse
-    ).presigned_urls
+def delete_reviews(self, review_ids: List[int]):
+    self._check_authorization()
+    response = self._make_request(
+        "DELETE", endpoint=f"{Endpoints.USERS_V1}/reviews",
+        params={"review_ids[]": review_ids}
+    )
+    self.logger.info("Reviews deleted.")
+    return response
 
 
-def get_id_checker_presigned_url(
-        self,
-        model: str,
-        action: str,
-        **params
-) -> str:
-    # TODO: @QueryMap @NotNull Map<String, String> map
-    """
-    Meow..
+def get_my_reviews(self, **params) -> ReviewsResponse:
     """
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.ID_CHECK_V1}/{model}/{action}",
-        params=params, data_type=IdCheckerPresignedUrlResponse
-    ).presigned_url
 
+    Parameters
+    ----------
 
-def get_old_file_upload_presigned_url(self, video_file_name: str) -> str:
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/presigned_url",
-        params={"video_file_name": video_file_name}, data_type=PresignedUrlResponse
-    ).presigned_url
-
+        - from_id: int (optional)
+        - number: int = (optional)
 
-def get_policy_agreements(self) -> PolicyAgreementsResponse:
+    """
+    self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/policy_agreements",
-        data_type=PolicyAgreementsResponse
+        "GET", endpoint=f"{Endpoints.USERS_V1}/reviews/mine",
+        params=params, data_type=ReviewsResponse
     )
 
 
-def get_promotions(self, **params) -> List[Promotion]:
+def get_reviews(self, user_id: int, **params) -> ReviewsResponse:
     """
 
-    Parameters:
+    Parameters
     ----------
 
-        - page: int - (Optional)
-        - number: int - (Optional)
+        - user_id: int (required)
+        - from_id: int = (optional)
+        - number: int = (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.PROMOTIONS_V1}",
-        params=params, data_type=PromotionsResponse
-    ).promotions
-
-
-def get_vip_game_reward_url(self, device_type: str) -> str:
-    # TODO: device_type
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.SKYFALL_V1}/url",
-        params={"device_type": device_type}, data_type=VipGameRewardUrlResponse
-    ).url
+        "GET", endpoint=f"{Endpoints.USERS_V1}/reviews/{user_id}",
+        params=params, data_type=ReviewsResponse
+    )
 
 
-def get_web_socket_token(self) -> str:
+def pin_review(self, review_id: int):
     self._check_authorization()
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/ws_token",
-        data_type=WebSocketTokenResponse
-    ).token
+    response = self._make_request(
+        "POST", endpoint=f"{Endpoints.PINNED_V1}/reviews",
+        payload={"id": review_id}
+    )
+    self.logger.info("Pinned the review.")
+    return response
 
 
-def verify_device(
-        self,
-        app_version: str,
-        device_uuid: str,
-        platform: str,
-        verification_string: str
-) -> VerifyDeviceResponse:
-    # TODO: check platform, verification_string
-    return self._make_request(
-        "POST", endpoint=f"{Endpoints.GENUINE_DEVICES_V1}/verify",
-        payload={
-            "app_version": app_version,
-            "device_uuid": device_uuid,
-            "platform": platform,
-            "verification_string": verification_string,
-        }, data_type=VerifyDeviceResponse
+def unpin_review(self, review_id: int):
+    self._check_authorization()
+    response = self._make_request(
+        "DELETE", endpoint=f"{Endpoints.PINNED_V1}/reviews{review_id}"
     )
+    self.logger.info("Review unpinned.")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/api/post.py` & `yaylib-0.1.2/yaylib/api/post.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,29 @@
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
 def add_bookmark(self, user_id: int, post_id: int) -> BookmarkPostResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
         data_type=BookmarkPostResponse
     )
+    self.logger.info("Added to bookmarks.")
+    return response
 
 
 def add_group_highlight_post(self, group_id: int, post_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
     )
+    self.logger.info("Added to group highlight.")
+    return response
 
 
 def create_call_post(
         self,
         text: str = None,
         font_size: int = None,
         color: int = None,
@@ -43,31 +47,33 @@
         attachment_6_filename: str = None,
         attachment_7_filename: str = None,
         attachment_8_filename: str = None,
         attachment_9_filename: str = None,
 ) -> ConferenceCall:
     self._check_authorization()
 
-    if "@:start:" in text and ":end:" in text:
-        text, message_tags = parse_mention_format(self, text)
+    if text is not None:
+        if "@:start:" in text and ":end:" in text:
+            text, message_tags = parse_mention_format(self, text)
 
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V2}/new_conference_call",
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "group_id": group_id,
             "call_type": call_type,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
             "category_id": category_id,
             "game_title": game_title,
             "joinable_by": joinable_by,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
@@ -76,30 +82,36 @@
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
         }, data_type=CreatePostResponse
     ).conference_call
+    self.logger.info("Call post created.")
+    return response
 
 
 def create_group_pin_post(self, post_id: int, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
         payload={"post_id": post_id, "group_id": group_id}
     )
+    self.logger.info("Pinned post in a group.")
+    return response
 
 
 def create_pin_post(self, post_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.PINNED_V1}/posts",
         payload={"id": post_id}
     )
+    self.logger.info("Pinned post")
+    return response
 
 
 def mention(self, user_id: int) -> str:
     if not (isinstance(user_id, int) or str(user_id).isdigit()):
         raise ValueError(
             "The value of 'user_id' must be an integer or a string containing only digits.")
     return "@:start:" + str(user_id) + ":end:"
@@ -112,15 +124,15 @@
     segments = text.split("@:start:")
 
     for i, segment in enumerate(segments):
         if i == 0:
             formatted_text += segment
             continue
         user_id, text = segment.split(":end:")
-        username = self.get_user(user_id).username
+        username = self.get_user(user_id).nickname
         formatted_text += "@" + username + " " + text
         user_ids.append(user_id)
 
     return formatted_text, user_ids
 
 
 def parse_mention_format(self, text) -> tuple:
@@ -153,18 +165,17 @@
 def create_post(
         self,
         text: str = None,
         font_size: int = 0,
         color: int = 0,
         in_reply_to: int = None,
         group_id: int = None,
-        post_type: str = None,
         mention_ids: List[int] = None,
         choices: List[str] = None,
-        shared_url: Dict[str, str | int] = None,
+        shared_url: str = None,
         message_tags: str = "[]",
         attachment_filename: str = None,
         attachment_2_filename: str = None,
         attachment_3_filename: str = None,
         attachment_4_filename: str = None,
         attachment_5_filename: str = None,
         attachment_6_filename: str = None,
@@ -173,42 +184,54 @@
         attachment_9_filename: str = None,
         video_file_name: str = None,
 ) -> Post:
     self._check_authorization()
     headers = self.session.headers
     headers["X-Jwt"] = self.get_web_socket_token()
 
-    if "@:start:" in text and ":end:" in text:
-        text, message_tags = parse_mention_format(self, text)
+    if text is not None:
+        if "@:start:" in text and ":end:" in text:
+            text, message_tags = parse_mention_format(self, text)
+
+    post_type = "survey" if choices else "shareable_url" if shared_url else "video" if video_file_name else "image" if attachment_filename else "text"
+
+    if shared_url is not None:
+        try:
+            shared_url = self.get_url_metadata(url=shared_url).data
+        except ForbiddenError:
+            self.logger.error("Unable to get the URL metadata")
+            shared_url = None
 
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V3}/new",
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
             "post_type": post_type,
             "mention_ids[]": mention_ids,
-            "choices[]": choices,
+            "choices": choices,
             "shared_url": shared_url,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
             "attachment_4_filename": attachment_4_filename,
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
         }, data_type=Post, headers=headers
     )
+    self.logger.info("Post created.")
+    return response
 
 
 def create_repost(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
@@ -231,73 +254,87 @@
         attachment_9_filename: str = None,
         video_file_name: str = None,
 ) -> Post:
     self._check_authorization()
     headers = self.session.headers
     headers["X-Jwt"] = self.get_web_socket_token()
 
-    if "@:start:" in text and ":end:" in text:
-        text, message_tags = parse_mention_format(self, text)
+    if text is not None:
+        if "@:start:" in text and ":end:" in text:
+            text, message_tags = parse_mention_format(self, text)
+
+    post_type = "survey" if choices else "shareable_url" if shared_url else "video" if video_file_name else "image" if attachment_filename else "text"
+
+    if shared_url is not None:
+        try:
+            shared_url = self.get_url_metadata(url=shared_url).data
+        except ForbiddenError:
+            self.logger.error("Unable to get the URL metadata")
+            shared_url = None
 
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V3}/repost",
         payload={
             "post_id": post_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
             "post_type": post_type,
             "mention_ids[]": mention_ids,
-            "choices[]": choices,
+            "choices": choices,
             "shared_url": shared_url,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
             "attachment_4_filename": attachment_4_filename,
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
         }, data_type=CreatePostResponse, headers=headers
     ).post
+    self.logger.info("Repost created.")
+    return response
 
 
 def create_share_post(
         self,
         shareable_type: str,
         shareable_id: int,
         text: str = None,
         font_size: int = None,
         color: int = None,
         group_id: int = None,
 ) -> Post:
     self._check_authorization()
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V2}/new_share_post",
         payload={
             "shareable_type": shareable_type,
             "shareable_id": shareable_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "group_id": group_id,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
         }, data_type=Post
     )
+    self.logger.info("Share post created.")
+    return response
 
 
 def create_thread_post(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
@@ -320,68 +357,89 @@
         attachment_9_filename: str = None,
         video_file_name: str = None,
 ) -> Post:
     self._check_authorization()
     headers = self.session.headers
     headers["X-Jwt"] = self.get_web_socket_token()
 
-    if "@:start:" in text and ":end:" in text:
-        text, message_tags = parse_mention_format(self, text)
+    if text is not None:
+        if "@:start:" in text and ":end:" in text:
+            text, message_tags = parse_mention_format(self, text)
+
+    post_type = "survey" if choices else "shareable_url" if shared_url else "video" if video_file_name else "image" if attachment_filename else "text"
+
+    if shared_url is not None:
+        try:
+            shared_url = self.get_url_metadata(url=shared_url).data
+        except ForbiddenError:
+            self.logger.error("Unable to get the URL metadata")
+            shared_url = None
 
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.THREADS_V1}/{post_id}/posts",
         payload={
             "id": post_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
             "post_type": post_type,
             "mention_ids[]": mention_ids,
-            "choices[]": choices,
+            "choices": choices,
             "shared_url": shared_url,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
             "attachment_4_filename": attachment_4_filename,
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
         }, data_type=Post, headers=headers
     )
+    self.logger.info("Thread post created.")
+    return response
 
 
 def delete_all_post(self):
     self._check_authorization()
-    return self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V1}/delete_all_post",
-    )
+    try:
+        response = self._make_request(
+            "POST", endpoint=f"{Endpoints.POSTS_V1}/delete_all_post",
+        )
+        self.logger.info("Post deletion requested.")
+        return response
+    except NotFoundError:
+        self.logger.info("Post not found.")
 
 
 def delete_group_pin_post(self, group_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
         payload={"group_id": group_id}
     )
+    self.logger.info("Unpinned post in a group.")
+    return response
 
 
 def delete_pin_post(self, post_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.PINNED_V1}/posts/{post_id}"
     )
+    self.logger.info("Unpinned post.")
+    return response
 
 
-def get_bookmark(self, user_id: int, *, from_str: str = None) -> PostsResponse:
+def get_bookmark(self, user_id: int, from_str: str = None) -> PostsResponse:
     self._check_authorization()
     params = {}
     if from_str:
         params = {"from": from_str}
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks",
         params=params, data_type=PostsResponse
@@ -401,15 +459,14 @@
         - call_type: str = "voice"
         - include_circle_call: bool = None
         - cross_generation: bool = None
         - exclude_recent_gomimushi: bool = None
         - shared_interest_categories: bool = None
 
     """
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V2}/call_timeline",
         params=params, data_type=PostsResponse
     )
 
 
 def get_conversation(self, conversation_id: int, **params) -> PostsResponse:
@@ -422,23 +479,21 @@
         - group_id: int = None
         - thread_id: int = None
         - from_post_id: int = None
         - number: int = 50
         - reverse: bool = True
 
     """
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.CONVERSATIONS_V2}/{conversation_id}",
         params=params, data_type=PostsResponse
     )
 
 
 def get_conversation_root_posts(self, post_ids: List[int]) -> PostsResponse:
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.CONVERSATIONS_V2}/root_posts",
         params={"ids[]": post_ids}, data_type=PostsResponse
     )
 
 
 def get_following_call_timeline(self, **params) -> PostsResponse:
@@ -491,15 +546,14 @@
     ----------
 
         - group_id: int
         - from_post: int = None
         - number: int = None
 
     """
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights",
         params=params, data_type=PostsResponse
     )
 
 
 def get_group_timeline_by_keyword(self, group_id: int, keyword: str, **params) -> PostsResponse:
@@ -511,15 +565,14 @@
         - group_id: int
         - keyword: str
         - from_post_id: int = None
         - number: int = None
         - only_thread_posts: bool = False
 
     """
-    self._check_authorization()
     params["keyword"] = keyword
     return self._make_request(
         "GET", endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/posts/search",
         params=params, data_type=PostsResponse
     )
 
 
@@ -533,15 +586,14 @@
         - from_post_id: int
         - reverse: bool
         - post_type: str
         - number: int
         - only_root: bool
 
     """
-    self._check_authorization()
     params["group_id"] = group_id
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V2}/group_timeline",
         params=params, data_type=PostsResponse
     )
 
 
@@ -552,15 +604,14 @@
     ----------
 
         - hashtag: str - (required)
         - from_post_id: int - (optional)
         - number: int - (optional)
 
     """
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V2}/tags/{hashtag}",
         params=params, data_type=PostsResponse
     )
 
 
 def get_my_posts(self, **params) -> PostsResponse:
@@ -619,44 +670,41 @@
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V2}/{post_id}/reposts",
         params=params, data_type=PostsResponse
     )
 
 
 def get_posts(self, post_ids: List[int]) -> PostsResponse:
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V2}/multiple",
         params={"post_ids[]": post_ids}, data_type=PostsResponse
     )
 
 
 def get_recommended_post_tags(
         self, tag: str = None, save_recent_search: bool = False
 ) -> PostTagsResponse:
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V1}/recommended_tag",
         payload={"tag": tag, "save_recent_search": save_recent_search},
         data_type=PostTagsResponse
     )
 
 
 def get_recommended_posts(self, **params) -> PostsResponse:
     """
 
     Parameters:
     ---------------
 
-        - experiment_num: int
-        - variant_num: int
-        - number: int
+        - experiment_num: int - (Required)
+        - variant_num: int - (Required)
+        - number: int - (Optional)
 
     """
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V2}/recommended_timeline",
         params=params, data_type=PostsResponse
     )
 
 
 def get_timeline_by_keyword(self, keyword: str = None, **params) -> PostsResponse:
@@ -666,15 +714,14 @@
     ---------------
 
         - keyword: str
         - from_post_id: int
         - number: int
 
     """
-    self._check_authorization()
     params["keyword"] = keyword
     return self._make_request(
         "GET", endpoint=f"{Endpoints.POSTS_V2}/search",
         params=params, data_type=PostsResponse
     )
 
 
@@ -731,73 +778,85 @@
         "GET", endpoint=f"{Endpoints.POSTS_V2}/user_timeline",
         params=params, data_type=PostsResponse
     )
 
 
 def like_posts(self, post_ids: List[int]) -> LikePostsResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V2}/like",
         payload={"post_ids[]": post_ids}, data_type=LikePostsResponse
     )
+    self.logger.info("Posts liked.")
+    return response
 
 
 def remove_bookmark(self, user_id: int, post_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
     )
+    self.logger.info("Bookmark removed.")
+    return response
 
 
 def remove_group_highlight_post(self, group_id: int, post_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
     )
+    self.logger.info("Group hightlight post removed.")
+    return response
 
 
 def remove_posts(self, post_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V2}/mass_destroy",
-        payload={"post_ids[]": post_ids}
+        payload={"posts_ids": post_ids}
     )
+    self.logger.info("Posts removed.")
+    return response
 
 
 def report_post(
         self,
         post_id: int,
         opponent_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/report",
         payload={
             "opponent_id": opponent_id,
             "category_id": category_id,
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
         }
     )
+    self.logger.info("Post reported.")
+    return response
 
 
 def unlike_post(self, post_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V1}/{post_id}/unlike",
     )
+    self.logger.info("Post unliked.")
+    return response
 
 
 def update_post(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
@@ -805,61 +864,72 @@
         message_tags: str = "[]",
 ) -> Post:
     self._check_authorization()
 
     if "@:start:" in text and ":end:" in text:
         text, message_tags = parse_mention_format(self, text)
 
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.POSTS_V3}/{post_id}",
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "message_tags": str(message_tags),
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
         }
     )
+    self.logger.info("Post updated.")
+    return response
 
 
 def update_recommendation_feedback(
         self, post_id: int, feedback_result: str, *,
         experiment_num: int, variant_num: int,
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V2}/{post_id}/recommendation_feedback",
         payload={
             "feedback_result": feedback_result,
             "experiment_num": experiment_num,
             "variant_num": variant_num
         }
     )
+    self.logger.info("Recommendation feedback updated.")
+    return response
 
 
 def validate_post(self, text: str, *, group_id: int = None, thread_id: int = None) -> ValidationPostResponse:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V1}/validate",
         payload={
             "text": text, "group_id": group_id, "thread_id": thread_id
         }, data_type=ValidationPostResponse
     )
+    self.logger.info("Post validated.")
+    return response
 
 
 def view_video(self, video_id: int):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V1}/videos/{video_id}/view"
     )
+    self.logger.info("Viewed a video")
+    return response
 
 
 def vote_survey(self, survey_id: int, choice_id: int) -> Survey:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.SURVEYS_V2}/{survey_id}/vote",
         payload={"choice_id": choice_id}, data_type=ValidationPostResponse
     ).survey
+    self.logger.info("Survey voted.")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/api/thread.py` & `yaylib-0.1.2/yaylib/api/thread.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,51 +6,57 @@
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
 def add_post_to_thread(self, post_id: int, thread_id: int) -> ThreadInfo:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread/{thread_id}",
         data_type=ThreadInfo
     )
+    self.logger.info("Post added to the thread.")
+    return response
 
 
 def convert_post_to_thread(
         self,
         post_id: int,
         title: str = None,
         thread_icon_filename: str = None
 ) -> ThreadInfo:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread",
         payload={
             "title": title,
             "thread_icon_filename": thread_icon_filename
         }, data_type=ThreadInfo
     )
+    self.logger.info("Post converted to a thread.")
+    return response
 
 
 def create_thread(
         self,
         group_id: int,
         title: str,
         thread_icon_filename: str
 ) -> ThreadInfo:
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.THREADS_V1}",
         payload={
             "group_id": group_id,
             "title": title,
             "thread_icon_filename": thread_icon_filename,
         }, data_type=ThreadInfo
     )
+    self.logger.info("Thread created.")
+    return response
 
 
 def get_group_thread_list(self, group_id: int, from_str: str = None, **params) -> GroupThreadListResponse:
     """
 
     Parameters:
     ----------
@@ -94,37 +100,45 @@
         "GET", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/posts",
         params=params, data_type=PostsResponse
     )
 
 
 def join_thread(self, thread_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
     )
+    self.logger.info("Joined the thread.")
+    return response
 
 
 def leave_thread(self, thread_id: int, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
     )
+    self.logger.info("Left the thread.")
+    return response
 
 
 def remove_thread(self, thread_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
     )
+    self.logger.info("Thread removed.")
+    return response
 
 
 def update_thread(
         self,
         thread_id: int,
         title: str,
         thread_icon_filename: str
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
         payload={"title": title, "thread_icon_filename": thread_icon_filename}
     )
+    self.logger.info("Thread updated.")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/api/user.py` & `yaylib-0.1.2/yaylib/api/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,27 +21,24 @@
         # @Nullable @Part("sns_info") SignUpSnsInfoRequest signUpSnsInfoRequest,
         email: str = None,
         password: str = None,
         email_grant_token: str = None,
         en: int = None,
         vn: int = None
 ) -> CreateUserResponse:
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V3}/edit",
         payload={
             "app_version": self.api_version,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "api_key": self.api_key,
-            "signed_version": signed_version_calculating(
-                self.yay_version_message, self.api_version_key,
-                int(datetime.now().timestamp())
-            ),
+            "signed_version": signed_version_calculating(),
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
             "uuid": self.uuid,
             "nickname": nickname,
             "birth_date": birth_date,
             "gender": gender,
             "country_code": country_code,
             "biography": biography,
@@ -51,59 +48,74 @@
             "email": email,
             "password": password,
             "email_grant_token": email_grant_token,
             "en": en,
             "vn": vn,
         }
     )
+    self.logger.info("Account created.")
+    return response
 
 
 def delete_contact_friends(self):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V1}/contact_friends"
     )
+    self.logger.info("Contact friends deleted.")
+    return response
 
 
 def delete_footprint(self, user_id: int, footprint_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V2}/{user_id}/footprints/{footprint_id}"
     )
+    self.logger.info("Footprint deleted.")
+    return response
 
 
 def destroy_user(self):
     self._check_authorization()
-    return self._make_request(
+    answer = input("Are you sure you want to delete your account? Y/N")
+    if answer.lower() != "y":
+        return
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/destroy",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
         }
     )
+    self.logger.info("User has been deleted.")
+    return response
 
 
 def follow_user(self, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/follow"
     )
+    self.logger.info(f"User '{user_id}' followed.")
+    return response
 
 
 def follow_users(self, user_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/follow",
         params={"user_ids[]": user_ids}
     )
+    self.logger.info("Users followed.")
+    return response
 
 
 def get_active_followings(self, **params) -> ActiveFollowingsResponse:
     """
 
     Parameters:
     ----------
@@ -294,15 +306,14 @@
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V2}/social_shared_users",
         params=params, data_type=SocialShareUsersResponse
     )
 
 
 def get_timestamp(self) -> UserTimestampResponse:
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V2}/timestamp",
         data_type=UserTimestampResponse
     )
 
 
 def get_user(self, user_id: int) -> User:
@@ -330,20 +341,20 @@
 
 def get_user_followers(self, user_id: int, **params) -> FollowUsersResponse:
     """
 
     Parameters:
     ----------
 
-        - user_id: int
-        - from_follow_id: int = None
-        - followed_by_me: int = None
+        - user_id: int - (required)
+        - from_follow_id: int - (optional)
+        - followed_by_me: int - (optional)
+        - number: int - (optional)
 
     """
-    self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V2}/{user_id}/followers",
         params=params, data_type=FollowUsersResponse
     )
 
 
 def get_user_followings(self, user_id: int, **params) -> FollowUsersResponse:
@@ -353,14 +364,15 @@
     Parameters:
     ----------
 
         - user_id: int
         - from_follow_id: int = None
         - from_timestamp: int = None
         - order_by: str = None
+        - number: int - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/list_followings",
         params=params, data_type=FollowUsersResponse
     )
@@ -400,98 +412,112 @@
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V2}/list_uuid/",
         params={"uuid": uuid}, data_type=UsersResponse
     )
 
 
 def post_social_shared(self, sns_name: str):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/social_shared",
         params={"sns_name": sns_name}
     )
+    self.logger.info("Social shared posted.")
+    return response
 
 
 def record_app_review_status(self):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/{self.url_uuid}/app_review_status",
         params={"uuid": self.uuid}
     )
+    self.logger.info("App review status recored.")
+    return response
 
 
 def reduce_kenta_penalty(self, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{self.host}api/v3/users/{user_id}/reduce_penalty",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
-            "signed_version": signed_version_calculating(
-                self.yay_version_message, self.api_version_key
-            )
+            "signed_version": signed_version_calculating()
         }, data_type=CreatePostResponse
     )
+    self.logger.info("Penalty reduced.")
+    return response
 
 
 def refresh_counter(self, counter: str):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/reset_counters",
         payload={"counter": counter}
     )
+    self.logger.info("Counter refreshed.")
+    return response
 
 
 def remove_user_avatar(self):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/remove_profile_photo"
     )
+    self.logger.info("User avatar removed.")
+    return response
 
 
 def remove_user_cover(self):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/remove_cover_image"
     )
+    self.logger.info("User cover removed.")
+    return response
 
 
 def report_user(
         self,
         user_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None
 ):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V3}/{user_id}/report",
         payload={
             "category_id": category_id,
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
         }
     )
+    self.logger.info("User reported.")
+    return response
 
 
 def reset_password(self, email: str, email_grant_token: str, password: str):
-    return self._make_request(
+    response = self._make_request(
         "PUT", endpoint=f"{Endpoints.USERS_V1}/reset_password",
         payload={
             "email": email,
             "email_grant_token": email_grant_token,
             "password": password,
         }
     )
+    self.logger.info("Password has been reset.")
+    return response
 
 
 def search_lobi_users(self, **params) -> UsersResponse:
     """
 
     Parameters:
     ----------
@@ -528,125 +554,140 @@
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V1}/search",
         params=params, data_type=UsersResponse,
     )
 
 
 def set_additional_setting_enabled(self, mode: str, on: int = None):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/additonal_notification_setting",
         payload={"mode": mode, "on": on}
     )
+    self.logger.info("Additional setting enabled.")
+    return response
 
 
 def set_follow_permission_enabled(self, nickname: str, is_private: bool = None):
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/edit",
         payload={
             "nickname": nickname,
             "is_private": is_private,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
-            "signed_version": signed_version_calculating(
-                self.yay_version_message, self.api_version_key
-            )
+            "signed_version": signed_version_calculating()
         }
     )
+    self.logger.info("Follow permission enabled.")
+    return response
 
 
 def set_setting_follow_recommendation_enabled(self, on: bool):
-    return self._make_request(
+    response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/visible_on_sns_friend_recommendation_setting",
         params={"on": on}
     )
+    self.logger.info("Follow recommendation enabled.")
+    return response
 
 
 def take_action_follow_request(self, target_id: int, action: str):
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{target_id}/follow_request",
         payload={"action": action}
     )
+    self.logger.info("Took action follow request.")
+    return response
 
 
 def turn_on_hima(self):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V1}/hima",
     )
+    self.logger.info("Turned on hima now.")
+    return response
 
 
 def unfollow_user(self, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/unfollow",
     )
+    self.logger.info("User unfollowed.")
+    return response
 
 
 def update_invite_contact_status(self, mobile_number: str):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/invite_contact",
         params={"mobile_number": mobile_number}
     )
+    self.logger.info("Invite contact status updated.")
+    return response
 
 
 def update_language(self, language: str):
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/language",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
-            ),
+                self.device_uuid, timestamp),
             "language": language,
         }
     )
+    self.logger.info("Language updated.")
+    return response
 
 
 def update_user(
         self,
         nickname: str,
         biography: str = None,
         prefecture: str = None,
         gender: int = None,
         country_code: str = None,
         profile_icon_filename: str = None,
         cover_image_filename: str = None,
         username: str = None,
 ):
     self._check_authorization()
-    return self._make_request(
+    timestamp = int(datetime.now().timestamp())
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V3}/edit",
         payload={
             "nickname": nickname,
             "biography": biography,
             "prefecture": prefecture,
             "gender": gender,
             "country_code": country_code,
             "profile_icon_filename": profile_icon_filename,
             "cover_image_filename": cover_image_filename,
             "username": username,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
+            "timestamp": timestamp,
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.device_uuid, timestamp
             ),
         }
     )
+    self.logger.info("User profile updated.")
+    return response
 
 
 def update_user_interests(
         self,
         # @Body @NotNull CommonIdsRequest commonIdsRequest,
         # @NotNull Continuation<? super Unit> continuation
 ):
@@ -658,28 +699,32 @@
         # @Body @Nullable UploadContactsRequest uploadContactsRequest
 ):
     pass
 
 
 def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/twitter_friends",
         payload={"twitter_friend_ids[]": twitter_friend_ids}
     )
+    self.logger.info("Twitter friend ids updated.")
+    return response
 
 
 # BlockApi
 
 
 def block_user(self, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/{user_id}/block",
     )
+    self.logger.info("User blocked.")
+    return response
 
 
 def get_blocked_user_ids(self) -> BlockedUserIdsResponse:
     self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V1}/block_ids",
         data_type=BlockedUserIdsResponse
@@ -696,17 +741,19 @@
         "GET", endpoint=f"{Endpoints.USERS_V2}/blocked",
         params=params, data_type=BlockedUsersResponse
     )
 
 
 def unblock_user(self, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/unblock"
     )
+    self.logger.info("User unblocked.")
+    return response
 
 
 # HiddenApi
 
 
 def get_hidden_users_list(self, **params: Union[str, int]) -> HiddenResponse:
     """
@@ -723,19 +770,23 @@
         "GET", endpoint=f"{Endpoints.HIDDEN_V1}/users",
         params=params, data_type=HiddenResponse
     )
 
 
 def hide_user(self, user_id: int):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "POST", endpoint=f"{Endpoints.HIDDEN_V1}/users",
         payload={"user_id": user_id}
     )
+    self.logger.info("user hidden.")
+    return response
 
 
 def unhide_users(self, user_ids: List[int]):
     self._check_authorization()
-    return self._make_request(
+    response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.HIDDEN_V1}/users",
         params={"user_ids[]": user_ids}
     )
+    self.logger.info("User unhidden.")
+    return response
```

### Comparing `yaylib-0.1.0/yaylib/client.py` & `yaylib-0.1.2/yaylib/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,373 +9,671 @@
 from .api.misc import *
 from .api.post import *
 from .api.review import *
 from .api.thread import *
 from .api.user import *
 
 from .config import *
-from .errors import *
+from .errors import (
+    YayError,
+    HTTPError,
+    BadRequestError,
+    AuthenticationError,
+    ForbiddenError,
+    NotFoundError,
+    RateLimitError,
+    YayServerError,
+)
 from .models import *
 from .utils import *
 
 
 class Client(API):
     """
-    Client( \
-        access_token=None, proxy=None, timeout=60, \
-        base_path=current_path, loglevel_stream=logging.INFO, \
-        host=Configs.YAY_PRODUCTION_HOST \
-    )
+
+    Yay!（イェイ）の API クライアント
+
+    #### Useage
+
+        >>> api = yaylib.Client()
+        >>> timeline = api.get_timeline(number=30)
+
+    #### Parameters
+
+        - access_token: str - (optional)
+        - refresh_token: str - (optional)
+        - proxy: str - (optional)
+        - timeout: int - (optional)
+        - base_path: str - (optional)
+        - loglevel_stream: int - (optional)
+        - host: str - (optional)
+
+    <https://github.com/qvco/yaylib>
 
     ---
 
-    #### Yay! API v3 Client
+    ### Yay! API v3 Client
+
+    Copyright (c) 2023 Qvco, Konn
 
     """
 
     # -CALL
 
-    def bump_call(self, call_id: int, participant_limit: int = None):
+    def bump_call(self, call_id: int, participant_limit: int = None) -> dict:
         return bump_call(self, call_id, participant_limit)
 
     def get_user_active_call(self, user_id: int) -> Post:
+        """
+
+        ユーザーが参加中の通話を取得します
+
+        """
         return get_user_active_call(self, user_id)
 
     def get_bgms(self) -> List[Bgm]:
+        """
+
+        通話のBGMを取得します
+
+        """
         return get_bgms(self)
 
     def get_call(self, call_id: int) -> ConferenceCall:
+        """
+
+        通話の詳細を取得します
+
+        """
         return get_call(self, call_id)
 
-    def get_call_invitable_users(self, call_id: int, **params) -> UsersByTimestampResponse:
+    def get_call_invitable_users(self, call_id: int, from_timestamp: int = None) -> UsersByTimestampResponse:
         # @Nullable @Query("user[nickname]")
         """
 
-        Parameters:
-        ---------------
-            - from_timestamp: int - (optional)
+        通話に招待可能なユーザーを取得します
 
         """
-        return UsersByTimestampResponse(self, call_id, **params)
+        return UsersByTimestampResponse(self, call_id, from_timestamp)
 
     def get_call_status(self, opponent_id: int) -> CallStatusResponse:
+        """
+
+        通話の状態を取得します
+
+        """
         return get_call_status(self, opponent_id)
 
     def get_games(self, **params) -> GamesResponse:
         """
 
-        Parameters:
-        ---------------
+        ゲームを取得します
+
+        Parameters
+        ----------
             - number: int - (optional)
             - ids: List[int] - (optional)
             - from_id: int - (optional)
 
         """
         return get_games(self, **params)
 
     def get_genres(self, **params) -> GenresResponse:
         """
 
-        Parameters:
-        ---------------
+        ジャンルを取得します
+
+        Parameters
+        ----------
             - number: int - (optional)
             - from: int - (optional)
 
         """
         return get_genres(self, **params)
 
     def get_group_calls(self, **params) -> PostsResponse:
+        """
+
+        サークルの通話を取得します
+
+        Parameters
+        ----------
+            - number: int - (optional)
+            - group_category_id: int - (optional)
+            - from_timestamp: int - (optional)
+            - scope: str - (optional)
+
+        """
         return get_group_calls(self, **params)
 
-    def invite_to_call_bulk(self, call_id: int, group_id: int = None):
+    def invite_to_call_bulk(self, call_id: int, group_id: int = None) -> dict:
         """
 
-        Parameters:
-        ---------------
+        Parameters
+        ----------
             - call_id: int - (required)
             - group_id: int - (optional)
 
         """
         return invite_to_call_bulk(self, call_id, group_id)
 
-    def invite_users_to_call(self, call_id: int, user_ids: List[int]):
+    def invite_users_to_call(self, call_id: int, user_ids: List[int]) -> dict:
         """
 
-        Parameters:
-        ---------------
+        ユーザーを通話に招待します
+
+        Parameters
+        ----------
             - call_id: int - (required)
             - user_ids: List[int] - (required)
 
         """
         return invite_users_to_call(self, call_id, user_ids)
 
     def invite_users_to_chat_call(
             self,
             chat_room_id: int,
             room_id: int,
             room_url: str
-    ):
+    ) -> dict:
+        """
+
+        チャット通話にユーザーを招待します
+
+        Parameters
+        ----------
+
+            - chat_room_id: int - (required)
+            - room_id: int - (required)
+            - room_url: int - (required)
+
+        """
         return invite_users_to_chat_call(self, chat_room_id, room_id, room_url)
 
-    def kick_and_ban_from_call(self, call_id: int, user_id: int):
+    def kick_and_ban_from_call(self, call_id: int, user_id: int) -> dict:
+        """
+
+        ユーザーを通話からキックします
+
+        Parameters
+        ----------
+
+            - call_id: int - (required)
+            - user_id: int - (required)
+
+        """
         return kick_and_ban_from_call(self, call_id, user_id)
 
     def notify_anonymous_user_leave_agora_channel(
             self,
             conference_id: int,
             agora_uid: str
-    ):
+    ) -> dict:
+        """
+
+        匿名ユーザーが通話から退出したことを通知します
+
+        """
         return notify_anonymous_user_leave_agora_channel(
             self, conference_id, agora_uid
         )
 
-    def notify_user_leave_agora_channel(self, conference_id: int, user_id: int):
+    def notify_user_leave_agora_channel(self, conference_id: int, user_id: int) -> dict:
+        """
+
+        ユーザーが通話から退出したことを通知します
+
+        """
         return notify_user_leave_agora_channel(self, conference_id, user_id)
 
     def send_call_screenshot(
             self,
             screenshot_filename: str,
             conference_id: int
-    ):
+    ) -> dict:
+        """
+
+        通話のスクリーンショットを送信します
+
+        """
         return send_call_screenshot(self, screenshot_filename, conference_id)
 
     def set_call(
             self,
             call_id: int,
             joinable_by: str,
             game_title: str = None,
             category_id: str = None
-    ):
+    ) -> dict:
+        """
+
+        通話を開始します
+
+        """
         return set_call(self, call_id, joinable_by, game_title, category_id)
 
     def set_user_role(
             self,
             call_id: int,
             user_id: int,
             role: str
-    ):
+    ) -> dict:
+        """
+
+        通話に参加中ののユーザーに役職を与えます
+
+        """
         return set_user_role(self, call_id, user_id, role)
 
     def start_call(
             self,
             conference_id: int,
             call_sid: str
     ) -> ConferenceCall:
+        """
+
+        通話に参加します
+
+        """
         return start_call(self, conference_id, call_sid)
 
     def stop_call(
             self,
             conference_id: int,
             call_sid: str
-    ):
+    ) -> dict:
+        """
+
+        通話から退出します
+
+        """
         return stop_call(self, conference_id, call_sid)
 
     # -CASSANDRA
 
     def get_user_activities(self, **params) -> ActivitiesResponse:
         """
 
-        Parameters:
-        ---------------
+        通知を取得します
+
+        Parameters
+        ----------
             - important: bool - (required)
             - from_timestamp: int - (optional)
             - number: int - (optional)
 
         """
         return get_user_activities(self, **params)
 
-    def get_user_merged_activities(self, from_timestamp: int = None) -> ActivitiesResponse:
-        return get_user_merged_activities(self, from_timestamp)
+    def get_user_merged_activities(self, **params) -> ActivitiesResponse:
+        """
+
+        全種類の通知を取得します
 
-    def received_notification(self, pid: str, type: str, opened_at: int = None):
+        Parameters
+        ----------
+
+            - from_timestamp: int - (optional)
+            - number: int - (optional)
+
+        """
+        return get_user_merged_activities(self, **params)
+
+    def received_notification(self, pid: str, type: str, opened_at: int = None) -> dict:
         return received_notification(self, pid, type, opened_at)
 
     # -CHAT
 
-    def accept_request(self, chat_room_ids: List[int]):
-        return accept_request(self, chat_room_ids)
+    def accept_chat_request(self, chat_room_ids: List[int]) -> dict:
+        """
+
+        チャットリクエストを承認します
+
+        Parameters
+        ----------
+
+            - chat_room_ids: List[int] - (required)
+
+        """
+        return accept_chat_request(self, chat_room_ids)
 
     def check_unread_status(self, from_time: int) -> UnreadStatusResponse:
+        """
+
+        チャットの未読ステータスを確認します
+
+        """
         return check_unread_status(self, from_time)
 
     def create_group_chat(
             self,
             name: str,
             with_user_ids: List[int],
             icon_filename: str = None,
             background_filename: str = None
     ) -> CreateChatRoomResponse:
+        """
+
+        グループチャットを作成します
+
+        Parameters
+        ----------
+
+            - name: str - (required)
+            - with_user_ids: List[int] - (required)
+            - chat_room_ids: List[int] - (required)
+            - icon_filename: str - (optional)
+            - background_filename: str - (optional)
+
+        """
         return create_group_chat(
             self,
             name,
             with_user_ids,
             icon_filename,
             background_filename
         )
 
     def create_private_chat(
             self,
             with_user_id: int,
             matching_id: int = None,
             hima_chat: bool = False
     ) -> CreateChatRoomResponse:
+        """
+
+        個人チャットを作成します
+
+        Parameters
+        ----------
+
+            - with_user_ids: List[int] - (required)
+            - matching_id: str - (optional)
+            - hima_chat: bool - (optional)
+
+        """
         return create_private_chat(
             self,
             with_user_id,
             matching_id,
             hima_chat
         )
 
-    def delete_background(self, room_id: int):
+    def delete_background(self, room_id: int) -> dict:
+        """
+
+        チャットの背景画像を削除します
+
+        Parameters
+        ----------
+
+            - room_id: int - (required)
+
+        """
         return delete_background(self, room_id)
 
-    def delete_message(self, room_id: int, message_id: int):
+    def delete_message(self, room_id: int, message_id: int) -> dict:
+        """
+
+        メッセージを削除します
+
+        Parameters
+        ----------
+
+            - room_id: int - (required)
+            - message_id: int - (required)
+
+        """
         return delete_message(self, room_id, message_id)
 
     def edit_chat_room(
             self,
             chat_room_id: int,
             name: str,
             icon_filename: str = None,
             background_filename: str = None
-    ):
+    ) -> dict:
+        """
+
+        チャットルームを編集します
+
+        """
         return edit_chat_room(
             self,
             chat_room_id,
             name,
             icon_filename,
             background_filename
         )
 
     def get_chatable_users(
             self,
             from_follow_id: int = None,
             from_timestamp: int = None,
             order_by: str = None
     ) -> FollowUsersResponse:
+        """
+
+        チャット可能なユーザーを取得します
+
+        """
         return get_chatable_users(from_follow_id, from_timestamp, order_by)
 
     def get_gifs_data(self) -> List[GifImageCategory]:
+        """
+
+        チャットルームのGIFデータを取得します
+
+        """
         return get_gifs_data(self)
 
     def get_hidden_chat_rooms(self, **params) -> ChatRoomsResponse:
         """
 
-        Parameters:
-        ---------------
+        非表示のチャットルームを取得します
+
+        Parameters
+        ----------
 
             - from_timestamp: int - (optional)
             - number: int - (optional)
 
         """
         return get_hidden_chat_rooms(self, **params)
 
     def get_main_chat_rooms(self, from_timestamp: int = None) -> ChatRoomsResponse:
+        """
+
+        メインのチャットルームを取得します
+
+        """
         return get_main_chat_rooms(self, from_timestamp)
 
     def get_messages(self, chat_room_id: int, **params) -> List[Message]:
         """
 
-        Parameters:
+        メッセージを取得します
+
+        Parameters
         ---------------
             - from_message_id: int - (optional)
             - to_message_id: int - (optional)
 
         """
         return get_messages(self, chat_room_id, **params)
 
     # def get_notification_settings(self, chat_room_id: int) -> Settings:
     #     return get_notification_settings(self, chat_room_id)
 
     def get_request_chat_rooms(self, from_timestamp: int = None) -> ChatRoomsResponse:
+        """
+
+        チャットリクエストを取得します
+
+        """
         return get_request_chat_rooms(self, from_timestamp)
 
     def get_chat_room(self, chat_room_id: int) -> ChatRoom:
+        """
+
+        チャットルームの詳細を取得します
+
+        """
         return get_chat_room(self, chat_room_id)
 
     def get_sticker_packs(self) -> List[StickerPack]:
+        """
+
+        スタンプを取得します
+
+        """
         return get_sticker_packs(self)
 
     def get_total_chat_requests(self) -> int:
+        """
+
+        チャットリクエストの数を取得します
+
+        """
         return get_total_chat_requests(self)
 
-    def hide_chat(self, chat_room_id: int):
+    def hide_chat(self, chat_room_id: int) -> dict:
+        """
+
+        チャットルームを非表示にします
+
+        """
         return hide_chat(self, chat_room_id)
 
-    def invite_to_chat(self, chat_room_id: int, user_ids: List[int]):
+    def invite_to_chat(self, chat_room_id: int, user_ids: List[int]) -> dict:
+        """
+
+        チャットルームにユーザーを招待します
+
+        """
         return invite_to_chat(self, chat_room_id, user_ids)
 
-    def kick_users_from_chat(self, chat_room_id: int, user_ids: List[int]):
+    def kick_users_from_chat(self, chat_room_id: int, user_ids: List[int]) -> dict:
+        """
+
+        チャットルームからユーザーを追放します
+
+        """
         return kick_users_from_chat(self, chat_room_id, user_ids)
 
-    def pin_chat(self, room_id: int):
+    def pin_chat(self, room_id: int) -> dict:
+        """
+
+        チャットルームをピン止めします
+
+        """
         return pin_chat(self, room_id)
 
     def read_attachment(
             self,
             room_id: int,
             attachment_msg_ids: List[int]
-    ):
+    ) -> dict:
+        """
+
+        アタッチメントを既読にします
+
+        """
         # TODO: check if this works
         return read_attachment(self, room_id, attachment_msg_ids)
 
-    def read_message(self, chat_room_id: int, message_id: int):
+    def read_message(self, chat_room_id: int, message_id: int) -> dict:
+        """
+
+        メッセージを既読にします
+
+        """
         return read_message(self, chat_room_id, message_id)
 
     def read_video_message(
             self,
             room_id: int,
             video_msg_ids: List[int]
-    ):
+    ) -> dict:
+        """
+
+        動画のメッセージを既読にします
+
+        """
         return read_video_message(self, room_id, video_msg_ids)
 
     def refresh_chat_rooms(self, from_time: int = None) -> ChatRoomsResponse:
+        """
+
+        チャットルームを更新します
+
+        """
         return refresh_chat_rooms(self, from_time)
 
-    def remove_chat_rooms(self, chat_room_ids: List[int]):
+    def remove_chat_rooms(self, chat_room_ids: List[int]) -> dict:
+        """
+
+        チャットルームを削除します
+
+        """
         return remove_chat_rooms(self, chat_room_ids)
 
     def report_chat_room(
         self,
         chat_room_id: int,
         opponent_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None
-    ):
+    ) -> dict:
+        """
+
+        チャットルームを通報します
+
+        """
         return report_chat_room(
             self,
             chat_room_id,
             opponent_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename
         )
 
-    def send_media_screenshot_notification(self, room_id: int):
+    def send_media_screenshot_notification(self, room_id: int) -> dict:
+        """
+
+        スクリーンショットを通知します
+
+        """
         return send_media_screenshot_notification(self, room_id)
 
     def send_message(
             self,
             chat_room_id: int,
             message_type: str,
             call_type: str = None,
             text: str = None,
             font_size: int = None,
             gif_image_id: int = None,
             attachment_file_name: str = None,
             sticker_pack_id: int = None,
             video_file_name: str = None
     ) -> MessageResponse:
+        """
+
+        チャットルームにメッセージを送信します
+
+        """
         return send_message(
             self,
             chat_room_id,
             message_type,
             call_type,
             text,
             font_size,
@@ -388,38 +686,78 @@
     # def set_notification_settings(
     #     self,
     #     chat_room_id: int,
     #     notification_chat: int
     # ) -> Settings:
     #     return set_notification_settings(self)
 
-    def unhide_chat(self, chat_room_ids: int):
+    def unhide_chat(self, chat_room_ids: int) -> dict:
+        """
+
+        チャットの非表示を解除します
+
+        """
         return unhide_chat(self, chat_room_ids)
 
-    def unpin_chat(self, chat_room_id: int):
+    def unpin_chat(self, chat_room_id: int) -> dict:
+        """
+
+        チャットルームのピン止めを解除します
+
+        """
         return unpin_chat(self, chat_room_id)
 
     # -GROUP
 
-    def accept_moderator_offer(self, group_id: int):
+    def accept_moderator_offer(self, group_id: int) -> dict:
+        """
+
+        グループ副管理人の権限オファーを引き受けます
+
+        """
         return accept_moderator_offer(self, group_id)
 
-    def accept_ownership_offer(self, group_id: int):
+    def accept_ownership_offer(self, group_id: int) -> dict:
+        """
+
+        グループ管理人の権限オファーを引き受けます
+
+        """
         return accept_ownership_offer(self, group_id)
 
-    def accept_group_join_request(self, group_id: int, user_id: int):
+    def accept_group_join_request(self, group_id: int, user_id: int) -> dict:
+        """
+
+        グループ参加リクエストを承認します
+
+        """
         return accept_group_join_request(self, group_id, user_id)
 
-    def add_related_groups(self, group_id: int, related_group_id: List[int]):
+    def add_related_groups(self, group_id: int, related_group_id: List[int]) -> dict:
+        """
+
+        関連グループを追加します
+
+        """
         return add_related_groups(self, group_id, related_group_id)
 
-    def ban_group_user(self, group_id: int, user_id: int):
+    def ban_group_user(self, group_id: int, user_id: int) -> dict:
+        """
+
+        グループからユーザーを追放します
+
+        """
         return ban_group_user(self, group_id, user_id)
 
     def check_unread_status(self, from_time: int = None) -> UnreadStatusResponse:
+        """
+
+        グループの未読ステータスを取得します
+
+        """
         return check_unread_status(self, from_time)
 
     def create_group(
             self,
             topic: str,
             description: str = None,
             secret: bool = None,
@@ -437,14 +775,19 @@
             cover_image_filename: str = None,
             sub_category_id: str = None,
             hide_from_game_eight: bool = None,
             allow_members_to_post_media: bool = None,
             allow_members_to_post_url: bool = None,
             guidelines: str = None,
     ) -> CreateGroupResponse:
+        """
+
+        グループを作成します
+
+        """
         return create_group(
             self,
             topic,
             description,
             secret,
             hide_reported_posts,
             hide_conference_call,
@@ -460,210 +803,334 @@
             sub_category_id,
             hide_from_game_eight,
             allow_members_to_post_media,
             allow_members_to_post_url,
             guidelines
         )
 
-    def create_pin_group(self, group_id: int):
+    def create_pin_group(self, group_id: int) -> dict:
+        """
+
+        グループの投稿をピンします
+
+        """
         return create_pin_group(self, group_id)
 
-    def decline_moderator_offer(self, group_id: int):
+    def decline_moderator_offer(self, group_id: int) -> dict:
+        """
+
+        グループ副管理人の権限オファーを断ります
+
+        """
         return decline_moderator_offer(self, group_id)
 
-    def decline_ownership_offer(self, group_id: int):
+    def decline_ownership_offer(self, group_id: int) -> dict:
+        """
+
+        グループ管理人の権限オファーを断ります
+
+        """
         return decline_ownership_offer(self, group_id)
 
-    def decline_group_join_request(self, group_id: int, user_id: int):
+    def decline_group_join_request(self, group_id: int, user_id: int) -> dict:
+        """
+
+        グループ参加リクエストを断ります
+
+        """
         return decline_ownership_offer(self, group_id, user_id)
 
-    def delete_pin_group(self, group_id: int):
+    def delete_pin_group(self, group_id: int) -> dict:
+        """
+
+        グループのピン投稿を解除します
+
+        """
         return delete_pin_group(self, group_id)
 
     def get_banned_group_members(self, group_id: int, page: int = None) -> UsersResponse:
+        """
+
+        追放されたグループメンバーを取得します
+
+        """
         return get_banned_group_members(self, group_id, page)
 
     def get_group_categories(self, **params) -> GroupCategoriesResponse:
         """
 
-        Parameters:
+        グループのカテゴリーを取得します
+
+        Parameters
         ----------
 
             - page: int - (optional)
             - number: int - (optional)
 
         """
         return get_group_categories(self, **params)
 
     def get_create_group_quota(self) -> CreateGroupQuota:
+        """
+
+        グループ作成可能な割当量を取得します
+
+        """
         return get_create_group_quota(self)
 
     def get_group(self, group_id: int) -> GroupResponse:
+        """
+
+        グループの詳細を取得します
+
+        """
         return get_group(self, group_id)
 
     # def get_group_notification_settings(self, group_id: int) -> GroupNotificationSettingsResponse:
     #     return get_group_notification_settings(self, group_id)
 
     def get_groups(self, **params) -> GroupsResponse:
         """
 
-        Parameters:
+        複数のグループの詳細を取得します
+
+        Parameters
         ----------
 
             - group_category_id: int = None
             - keyword: str = None
             - from_timestamp: int = None
             - sub_category_id: int = None
 
         """
         return get_groups(self, **params)
 
     def get_invitable_users(self, group_id: int, **params) -> UsersByTimestampResponse:
         """
 
-        Parameters:
+        グループに招待可能なユーザーを取得します
+
+        Parameters
         ----------
 
             - from_timestamp: int - (optional)
             - user[nickname]: str - (optional)
 
         """
         return get_invitable_users(self, group_id, **params)
 
     def get_joined_statuses(self, ids: List[int]) -> dict:
         return get_joined_statuses(self, ids)
 
     def get_group_member(self, group_id: int, user_id: int) -> GroupUserResponse:
+        """
+
+        特定のグループメンバーの情報を取得します
+
+        """
         return get_group_member(self, group_id, user_id)
 
     def get_group_members(self, group_id: int, **params) -> GroupUsersResponse:
         """
 
-        Parameters:
+        グループメンバーを取得します
+
+        Parameters
         ----------
 
             - id: int - (required)
             - mode: str - (optional)
             - keyword: str - (optional)
             - from_id: int - (optional)
             - from_timestamp: int - (optional)
             - order_by: str - (optional)
             - followed_by_me: bool - (optional)
 
         """
         return get_group_members(self, group_id, **params)
 
     def get_my_groups(self, from_timestamp: None) -> GroupsResponse:
+        """
+
+        自分のグループを取得します
+
+        """
         return get_my_groups(self, from_timestamp)
 
     def get_relatable_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
         """
 
-        Parameters:
+        関連がある可能性があるグループを取得します
+
+        Parameters
         ----------
 
             - group_id: int - (required)
             - keyword: str - (optional)
             - from: str - (optional)
 
         """
         return get_relatable_groups(self, group_id, **params)
 
     def get_related_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
         """
 
-        Parameters:
+        関連があるグループを取得します
+
+        Parameters
         ----------
 
             - group_id: int - (required)
             - keyword: str - (optional)
             - from: str - (optional)
 
         """
         return get_related_groups(self, group_id, **params)
 
     def get_user_groups(self, **params) -> GroupsResponse:
         """
 
-        Parameters:
+        特定のユーザーが参加しているグループを取得します
+
+        Parameters
         ----------
 
             - user_id: int - (required)
             - page: int - (optional)
 
         """
         return get_user_groups(self, **params)
 
-    def invite_users_to_group(self, group_id: int, user_ids: List[int]):
+    def invite_users_to_group(self, group_id: int, user_ids: List[int]) -> dict:
+        """
+
+        グループにユーザーを招待します
+
+        """
         return invite_users_to_group(self, group_id, user_ids)
 
-    def join_group(self, group_id: int):
+    def join_group(self, group_id: int) -> dict:
+        """
+
+        グループに参加します
+
+        """
         return join_group(self, group_id)
 
-    def leave_group(self, group_id: int):
+    def leave_group(self, group_id: int) -> dict:
+        """
+
+        グループから脱退します
+
+        """
         return leave_group(self, group_id)
 
-    def post_gruop_social_shared(self, group_id: int, sns_name: str):
+    def post_gruop_social_shared(self, group_id: int, sns_name: str) -> dict:
         return post_gruop_social_shared(self, group_id, sns_name)
 
-    def remove_group_cover(self, group_id: int):
+    def remove_group_cover(self, group_id: int) -> dict:
+        """
+
+        グループのカバー画像を削除します
+
+        """
         return remove_group_cover(self, group_id)
 
-    def remove_moderator(self, group_id: int, user_id: int):
+    def remove_moderator(self, group_id: int, user_id: int) -> dict:
+        """
+
+        グループの副管理人を削除します
+
+        """
         return remove_moderator(self, group_id, user_id)
 
-    def remove_related_groups(self, group_id: int, related_group_ids: List[int]):
+    def remove_related_groups(self, group_id: int, related_group_ids: List[int]) -> dict:
+        """
+
+        関連のあるグループを削除します
+
+        """
         return remove_related_groups(self, group_id, related_group_ids)
 
     def report_group(
             self,
             group_id: int,
             category_id: int,
             reason: str = None,
             opponent_id: int = None,
             screenshot_filename: str = None,
             screenshot_2_filename: str = None,
             screenshot_3_filename: str = None,
             screenshot_4_filename: str = None,
-    ):
+    ) -> dict:
+        """
+
+        グループを通報します
+
+        """
         return report_group(
             self,
             group_id,
             category_id,
             reason,
             opponent_id,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename
         )
 
-    def send_moderator_offers(self, group_id: int, user_ids: List[int]):
+    def send_moderator_offers(self, group_id: int, user_ids: List[int]) -> dict:
+        """
+
+        複数人に副管理人のオファーを送信します
+
+        """
         return send_moderator_offers(self, group_id, user_ids)
 
-    def send_ownership_offer(self, group_id: int, user_id: int):
+    def send_ownership_offer(self, group_id: int, user_id: int) -> dict:
+        """
+
+        グループ管理人権限のオファーを送信します
+
+        """
         return send_ownership_offer(self, group_id, user_id)
 
     # def set_group_notification_settings(
     #         self,
     #         group_id: int,
     #         notification_group_post: int = None,
     #         notification_group_join: int = None,
     #         notification_group_request: int = None,
     #         notification_group_message_tag_all: int = None,
     # ) -> AdditionalSettingsResponse:
     #     return set_group_notification_settings(self)
 
-    def set_group_title(self, group_id: int, title: str):
+    def set_group_title(self, group_id: int, title: str) -> dict:
+        """
+
+        グループのタイトルを設定します
+
+        """
         return set_group_title(self, group_id, title)
 
-    def take_over_group_ownership(self, group_id: int):
+    def take_over_group_ownership(self, group_id: int) -> dict:
+        """
+
+        グループ管理人の権限を引き継ぎます
+
+        """
         return take_over_group_ownership(self, group_id)
 
-    def unban_group_member(self, group_id: int, user_id: int):
+    def unban_group_member(self, group_id: int, user_id: int) -> dict:
+        """
+
+        特定のグループメンバーの追放を解除します
+
+        """
         return unban_group_member(self, group_id, user_id)
 
     def update_group(
             self,
             group_id: int,
             topic: str,
             description: str = None,
@@ -682,14 +1149,19 @@
             cover_image_filename: str = None,
             sub_category_id: str = None,
             hide_from_game_eight: bool = None,
             allow_members_to_post_media: bool = None,
             allow_members_to_post_url: bool = None,
             guidelines: str = None,
     ) -> GroupResponse:
+        """
+
+        グループを編集します
+
+        """
         return update_group(
             group_id,
             topic,
             description,
             secret,
             hide_reported_posts,
             hide_conference_call,
@@ -706,177 +1178,274 @@
             sub_category_id,
             hide_from_game_eight,
             allow_members_to_post_media,
             allow_members_to_post_url,
             guidelines,
         )
 
-    def visit_group(self, group_id: int):
+    def visit_group(self, group_id: int) -> dict:
+        """
+
+        グループを訪問します
+
+        """
         return visit_group(self, group_id)
 
-    def withdraw_moderator_offer(self, group_id: int, user_id: int):
+    def withdraw_moderator_offer(self, group_id: int, user_id: int) -> dict:
+        """
+
+        グループ副管理人のオファーを取り消します
+
+        """
         return withdraw_moderator_offer(self, group_id, user_id)
 
-    def withdraw_ownership_offer(self, group_id: int, user_id: int):
+    def withdraw_ownership_offer(self, group_id: int, user_id: int) -> dict:
+        """
+
+        グループ管理人のオファーを取り消します
+
+        """
         return withdraw_ownership_offer(self, group_id, user_id)
 
     # -LOGIN
 
     def change_email(
             self,
             email: str,
             password: str,
             email_grant_token: str = None
     ) -> LoginUpdateResponse:
+        """
+
+        メールアドレスを変更します
+
+        """
         return change_email(self, email, password, email_grant_token)
 
     def change_password(
             self,
             current_password: str,
             new_password: str
     ) -> LoginUpdateResponse:
+        """
+
+        パスワードを変更します
+
+        """
         return change_password(self, current_password, new_password)
 
-    # def connect_account_with_sns(self):
+    # def connect_account_with_sns(self) -> dict:
     #     return connect_account_with_sns(self)
 
-    # def disconnect_account_with_sns(self):
+    # def disconnect_account_with_sns(self) -> dict:
     #     return disconnect_account_with_sns(self)
 
     def get_token(
             self,
             grant_type: str,
             refresh_token: str = None,
             email: str = None,
             password: str = None
     ) -> TokenResponse:
+        """
+
+        トークンを再取得します
+
+        """
         return get_token(
             self,
             grant_type,
             refresh_token,
             email,
             password
         )
 
-    def login_with_email(self, email: str, password: str) -> LoginUserResponse:
-        return login_with_email(self, email, password)
+    def login(self, email: str, password: str) -> LoginUserResponse:
+        """
+
+        メールアドレスでログインします
+
+        """
+        return login(self, email, password)
 
-    # def login_with_sns(self):
+    # def login_with_sns(self) -> dict:
     #     return login_with_sns(self)
 
-    def logout(self):
+    def logout(self) -> dict:
+        """
+
+        ログアウトします
+
+        """
         return logout(self)
 
-    # def migrate_token(self):
+    # def migrate_token(self) -> dict:
     #     return migrate_token(self)
 
-    # def register_device_token(self):
+    # def register_device_token(self) -> dict:
     #     return register_device_token(self)
 
-    def resend_confirm_email(self):
+    def resend_confirm_email(self) -> dict:
         return resend_confirm_email(self)
 
     def restore_user(self, user_id: int) -> LoginUserResponse:
         return restore_user(self, user_id)
 
-    def revoke_tokens(self):
+    def revoke_tokens(self) -> dict:
+        """
+
+        トークンを無効化します
+
+        """
         return revoke_tokens(self)
 
     def save_account_with_email(
             self,
             email: str,
             password: str = None,
             current_password: str = None,
             email_grant_token: str = None
     ) -> LoginUpdateResponse:
+        """
+
+        メールアドレスでアカウントを保存します
+
+        """
         return save_account_with_email(
             self,
             email,
             password,
             current_password,
             email_grant_token,
         )
 
     # -MISC
 
-    def accept_policy_agreement(self, type: str):
+    def accept_policy_agreement(self, type: str) -> dict:
         return accept_policy_agreement(self, type)
 
-    def generate_sns_thumbnail(self, **params):
+    def generate_sns_thumbnail(self, **params) -> dict:
         """
 
-        Parameters:
+        Parameters
         ----------
 
             - resource_type: str - (Required)
             - resource_id: int - (Required)
 
         """
         return generate_sns_thumbnail(self, **params)
 
     def get_email_verification_presigned_url(self, email: str, locale: str, intent: str = None) -> str:
+        """
+
+        メールアドレス確認用の署名付きURLを取得します
+
+        """
         return get_email_verification_presigned_url(self, email, locale, intent)
 
     def get_file_upload_presigned_urls(self, file_names: List[str]) -> List[PresignedUrl]:
+        """
+
+        ファイルアップロード用の署名付きURLを取得します
+
+        """
         return get_file_upload_presigned_urls(self, file_names)
 
     # def get_id_checker_presigned_url(
     #         self,
     #         model: str,
     #         action: str,
     #         **params
     # ) -> str:
     #     return get_id_checker_presigned_url(self, model, action, **params)
 
     def get_old_file_upload_presigned_url(self, video_file_name: str) -> str:
+        """
+
+        ファイルアップロード用の署名付きURLを取得します
+
+        """
         return get_old_file_upload_presigned_url(self, video_file_name)
 
     def get_policy_agreements(self) -> PolicyAgreementsResponse:
         return get_policy_agreements(self)
 
     def get_promotions(self, **params) -> List[Promotion]:
         """
 
-        Parameters:
+        プロモーションを取得します
+
+        Parameters
         ----------
 
             - page: int - (Optional)
             - number: int - (Optional)
 
         """
         return get_promotions(self, **params)
 
     def get_vip_game_reward_url(self, device_type: str) -> str:
         return get_vip_game_reward_url(self, device_type)
 
     def get_web_socket_token(self) -> str:
+        """
+
+        Web Socket Token を取得します
+
+        """
         return get_web_socket_token(self)
 
     def verify_device(
             self,
             app_version: str,
             device_uuid: str,
             platform: str,
             verification_string: str
     ) -> VerifyDeviceResponse:
+        """
+
+        デバイスを検証します
+
+        """
         # TODO: check platform, verification_string
         return verify_device(
             self,
             app_version,
             device_uuid,
             platform,
             verification_string
         )
 
+    def upload_image(self, image_type: str, image_path: str) -> str:
+        """
+
+        画像をアップロードしてattachment_filenameを返します。
+
+        ※ 対応形式: jpeg, png, gif
+
+        Parameteres
+        -----------
+            - image_type: str - (required): "post", "user_avatar" のどちらか
+            - image_path: str - (required): "画像のパス
+
+        """
+        return upload_image(self, image_type, image_path)
+
     # -POST
 
     def add_bookmark(self, user_id: int, post_id: int) -> BookmarkPostResponse:
+        """
+
+        ブックマークに追加します
+
+        """
         return add_bookmark(self, user_id, post_id)
 
-    def add_group_highlight_post(self, group_id: int, post_id: int):
+    def add_group_highlight_post(self, group_id: int, post_id: int) -> dict:
         return add_group_highlight_post(self, group_id, post_id)
 
     def create_call_post(
             self,
             text: str = None,
             font_size: int = None,
             color: int = None,
@@ -892,14 +1461,19 @@
             attachment_4_filename: str = None,
             attachment_5_filename: str = None,
             attachment_6_filename: str = None,
             attachment_7_filename: str = None,
             attachment_8_filename: str = None,
             attachment_9_filename: str = None,
     ) -> ConferenceCall:
+        """
+
+        通話の投稿を作成します
+
+        """
         return create_call_post(
             self,
             text,
             font_size,
             color,
             group_id,
             call_type,
@@ -914,31 +1488,45 @@
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename
         )
 
-    def create_group_pin_post(self, post_id: int, group_id: int):
+    def create_group_pin_post(self, post_id: int, group_id: int) -> dict:
+        """
+
+        グループの投稿をピンします
+
+        """
         return create_group_pin_post(self, post_id, group_id)
 
-    def create_pin_post(self, post_id: int):
+    def create_pin_post(self, post_id: int) -> dict:
+        """
+
+        投稿をピンします
+
+        """
         return create_pin_post(self, post_id)
 
     def mention(self, user_id: int) -> str:
+        """
+
+        メンション用文字列を返します
+
+        """
         return mention(self, user_id)
 
     def create_post(
             self,
             text: str = None,
             font_size: int = 0,
             color: int = 0,
             in_reply_to: int = None,
             group_id: int = None,
-            post_type: str = None,
             mention_ids: List[int] = None,
             choices: List[str] = None,
             shared_url: Dict[str, str | int] = None,
             message_tags: str = "[]",
             attachment_filename: str = None,
             attachment_2_filename: str = None,
             attachment_3_filename: str = None,
@@ -946,22 +1534,26 @@
             attachment_5_filename: str = None,
             attachment_6_filename: str = None,
             attachment_7_filename: str = None,
             attachment_8_filename: str = None,
             attachment_9_filename: str = None,
             video_file_name: str = None,
     ) -> Post:
+        """
+
+        投稿を作成します
+
+        """
         return create_post(
             self,
             text,
             font_size,
             color,
             in_reply_to,
             group_id,
-            post_type,
             mention_ids,
             choices,
             shared_url,
             message_tags,
             attachment_filename,
             attachment_2_filename,
             attachment_3_filename,
@@ -994,14 +1586,19 @@
             attachment_5_filename: str = None,
             attachment_6_filename: str = None,
             attachment_7_filename: str = None,
             attachment_8_filename: str = None,
             attachment_9_filename: str = None,
             video_file_name: str = None,
     ) -> Post:
+        """
+
+        投稿を(´∀｀∩)↑age↑します
+
+        """
         return create_repost(
             self,
             post_id,
             text,
             font_size,
             color,
             in_reply_to,
@@ -1062,14 +1659,19 @@
             attachment_5_filename: str = None,
             attachment_6_filename: str = None,
             attachment_7_filename: str = None,
             attachment_8_filename: str = None,
             attachment_9_filename: str = None,
             video_file_name: str = None,
     ) -> Post:
+        """
+
+        スレッドの投稿を作成します
+
+        """
         return create_thread_post(
             self,
             post_id,
             text,
             font_size,
             color,
             in_reply_to,
@@ -1087,30 +1689,52 @@
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename,
             video_file_name,
         )
 
-    def delete_all_post(self):
+    def delete_all_post(self) -> dict:
+        """
+
+        すべての投稿を削除します
+
+        """
         return delete_all_post(self)
 
-    def delete_group_pin_post(self, group_id: int):
+    def delete_group_pin_post(self, group_id: int) -> dict:
+        """
+
+        グループのピン投稿を削除します
+
+        """
         return delete_group_pin_post(self, group_id)
 
-    def delete_pin_post(self, post_id: int):
+    def delete_pin_post(self, post_id: int) -> dict:
+        """
+
+        ピン投稿を削除します
+
+        """
         return delete_pin_post(self, post_id)
 
-    def get_bookmark(self, user_id: int, *, from_str: str = None) -> PostsResponse:
+    def get_bookmark(self, user_id: int, from_str: str = None) -> PostsResponse:
+        """
+
+        ブックマークを取得します
+
+        """
         return get_bookmark(self, user_id, from_str)
 
     def get_timeline_calls(self, **params) -> PostsResponse:
         """
 
-        Parameters:
+        誰でも通話を取得します
+
+        Parameters
         ----------
 
             - group_id: int = None
             - from_timestamp: int = None
             - number: int = None
             - category_id: int = None
             - call_type: str = "voice"
@@ -1121,34 +1745,43 @@
 
         """
         return get_timeline_calls(self, **params)
 
     def get_conversation(self, conversation_id: int, **params) -> PostsResponse:
         """
 
-        Parameters:
+        会話を取得します
+
+        Parameters
         ----------
 
             - conversation_id: int
             - group_id: int = None
             - thread_id: int = None
             - from_post_id: int = None
             - number: int = 50
             - reverse: bool = True
 
         """
         return get_conversation(self, conversation_id, **params)
 
     def get_conversation_root_posts(self, post_ids: List[int]) -> PostsResponse:
+        """
+
+        会話の原点の投稿を取得します
+
+        """
         return get_conversation_root_posts(self, post_ids)
 
     def get_following_call_timeline(self, **params) -> PostsResponse:
         """
 
-        Parameters:
+        フォロー中の通話を取得します
+
+        Parameters
         ----------
 
             - from_timestamp: int = None
             - number: int = None
             - category_id: int = None
             - call_type: str = None
             - include_circle_call: bool = None
@@ -1156,15 +1789,17 @@
 
         """
         return get_following_call_timeline(self, **params)
 
     def get_following_timeline(self, **params) -> PostsResponse:
         """
 
-        Parameters:
+        フォロー中のタイムラインを取得します
+
+        Parameters
         ----------
 
             - from_str: str = None
             - only_root: bool = None
             - order_by: str = None
             - number: int = None
             - mxn: int = None
@@ -1173,43 +1808,47 @@
 
         """
         return get_following_timeline(self, **params)
 
     def get_group_highlight_posts(self, group_id: int, **params) -> PostsResponse:
         """
 
-        Parameters:
+        Parameters
         ----------
 
             - group_id: int
             - from_post: int = None
             - number: int = None
 
         """
         return get_group_highlight_posts(self, group_id, **params)
 
     def get_group_timeline_by_keyword(self, group_id: int, keyword: str, **params) -> PostsResponse:
         """
 
-        Parameters:
+        グループの投稿をキーワードで検索します
+
+        Parameters
         ----------
 
             - group_id: int
             - keyword: str
             - from_post_id: int = None
             - number: int = None
             - only_thread_posts: bool = False
 
         """
         return get_group_timeline_by_keyword(self, group_id, keyword, **params)
 
     def get_group_timeline(self, group_id: int, **params) -> PostsResponse:
         """
 
-        Parameters:
+        グループのタイムラインを取得します
+
+        Parameters
         ----------
 
             - group_id: int
             - from_post_id: int
             - reverse: bool
             - post_type: str
             - number: int
@@ -1217,105 +1856,129 @@
 
         """
         return get_group_timeline(self, group_id, **params)
 
     def get_timeline_by_hashtag(self, hashtag: str, **params) -> PostsResponse:
         """
 
-        Parameters:
+        ハッシュタグでタイムラインを検索します
+
+        Parameters
         ----------
 
             - hashtag: str - (required)
             - from_post_id: int - (optional)
             - number: int - (optional)
 
         """
         return get_timeline_by_hashtag(self, hashtag, **params)
 
     def get_my_posts(self, **params) -> PostsResponse:
         """
 
-        Parameters:
-        ---------------
+        自分の投稿を取得します
+
+        Parameters
+        ----------
 
             - from_post_id: int - (optional)
             - number: int - (optional)
             - include_group_post: bool - (optional)
 
         """
         return get_my_posts(self, **params)
 
     def get_post(self, post_id: int) -> Post:
+        """
+
+        投稿の詳細を取得します
+
+        """
         return get_post(self, post_id)
 
     def get_post_likers(self, post_id: int, **params) -> PostLikersResponse:
         """
 
-        Parameters:
-        ---------------
+        投稿にいいねしたユーザーを取得します
+
+        Parameters
+        ----------
 
             - from_id: int - (optional)
             - number: int - (optional)
 
         """
         return get_post_likers(self, post_id, **params)
 
     def get_post_reposts(self, post_id: int, **params: int) -> PostsResponse:
         """
 
-        Parameters:
-        ---------------
+        投稿の(´∀｀∩)↑age↑を取得します
+
+        Parameters
+        ----------
 
             - post_id: int - (required)
             - from_post_id: int - (optional)
             - number: int - (optional)
 
         """
         return get_post_reposts(self, post_id, **params)
 
     def get_posts(self, post_ids: List[int]) -> PostsResponse:
+        """
+
+        複数の投稿を取得します
+
+        """
         return get_posts(self, post_ids)
 
     def get_recommended_post_tags(
         self, tag: str = None, save_recent_search: bool = False
     ) -> PostTagsResponse:
         return get_recommended_post_tags(self, tag, save_recent_search)
 
     def get_recommended_posts(self, **params) -> PostsResponse:
         """
 
-        Parameters:
-        ---------------
+        おすすめの投稿を取得します
+
+        Parameters
+        ----------
 
             - experiment_num: int
             - variant_num: int
             - number: int
 
         """
         return get_recommended_posts(self, **params)
 
     def get_timeline_by_keyword(self, keyword: str = None, **params) -> PostsResponse:
         """
 
-        Parameters:
-        ---------------
+        キーワードでタイムラインを検索します
+
+        Parameters
+        ----------
 
             - keyword: str
             - from_post_id: int
             - number: int
 
         """
         return get_timeline_by_keyword(self, keyword, **params)
 
     def get_timeline(self, **params: int | str | bool) -> PostsResponse:
         # - from: str - (optional)
         """
 
-        Parameters:
-        ---------------
+        タイムラインを取得します
+
+        Parameters
+        ----------
 
             - noreply_mode: bool - (optional)
             - from_post_id: int - (optional)
             - number: int - (optional)
             - order_by: str - (optional)
             - experiment_older_age_rules: bool - (optional)
             - shared_interest_categories: bool - (optional)
@@ -1330,189 +1993,323 @@
 
     def get_url_metadata(self, url: str) -> SharedUrl:
         return get_url_metadata(self, url)
 
     def get_user_timeline(self, user_id: int, **params) -> PostsResponse:
         """
 
-        Parameters:
-        ---------------
+        ユーザーのタイムラインを取得します
+
+        Parameters
+        ----------
 
             - from_post_id: int - (optional)
             - number: int - (optional)
             - post_type: str - (optional)
 
         """
         return get_user_timeline(self, user_id, **params)
 
     def like_posts(self, post_ids: List[int]) -> LikePostsResponse:
+        """
+
+        投稿にいいねします
+
+        """
         return like_posts(self, post_ids)
 
-    def remove_bookmark(self, user_id: int, post_id: int):
+    def remove_bookmark(self, user_id: int, post_id: int) -> dict:
+        """
+
+        ブックマークを削除します
+
+        """
         return remove_bookmark(self, user_id, post_id)
 
-    def remove_group_highlight_post(self, group_id: int, post_id: int):
+    def remove_group_highlight_post(self, group_id: int, post_id: int) -> dict:
         return remove_group_highlight_post(self, group_id, post_id)
 
-    def remove_posts(self, post_ids: List[int]):
+    def remove_posts(self, post_ids: List[int]) -> dict:
+        """
+
+        複数の投稿を削除します
+
+        """
         return remove_posts(self, post_ids)
 
     def report_post(
             self,
             post_id: int,
             opponent_id: int,
             category_id: int,
             reason: str = None,
             screenshot_filename: str = None,
             screenshot_2_filename: str = None,
             screenshot_3_filename: str = None,
             screenshot_4_filename: str = None
-    ):
+    ) -> dict:
+        """
+
+        投稿を通報します
+
+        """
         return report_post(
             self,
             post_id,
             opponent_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename
         )
 
-    def unlike_post(self, post_id: int):
+    def unlike_post(self, post_id: int) -> dict:
+        """
+
+        投稿のいいねを解除します
+
+        """
         return unlike_post(self, post_id)
 
     def update_post(
             self,
             post_id: int,
             text: str = None,
             font_size: int = None,
             color: int = None,
             message_tags: str = "[]",
     ) -> Post:
+        """
+
+        投稿を編集します
+
+        """
         return update_post(
             self, post_id, text, font_size, color, message_tags
         )
 
     def update_recommendation_feedback(
         self, post_id: int, feedback_result: str, *,
         experiment_num: int, variant_num: int,
-    ):
+    ) -> dict:
         return update_recommendation_feedback(
             self, post_id, feedback_result, experiment_num, variant_num
         )
 
     def validate_post(self, text: str, *, group_id: int = None, thread_id: int = None) -> ValidationPostResponse:
         return validate_post(self, text, group_id, thread_id)
 
-    def view_video(self, video_id: int):
+    def view_video(self, video_id: int) -> dict:
+        """
+
+        動画を視聴します
+
+        """
         return view_video(self, video_id)
 
     def vote_survey(self, survey_id: int, choice_id: int) -> Survey:
+        """
+
+        アンケートに投票します
+
+        """
         return vote_survey(self, survey_id, choice_id)
 
     # -REVIEW
 
-    def create_review(self, user_id: int, comment: str):
+    def create_review(self, user_id: int, comment: str) -> dict:
+        """
+
+        レターを送信します
+
+        """
         return create_review(self, user_id, comment)
 
-    def create_reviews(self, user_ids: List[int], comment: str):
+    def create_reviews(self, user_ids: List[int], comment: str) -> dict:
+        """
+
+        複数人にレターを送信します
+
+        """
         return create_reviews(self, user_ids, comment)
 
-    def delete_reviews(self, review_ids: List[int]):
+    def delete_reviews(self, review_ids: List[int]) -> dict:
+        """
+
+        レターを削除します
+
+        """
         return delete_reviews(self, review_ids)
 
-    def get_my_reviews(self, from_id: int = None) -> ReviewsResponse:
-        return get_my_reviews(self, from_id)
+    def get_my_reviews(self, **params) -> ReviewsResponse:
+        """
+
+        送信したレターを取得します
+
+        Parameters
+        ----------
+
+            - from_id: int (optional)
+            - number: int = (optional)
+
+        """
+        return get_my_reviews(self, **params)
+
+    def get_reviews(self, user_id: int, **params) -> ReviewsResponse:
+        """
+
+        受け取ったレターを取得します
+
+        Parameters
+        ----------
+
+            - user_id: int (required)
+            - from_id: int = (optional)
+            - number: int = (optional)
 
-    def get_reviews(self, user_id: int, from_id: int = None) -> ReviewsResponse:
-        return get_reviews(self, user_id, from_id)
+        """
+        return get_reviews(self, user_id, **params)
+
+    def pin_review(self, review_id: int) -> dict:
+        """
 
-    def pin_review(self, review_id: int):
+        レターをピンします
+
+        """
         return pin_review(self, review_id)
 
-    def unpin_review(self, review_id: int):
+    def unpin_review(self, review_id: int) -> dict:
+        """
+
+        レターのピンを解除します
+
+        """
         return unpin_review(self, review_id)
 
     # -THREAD
 
     def add_post_to_thread(self, post_id: int, thread_id: int) -> ThreadInfo:
+        """
+
+        投稿をスレッドに追加します
+
+        """
         return add_post_to_thread(self, post_id, thread_id)
 
     def convert_post_to_thread(
             self,
             post_id: int,
             title: str = None,
             thread_icon_filename: str = None
     ) -> ThreadInfo:
+        """
+
+        投稿をスレッドに変換します
+
+        """
         return convert_post_to_thread(
             self,
             post_id,
             title,
             thread_icon_filename
         )
 
     def create_thread(
             self,
             group_id: int,
             title: str,
             thread_icon_filename: str
     ) -> ThreadInfo:
+        """
+
+        スレッドを作成します
+
+        """
         return create_thread(
             self,
             group_id,
             title,
             thread_icon_filename
         )
 
     def get_group_thread_list(self, group_id: int, from_str: str = None, **params) -> GroupThreadListResponse:
         """
 
-        Parameters:
+        グループのスレッド一覧を取得します
+
+        Parameters
         ----------
 
             - group_id: int
             - from_str: str = None
             - join_status: str = None
 
         """
         return get_group_thread_list(self, group_id, from_str, **params)
 
     def get_thread_joined_statuses(self, ids: List[int]) -> dict:
+        """
+
+        スレッド参加ステータスを取得します
+
+        """
         return get_thread_joined_statuses(self, ids)
 
     def get_thread_posts(self, thread_id: int, from_str: str = None, **params) -> PostsResponse:
         """
 
-        Parameters:
+        スレッドの投稿を取得します
+
+        Parameters
         ----------
 
             - post_type: str
             - number: int = None
             - from_str: str = None
 
         """
         return get_thread_posts(self, thread_id, from_str, **params)
 
-    def join_thread(self, thread_id: int, user_id: int):
+    def join_thread(self, thread_id: int, user_id: int) -> dict:
+        """
+
+        スレッドに参加します
+
+        """
         return join_thread(self, thread_id, user_id)
 
-    def leave_thread(self, thread_id: int, user_id: int):
+    def leave_thread(self, thread_id: int, user_id: int) -> dict:
+        """
+
+        スレッドから脱退します
+
+        """
         return leave_thread(self, thread_id, user_id)
 
-    def remove_thread(self, thread_id: int):
+    def remove_thread(self, thread_id: int) -> dict:
+        """
+
+        スレッドを削除します
+
+        """
         return remove_thread(self, thread_id)
 
     def update_thread(
             self,
             thread_id: int,
             title: str,
             thread_icon_filename: str
-    ):
+    ) -> dict:
+        """
+
+        スレッドを編集します
+
+        """
         return update_thread(
             self,
             thread_id,
             title,
             thread_icon_filename
         )
 
@@ -1532,14 +2329,17 @@
             email: str = None,
             password: str = None,
             email_grant_token: str = None,
             en: int = None,
             vn: int = None
     ) -> CreateUserResponse:
         """
+
+        アカウントを作成します
+
         birth_date: 2000-01-01の形式
         """
         return create_user(
             self,
             nickname,
             birth_date,
             gender,
@@ -1551,33 +2351,58 @@
             email,
             password,
             email_grant_token,
             en,
             vn
         )
 
-    def delete_contact_friends(self):
+    def delete_contact_friends(self) -> dict:
+        """
+
+        連絡先の友人を削除します
+
+        """
         return delete_contact_friends(self)
 
-    def delete_footprint(self, user_id: int, footprint_id: int):
+    def delete_footprint(self, user_id: int, footprint_id: int) -> dict:
+        """
+
+        足跡を削除します
+
+        """
         return delete_footprint(self, user_id, footprint_id)
 
-    def destroy_user(self):
+    def destroy_user(self) -> dict:
+        """
+
+        アカウントを削除します
+
+        """
         return destroy_user(self)
 
-    def follow_user(self, user_id: int):
+    def follow_user(self, user_id: int) -> dict:
+        """
+
+        ユーザーをフォローします
+
+        """
         return follow_user(self, user_id)
 
-    def follow_users(self, user_ids: List[int]):
+    def follow_users(self, user_ids: List[int]) -> dict:
+        """
+
+        複数のユーザーをフォローします
+
+        """
         return follow_users(self, user_ids)
 
     def get_active_followings(self, **params) -> ActiveFollowingsResponse:
         """
 
-        Parameters:
+        Parameters
         ----------
 
             - only_online: bool
             - from_loggedin_at: int = None
 
         """
         return get_active_followings(self, **params)
@@ -1593,37 +2418,51 @@
 
     # def get_default_settings(self) -> TimelineSettings:
     #     return get_default_settings(self)
 
     def get_follow_recommendations(self, **params) -> FollowRecommendationsResponse:
         """
 
-        Parameters:
+        フォローするのにおすすめのユーザーを取得します
+
+        Parameters
         ----------
 
             - from_timestamp: int = None,
             - number: int = None,
             - sources: List[str] = None
 
         """
         return get_follow_recommendations(self, **params)
 
     def get_follow_request(self, from_timestamp: int = None) -> UsersByTimestampResponse:
+        """
+
+        フォローリクエストを取得します
+
+        """
         return get_follow_request(self, from_timestamp)
 
     def get_follow_request_count(self) -> int:
+        """
+
+        フォローリクエストの数を取得します
+
+        """
         return get_follow_request_count(self)
 
     def get_following_users_born(self, birthdate: int = None) -> UsersResponse:
         return get_following_users_born(self, birthdate)
 
     def get_footprints(self, **params) -> List[Footprint]:
         """
 
-        Parameters:
+        足跡を取得します
+
+        Parameters
         ----------
 
             - from_id: int = None
             - number: int = None
             - mode: str = None
 
         """
@@ -1631,15 +2470,17 @@
 
     def get_fresh_user(self, user_id: int) -> UserResponse:
         return get_fresh_user(self, user_id)
 
     def get_hima_users(self, **params) -> List[UserWrapper]:
         """
 
-        Parameters:
+        暇なユーザーを取得する
+
+        Parameters
         ----------
 
             - from_hima_id: int = None
             - number: int = None
 
         """
         return get_hima_users(self, **params)
@@ -1648,15 +2489,15 @@
         return get_initial_recommended_users_to_follow(self, **params)
 
     def get_recommended_users_to_follow_for_profile(
             self, user_id: int, **params
     ) -> UsersResponse:
         """
 
-        Parameters:
+        Parameters
         ----------
 
             - user_id: int - (Required)
             - number: int - (Optional)
             - page: int - (Optional)
 
         """
@@ -1666,137 +2507,203 @@
 
     def get_refresh_counter_requests(self) -> RefreshCounterRequestsResponse:
         return get_refresh_counter_requests(self)
 
     def get_social_shared_users(self, **params) -> SocialShareUsersResponse:
         """
 
-        Parameters:
+        Parameters
         ----------
 
             - sns_name: str - (Required)
             - number: int - (Optional)
             - from_id: int - (Optional)
 
         """
         return get_social_shared_users(self, **params)
 
     def get_timestamp(self) -> UserTimestampResponse:
+        """
+
+        タイムスタンプを取得します
+
+        """
         return get_timestamp(self)
 
     def get_user(self, user_id: int) -> User:
+        """
+
+        ユーザーの情報を取得します
+
+        """
         return get_user(self, user_id)
 
     def get_user_custom_definitions(self) -> UserCustomDefinitionsResponse:
         return get_user_custom_definitions(self)
 
     def get_user_email(self, user_id: int) -> str:
+        """
+
+        ユーザーのメールアドレスを取得します
+
+        """
         return get_user_email(self, user_id)
 
     def get_user_followers(self, user_id: int, **params) -> FollowUsersResponse:
         """
 
-        Parameters:
+        ユーザーのフォロワーを取得します
+
+        Parameters
         ----------
 
             - user_id: int
             - from_follow_id: int = None
             - followed_by_me: int = None
 
         """
         return get_user_followers(self, user_id, **params)
 
     def get_user_followings(self, user_id: int, **params) -> FollowUsersResponse:
         """
 
-        Parameters:
+        フォロー中のユーザーを取得します
+
+        Parameters
         ----------
 
             - user_id: int
             - from_follow_id: int = None
             - from_timestamp: int = None
             - order_by: str = None
 
         """
         return get_user_followings(self, user_id, **params)
 
     def get_user_from_qr(self, qr: str) -> UserResponse:
+        """
+
+        QRコードからユーザーを取得します
+
+        """
         return get_user_from_qr(self, qr)
 
-    # def get_user_interests(self):
+    # def get_user_interests(self) -> dict:
     #     return get_user_interests(self)
 
     def get_user_without_leaving_footprint(self, user_id: int) -> UserResponse:
+        """
+        ユーザーの情報を取得します
+        """
         return get_user_without_leaving_footprint(self, user_id)
 
     def get_users(self, user_ids: List[int]) -> UsersResponse:
+        """
+
+        複数のユーザーの情報を取得します
+
+        """
         return get_users(self, user_ids)
 
     def get_users_from_uuid(self, uuid: str) -> UsersResponse:
+        """
+
+        UUIDからユーザーを取得します
+
+        """
         return get_users_from_uuid(self, uuid)
 
-    def post_social_shared(self, sns_name: str):
+    def post_social_shared(self, sns_name: str) -> dict:
         return post_social_shared(self, sns_name)
 
-    def record_app_review_status(self):
+    def record_app_review_status(self) -> dict:
         return record_app_review_status(self)
 
-    def reduce_kenta_penalty(self, user_id: int):
+    def reduce_kenta_penalty(self, user_id: int) -> dict:
+        """
+
+        ペナルティーを緩和します
+
+        """
         return reduce_kenta_penalty(self, user_id)
 
-    def refresh_counter(self, counter: str):
+    def refresh_counter(self, counter: str) -> dict:
         return refresh_counter(self, counter)
 
-    def remove_user_avatar(self):
+    def remove_user_avatar(self) -> dict:
+        """
+
+        ユーザーのアイコンを削除します
+
+        """
         return remove_user_avatar(self)
 
-    def remove_user_cover(self):
+    def remove_user_cover(self) -> dict:
+        """
+
+        ユーザーのカバー画像を削除します
+
+        """
         return remove_user_cover(self)
 
     def report_user(
             self,
             user_id: int,
             category_id: int,
             reason: str = None,
             screenshot_filename: str = None,
             screenshot_2_filename: str = None,
             screenshot_3_filename: str = None,
             screenshot_4_filename: str = None
-    ):
+    ) -> dict:
+        """
+
+        ユーザーを通報します
+
+        """
         return report_user(
             self,
             user_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename
         )
 
-    def reset_password(self, email: str, email_grant_token: str, password: str):
+    def reset_password(self, email: str, email_grant_token: str, password: str) -> dict:
+        """
+
+        パスワードをリセットします
+
+        """
         return reset_password(self, email, email_grant_token, password)
 
     def search_lobi_users(self, **params) -> UsersResponse:
         """
 
-        Parameters:
+        Lobiのユーザーを検索します
+
+        Parameters
         ----------
 
             - nickname: str = None
             - number: int = None
             - from_str: str = None
 
         """
         return search_lobi_users(self ** params)
 
     def search_users(self, **params) -> UsersResponse:
         """
 
-        Parameters:
+        ユーザーを検索します
+
+        Parameters
         ----------
 
             - gender: int = None
             - nickname: str = None
             - title: str = None
             - biography: str = None
             - from_timestamp: int = None
@@ -1805,87 +2712,139 @@
             - recently_created: bool = None
             - same_prefecture: bool = None
             - save_recent_search: bool = None
 
         """
         return search_users(self, **params)
 
-    def set_additional_setting_enabled(self, mode: str, on: int = None):
+    def set_additional_setting_enabled(self, mode: str, on: int = None) -> dict:
         return set_additional_setting_enabled(self, mode, on)
 
     def set_follow_permission_enabled(
             self, nickname: str, is_private: bool = None
-    ):
+    ) -> dict:
         return set_follow_permission_enabled(self, nickname, is_private)
 
-    def set_setting_follow_recommendation_enabled(self, on: bool):
-        return set_setting_follow_recommendation_enabled(self, bool)
+    def set_setting_follow_recommendation_enabled(self, on: bool) -> dict:
+        return set_setting_follow_recommendation_enabled(self, on)
 
-    def take_action_follow_request(self, target_id: int, action: str):
+    def take_action_follow_request(self, target_id: int, action: str) -> dict:
         return take_action_follow_request(self, target_id, action)
 
-    def turn_on_hima(self):
+    def turn_on_hima(self) -> dict:
+        """
+
+        ひまなう
+
+        """
         return turn_on_hima(self)
 
-    def unfollow_user(self, user_id: int):
+    def unfollow_user(self, user_id: int) -> dict:
+        """
+
+        ユーザーをアンフォローします
+
+        """
         return unfollow_user(self, user_id)
 
-    def update_invite_contact_status(self, mobile_number: str):
+    def update_invite_contact_status(self, mobile_number: str) -> dict:
         return update_invite_contact_status(self, mobile_number)
 
-    def update_language(self, language: str):
+    def update_language(self, language: str) -> dict:
+        """
+
+        言語を更新します
+
+        """
         return update_language(self, language)
 
     def update_user(
             self,
             nickname: str,
             biography: str = None,
             prefecture: str = None,
             gender: int = None,
             country_code: str = None,
             profile_icon_filename: str = None,
             cover_image_filename: str = None,
             username: str = None,
-    ):
+    ) -> dict:
+        """
+
+        プロフィールを更新します
+
+        """
         return update_user(
             self, nickname, biography, prefecture, gender, country_code,
             profile_icon_filename, cover_image_filename, username
         )
 
-    # def update_user_interests(self):
+    # def update_user_interests(self) -> dict:
     #     return update_user_interests(self)
 
-    # def upload_contacts_friends(self):
+    # def upload_contacts_friends(self) -> dict:
     #     return upload_contacts_friends(self)
 
-    def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]):
+    def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]) -> dict:
         return upload_twitter_friend_ids(self, twitter_friend_ids)
 
-    def block_user(self, user_id: int):
+    def block_user(self, user_id: int) -> dict:
+        """
+
+        ユーザーをブロックします
+
+        """
         return block_user(self, user_id)
 
     def get_blocked_user_ids(self) -> BlockedUserIdsResponse:
+        """
+
+        あなたをブロックしたユーザーを取得します
+
+        """
         return get_blocked_user_ids(self)
 
     def get_blocked_users(self, from_id: int = None) -> BlockedUsersResponse:
+        """
+
+        ブロックしたユーザーを取得します
+
+        """
         return get_blocked_users(self, from_id)
 
-    def unblock_user(self, user_id: int):
+    def unblock_user(self, user_id: int) -> dict:
+        """
+
+        ユーザーをアンブロックします
+
+        """
         return unblock_user(self, user_id)
 
     def get_hidden_users_list(self, **params: Union[str, int]) -> HiddenResponse:
         """
 
-        Parameters:
+        非表示のユーザー一覧を取得します
+
+        Parameters
         ----------
 
             - from: str = None
             - number: int = None
 
         """
         return get_hidden_users_list(self, **params)
 
-    def hide_user(self, user_id: int):
+    def hide_user(self, user_id: int) -> dict:
+        """
+
+        ユーザーを非表示にします
+
+        """
         return hide_user(self, user_id)
 
-    def unhide_users(self, user_ids: List[int]):
+    def unhide_users(self, user_ids: List[int]) -> dict:
+        """
+
+        ユーザーの非表示を解除します
+
+        """
         return unhide_users(self, user_ids)
```

### Comparing `yaylib-0.1.0/yaylib/config.py` & `yaylib-0.1.2/yaylib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 class Configs:
 
-    YAYLIB_VERSION = "0.1.0"
+    YAYLIB_VERSION = "0.1.2"
     YAY_API_VERSION = "3.16"
     YAY_VERSION_NAME = "3.16.1"
-    YAY_VERSION_MESSAGE = "yay_android/" + YAY_API_VERSION
     YAY_API_VERSION_KEY = "e83a1d2588918c2061280427c88e6f56"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
     YAY_REVIEW_HOST_1 = "review.yay.space"
     YAY_REVIEW_HOST_2 = "cas-stg.yay.space"
```

### Comparing `yaylib-0.1.0/yaylib/models.py` & `yaylib-0.1.2/yaylib/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1339,46 +1339,46 @@
 
 
 class User:
 
     # TODO: last_logged_in_at, created_at, updated_time_millis 確かめる
 
     __slots__ = (
-        "data", "id", "username", "prefecture", "biography", "gender", "generation",
+        "data", "id", "nickname", "prefecture", "biography", "gender", "generation",
         "last_logged_in_at", "last_logged_in_at_parsed", "created_at",
         "created_at_parsed", "badge", "followers_count", "followings_count",
-        "posts_count", "joined_groups_count", "reviews_count", "login_streak_count",
+        "posts_count", "groups_users_count", "reviews_count", "login_streak_count",
         "profile_icon", "profile_icon_thumbnail", "cover_image",
         "cover_image_thumbnail", "is_private", "is_vip", "is_vip_hidden",
         "is_chat_request_on", "mobile_number", "is_age_verified", "is_new_user",
         "online_status", "country_code", "is_recently_banned", "is_dangerous_user",
         "is_trusted_different_generation", "is_selected_interests", "group_user",
         "restricted_review_by", "is_following", "is_followed_by",
         "is_follow_pending", "is_hidden", "connected_by", "contact_phones",
         "updated_time_millis", "updated_time_millis_parsed"
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
-        self.username = data.get("nickname")
+        self.nickname = data.get("nickname")
         self.prefecture = data.get("prefecture")
         self.biography = data.get("biography")
         self.gender = data.get("gender")
         self.generation = data.get("generation")
-        self.last_logged_in_at = data.get("last_logged_in_at_seconds")
+        self.last_logged_in_at = data.get("last_logged_in_at")
         self.last_logged_in_at_parsed = parse_datetime(
-            data.get("last_logged_in_at_seconds"))
-        self.created_at = data.get("created_at_seconds")
-        self.created_at_parsed = parse_datetime(data.get("created_at_seconds"))
+            data.get("last_logged_in_at"))
+        self.created_at = data.get("created_at")
+        self.created_at_parsed = parse_datetime(data.get("created_at"))
         self.badge = data.get("title")
         self.followers_count = data.get("followers_count")
         self.followings_count = data.get("followings_count")
         self.posts_count = data.get("posts_count")
-        self.joined_groups_count = data.get("groups_users_count")
+        self.groups_users_count = data.get("groups_users_count")
         self.reviews_count = data.get("reviews_count")
         self.login_streak_count = data.get("login_streak_count")
         self.profile_icon = data.get("profile_icon")
         self.profile_icon_thumbnail = data.get("profile_icon_thumbnail")
         self.cover_image = data.get("cover_image")
         self.cover_image_thumbnail = data.get("cover_image_thumbnail")
         self.is_private = data.get("is_private")
```

### Comparing `yaylib-0.1.0/yaylib/responses.py` & `yaylib-0.1.2/yaylib/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1148,15 +1148,15 @@
 
 class UserTimestampResponse:
 
     __slots__ = ("data", "time", "ip_address", "country")
 
     def __init__(self, data):
         self.data = data
-        self.id = data.get("time")
+        self.time = data.get("time")
         self.ip_address = data.get("ip_address")
         self.country = data.get("country")
 
     def __repr__(self):
         return f"UserTimestampResponse(data={self.data})"
```

### Comparing `yaylib-0.1.0/yaylib.egg-info/PKG-INFO` & `yaylib-0.1.2/yaylib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 0.1.0
-Summary: This Python package provides an easy-to-use interface for accessing data from Yay!, a social networking platform. With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts. Compatible with Yay! version 3.16 and later. Please note that some API calls may be subject to rate limits or require authentication.
+Version: 0.1.2
+Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
-Author: qvco, Konn
+Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
-Maintainer: qvco, Konn
+Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
-Keywords: yay,yaylib,api,bot,library,wrapper
+Keywords: yay,yaylib,api,bot,library,wrapper,ボット,ライブラリ
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
@@ -36,15 +36,15 @@
     </a> -->
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
         このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
-        <a href="https://github.com/qvco/yaylib">
+        <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
             <strong>詳しい機能の詳細や使い方はこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
@@ -128,17 +128,17 @@
 メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 
-api.login_with_email(email="hello@example.com", password="abc123")
+api.login(email="メールアドレス", password="パスワード")
 
-api.create_post(text="Hi there.", color=2)
+api.create_post(text="初めての投稿！", color=2)
 ```
 
 より詳細な使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
@@ -154,25 +154,25 @@
             <th>Funktion (架空)</th>
             <th>香ばしいボット (架空)</th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/MindReaderAI.jpg" width="200px"></a>
+                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/Funktion.jpg" width="200px"></a>
+                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/blob/main/assets/bot-icons/香ばしいボット.jpg" width="200px"></a>
+                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px"></a>
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
             </td>
         </tr>
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: yaylib Version: 0.1.0 Summary: This Python package
-provides an easy-to-use interface for accessing data from Yay!, a social
-networking platform. With this API Client, you can retrieve user profiles,
-posts, comments, and other content from Yay!, as well as perform common tasks
-like liking and commenting on posts. Compatible with Yay! version 3.16 and
-later. Please note that some API calls may be subject to rate limits or require
-authentication. Home-page: https://github.com/qvco/yaylib Download-URL: https:/
-/github.com/qvco/yaylib Author: qvco, Konn Author-email:
-nikola.desuga@gmail.com Maintainer: qvco, Konn Maintainer-email:
+Metadata-Version: 2.1 Name: yaylib Version: 0.1.2 Summary: This Python package
+provides an easy-to-use interface for accessing data from Yay! (https://
+yay.space/). With this API Client, you can retrieve user profiles, posts,
+comments, and other content from Yay!, as well as perform common tasks like
+liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
+Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
+nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
-yay,yaylib,api,bot,library,wrapper Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE
+yay,yaylib,api,bot,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
+Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
@@ -46,26 +44,27 @@
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```  ## ä½¿ç¨ä¾
 ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
-```python import yaylib api = yaylib.Client() api.login_with_email
-(email="hello@example.com", password="abc123") api.create_post(text="Hi
-there.", color=2) ``` ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã]
-(https://github.com/qvco/yaylib/blob/master/examples)
-ãåç§ãã¦ãã ããã
+```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+(text="åãã¦ã®æç¨¿ï¼", color=2) ```
+ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
+yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## yaylib ã§èªçããã­ããããã¡ yaylib
 ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader AI                                      Funktion (æ¶ç©º)                é¦ã°ããããã (æ¶ç©º)
-[https://github.com/qvco/yaylib/blob/main/assets/  [https://github.com/qvco/yaylib/blob/      [https://github.com/qvco/yaylib/blob/main/assets/bot-icons/
-           bot-icons/MindReaderAI.jpg]              main/assets/bot-icons/Funktion.jpg]                       é¦ã°ããããã.jpg]
-            éçºè: æ¯ã®å¯�         éçºè: ãºã                éçºè: ããã¶ãå¤©ç¶æ°´ã
+ [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
+      472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
+            éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
+                                                            éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
 ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
 ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ããï¼    ##
 åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
```

### Comparing `yaylib-0.1.0/yaylib.egg-info/SOURCES.txt` & `yaylib-0.1.2/yaylib.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 LICENSE
 README.md
 setup.py
+tests/test_call.py
+tests/test_cassandra.py
+tests/test_chat.py
+tests/test_group.py
+tests/test_misc.py
+tests/test_post.py
+tests/test_review.py
+tests/test_thread.py
+tests/test_user.py
 yaylib/__init__.py
 yaylib/client.py
 yaylib/config.py
 yaylib/errors.py
 yaylib/models.py
 yaylib/responses.py
 yaylib/utils.py
```

