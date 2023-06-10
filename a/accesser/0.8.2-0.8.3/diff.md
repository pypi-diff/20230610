# Comparing `tmp/accesser-0.8.2.tar.gz` & `tmp/accesser-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accesser-0.8.2.tar", last modified: Fri May 26 03:10:02 2023, max compression
+gzip compressed data, was "accesser-0.8.3.tar", last modified: Sat Jun 10 10:30:29 2023, max compression
```

## Comparing `accesser-0.8.2.tar` & `accesser-0.8.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.889395 accesser-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 03:09:52.000000 accesser-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-26 03:10:02.889395 accesser-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-26 03:09:52.000000 accesser-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.885395 accesser-0.8.2/accesser/
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/pac
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.889395 accesser-0.8.2/accesser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/cert_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/certmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/importca.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/sysproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.885395 accesser-0.8.2/accesser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-26 03:09:52.000000 accesser-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:10:02.889395 accesser-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:30:29.296248 accesser-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-10 10:30:20.000000 accesser-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-10 10:30:29.296248 accesser-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-10 10:30:20.000000 accesser-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:30:29.296248 accesser-0.8.3/accesser/
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/pac
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:30:29.296248 accesser-0.8.3/accesser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/utils/cert_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/utils/certmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/utils/importca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/utils/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-10 10:30:20.000000 accesser-0.8.3/accesser/utils/sysproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:30:29.296248 accesser-0.8.3/accesser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-10 10:30:29.000000 accesser-0.8.3/accesser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-10 10:30:29.000000 accesser-0.8.3/accesser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 10:30:29.000000 accesser-0.8.3/accesser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-10 10:30:29.000000 accesser-0.8.3/accesser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 10:30:29.000000 accesser-0.8.3/accesser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 10:30:29.000000 accesser-0.8.3/accesser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-10 10:30:20.000000 accesser-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 10:30:29.296248 accesser-0.8.3/setup.cfg
```

### Comparing `accesser-0.8.2/LICENSE` & `accesser-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `accesser-0.8.2/PKG-INFO` & `accesser-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.8.2
+Version: 0.8.3
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.2/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.3/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U accesser[doh]
 ```
 如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.8.2/README.md` & `accesser-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.2/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.3/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U accesser[doh]
 ```
 如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.8.2/accesser/__init__.py` & `accesser-0.8.3/accesser/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = '0.8.2'
+__version__ = '0.8.3'
 
 import os, sys
 import json
+import fnmatch
 import random
 import ssl
 import asyncio
 import traceback
 from contextlib import closing
 from urllib import request
 from pkg_resources import parse_version
@@ -118,24 +119,25 @@
         writer.write(b'HTTP/1.1 200 Connection Established\r\n\r\n')
 
         await update_cert(host)
         if sys.version_info[1] >= 11:
             await writer.start_tls(context)
         else:
             writer._transport = await writer._loop.start_tls(writer.transport, writer._protocol, context, server_side=True)
-        server_hostname = setting.config['alter_hostname'].get(host, '')
+        server_hostname_key = next(filter(lambda h:fnmatch.fnmatchcase(host, h), setting.config['alter_hostname']), None)
+        server_hostname = '' if server_hostname_key is None else setting.config['alter_hostname'][server_hostname_key]
         logger.debug(f'[{i_port:5}] {server_hostname=}')
         remote_context = ssl.create_default_context()
         remote_context.check_hostname = False
         remote_reader, remote_writer = await asyncio.open_connection(remote_ip, port, ssl=remote_context, server_hostname=server_hostname)
         cert = remote_writer.get_extra_info('peercert')
         logger.debug(f"[{i_port:5}] {cert.get('subjectAltName', ())=}")
         if setting.config['check_hostname'] is not False:
             try:
-                match_hostname(cert, setting.config['alter_hostname'].get(host, host))
+                match_hostname(cert, host if server_hostname_key is None else setting.config['alter_hostname'][server_hostname_key])
             except ssl.CertificateError as err:
                 logger.warning(f'[{i_port:5}] {err}')
                 return
         
         await asyncio.gather(
             forward_stream(reader, remote_writer),
             forward_stream(remote_reader, writer)
```

### Comparing `accesser-0.8.2/accesser/config.toml` & `accesser-0.8.3/accesser/config.toml`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 "www.google.com/recaptcha/" = "www.recaptcha.net/recaptcha/"
 "tumblr.com/" = "www.tumblr.com/"
 "instagram.com/" = "www.instagram.com/"
 
 
 [alter_hostname]
 
-# 与键对应的域名的TLS连接会使用其值对应的域名作为server_name字段，并且校验证书时也使用这一域名。
-# A TLS connection to the domain corresponding to the key will use the domain name corresponding to its value as the server_name field, and this domain name is also used when verifying the certificate.
+# 与键对应的域名的TLS连接会使用其值对应的域名作为server_name字段，并且校验证书时也使用这一域名。键支持Unix shell风格的通配符。
+# A TLS connection to the domain corresponding to the key will use the domain name corresponding to its value as the server_name field, and this domain name is also used when verifying the certificate. The key supports Unix shell-style wildcards.
 
 "www.quora.com" = "fs.quoracdn.net"
 "sketch.pixiv.net" = "pixivsketch.net"
 "cdn1-smallimg.phncdn.com" = "pabbp.com"
 "nyaa.si" = "ddos-guard.net"
 "site.nicovideo.jp" = "d4fsvsnk8os9s.cloudfront.net"
 "blog.nicovideo.jp" = "d11c2xcc0ucqv1.cloudfront.net"
```

### Comparing `accesser-0.8.2/accesser/pac` & `accesser-0.8.3/accesser/pac`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   "*://*.bbci.co.uk/*": 1,
   "*://*.japantimes.co.jp/*": 1,
   "*://*.yahoo.co.jp/*": 1,
   "*://*.cna.com.tw/*": 1,
   "*://*.discord.com/*": 1,
   "*://*.discordapp.com/*": 1,
   "*://*.discord.gg/*": 1,
-  "*://images-ext-*.discordapp.net/*": 1,
+  "*://media.discordapp.net/*": 1,
   "*://*.duckduckgo.com/*": 1,
   "*://*.v2ex.com/*":1,
   "*://*.twitch.tv/*":1
 };
 
 var proxy = "PROXY {{host}}:{{port}};";
```

### Comparing `accesser-0.8.2/accesser/utils/cert_verify.py` & `accesser-0.8.3/accesser/utils/cert_verify.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.2/accesser/utils/certmanager.py` & `accesser-0.8.3/accesser/utils/certmanager.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.2/accesser/utils/importca.py` & `accesser-0.8.3/accesser/utils/importca.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.2/accesser/utils/log.py` & `accesser-0.8.3/accesser/utils/log.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.2/accesser/utils/setting.py` & `accesser-0.8.3/accesser/utils/setting.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.2/accesser/utils/sysproxy.py` & `accesser-0.8.3/accesser/utils/sysproxy.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.2/accesser.egg-info/PKG-INFO` & `accesser-0.8.3/accesser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.8.2
+Version: 0.8.3
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.2/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.3/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U accesser[doh]
 ```
 如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
```

