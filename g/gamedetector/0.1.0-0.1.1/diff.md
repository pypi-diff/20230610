# Comparing `tmp/gamedetector-0.1.0.tar.gz` & `tmp/gamedetector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamedetector-0.1.0.tar", max compression
+gzip compressed data, was "gamedetector-0.1.1.tar", max compression
```

## Comparing `gamedetector-0.1.0.tar` & `gamedetector-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.1.0/gamedetector/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-09 18:22:23.018869 gamedetector-0.1.0/gamedetector/app_exes.json
--rw-r--r--   0        0        0    15294 2023-06-10 18:58:13.203059 gamedetector-0.1.0/gamedetector/game_detect.py
--rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.1.0/LICENSE
--rw-r--r--   0        0        0      805 2023-06-10 18:25:31.944556 gamedetector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-09 18:24:36.455517 gamedetector-0.1.0/README.md
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 gamedetector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 17:01:09.805215 gamedetector-0.1.1/gamedetector/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-09 18:22:23.018869 gamedetector-0.1.1/gamedetector/app_exes.json
+-rw-r--r--   0        0        0    15551 2023-06-10 19:25:11.892081 gamedetector-0.1.1/gamedetector/game_detect.py
+-rw-r--r--   0        0        0     1093 2023-06-08 17:00:52.471193 gamedetector-0.1.1/LICENSE
+-rw-r--r--   0        0        0      805 2023-06-10 19:15:54.347952 gamedetector-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-09 18:24:36.455517 gamedetector-0.1.1/README.md
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 gamedetector-0.1.1/PKG-INFO
```

### Comparing `gamedetector-0.1.0/gamedetector/app_exes.json` & `gamedetector-0.1.1/gamedetector/app_exes.json`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.0/gamedetector/game_detect.py` & `gamedetector-0.1.1/gamedetector/game_detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,17 +265,20 @@
 def check_launcher_settings_json(game_folder: Path) -> str | None:
     """Get game version from `launcher-settings.json`.
     Created to detect Prison Architect as a last ditch effort."""
     game_version = None
     logging.debug("Checking for `launcher-settings.json`")
     for fp in game_folder.glob("**/*.json"):
         if fp.name.endswith("launcher-settings.json"):
-            with open(fp) as f:
-                game_version = json.load(f)["version"]
-                return game_version
+            try:
+                with open(fp) as f:
+                    game_version = json.load(f)["version"]
+                    return game_version
+            except UnicodeDecodeError as e:
+                logging.debug(f"An error occurred reading `launcher-settings.json`. Error: {str(e)}", exc_info=True)
 
 
 def get_game_name(
     game_folder: Path, game_version: str = None, delimiter: str = "."
 ) -> str:
     """Using the path to a game, get the game name."""
     if game_version and game_version in game_folder.name:
@@ -411,20 +414,21 @@
         # attempt to remove launcher binaries and check version on left over EXE (if 1)
         no_launchers = [
             exe for exe in possible_exes if "launcher" not in exe.name.lower()
         ]
         logging.debug(f"EXEs not including launchers: {no_launchers}")
         # fuzzy match best choice
         if game_version is None:
-            for exe in no_launchers:
-                m = fuzz.find_near_matches(game_name, exe.name, max_l_dist=1)
-                if m:
-                    logging.debug(f"Fuzzy matched EXE: `{exe}`, match: {m}")
-                    logging.debug("Attempting to get version number using win32 api")
-                    game_version = get_version_number(exe)
+            if len(no_launchers) != 0:
+                for exe in no_launchers:
+                    m = fuzz.find_near_matches(game_name, exe.name, max_l_dist=1)
+                    if m:
+                        logging.debug(f"Fuzzy matched EXE: `{exe}`, match: {m}")
+                        logging.debug("Attempting to get version number using win32 api")
+                        game_version = get_version_number(exe)
 
     if game_version is None:
         # Some games offer `launcher-settings.json` (i.e. Prison Architect)
         game_version = check_launcher_settings_json(game_folder)
 
     logging.info(f"Detected game version: '{game_version or 'Unknown'}'")
     return game_name
```

### Comparing `gamedetector-0.1.0/LICENSE` & `gamedetector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.0/pyproject.toml` & `gamedetector-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gamedetector"
-version = "0.1.0"
+version = "0.1.1"
 description = "The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version."
 authors = ["Aareon Sullivan <askully13@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gamedetector-0.1.0/README.md` & `gamedetector-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gamedetector-0.1.0/PKG-INFO` & `gamedetector-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamedetector
-Version: 0.1.0
+Version: 0.1.1
 Summary: The GameDetector library allows you to detect a game within a folder, returning information like Steam AppId, game name, and version.
 License: MIT
 Author: Aareon Sullivan
 Author-email: askully13@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

