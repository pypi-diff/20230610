# Comparing `tmp/wclone-1.0.1.tar.gz` & `tmp/wclone-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wclone-1.0.1.tar", last modified: Fri Jun  9 16:19:42 2023, max compression
+gzip compressed data, was "wclone-1.0.2.tar", last modified: Sat Jun 10 09:48:45 2023, max compression
```

## Comparing `wclone-1.0.1.tar` & `wclone-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:19:42.568390 wclone-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 16:19:42.568390 wclone-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-09 16:19:26.000000 wclone-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:19:42.568390 wclone-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-09 16:19:26.000000 wclone-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:19:42.568390 wclone-1.0.1/wclone/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 16:19:26.000000 wclone-1.0.1/wclone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 16:19:26.000000 wclone-1.0.1/wclone/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-06-09 16:19:26.000000 wclone-1.0.1/wclone/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:19:42.568390 wclone-1.0.1/wclone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:48:45.559337 wclone-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-10 09:48:45.559337 wclone-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-10 09:48:34.000000 wclone-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:48:45.559337 wclone-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-10 09:48:34.000000 wclone-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:48:45.559337 wclone-1.0.2/wclone/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-10 09:48:34.000000 wclone-1.0.2/wclone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-10 09:48:34.000000 wclone-1.0.2/wclone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-10 09:48:34.000000 wclone-1.0.2/wclone/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:48:45.559337 wclone-1.0.2/wclone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-10 09:48:45.000000 wclone-1.0.2/wclone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-10 09:48:45.000000 wclone-1.0.2/wclone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:48:45.000000 wclone-1.0.2/wclone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-10 09:48:45.000000 wclone-1.0.2/wclone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-10 09:48:45.000000 wclone-1.0.2/wclone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 09:48:45.000000 wclone-1.0.2/wclone.egg-info/top_level.txt
```

### Comparing `wclone-1.0.1/PKG-INFO` & `wclone-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wclone
-Version: 1.0.1
+Version: 1.0.2
 Summary: Basic website cloner written in Python
 Home-page: https://github.com/ZKAW/website-cloner
 Author: ZKAW
 Maintainer: Smartwa
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/ZKAW/website-cloner/issues/new
```

### Comparing `wclone-1.0.1/README.md` & `wclone-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wclone-1.0.1/setup.py` & `wclone-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `wclone-1.0.1/wclone/app.py` & `wclone-1.0.2/wclone/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 import os
 import logging
 import cloudscraper
 from bs4 import BeautifulSoup
 from urllib.parse import urljoin, urlparse
 from . import __version__, __description__
+from json import load
 
 platforms = ["darwin", "ios", "android", "windows", "linux"]
 browsers = ["chrome", "firefox"]
 
 
 class Extractor:
     def __init__(self, url):
@@ -24,15 +25,15 @@
 
     def run(self):
         self.save_files(self.scraped_urls)
         self.save_html()
 
     def get_page_content(self, url):
         try:
-            content = session.get(url)
+            content = session.get(url, timeout=args.timeout)
             content.encoding = "utf-8"
             return content.text
         except Exception as e:
             sys.exit(logging.critical(get_excep(e)))
 
     # get the script files
     def scrap_scripts(self):
@@ -251,15 +252,15 @@
 
 def error_handler():
     def decorator(func):
         def main(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except (KeyboardInterrupt, EOFError) as e:
-                logging.warning(f'^{e} - Exitting"')
+                logging.warning(f"^{e} - Exitting")
             except Exception as e:
                 # logging.exception(e)
                 logging.critical(get_excep(e))
 
         return main
 
     return decorator
@@ -281,15 +282,27 @@
         help="Proxy server url without schema - %(default)s",
         default="localhost:9050",
     )
     parser.add_argument(
         "-o", "--output", metavar="FOLDER", help="Folder for saving contents - host"
     )
     parser.add_argument(
-        "--headers", help="Path to .json file containing request headers"
+        "-t",
+        "--timeout",
+        help="Timeout while awaiting response (s) - %(default)s",
+        type=int,
+        default=20,
+    )
+    parser.add_argument(
+        "--headers",
+        help="Path to .json file containing request headers",
+        metavar="PATH",
+    )
+    parser.add_argument(
+        "--cookies", help="Path to .json file containing cookies", metavar="PATH"
     )
     parser.add_argument(
         "--browser",
         help="Browser name to be used - %(default)s",
         choices=browsers,
         default="firefox",
         metavar="|".join(browsers),
@@ -307,17 +320,18 @@
         metavar="PATH",
         help="Directory for saving contents - %(default)s",
         default=os.getcwd(),
     )
     parser.add_argument(
         "--use-tor", action="store_true", help="Use tor proxy - %(default)s"
     )
-    args = parser.parse_args()
 
-    global url, workspace, get_excep, output_folder, session
+    global url, workspace, get_excep, output_folder, session, args
+
+    args = parser.parse_args()
 
     logging.basicConfig(
         format="[%(asctime)s : %(levelname)s] - %(message)s",
         datefmt="%H:%M:%S",
         level=logging.INFO,
     )
     # URL of the web page you want to extract data from
@@ -337,35 +351,38 @@
         session_def.request = functools.partial(session.request, timeout=30)
         session_def.proxies = {
             "http": f"socks5h://{args.tor_proxy}",
             "https": f"socks5h://{args.tor_proxy}",
         }
 
     if args.headers:
-        from json import load
-
         with open(args.headers) as fh:
             session_def.headers = load(fh)
     else:
-        session_def.headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-            "User-Agent": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Accept-Language": "en-US,en;q=0.9",
-        }
+        session_def.headers.update(
+            {
+                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+                "User-Agent": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36",
+                "Accept-Encoding": "gzip, deflate, br",
+                "Accept-Language": "en-US,en;q=0.9",
+            }
+        )
+    if args.cookies:
+        with open(args.cookies) as fh:
+            session_def.cookies.update(load(fh))
 
     session = cloudscraper.create_scraper(
         sess=session_def,
         browser={
             "browser": args.browser,
             "platform": args.platform,
             "desktop": True,
         },
     )
     logging.info(f"Extracting files from '{url}'")
     extractor = Extractor(url)
     extractor.run()
-    logging.info(f"Total extracted files: {len(extractor.scraped_urls)}")
+    logging.info(f"Total extracted files : {len(extractor.scraped_urls)}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wclone-1.0.1/wclone.egg-info/PKG-INFO` & `wclone-1.0.2/wclone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wclone
-Version: 1.0.1
+Version: 1.0.2
 Summary: Basic website cloner written in Python
 Home-page: https://github.com/ZKAW/website-cloner
 Author: ZKAW
 Maintainer: Smartwa
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/ZKAW/website-cloner/issues/new
```

