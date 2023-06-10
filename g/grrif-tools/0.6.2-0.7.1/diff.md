# Comparing `tmp/grrif_tools-0.6.2.tar.gz` & `tmp/grrif_tools-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.6.2.tar", last modified: Wed May 24 20:45:41 2023, max compression
+gzip compressed data, was "grrif_tools-0.7.1.tar", last modified: Sat Jun 10 16:08:02 2023, max compression
```

## Comparing `grrif_tools-0.6.2.tar` & `grrif_tools-0.7.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/grrif_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/grrif_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/grrif_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/grrif_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:08:02.861634 grrif_tools-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-10 16:08:02.861634 grrif_tools-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:08:02.861634 grrif_tools-0.7.1/grrif_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/grrif_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/grrif_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/grrif_tools/grrif_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/grrif_tools/grrif_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/grrif_tools/grrif_scrobbler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/grrif_tools/grrif_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:08:02.861634 grrif_tools-0.7.1/grrif_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-10 16:08:02.000000 grrif_tools-0.7.1/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-10 16:08:02.000000 grrif_tools-0.7.1/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:08:02.000000 grrif_tools-0.7.1/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 16:08:02.000000 grrif_tools-0.7.1/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-10 16:08:02.000000 grrif_tools-0.7.1/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 16:08:02.000000 grrif_tools-0.7.1/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:08:02.861634 grrif_tools-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-10 16:07:54.000000 grrif_tools-0.7.1/setup.py
```

### Comparing `grrif_tools-0.6.2/LICENSE` & `grrif_tools-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.2/PKG-INFO` & `grrif_tools-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grrif_tools
-Version: 0.6.2
+Version: 0.7.1
 Summary: An unofficial set of tools for Cool Cats™.
 Home-page: https://github.com/fetzu/grrif-tools
 Download-URL: https://github.com/fetzu/grrif-tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: MIT License
         
         Copyright (c) 2023 Julien 'fetzu' Bono
@@ -34,25 +34,26 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GRRIF Tools
 
-A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database (or text files), compute/display some stats (top 10/25/100 artists and tracks), ~~and scrobble it to last.fm~~ (upcoming).
+A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database (or text files), compute/display some stats (top 10/25/100 artists and tracks), stream the radio live in your console,~~and scrobble it to last.fm~~ (upcoming).
 
 ```
 usage: grrif_tools [-h] {archive,stats,scrobble} ...
 
 A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming).
 
 positional arguments:
   {archive,stats,scrobble}
     archive             Archive GRRIF's play history.
     stats               Get some stats out of the database.
+    play                Streams GRRIF to the console and displays the currently playing track.
     scrobble            Scrobble to Last.fm.
 
 options:
   -h, --help            show this help message and exit
   ```
   
   **NOTE:** This package is unofficial and meant mostly as a playground to experiment with some new things (argparse, python packaging, etc...). Please do not DDoS GRRIF's website !
```

### Comparing `grrif_tools-0.6.2/README.md` & `grrif_tools-0.7.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # GRRIF Tools
 
-A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database (or text files), compute/display some stats (top 10/25/100 artists and tracks), ~~and scrobble it to last.fm~~ (upcoming).
+A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database (or text files), compute/display some stats (top 10/25/100 artists and tracks), stream the radio live in your console,~~and scrobble it to last.fm~~ (upcoming).
 
 ```
 usage: grrif_tools [-h] {archive,stats,scrobble} ...
 
 A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming).
 
 positional arguments:
   {archive,stats,scrobble}
     archive             Archive GRRIF's play history.
     stats               Get some stats out of the database.
+    play                Streams GRRIF to the console and displays the currently playing track.
     scrobble            Scrobble to Last.fm.
 
 options:
   -h, --help            show this help message and exit
   ```
   
   **NOTE:** This package is unofficial and meant mostly as a playground to experiment with some new things (argparse, python packaging, etc...). Please do not DDoS GRRIF's website !
```

### Comparing `grrif_tools-0.6.2/grrif_tools/cli.py` & `grrif_tools-0.7.1/grrif_tools/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### [ GRRIF Tools by Julien 'fetzu' Bono ]
 ## [ IMPORTS ]
 import sys
 import argparse
 from datetime import date, datetime
 
 ## [ CONFIGURATION ]
-__version__ = "0.6.2"
+__version__ = "0.7.1"
 
 ## [ Is CLI even cooler with argparse? ]
 parser = argparse.ArgumentParser(
     description="A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming)."
 )
 
 subparsers = parser.add_subparsers(dest="command")
@@ -89,14 +89,25 @@
 scrobble_parser.add_argument(
     "to_date",
     nargs="?",
     default=date.today().strftime("%Y-%m-%d"),
     help=f"Specify the start date for the archive in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')}).",
 )
 
+stream_parser = subparsers.add_parser(
+    "play",
+    help="Play GRRIF in your terminal!",
+).add_argument(
+    "quality",
+    choices=["mp3_high", "mp3_low", "aac_high"],
+    nargs="?",
+    default="mp3_high",
+    help="Specify streaming quality (default: mp3_high)",
+)
+
 args = parser.parse_args()
 
 
 ## [ MAIN ]
 def main():
     print(
         "##########################################\n"
@@ -105,20 +116,21 @@
     )
 
     # Displays argparse's help message if no arguments are given
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
 
-    # Set the base URL to scrape data from
-    BASE_URL = "https://www.grrif.ch/recherche-de-titres/?date={}"
-
-    # Set the date range to scrape data for
-    START_DATE = datetime.strptime(args.from_date, "%Y-%m-%d")
-    END_DATE = datetime.strptime(args.to_date, "%Y-%m-%d")
+    if args.command == "archive" or args.command == "stats":
+        # Set the base URL to scrape data from
+        BASE_URL = "https://www.grrif.ch/recherche-de-titres/?date={}"
+
+        # Set the date range to scrape data for
+        START_DATE = datetime.strptime(args.from_date, "%Y-%m-%d")
+        END_DATE = datetime.strptime(args.to_date, "%Y-%m-%d")
 
     # Archive was passed !
     if args.command == "archive":
         # The "save to SQLite database" option was chosen
         if args.destination == "db":
             # Let the user know what we are attempting
             print(
@@ -154,29 +166,35 @@
             # Import the necessary functions
             from .grrif_archiver import plays_to_stdout
 
             # Create/open the database
             plays_to_stdout(BASE_URL, START_DATE, END_DATE)
 
     # Stats was passed !
-    # Import the necessary functions
-    from .grrif_stats import topofthepop
-
-    if args.stats_command == "artists":
-        if args.topofthepop == "top10":
-            topofthepop("artist", "10", START_DATE, END_DATE)
-        if args.topofthepop == "top25":
-            topofthepop("artist", "25", START_DATE, END_DATE)
-        if args.topofthepop == "top100":
-            topofthepop("artist", "100", START_DATE, END_DATE)
-
-    if args.stats_command == "tracks":
-        if args.topofthepop == "top10":
-            topofthepop("artist, title", "10", START_DATE, END_DATE)
-        if args.topofthepop == "top25":
-            topofthepop("artist, title", "25", START_DATE, END_DATE)
-        if args.topofthepop == "top100":
-            topofthepop("title", "100", START_DATE, END_DATE)
+    if args.command == "stats":
+        # Import the necessary functions
+        from .grrif_stats import topofthepop
+
+        if args.stats_command == "artists":
+            if args.topofthepop == "top10":
+                topofthepop("artist", "10", START_DATE, END_DATE)
+            if args.topofthepop == "top25":
+                topofthepop("artist", "25", START_DATE, END_DATE)
+            if args.topofthepop == "top100":
+                topofthepop("artist", "100", START_DATE, END_DATE)
+
+        if args.stats_command == "tracks":
+            if args.topofthepop == "top10":
+                topofthepop("artist, title", "10", START_DATE, END_DATE)
+            if args.topofthepop == "top25":
+                topofthepop("artist, title", "25", START_DATE, END_DATE)
+            if args.topofthepop == "top100":
+                topofthepop("title", "100", START_DATE, END_DATE)
 
     # Scrobble was passed !
     if args.command == "scrobble":
         print("Uh-oh, this doesn't exist yet!")
+
+    # Play was passed !
+    if args.command == "play":
+        from .grrif_player import start_playback
+        start_playback(args.quality)
```

### Comparing `grrif_tools-0.6.2/grrif_tools/grrif_archiver.py` & `grrif_tools-0.7.1/grrif_tools/grrif_archiver.py`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.2/grrif_tools/grrif_stats.py` & `grrif_tools-0.7.1/grrif_tools/grrif_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+GRRIF Stats helper functions
+"""
+
 import os
 import sqlite3
 from .grrif_archiver import database_handler
 
 # connect to the SQLite database
 database_path = database_handler()
 conn = sqlite3.connect(database_path)
```

### Comparing `grrif_tools-0.6.2/grrif_tools.egg-info/PKG-INFO` & `grrif_tools-0.7.1/grrif_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grrif-tools
-Version: 0.6.2
+Version: 0.7.1
 Summary: An unofficial set of tools for Cool Cats™.
 Home-page: https://github.com/fetzu/grrif-tools
 Download-URL: https://github.com/fetzu/grrif-tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: MIT License
         
         Copyright (c) 2023 Julien 'fetzu' Bono
@@ -34,25 +34,26 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GRRIF Tools
 
-A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database (or text files), compute/display some stats (top 10/25/100 artists and tracks), ~~and scrobble it to last.fm~~ (upcoming).
+A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database (or text files), compute/display some stats (top 10/25/100 artists and tracks), stream the radio live in your console,~~and scrobble it to last.fm~~ (upcoming).
 
 ```
 usage: grrif_tools [-h] {archive,stats,scrobble} ...
 
 A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming).
 
 positional arguments:
   {archive,stats,scrobble}
     archive             Archive GRRIF's play history.
     stats               Get some stats out of the database.
+    play                Streams GRRIF to the console and displays the currently playing track.
     scrobble            Scrobble to Last.fm.
 
 options:
   -h, --help            show this help message and exit
   ```
   
   **NOTE:** This package is unofficial and meant mostly as a playground to experiment with some new things (argparse, python packaging, etc...). Please do not DDoS GRRIF's website !
```

### Comparing `grrif_tools-0.6.2/pyproject.toml` & `grrif_tools-0.7.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [project]
 name = "grrif_tools"
-version = "0.6.2"
+version = "0.7.1"
 authors = [
   { name="Julien 'fetzu' Bono" },
 ]
 description = "An unofficial set of tools for Cool Cats™."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "Requests==2.30.0",
-    "beautifulsoup4==4.11.1",
+    "Requests==2.31.0",
+    "beautifulsoup4==4.12.2",
     "titlecase==2.4",
+    "miniaudio==1.57",
 ]
 
 [project.entry-points.'console_scripts']
 grrif_tools = "grrif_tools.cli:main"
 
 [project.urls]
 "Homepage" = "https://github.com/fetzu/grrif-tools"
```

### Comparing `grrif_tools-0.6.2/setup.py` & `grrif_tools-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 setup(
     name="grrif_tools",
     description="An unofficial set of tools for Cool Cats™.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Julien 'fetzu' Bono",
     url="https://github.com/fetzu/grrif-tools",
-    version="0.6.2",
+    version="0.7.1",
     download_url="https://github.com/fetzu/grrif-tools/releases/latest",
     packages=find_packages(include=["grrif_tools", "grrif_tools.*"]),
     license="License :: OSI Approved :: MIT License",
     install_requires=[
-        "Requests==2.30.0",
-        "beautifulsoup4==4.11.1",
+        "Requests==2.31.0",
+        "beautifulsoup4==4.12.2",
         "titlecase==2.4",
+        "miniaudio==1.57",
     ],
     entry_points={"console_scripts": ["grrif_tools=grrif_tools.cli:main"]},
 )
```

