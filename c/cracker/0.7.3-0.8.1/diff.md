# Comparing `tmp/cracker-0.7.3.tar.gz` & `tmp/cracker-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cracker-0.7.3.tar", last modified: Sun May 28 18:03:37 2023, max compression
+gzip compressed data, was "cracker-0.8.1.tar", last modified: Sat Jun 10 19:54:47 2023, max compression
```

## Comparing `cracker-0.7.3.tar` & `cracker-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.319802 cracker-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.307801 cracker-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.311801 cracker-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-28 18:03:23.000000 cracker-0.7.3/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-28 18:03:23.000000 cracker-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 18:03:23.000000 cracker-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 18:03:23.000000 cracker-0.7.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-28 18:03:37.319802 cracker-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-28 18:03:23.000000 cracker-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.311801 cracker-0.7.3/cracker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/config/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/parser.json
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/cracker_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/icon.jpeg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/keylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/mp3_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/speaker/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/abstract_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/espeak.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/polly.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/ssml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/tests/test_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/config_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/parser_config_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/speaker_config_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-28 18:03:23.000000 cracker-0.7.3/docs/macos.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 18:03:23.000000 cracker-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 18:03:37.319802 cracker-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.319802 cracker-0.7.3/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-28 18:03:23.000000 cracker-0.7.3/ubuntu/cracker.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-28 18:03:23.000000 cracker-0.7.3/ubuntu/icon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-05-28 18:03:23.000000 cracker-0.7.3/ubuntu/install_ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.905080 cracker-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.897080 cracker-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.901080 cracker-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-10 19:54:35.000000 cracker-0.8.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-10 19:54:35.000000 cracker-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 19:54:35.000000 cracker-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-10 19:54:35.000000 cracker-0.8.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-10 19:54:47.905080 cracker-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-10 19:54:35.000000 cracker-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.901080 cracker-0.8.1/cracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.901080 cracker-0.8.1/cracker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/config/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/config/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/config/parser.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/cracker_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/icon.jpeg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/keylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/mp3_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.905080 cracker-0.8.1/cracker/speaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/speaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/speaker/abstract_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/speaker/espeak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/speaker/frogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/speaker/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/speaker/polly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/ssml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.905080 cracker-0.8.1/cracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/tests/test_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.905080 cracker-0.8.1/cracker/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/view/config_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/view/parser_config_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-10 19:54:35.000000 cracker-0.8.1/cracker/view/speaker_config_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.901080 cracker-0.8.1/cracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-10 19:54:47.000000 cracker-0.8.1/cracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-10 19:54:47.000000 cracker-0.8.1/cracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:54:47.000000 cracker-0.8.1/cracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-10 19:54:47.000000 cracker-0.8.1/cracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 19:54:47.000000 cracker-0.8.1/cracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 19:54:47.000000 cracker-0.8.1/cracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.905080 cracker-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-10 19:54:35.000000 cracker-0.8.1/docs/macos.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 19:54:35.000000 cracker-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:54:47.905080 cracker-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:54:47.905080 cracker-0.8.1/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-10 19:54:35.000000 cracker-0.8.1/ubuntu/cracker.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-10 19:54:35.000000 cracker-0.8.1/ubuntu/icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-06-10 19:54:35.000000 cracker-0.8.1/ubuntu/install_ubuntu.sh
```

### Comparing `cracker-0.7.3/.github/workflows/publish-pypi.yml` & `cracker-0.8.1/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/LICENSE` & `cracker-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/PKG-INFO` & `cracker-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.3
+Version: 0.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.3/README.md` & `cracker-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/config/configuration.py` & `cracker-0.8.1/cracker/config/configuration.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/config/parser.json` & `cracker-0.8.1/cracker/config/parser.json`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/cracker.py` & `cracker-0.8.1/cracker/cracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from PyQt5.QtWidgets import QApplication
 
 from cracker.config import Configuration
 from cracker.cracker_gui import MainWindow
 from cracker.keylogger import KeyBoardManager
 from cracker.speaker.abstract_speaker import AbstractSpeaker
 from cracker.speaker.espeak import Espeak
+from cracker.speaker.frogger import Frogger
 from cracker.speaker.google import Google
 from cracker.speaker.polly import Polly
 from cracker.text_parser import TextParser
 from cracker.utils import get_logger
 
 
 class Cracker(object):
     """Logic for running the Cracker program"""
 
-    SPEAKER = {Polly.__name__: Polly, Espeak.__name__: Espeak, Google.__name__: Google}
+    SPEAKER = {p.__name__.lower(): p for p in [Polly, Espeak, Google, Frogger]}
     _logger = get_logger(__name__)
 
     def __init__(self, app: QApplication):
         super().__init__()
         self.app = app
 
         self.config = Configuration()
@@ -45,25 +46,31 @@
     def _close(self):
         "Handles closing whole application"
         self.key_manager.stop()
 
     def get_speaker(self, speaker_name, player) -> AbstractSpeaker:
         config = self.config.read_config()
         _name = speaker_name.lower()
+        speaker = self.SPEAKER.get(_name)
         if _name == Polly.__name__.lower():
             self._logger.info("Using AWS Polly")
             return Polly(player)
         elif _name == Google.__name__.lower():
             self._logger.info("Using Google TTS")
             credentials_file = config.get("google", {}).get("credentials_file")
             self._logger.debug("Using credentials file: %s", credentials_file)
             return Google(player, credentials_file)
         elif _name == Espeak.__name__.lower():
             self._logger.info("Using ESpeak")
             return Espeak(player)
+        elif _name == Frogger.__name__.lower():
+            self._logger.info("Using Frogger")
+            return Frogger(player)
+        # if speaker:
+        #     return speaker(player)
         raise ValueError(f"No speaker was selected. Provided speaker name '{speaker_name}'")
 
     def run(self):
         self.gui.init()
         self.set_action()
         self.gui.show()
 
@@ -117,14 +124,15 @@
         if self.player.state() == QMediaPlayer.PausedState:
             self.player.play()
         else:
             self.player.pause()
 
     def stop_text(self):
         self.speaker.stop_text()
+        self.player.stop()
 
     def _prepare_config(self):
         config = dict(rate=self.gui.rate, volume=self.gui.volume, voice=self.gui.config.voice)
         return config
 
     def change_speaker(self, speaker_name):
         """Action on changing speaker.
```

### Comparing `cracker-0.7.3/cracker/cracker_gui.py` & `cracker-0.8.1/cracker/cracker_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         super().__init__()
 
         self.resize(800, 250)
         self.setWindowTitle("Cracker GUI")
 
         self.config = config
 
+        self.speaker = None
         self.speakers = speakers
         self.speaker: Optional[AbstractSpeaker] = None
         self.player: Optional[QMediaPlayer] = None
 
         self.config_window = ConfigWindow()
 
     def init(self):
@@ -137,19 +138,20 @@
         # LAYOUT
         layout = QVBoxLayout(self.mainWidget)
         menuLayout = QGridLayout()
 
         # Speaker - label and widget
         assert self.config.speaker, "Speaker needs to be defined"
 
+        _speakers = [k.capitalize() for k in self.speakers.keys()]
         self.speakerLabel = QLabel("Speaker:")
         self.speakerW = QComboBox(self)
-        self.speakerW.addItems(self.speakers.keys())
+        self.speakerW.addItems(_speakers)
         self.speakerW.setMinimumContentsLength(10)
-        self.speakerW.setCurrentIndex(list(self.speakers.keys()).index(self.config.speaker.capitalize()))
+        self.speakerW.setCurrentIndex(_speakers.index(self.config.speaker.capitalize()))
         self.speakerW.currentTextChanged.connect(self.change_speaker)
         menuLayout.addWidget(self.speakerLabel, 0, 0)
         menuLayout.addWidget(self.speakerW, 1, 0)
 
         # Voice - label and selector
         self.speedLabel = QLabel("Speed:")
         self.speedW = QSpinBox()
@@ -200,28 +202,29 @@
         self.change_volume(self.volumeW.value())
         self.change_speed(self.speedW.value())
         self.change_language(self.config.language)
 
     def closeEvent(self, close_event):
         """Triggers CloseEvent and handles closing gracefully"""
         self.closeAppEvent.emit()
-        del self.speaker
+        if hasattr(self, "speaker"):
+            del self.speaker
         self.close()
 
     def save_config(self):
         self._logger.debug("Saving user config")
         self.config.save_user_config()
 
     def change_speaker(self, speaker_name: str):
         """Action on changing speaker.
 
         Important: Each speaker has its own configuration.
         These values should be updated on change.
         """
-        self.speaker = self.speakers[speaker_name](self.player)
+        self.speaker = self.speakers[speaker_name.lower()](self.player)
         self.config.speaker = speaker_name
         self.config.load_speaker_config(speaker_name)
         self.init_values()
 
     def change_volume(self, volume):
         """Volume should be on a percentage scale"""
         assert self.speaker, "Speaker doesn't exist. Can't change volume."
```

### Comparing `cracker-0.7.3/cracker/icon.jpeg` & `cracker-0.8.1/cracker/icon.jpeg`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/icon.png` & `cracker-0.8.1/cracker/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/keylogger.py` & `cracker-0.8.1/cracker/keylogger.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/main.py` & `cracker-0.8.1/cracker/main.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/mp3_helper.py` & `cracker-0.8.1/cracker/mp3_helper.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/speaker/abstract_speaker.py` & `cracker-0.8.1/cracker/speaker/abstract_speaker.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/speaker/espeak.py` & `cracker-0.8.1/cracker/speaker/espeak.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(self, player):
         self.player = player
 
     def __del__(self):
         self.stop_text()
 
     def read_text(self, text: str, **config) -> None:
-        self._logger.debug("Reading test: %s", text)
+        self._logger.debug("Reading text: %s", text)
         filepath = os.path.abspath(AbstractSpeaker.TMP_FILEPATH)
         command = ["espeak"]
         command += self._process_config(**config)
         command += ["-w", filepath]
         command.append("'{}'".format(self.clean_text(text)))
         subprocess.call(command)
         self.play_file(filepath)
```

### Comparing `cracker-0.7.3/cracker/speaker/google.py` & `cracker-0.8.1/cracker/speaker/google.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/speaker/polly.py` & `cracker-0.8.1/cracker/speaker/polly.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/ssml.py` & `cracker-0.8.1/cracker/ssml.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/tests/test_config.py` & `cracker-0.8.1/cracker/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/tests/test_text_parser.py` & `cracker-0.8.1/cracker/tests/test_text_parser.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/text_parser.py` & `cracker-0.8.1/cracker/text_parser.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/themes.py` & `cracker-0.8.1/cracker/themes.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/utils.py` & `cracker-0.8.1/cracker/utils.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/view/config_window.py` & `cracker-0.8.1/cracker/view/config_window.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/view/parser_config_tab.py` & `cracker-0.8.1/cracker/view/parser_config_tab.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker/view/speaker_config_tab.py` & `cracker-0.8.1/cracker/view/speaker_config_tab.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/cracker.egg-info/PKG-INFO` & `cracker-0.8.1/cracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.3
+Version: 0.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.3/cracker.egg-info/SOURCES.txt` & `cracker-0.8.1/cracker.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 cracker/config/__init__.py
 cracker/config/configuration.py
 cracker/config/default.yaml
 cracker/config/parser.json
 cracker/speaker/__init__.py
 cracker/speaker/abstract_speaker.py
 cracker/speaker/espeak.py
+cracker/speaker/frogger.py
 cracker/speaker/google.py
 cracker/speaker/polly.py
 cracker/tests/test_config.py
 cracker/tests/test_text_parser.py
 cracker/view/__init__.py
 cracker/view/config_window.py
 cracker/view/parser_config_tab.py
```

### Comparing `cracker-0.7.3/pyproject.toml` & `cracker-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/ubuntu/icon.png` & `cracker-0.8.1/ubuntu/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.3/ubuntu/install_ubuntu.sh` & `cracker-0.8.1/ubuntu/install_ubuntu.sh`

 * *Files identical despite different names*

