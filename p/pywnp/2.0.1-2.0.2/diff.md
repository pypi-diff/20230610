# Comparing `tmp/pywnp-2.0.1.tar.gz` & `tmp/pywnp-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywnp-2.0.1.tar", last modified: Wed May 10 14:13:31 2023, max compression
+gzip compressed data, was "pywnp-2.0.2.tar", last modified: Sat Jun 10 12:07:22 2023, max compression
```

## Comparing `pywnp-2.0.1.tar` & `pywnp-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.144901 pywnp-2.0.1/
--rw-rw-rw-   0        0        0     1060 2023-04-26 13:11:28.000000 pywnp-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     6632 2023-05-10 14:13:31.144901 pywnp-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4908 2023-05-10 12:49:48.000000 pywnp-2.0.1/README.md
--rw-rw-rw-   0        0        0      705 2023-05-10 14:10:37.000000 pywnp-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 14:13:31.144901 pywnp-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.126355 pywnp-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.128870 pywnp-2.0.1/src/pywnp/
--rw-rw-rw-   0        0        0       27 2023-05-08 22:50:56.000000 pywnp-2.0.1/src/pywnp/__init__.py
--rw-rw-rw-   0        0        0    30394 2023-05-10 14:09:46.000000 pywnp-2.0.1/src/pywnp/pywnp.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.144901 pywnp-2.0.1/src/pywnp.egg-info/
--rw-rw-rw-   0        0        0     6632 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 12:07:22.205290 pywnp-2.0.2/
+-rw-rw-rw-   0        0        0     1060 2023-04-26 13:11:28.000000 pywnp-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6632 2023-06-10 12:07:22.204291 pywnp-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4908 2023-05-10 12:49:48.000000 pywnp-2.0.2/README.md
+-rw-rw-rw-   0        0        0      705 2023-06-10 12:07:03.000000 pywnp-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 12:07:22.205290 pywnp-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 12:07:22.185763 pywnp-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 12:07:22.188772 pywnp-2.0.2/src/pywnp/
+-rw-rw-rw-   0        0        0       27 2023-05-08 22:50:56.000000 pywnp-2.0.2/src/pywnp/__init__.py
+-rw-rw-rw-   0        0        0    30591 2023-06-10 12:03:59.000000 pywnp-2.0.2/src/pywnp/pywnp.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:07:22.203290 pywnp-2.0.2/src/pywnp.egg-info/
+-rw-rw-rw-   0        0        0     6632 2023-06-10 12:07:22.000000 pywnp-2.0.2/src/pywnp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-10 12:07:22.000000 pywnp-2.0.2/src/pywnp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 12:07:22.000000 pywnp-2.0.2/src/pywnp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-10 12:07:22.000000 pywnp-2.0.2/src/pywnp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-10 12:07:22.000000 pywnp-2.0.2/src/pywnp.egg-info/top_level.txt
```

### Comparing `pywnp-2.0.1/LICENSE` & `pywnp-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywnp-2.0.1/PKG-INFO` & `pywnp-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywnp
-Version: 2.0.1
+Version: 2.0.2
 Summary: A python library to communicate with the WebNowPlaying-Redux browser extension
 Author-email: keifufu <pypi@keifufu.dev>
 License: Copyright 2023 keifufu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `pywnp-2.0.1/README.md` & `pywnp-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pywnp-2.0.1/pyproject.toml` & `pywnp-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywnp"
-version = "2.0.1"
+version = "2.0.2"
 description = "A python library to communicate with the WebNowPlaying-Redux browser extension"
 authors = [ { name="keifufu", email="pypi@keifufu.dev" } ]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [ "webnowplaying", "wnp", "youtube", "spotify", "media", "music" ]
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywnp-2.0.1/src/pywnp/pywnp.py` & `pywnp-2.0.2/src/pywnp/pywnp.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,20 @@
     time_in_minutes = math.floor(time_in_seconds / 60)
     if time_in_minutes < 60:
       return str(time_in_minutes) + ':' + str(pad(math.floor(time_in_seconds % 60), 2))
 
     return str(math.floor(time_in_minutes / 60)) + ':' + str(pad(math.floor(time_in_minutes % 60), 2)) + ':' + str(pad(math.floor(time_in_seconds % 60), 2))
   except:
     return '0:00'
-  
+
+def get_wnp_path() -> str:
+  # Note: I was going to clean up the old unused folder here but that might conflict with older WNP adapters, so I won't.
+  if is_windows: return os.path.expandvars(r'%LocalAppData%\\WebNowPlaying')
+  else: return os.path.expanduser(r'~\\.config\\WebNowPlaying')
+
 # === END UTILS ===
 
 # === START MEDIA CONTROLS ===
 
 class MediaControls:
   def __init__(self, supports_play_pause = False, supports_skip_previous = False, supports_skip_next = False, supports_set_position = False, supports_set_volume = False, supports_toggle_repeat_mode = False, supports_toggle_shuffle_active = False, supports_set_rating = False, rating_system = 'NONE'):
     self.supports_play_pause = supports_play_pause
@@ -236,15 +241,15 @@
       HttpServer._start_threaded()
 
   @staticmethod
   def handle_cover_route(request: web.Request) -> web.Response:
     if not 'name' in request.query: return web.Response(text='No name was provided', content_type='text/html', status=400)
     file_name = request.query['name']
     if not file_name.endswith('.jpg'): return web.Response(text='Invalid image name', content_type='text/html', status=400)
-    file_path = f'{WNPRedux._wnp_path}\\{file_name}'
+    file_path = f'{get_wnp_path()}\\{file_name}'
     if not os.path.exists(file_path): return web.Response(text='Image not found', content_type='text/html', status=404)
     with open(file_path, 'rb') as f:
       image_data = f.read()
     return web.Response(body=image_data, content_type='image/jpeg', status=200)
   
   async def web_websocket_handler(request: web.Request) -> web.WebSocketResponse:
     ws = web.WebSocketResponse()
@@ -271,30 +276,28 @@
             except ValueError:
               # The message doesn't have a space
               type: str = message.upper()
               data: str = ''
 
             if (type == 'USE_NATIVE_APIS'):
               WNPRedux.is_using_native_apis = bool(data)
-              if WNPRedux.is_using_native_apis and not os.path.isdir(WNPRedux._use_native_apis_path):
-                os.makedirs(WNPRedux._use_native_apis_path, exist_ok=True)
-              elif not WNPRedux.is_using_native_apis and os.path.isdir(WNPRedux._use_native_apis_path):
-                os.rmdir(WNPRedux._use_native_apis_path)
+              if WNPRedux.is_using_native_apis and os.path.isdir(WNPRedux._disable_native_apis_path):
+                os.rmdir(WNPRedux._disable_native_apis_path)
+              elif not WNPRedux.is_using_native_apis and not os.path.isdir(WNPRedux._disable_native_apis_path):
+                os.makedirs(WNPRedux._disable_native_apis_path, exist_ok=True)
               WNPRedux.update_media_info()
               HttpServer.update_recipients()
               continue
 
             media_info = WNPRedux.get_media_info(ws.id)
 
             if type == 'PLAYER_NAME':
               media_info.player_name = data
             elif type == 'IS_NATIVE':
               media_info.is_native = bool(data)
-            elif type == 'TIMESTAMP_OFFSET_SECONDS':
-              media_info.timestamp_offset_in_seconds = int(data)
             elif type == 'PLAYER_CONTROLS':
               media_info.controls = MediaControls.from_json(data)
             elif type == 'STATE':
               media_info.state = data
             elif type == 'TITLE':
               media_info.title = data
             elif type == 'ARTIST':
@@ -378,30 +381,29 @@
 
 # === END HTTPSERVER ===
 
 # === START WNP REDUX ===
 
 class WNPRedux:
   is_started: bool = False
-  is_using_native_apis: bool = False
-  _wnp_path = os.path.expanduser('~\\WebNowPlaying')
-  _use_native_apis_path = os.path.join(_wnp_path, 'use_native_apis')
+  is_using_native_apis: bool = True
+  _disable_native_apis_path = os.path.join(get_wnp_path(), 'use_native_apis');
   media_info: MediaInfo = MediaInfo()
   media_info_dictionary: List[MediaInfo] = list()
   clients: int = 0
   _version: str = '0.0.0'
   _logger: Callable = None
 
   @staticmethod
   def start(port: int, version: str, logger: Callable) -> None:
     if WNPRedux.is_started: return
     WNPRedux.is_started = True
     HttpServer.start(port)
     if is_windows: WNPReduxNative.start(port)
-    WNPRedux.is_using_native_apis = os.path.isdir(WNPRedux._use_native_apis_path)
+    WNPRedux.is_using_native_apis = not os.path.isdir(WNPRedux._disable_native_apis_path)
     WNPRedux._version = version
     WNPRedux._logger = logger
   
   @staticmethod
   def stop() -> None:
     if not WNPRedux.is_started: return
     WNPRedux.is_started = False
@@ -644,15 +646,16 @@
       try:
         readable_stream = await thumbnail.open_read_async()
         buffer = Buffer(readable_stream.size)
         await readable_stream.read_async(buffer, buffer.capacity, InputStreamOptions.READ_AHEAD)
         if buffer.length == 0: return
         buffer_reader = DataReader.from_buffer(buffer)
         byte_buffer = buffer_reader.read_buffer(buffer.length)
-        path = f'{WNPRedux._wnp_path}\\cover-{WNPReduxNative.port}.jpg'
+        os.makedirs(get_wnp_path(), exist_ok=True)
+        path = f'{get_wnp_path()}\\cover-{WNPReduxNative.port}.jpg'
         with open(path, 'wb+') as fobj:
           fobj.write(bytearray(byte_buffer))
         return f'http://127.0.0.1:{WNPReduxNative.port}/cover?name=cover-{WNPReduxNative.port}.jpg&r={random.randint(0, 999999)}'
       except: return ''
 
     @staticmethod
     def playback_info_changed_native(session: Session, e) -> None:
```

### Comparing `pywnp-2.0.1/src/pywnp.egg-info/PKG-INFO` & `pywnp-2.0.2/src/pywnp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywnp
-Version: 2.0.1
+Version: 2.0.2
 Summary: A python library to communicate with the WebNowPlaying-Redux browser extension
 Author-email: keifufu <pypi@keifufu.dev>
 License: Copyright 2023 keifufu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

