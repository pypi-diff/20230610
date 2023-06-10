# Comparing `tmp/gamedetector-0.1.1.tar.gz` & `tmp/gamedetector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamedetector-0.1.1.tar", max compression
+gzip compressed data, was "gamedetector-0.1.3.tar", max compression
```

## Comparing `gamedetector-0.1.1.tar` & `gamedetector-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.1.1/gamedetector/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-09 18:22:23.018869 gamedetector-0.1.1/gamedetector/app_exes.json
--rw-r--r--   0        0        0    15551 2023-06-10 19:25:11.892081 gamedetector-0.1.1/gamedetector/game_detect.py
--rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.1.1/LICENSE
--rw-r--r--   0        0        0      805 2023-06-10 19:15:54.347952 gamedetector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-09 18:24:36.455517 gamedetector-0.1.1/README.md
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 gamedetector-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.1.3/gamedetector/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-09 18:22:23.018869 gamedetector-0.1.3/gamedetector/app_exes.json
+-rw-r--r--   0        0        0    16162 2023-06-10 19:37:18.622896 gamedetector-0.1.3/gamedetector/game_detect.py
+-rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.1.3/LICENSE
+-rw-r--r--   0        0        0      805 2023-06-10 19:37:49.498852 gamedetector-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-09 18:24:36.455517 gamedetector-0.1.3/README.md
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 gamedetector-0.1.3/PKG-INFO
```

### Comparing `gamedetector-0.1.1/gamedetector/app_exes.json` & `gamedetector-0.1.3/gamedetector/app_exes.json`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.1/gamedetector/game_detect.py` & `gamedetector-0.1.3/gamedetector/game_detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,18 @@
     for fp in game_folder.glob("**/*.json"):
         if fp.name.endswith("launcher-settings.json"):
             try:
                 with open(fp) as f:
                     game_version = json.load(f)["version"]
                     return game_version
             except UnicodeDecodeError as e:
-                logging.debug(f"An error occurred reading `launcher-settings.json`. Error: {str(e)}", exc_info=True)
+                logging.debug(
+                    f"An error occurred reading `launcher-settings.json`. Error: {str(e)}",
+                    exc_info=True,
+                )
 
 
 def get_game_name(
     game_folder: Path, game_version: str = None, delimiter: str = "."
 ) -> str:
     """Using the path to a game, get the game name."""
     if game_version and game_version in game_folder.name:
@@ -329,37 +332,38 @@
 
     for game in app_list["applist"]["apps"]:
         if game["appid"] == appid:
             game_name = game["name"]
             return game_name
 
 
-def detect_folder(game_folder: Path) -> str:
+def detect_folder(game_folder: Path) -> SteamGame | NonSteamGame:
     """Perform detection on a game folder.
 
     Args:
         [Optional] game_folder: Path
     Returns:
         game_name: str
     """
-    game_appid = None
-    game_version = None
     game_name = None
+    game_publisher = None
+    game_version = None
+    game_appid = None
 
     app_list = get_app_list()
     logging.debug("Got app_list, proceeding...")
 
     # Check for `steam_emu.ini`
     game_appid = check_steam_emu(game_folder)
     if game_appid is None:
         # Check `steam_appid.txt`
         game_appid = check_appid_txt(game_folder)
         if game_appid is None:
             # Check for `app.info`
-            _, game_name = check_app_info(game_folder)
+            game_publisher, game_name = check_app_info(game_folder)
             if game_name is not None:
                 game_appid = get_appid_from_name(game_name, app_list)
                 logging.debug(f"Found `app.info` - AppId: {game_appid}")
         else:
             logging.debug(f"Found `steam_appid.txt` - AppId: {game_appid}")
     else:
         logging.debug(f"Found `steam_emu.ini` - AppId: {game_appid}")
@@ -419,23 +423,40 @@
         # fuzzy match best choice
         if game_version is None:
             if len(no_launchers) != 0:
                 for exe in no_launchers:
                     m = fuzz.find_near_matches(game_name, exe.name, max_l_dist=1)
                     if m:
                         logging.debug(f"Fuzzy matched EXE: `{exe}`, match: {m}")
-                        logging.debug("Attempting to get version number using win32 api")
+                        logging.debug(
+                            "Attempting to get version number using win32 api"
+                        )
                         game_version = get_version_number(exe)
 
     if game_version is None:
         # Some games offer `launcher-settings.json` (i.e. Prison Architect)
         game_version = check_launcher_settings_json(game_folder)
 
     logging.info(f"Detected game version: '{game_version or 'Unknown'}'")
-    return game_name
+    if game_appid is not None:
+        game = SteamGame(
+            name=game_name,
+            publisher=game_publisher,
+            version=get_game_executables,
+            path=game_folder,
+            appid=game_appid,
+        )
+    else:
+        game = NonSteamGame(
+            name=game_name,
+            publisher=game_publisher,
+            version=get_game_executables,
+            path=game_folder,
+        )
+    return game
 
 
 def main() -> str:
     # Open a folder select dialog and return Steam appid if game is detected.
     game_folder = Path(filedialog.askdirectory())
     logging.info(f"Game folder selected: {game_folder.name}")
     detect_folder(game_folder)
```

### Comparing `gamedetector-0.1.1/LICENSE` & `gamedetector-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.1/pyproject.toml` & `gamedetector-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gamedetector"
-version = "0.1.1"
+version = "0.1.3"
 description = "The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version."
 authors = ["Aareon Sullivan <askully13@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gamedetector-0.1.1/README.md` & `gamedetector-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.1/PKG-INFO` & `gamedetector-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamedetector
-Version: 0.1.1
+Version: 0.1.3
 Summary: The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version.
 License: MIT
 Author: Aareon Sullivan
 Author-email: askully13@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

