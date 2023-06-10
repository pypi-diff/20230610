# Comparing `tmp/gamedetector-0.1.3.tar.gz` & `tmp/gamedetector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamedetector-0.1.3.tar", max compression
+gzip compressed data, was "gamedetector-0.1.4.tar", max compression
```

## Comparing `gamedetector-0.1.3.tar` & `gamedetector-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.1.3/gamedetector/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-09 18:22:23.018869 gamedetector-0.1.3/gamedetector/app_exes.json
--rw-r--r--   0        0        0    16162 2023-06-10 19:37:18.622896 gamedetector-0.1.3/gamedetector/game_detect.py
--rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.1.3/LICENSE
--rw-r--r--   0        0        0      805 2023-06-10 19:37:49.498852 gamedetector-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-09 18:24:36.455517 gamedetector-0.1.3/README.md
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 gamedetector-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.1.4/gamedetector/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-09 18:22:23.018869 gamedetector-0.1.4/gamedetector/app_exes.json
+-rw-r--r--   0        0        0    16146 2023-06-10 19:57:53.452187 gamedetector-0.1.4/gamedetector/game_detect.py
+-rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.1.4/LICENSE
+-rw-r--r--   0        0        0      805 2023-06-10 19:57:49.201527 gamedetector-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-09 18:24:36.455517 gamedetector-0.1.4/README.md
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 gamedetector-0.1.4/PKG-INFO
```

### Comparing `gamedetector-0.1.3/gamedetector/app_exes.json` & `gamedetector-0.1.4/gamedetector/app_exes.json`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.3/gamedetector/game_detect.py` & `gamedetector-0.1.4/gamedetector/game_detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,23 +437,23 @@
         game_version = check_launcher_settings_json(game_folder)
 
     logging.info(f"Detected game version: '{game_version or 'Unknown'}'")
     if game_appid is not None:
         game = SteamGame(
             name=game_name,
             publisher=game_publisher,
-            version=get_game_executables,
+            version=game_version,
             path=game_folder,
             appid=game_appid,
         )
     else:
         game = NonSteamGame(
             name=game_name,
             publisher=game_publisher,
-            version=get_game_executables,
+            version=game_version,
             path=game_folder,
         )
     return game
 
 
 def main() -> str:
     # Open a folder select dialog and return Steam appid if game is detected.
```

### Comparing `gamedetector-0.1.3/LICENSE` & `gamedetector-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.3/pyproject.toml` & `gamedetector-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gamedetector"
-version = "0.1.3"
+version = "0.1.4"
 description = "The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version."
 authors = ["Aareon Sullivan <askully13@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gamedetector-0.1.3/README.md` & `gamedetector-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.3/PKG-INFO` & `gamedetector-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamedetector
-Version: 0.1.3
+Version: 0.1.4
 Summary: The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version.
 License: MIT
 Author: Aareon Sullivan
 Author-email: askully13@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

