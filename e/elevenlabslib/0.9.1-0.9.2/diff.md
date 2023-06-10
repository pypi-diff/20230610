# Comparing `tmp/elevenlabslib-0.9.1.tar.gz` & `tmp/elevenlabslib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.9.1.tar", last modified: Thu Jun  1 12:13:03 2023, max compression
+gzip compressed data, was "elevenlabslib-0.9.2.tar", last modified: Sat Jun 10 20:52:53 2023, max compression
```

## Comparing `elevenlabslib-0.9.1.tar` & `elevenlabslib-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 12:13:03.599790 elevenlabslib-0.9.1/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     3379 2023-06-01 12:13:03.599790 elevenlabslib-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2023-06-01 12:12:53.000000 elevenlabslib-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 12:13:03.592790 elevenlabslib-0.9.1/elevenlabslib/
--rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    40774 2023-06-01 12:00:13.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.1/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     8403 2023-05-31 21:35:21.000000 elevenlabslib-0.9.1/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:13:03.597790 elevenlabslib-0.9.1/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     3379 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-06-01 12:12:34.000000 elevenlabslib-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 12:13:03.599790 elevenlabslib-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 20:52:53.840947 elevenlabslib-0.9.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0     3379 2023-06-10 20:52:53.840947 elevenlabslib-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2023-06-01 12:12:53.000000 elevenlabslib-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 20:52:53.834947 elevenlabslib-0.9.2/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    40835 2023-06-10 20:51:36.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.2/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     8403 2023-05-31 21:35:21.000000 elevenlabslib-0.9.2/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:52:53.839950 elevenlabslib-0.9.2/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     3379 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-06-10 20:52:35.000000 elevenlabslib-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 20:52:53.840947 elevenlabslib-0.9.2/setup.cfg
```

### Comparing `elevenlabslib-0.9.1/LICENSE` & `elevenlabslib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.1/PKG-INFO` & `elevenlabslib-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.1 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.2 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `elevenlabslib-0.9.1/README.md` & `elevenlabslib-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsVoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,16 +455,16 @@
         Args:
             sharingEnabled (bool): Whether to enable or disable sharing.
 
         Returns:
             str|None: The share URL for the voice, if you enabled sharing, or None if you disabled it.
         """
         sharingEnabledString = str(sharingEnabled).lower()
-
-        if self.get_info()["sharing"]["status"] == "copied":
+        sharingInfo = self.get_info()["sharing"]
+        if sharingInfo is not None and sharingInfo["status"] == "copied":
             raise RuntimeError("Cannot change sharing status of copied voices!")
 
         response = _api_multipart("/voices/" + self._voiceID + "/share", self._linkedUser.headers, data=sharingEnabledString)
         if sharingEnabled:
             return self.get_share_link()
         else:
             return None
```

### Comparing `elevenlabslib-0.9.1/elevenlabslib/__init__.py` & `elevenlabslib-0.9.2/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.1/elevenlabslib/helpers.py` & `elevenlabslib-0.9.2/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.1/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.9.2/elevenlabslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.1 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.2 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `elevenlabslib-0.9.1/pyproject.toml` & `elevenlabslib-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

