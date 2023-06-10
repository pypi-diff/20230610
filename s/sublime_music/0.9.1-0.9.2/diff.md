# Comparing `tmp/sublime-music-0.9.1.tar.gz` & `tmp/sublime-music-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sublime-music-0.9.1.tar", last modified: Mon Apr 27 04:08:17 2020, max compression
+gzip compressed data, was "dist/sublime-music-0.9.2.tar", last modified: Sun May 24 22:58:58 2020, max compression
```

## Comparing `sublime-music-0.9.1.tar` & `sublime-music-0.9.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     1870 2020-04-27 04:08:17.000000 sublime-music-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1041 2020-04-27 04:05:22.000000 sublime-music-0.9.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1218 2020-04-27 04:08:17.000000 sublime-music-0.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2613 2020-04-27 04:05:22.000000 sublime-music-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime/
--rw-rw-rw-   0 root         (0) root         (0)       22 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    39972 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/app.py
--rw-rw-rw-   0 root         (0) root         (0)    41671 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/cache_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4853 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/config.py
--rw-rw-rw-   0 root         (0) root         (0)    13879 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/dbus_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2979 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/from_json.py
--rw-rw-rw-   0 root         (0) root         (0)    15959 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/players.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime/server/
--rw-rw-rw-   0 root         (0) root         (0)      136 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/server/api_object.py
--rw-rw-rw-   0 root         (0) root         (0)    14920 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/server/api_objects.py
--rw-rw-rw-   0 root         (0) root         (0)    51515 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/server/server.py
--rw-rw-rw-   0 root         (0) root         (0)     8933 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/state_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22020 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/albums.py
--rw-rw-rw-   0 root         (0) root         (0)     3488 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/app_styles.css
--rw-rw-rw-   0 root         (0) root         (0)    17613 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/artists.py
--rw-rw-rw-   0 root         (0) root         (0)    15007 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/browse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime/ui/common/
--rw-rw-rw-   0 root         (0) root         (0)      372 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10730 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/common/album_with_songs.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/common/edit_form_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/common/icon_button.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/common/song_list_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1393 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/common/spinner_image.py
--rw-rw-rw-   0 root         (0) root         (0)     9385 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/configure_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime/ui/images/
--rw-rw-rw-   0 root         (0) root         (0)     3845 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/images/default-album-art.png
--rw-rw-rw-   0 root         (0) root         (0)      903 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/images/play-queue-play.png
--rw-rw-rw-   0 root         (0) root         (0)    16586 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime/ui/mpris_specs/
--rw-rw-rw-   0 root         (0) root         (0)    28131 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Player.xml
--rw-rw-rw-   0 root         (0) root         (0)    10137 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Playlists.xml
--rw-rw-rw-   0 root         (0) root         (0)    14928 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.TrackList.xml
--rw-rw-rw-   0 root         (0) root         (0)     8820 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.xml
--rw-rw-rw-   0 root         (0) root         (0)    28544 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/player_controls.py
--rw-rw-rw-   0 root         (0) root         (0)    28450 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/playlists.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11832 2020-04-27 04:05:22.000000 sublime-music-0.9.1/sublime/ui/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime_music.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1870 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime_music.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1328 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime_music.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime_music.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime_music.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      170 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime_music.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2020-04-27 04:08:17.000000 sublime-music-0.9.1/sublime_music.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)     1889 2020-05-24 22:58:58.000000 sublime-music-0.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2020-05-24 22:56:02.000000 sublime-music-0.9.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2020-05-24 22:58:58.000000 sublime-music-0.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2655 2020-05-24 22:56:02.000000 sublime-music-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39972 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    41676 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/cache_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5121 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    13879 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/dbus_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/from_json.py
+-rw-rw-rw-   0 root         (0) root         (0)    15959 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/players.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime/server/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/server/api_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    14920 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/server/api_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    51515 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/server/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8933 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/state_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22020 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/albums.py
+-rw-rw-rw-   0 root         (0) root         (0)     3488 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/app_styles.css
+-rw-rw-rw-   0 root         (0) root         (0)    17613 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/artists.py
+-rw-rw-rw-   0 root         (0) root         (0)    15007 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/browse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime/ui/common/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10730 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/common/album_with_songs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/common/edit_form_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/common/icon_button.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/common/song_list_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/common/spinner_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9385 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/configure_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime/ui/images/
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/images/default-album-art.png
+-rw-rw-rw-   0 root         (0) root         (0)      903 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/images/play-queue-play.png
+-rw-rw-rw-   0 root         (0) root         (0)    16586 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime/ui/mpris_specs/
+-rw-rw-rw-   0 root         (0) root         (0)    28131 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Player.xml
+-rw-rw-rw-   0 root         (0) root         (0)    10137 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Playlists.xml
+-rw-rw-rw-   0 root         (0) root         (0)    14928 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.TrackList.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8820 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.xml
+-rw-rw-rw-   0 root         (0) root         (0)    28544 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/player_controls.py
+-rw-rw-rw-   0 root         (0) root         (0)    28450 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/playlists.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11832 2020-05-24 22:56:02.000000 sublime-music-0.9.2/sublime/ui/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime_music.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1889 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime_music.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1328 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime_music.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime_music.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime_music.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime_music.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2020-05-24 22:58:58.000000 sublime-music-0.9.2/sublime_music.egg-info/top_level.txt
```

### Comparing `sublime-music-0.9.1/PKG-INFO` & `sublime-music-0.9.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sublime-music
-Version: 0.9.1
+Version: 0.9.2
 Summary: A native GTK *sonic client.
 Home-page: https://gitlab.com/sumner/sublime-music
 Author: Sumner Evans
 Author-email: inquiries@sumnerevans.com
 License: GPL3
-Description: .. image:: https://gitlab.com/sumner/sublime-music/-/raw/master/docs/logo/logo.png
+Description: .. image:: https://gitlab.com/sumner/sublime-music/-/raw/master/logo/logo.png
            :alt: Sublime Music Logo
         
         Sublime Music is a GTK3
         `Subsonic`_/`Airsonic`_/`Revel`_/`Gonic`_/`Navidrome`_/\*sonic client for the
         Linux Desktop.
         
         .. _Subsonic: http://www.subsonic.org/pages/index.jsp
@@ -38,7 +38,8 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: keyring
```

### Comparing `sublime-music-0.9.1/README.rst` & `sublime-music-0.9.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. image:: https://gitlab.com/sumner/sublime-music/-/raw/master/docs/logo/logo.png
+.. image:: https://gitlab.com/sumner/sublime-music/-/raw/master/logo/logo.png
    :alt: Sublime Music Logo
 
 Sublime Music is a GTK3
 `Subsonic`_/`Airsonic`_/`Revel`_/`Gonic`_/`Navidrome`_/\*sonic client for the
 Linux Desktop.
 
 .. _Subsonic: http://www.subsonic.org/pages/index.jsp
```

### Comparing `sublime-music-0.9.1/setup.cfg` & `sublime-music-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/setup.py` & `sublime-music-0.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,24 +55,27 @@
         ]
     },
     install_requires=[
         'bottle',
         'deepdiff',
         'Deprecated',
         'fuzzywuzzy',
-        'keyring',
         'osxmmkeys ; sys_platform=="darwin"',
         'pychromecast',
         'PyGObject',
         'python-dateutil',
         'python-Levenshtein',
         'python-mpv',
         'pyyaml',
         'requests',
     ],
+    extras_require={
+        "keyring": ["keyring"],
+    },
+
 
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and
     # allow pip to create the appropriate form of executable for the target
     # platform.
     entry_points={
         'console_scripts': [
```

### Comparing `sublime-music-0.9.1/sublime/__main__.py` & `sublime-music-0.9.2/sublime/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         '-l',
         '--logfile',
         help='the filename to send logs to',
     )
     parser.add_argument(
         '-m',
         '--loglevel',
-        help='the minium level of logging to do',
+        help='the minimum level of logging to do',
         default='WARNING',
     )
     parser.add_argument(
         '-c',
         '--config',
         help='specify a configuration file. Defaults to '
         '~/.config/sublime-music/config.json',
```

### Comparing `sublime-music-0.9.1/sublime/app.py` & `sublime-music-0.9.2/sublime/app.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/cache_manager.py` & `sublime-music-0.9.2/sublime/cache_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
                     except requests.exceptions.ConnectionError:
                         with self.download_set_lock:
                             self.current_downloads.discard(abs_path_str)
 
                     # Move the file to its cache download location.
                     os.makedirs(abs_path.parent, exist_ok=True)
                     if download_path.exists():
-                        shutil.move(download_path, abs_path)
+                        shutil.move(str(download_path), abs_path)
 
                 logging.info(f'{abs_path} downloaded. Returning.')
                 return abs_path_str
 
             def after_download(path: str):
                 with self.download_set_lock:
                     self.current_downloads.discard(path)
```

### Comparing `sublime-music-0.9.1/sublime/config.py` & `sublime-music-0.9.2/sublime/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import logging
 import os
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
-import keyring
+try:
+    import keyring
+
+    has_keyring = True
+except ImportError:
+    has_keyring = False
 
 
 class ReplayGainType(Enum):
     NO = 0
     TRACK = 1
     ALBUM = 2
 
@@ -52,39 +57,45 @@
         self.local_network_ssid = local_network_ssid
         self.username = username
         self.sync_enabled = sync_enabled
         self.disable_cert_verify = disable_cert_verify
 
         # Try to save the password in the keyring, but if we can't, then save
         # it in the config JSON.
-        try:
-            keyring.set_password(
-                'com.sumnerevans.SublimeMusic',
-                f'{self.username}@{self.server_address}',
-                password,
-            )
-        except Exception:
+        if not has_keyring:
             self._password = password
+        else:
+            try:
+                keyring.set_password(
+                    'com.sumnerevans.SublimeMusic',
+                    f'{self.username}@{self.server_address}',
+                    password,
+                )
+            except Exception:
+                self._password = password
 
     def migrate(self):
         # Try and migrate to use the system keyring, but if it fails, then we
         # don't care.
-        if self._password:
+        if self._password and has_keyring:
             try:
                 keyring.set_password(
                     'com.sumnerevans.SublimeMusic',
                     f'{self.username}@{self.server_address}',
                     self._password,
                 )
                 self._password = None
             except Exception:
                 pass
 
     @property
     def password(self) -> str:
+        if not has_keyring:
+            return self._password
+
         try:
             return keyring.get_password(
                 'com.sumnerevans.SublimeMusic',
                 f'{self.username}@{self.server_address}',
             )
         except Exception:
             return self._password
```

### Comparing `sublime-music-0.9.1/sublime/dbus_manager.py` & `sublime-music-0.9.2/sublime/dbus_manager.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/from_json.py` & `sublime-music-0.9.2/sublime/from_json.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/players.py` & `sublime-music-0.9.2/sublime/players.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/server/api_object.py` & `sublime-music-0.9.2/sublime/server/api_object.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/server/api_objects.py` & `sublime-music-0.9.2/sublime/server/api_objects.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/server/server.py` & `sublime-music-0.9.2/sublime/server/server.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/state_manager.py` & `sublime-music-0.9.2/sublime/state_manager.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/albums.py` & `sublime-music-0.9.2/sublime/ui/albums.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/app_styles.css` & `sublime-music-0.9.2/sublime/ui/app_styles.css`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/artists.py` & `sublime-music-0.9.2/sublime/ui/artists.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/browse.py` & `sublime-music-0.9.2/sublime/ui/browse.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/common/album_with_songs.py` & `sublime-music-0.9.2/sublime/ui/common/album_with_songs.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/common/edit_form_dialog.py` & `sublime-music-0.9.2/sublime/ui/common/edit_form_dialog.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/common/icon_button.py` & `sublime-music-0.9.2/sublime/ui/common/icon_button.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/common/song_list_column.py` & `sublime-music-0.9.2/sublime/ui/common/song_list_column.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/common/spinner_image.py` & `sublime-music-0.9.2/sublime/ui/common/spinner_image.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/configure_servers.py` & `sublime-music-0.9.2/sublime/ui/configure_servers.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/images/default-album-art.png` & `sublime-music-0.9.2/sublime/ui/images/default-album-art.png`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/images/play-queue-play.png` & `sublime-music-0.9.2/sublime/ui/images/play-queue-play.png`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/main.py` & `sublime-music-0.9.2/sublime/ui/main.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Player.xml` & `sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Player.xml`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Playlists.xml` & `sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.Playlists.xml`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.TrackList.xml` & `sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.TrackList.xml`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.xml` & `sublime-music-0.9.2/sublime/ui/mpris_specs/org.mpris.MediaPlayer2.xml`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/player_controls.py` & `sublime-music-0.9.2/sublime/ui/player_controls.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/playlists.py` & `sublime-music-0.9.2/sublime/ui/playlists.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/settings.py` & `sublime-music-0.9.2/sublime/ui/settings.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime/ui/util.py` & `sublime-music-0.9.2/sublime/ui/util.py`

 * *Files identical despite different names*

### Comparing `sublime-music-0.9.1/sublime_music.egg-info/PKG-INFO` & `sublime-music-0.9.2/sublime_music.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sublime-music
-Version: 0.9.1
+Version: 0.9.2
 Summary: A native GTK *sonic client.
 Home-page: https://gitlab.com/sumner/sublime-music
 Author: Sumner Evans
 Author-email: inquiries@sumnerevans.com
 License: GPL3
-Description: .. image:: https://gitlab.com/sumner/sublime-music/-/raw/master/docs/logo/logo.png
+Description: .. image:: https://gitlab.com/sumner/sublime-music/-/raw/master/logo/logo.png
            :alt: Sublime Music Logo
         
         Sublime Music is a GTK3
         `Subsonic`_/`Airsonic`_/`Revel`_/`Gonic`_/`Navidrome`_/\*sonic client for the
         Linux Desktop.
         
         .. _Subsonic: http://www.subsonic.org/pages/index.jsp
@@ -38,7 +38,8 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: keyring
```

### Comparing `sublime-music-0.9.1/sublime_music.egg-info/SOURCES.txt` & `sublime-music-0.9.2/sublime_music.egg-info/SOURCES.txt`

 * *Files identical despite different names*

