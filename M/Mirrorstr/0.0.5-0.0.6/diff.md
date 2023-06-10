# Comparing `tmp/Mirrorstr-0.0.5.tar.gz` & `tmp/Mirrorstr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mirrorstr-0.0.5.tar", last modified: Thu Jun  8 13:42:06 2023, max compression
+gzip compressed data, was "Mirrorstr-0.0.6.tar", last modified: Sat Jun 10 02:23:22 2023, max compression
```

## Comparing `Mirrorstr-0.0.5.tar` & `Mirrorstr-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-08 13:42:06.580687 Mirrorstr-0.0.5/
--rw-r--r--   0 lira       (501) staff       (20)     1073 2023-06-08 02:56:19.000000 Mirrorstr-0.0.5/LICENSE
--rw-r--r--   0 lira       (501) staff       (20)     3373 2023-06-08 13:42:06.580852 Mirrorstr-0.0.5/PKG-INFO
--rw-r--r--   0 lira       (501) staff       (20)     2838 2023-06-08 03:38:59.000000 Mirrorstr-0.0.5/README.md
--rw-r--r--   0 lira       (501) staff       (20)      724 2023-06-08 13:41:02.000000 Mirrorstr-0.0.5/pyproject.toml
--rw-r--r--   0 lira       (501) staff       (20)      114 2023-06-08 13:42:06.581281 Mirrorstr-0.0.5/setup.cfg
-drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-08 13:42:06.575489 Mirrorstr-0.0.5/src/
-drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-08 13:42:06.578355 Mirrorstr-0.0.5/src/Mirrorstr.egg-info/
--rw-r--r--   0 lira       (501) staff       (20)     3373 2023-06-08 13:42:06.000000 Mirrorstr-0.0.5/src/Mirrorstr.egg-info/PKG-INFO
--rw-r--r--   0 lira       (501) staff       (20)      419 2023-06-08 13:42:06.000000 Mirrorstr-0.0.5/src/Mirrorstr.egg-info/SOURCES.txt
--rw-r--r--   0 lira       (501) staff       (20)        1 2023-06-08 13:42:06.000000 Mirrorstr-0.0.5/src/Mirrorstr.egg-info/dependency_links.txt
--rw-r--r--   0 lira       (501) staff       (20)       50 2023-06-08 13:42:06.000000 Mirrorstr-0.0.5/src/Mirrorstr.egg-info/entry_points.txt
--rw-r--r--   0 lira       (501) staff       (20)       73 2023-06-08 13:42:06.000000 Mirrorstr-0.0.5/src/Mirrorstr.egg-info/requires.txt
--rw-r--r--   0 lira       (501) staff       (20)       10 2023-06-08 13:42:06.000000 Mirrorstr-0.0.5/src/Mirrorstr.egg-info/top_level.txt
-drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-08 13:42:06.580373 Mirrorstr-0.0.5/src/mirrorstr/
--rw-r--r--   0 lira       (501) staff       (20)        0 2023-06-08 13:35:02.000000 Mirrorstr-0.0.5/src/mirrorstr/__init__.py
--rw-r--r--   0 lira       (501) staff       (20)     6625 2023-06-08 13:38:46.000000 Mirrorstr-0.0.5/src/mirrorstr/main.py
--rw-r--r--   0 lira       (501) staff       (20)      677 2023-06-06 14:59:35.000000 Mirrorstr-0.0.5/src/mirrorstr/mp4_to_gif.py
--rw-r--r--   0 lira       (501) staff       (20)     1712 2023-05-30 03:13:12.000000 Mirrorstr-0.0.5/src/mirrorstr/post_note.py
--rw-r--r--   0 lira       (501) staff       (20)      558 2023-06-03 00:24:11.000000 Mirrorstr-0.0.5/src/mirrorstr/upload_to_voidcat_and_return_url.py
+drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-10 02:23:22.247808 Mirrorstr-0.0.6/
+-rw-r--r--   0 lira       (501) staff       (20)     1073 2023-06-08 02:56:19.000000 Mirrorstr-0.0.6/LICENSE
+-rw-r--r--   0 lira       (501) staff       (20)     3373 2023-06-10 02:23:22.247674 Mirrorstr-0.0.6/PKG-INFO
+-rw-r--r--   0 lira       (501) staff       (20)     2838 2023-06-08 03:38:59.000000 Mirrorstr-0.0.6/README.md
+-rw-r--r--   0 lira       (501) staff       (20)      912 2023-06-10 02:11:27.000000 Mirrorstr-0.0.6/pyproject.toml
+-rw-r--r--   0 lira       (501) staff       (20)       38 2023-06-10 02:23:22.247849 Mirrorstr-0.0.6/setup.cfg
+drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-10 02:23:22.244526 Mirrorstr-0.0.6/src/
+drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-10 02:23:22.245966 Mirrorstr-0.0.6/src/Mirrorstr.egg-info/
+-rw-r--r--   0 lira       (501) staff       (20)     3373 2023-06-10 02:23:22.000000 Mirrorstr-0.0.6/src/Mirrorstr.egg-info/PKG-INFO
+-rw-r--r--   0 lira       (501) staff       (20)      472 2023-06-10 02:23:22.000000 Mirrorstr-0.0.6/src/Mirrorstr.egg-info/SOURCES.txt
+-rw-r--r--   0 lira       (501) staff       (20)        1 2023-06-10 02:23:22.000000 Mirrorstr-0.0.6/src/Mirrorstr.egg-info/dependency_links.txt
+-rw-r--r--   0 lira       (501) staff       (20)       60 2023-06-10 02:23:22.000000 Mirrorstr-0.0.6/src/Mirrorstr.egg-info/entry_points.txt
+-rw-r--r--   0 lira       (501) staff       (20)       93 2023-06-10 02:23:22.000000 Mirrorstr-0.0.6/src/Mirrorstr.egg-info/requires.txt
+-rw-r--r--   0 lira       (501) staff       (20)       10 2023-06-10 02:23:22.000000 Mirrorstr-0.0.6/src/Mirrorstr.egg-info/top_level.txt
+drwxr-xr-x   0 lira       (501) staff       (20)        0 2023-06-10 02:23:22.247321 Mirrorstr-0.0.6/src/mirrorstr/
+-rw-r--r--   0 lira       (501) staff       (20)        0 2023-06-10 00:18:43.000000 Mirrorstr-0.0.6/src/mirrorstr/__init__.py
+-rw-r--r--   0 lira       (501) staff       (20)       41 2023-06-10 01:30:15.000000 Mirrorstr-0.0.6/src/mirrorstr/hello_world.py
+-rw-r--r--   0 lira       (501) staff       (20)     6906 2023-06-10 02:22:12.000000 Mirrorstr-0.0.6/src/mirrorstr/mirrorstr.py
+-rw-r--r--   0 lira       (501) staff       (20)      677 2023-06-06 14:59:35.000000 Mirrorstr-0.0.6/src/mirrorstr/mp4_to_gif.py
+-rw-r--r--   0 lira       (501) staff       (20)     1831 2023-06-10 02:05:37.000000 Mirrorstr-0.0.6/src/mirrorstr/post_note.py
+-rw-r--r--   0 lira       (501) staff       (20)      148 2023-05-30 02:48:59.000000 Mirrorstr-0.0.6/src/mirrorstr/relay_list.txt
+-rw-r--r--   0 lira       (501) staff       (20)      558 2023-06-03 00:24:11.000000 Mirrorstr-0.0.6/src/mirrorstr/upload_to_voidcat_and_return_url.py
```

### Comparing `Mirrorstr-0.0.5/LICENSE` & `Mirrorstr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Mirrorstr-0.0.5/PKG-INFO` & `Mirrorstr-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mirrorstr
-Version: 0.0.5
+Version: 0.0.6
 Summary: An application to mirror Nostr posts on twitter, and vice-versa
 Author-email: pleblira <pleblira@gmail.com>
 Project-URL: Homepage, https://github.com/pleblira/mirrorstr
 Project-URL: Bug Tracker, https://github.com/pleblira/mirrorstr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Mirrorstr-0.0.5/README.md` & `Mirrorstr-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Mirrorstr-0.0.5/pyproject.toml` & `Mirrorstr-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Mirrorstr"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="pleblira", email="pleblira@gmail.com" },
 ]
 description = "An application to mirror Nostr posts on twitter, and vice-versa"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,13 +17,23 @@
     "Operating System :: OS Independent"]
 
 dependencies = [
 "moviepy==1.0.3",
 "nostr==0.0.2",
 "numpy==1.24.3",
 "Pillow==9.5.0",
-"Requests==2.31.0"]
+"Requests==2.31.0",
+"APScheduler==3.10.1"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/pleblira/mirrorstr"
 "Bug Tracker" = "https://github.com/pleblira/mirrorstr/issues"
 
+[project.scripts]
+mirrorstr = "mirrorstr.mirrorstr:mirrorstr"
+
+[tool.setuptools.package-data]
+myModule = ["*.txt"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
```

### Comparing `Mirrorstr-0.0.5/src/Mirrorstr.egg-info/PKG-INFO` & `Mirrorstr-0.0.6/src/Mirrorstr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mirrorstr
-Version: 0.0.5
+Version: 0.0.6
 Summary: An application to mirror Nostr posts on twitter, and vice-versa
 Author-email: pleblira <pleblira@gmail.com>
 Project-URL: Homepage, https://github.com/pleblira/mirrorstr
 Project-URL: Bug Tracker, https://github.com/pleblira/mirrorstr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Mirrorstr-0.0.5/src/mirrorstr/main.py` & `Mirrorstr-0.0.6/src/mirrorstr/mirrorstr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from apscheduler.schedulers.background import BackgroundScheduler
 import time
 import random
 import subprocess
 import sys
 import json
 import datetime
-from post_note import *
+from mirrorstr.post_note import *
 from nostr.key import PrivateKey
-from upload_to_voidcat_and_return_url import *
+from mirrorstr.upload_to_voidcat_and_return_url import *
 import requests
-from mp4_to_gif import *
+from mirrorstr.mp4_to_gif import *
    
-TWITTER_HANDLE = "jusabitcoiner"
+TWITTER_HANDLE = ""
 NOSTR_PRIVATE_KEY = ""
 
 # print(type(result.stdout))
 # repr shows escape characters - searching for \n
 # print(repr(result.stdout))
 
-def scrape_and_post():
-    print('running scrape_and_post')
+def scrape_and_post(TWITTER_HANDLE, NOSTR_PRIVATE_KEY):
+    print('running scrape_and_post. Analyzing last 5 scraped tweets')
     scrape = subprocess.run(['snscrape','--jsonl','-n','5','twitter-user', TWITTER_HANDLE], capture_output=True, text=True)
     json_from_scraper_output = json.loads("["+scrape.stdout.strip().replace("\n",",")+"]")
     # print(json_from_scraper_output)
     with open('tweets.json','r+') as f:
         stored_json = json.load(f)
         for scraped_tweet in json_from_scraper_output:
-            print("")
             if scraped_tweet["inReplyToTweetId"] == None:
                 new_tweet = True
                 while new_tweet == True:
                     for stored_tweet in stored_json:
                         if scraped_tweet["id"] == stored_tweet["id"]:
                             print('tweet already scraped')
                             new_tweet = False
@@ -70,15 +69,15 @@
 
                                     filetype = temporary_variant_list[0]["url"]
                                     filetype = filetype[:filetype.find("?tag=")]
                                     filetype = filetype[filetype.rfind(".")+1:]
 
                                     downloaded_media = requests.get(temporary_variant_list[0]["url"])
                                 
-                                with open("temp."+filetype,'wb') as te  mp_media_file:
+                                with open("temp."+filetype,'wb') as temp_media_file:
                                     temp_media_file.write(downloaded_media.content)
 
                                 if media_file["_type"] == "snscrape.modules.twitter.Gif":
                                     with open("gifcopy."+filetype,'wb') as temp_media_file:
                                         temp_media_file.write(downloaded_media.content)
                                     mp4_to_gif("temp.mp4", "temp.gif")
                                     filetype = "gif"
@@ -90,30 +89,34 @@
                         f.write(json.dumps(stored_json, indent=2))
                         post_note(NOSTR_PRIVATE_KEY, scraped_tweet["rawContent"])
                         new_tweet = False
                 # print('exited while loop')
             else:
                 print('tweet is a reply')
 
-def main():
-        # NOSTR_PRIVATE_KEY = input("Please type your Nostr private key: ")
-    NOSTR_PRIVATE_KEY = PrivateKey.from_nsec("nsec16pejvh2hdkf4rzrpejk93tmvuhaf8pv7eqenevk576492zqy6pfqguu985")
+def mirrorstr():
+    NOSTR_PRIVATE_KEY = input("Type Nostr nsec private key (enter 'test' to use test key nsec16pejvh2hdkf4rzrpejk93tmvuhaf8pv7eqenevk576492zqy6pfqguu985): ")
+
+    TWITTER_HANDLE = input("Type Twitter handle: ")
+
+    if NOSTR_PRIVATE_KEY == "test":
+        NOSTR_PRIVATE_KEY = PrivateKey.from_nsec("nsec16pejvh2hdkf4rzrpejk93tmvuhaf8pv7eqenevk576492zqy6pfqguu985")
 
     with open('tweets.json','w') as f:
         f.write("[]")
 
     scrape = subprocess.run(['snscrape','--jsonl','-n','5','twitter-user',TWITTER_HANDLE], capture_output=True, text=True)
     json_from_output = json.loads("["+scrape.stdout.strip().replace("\n",",")+"]")
     json_from_output.reverse()
     with open('tweets.json','r+') as f:
         f.seek(0)
         f.write(json.dumps(json_from_output, indent=2))
     
     scheduler = BackgroundScheduler()
-    scheduler.add_job(scrape_and_post, 'interval', seconds=10)
+    scheduler.add_job(scrape_and_post, 'interval', seconds=10, args=[TWITTER_HANDLE,NOSTR_PRIVATE_KEY])
     print('\nstarting scheduler')
     scheduler.start()
 
     while True:
 #     with open('tweets.json', 'r') as f:
 #         tweets = json.load(f)
 #         last_queried_event_datetime = int(datetime.fromisoformat(tweets[len(tweets)-1]['date']).timestamp())
```

### Comparing `Mirrorstr-0.0.5/src/mirrorstr/mp4_to_gif.py` & `Mirrorstr-0.0.6/src/mirrorstr/mp4_to_gif.py`

 * *Files identical despite different names*

### Comparing `Mirrorstr-0.0.5/src/mirrorstr/post_note.py` & `Mirrorstr-0.0.6/src/mirrorstr/post_note.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 from nostr.event import Event
 # from python_nostr import Event
 # from python_nostr import RelayManager
 # from python_nostr import PrivateKey
 # from nostr.event import Event
 # from nostr.relay_manager import RelayManager
 # from nostr.key import PrivateKey
-import random
+# import random
+import os
 
 # private_key = PrivateKey()
 # print(private_key.bech32())
 # public_key = private_key.public_key
 # print("https://snort.social/p/"+private_key.public_key.bech32())
 # print(private_key.public_key.bech32())
 
 tags = []
 
+__location__ = os.path.realpath(
+    os.path.join(os.getcwd(), os.path.dirname(__file__)))
+
+
 def post_note(private_key, content, tags=""):
     relay_manager = RelayManager()
-    with open('relay_list.txt', 'r') as f:
+    with open(__location__+'/relay_list.txt', 'r') as f:
         for line in f:
             relay_manager.add_relay(line.strip())
     # relay_manager.add_relay("wss://relay.nostr.bg")
     relay_manager.open_connections({"cert_reqs": ssl.CERT_NONE}) # NOTE: This disables ssl certificate verification
     time.sleep(1.25) # allow the connections to open
 
     event = Event(private_key.public_key.hex(), content)
```

### Comparing `Mirrorstr-0.0.5/src/mirrorstr/upload_to_voidcat_and_return_url.py` & `Mirrorstr-0.0.6/src/mirrorstr/upload_to_voidcat_and_return_url.py`

 * *Files identical despite different names*

