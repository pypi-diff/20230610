# Comparing `tmp/libretrofuzz-3.0.6.tar.gz` & `tmp/libretrofuzz-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.0.6.tar", max compression
+gzip compressed data, was "libretrofuzz-3.0.7.tar", max compression
```

## Comparing `libretrofuzz-3.0.6.tar` & `libretrofuzz-3.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/LICENSE
--rw-r--r--   0        0        0     7682 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/README.rst
--rw-r--r--   0        0        0       22 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    54164 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/pyproject.toml
--rw-r--r--   0        0        0     8859 2023-06-10 04:49:32.177276 libretrofuzz-3.0.6/setup.py
--rw-r--r--   0        0        0     8870 2023-06-10 04:49:32.178208 libretrofuzz-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/LICENSE
+-rw-r--r--   0        0        0     7682 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/README.rst
+-rw-r--r--   0        0        0       22 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    54358 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8859 2023-06-10 12:08:43.427276 libretrofuzz-3.0.7/setup.py
+-rw-r--r--   0        0        0     8870 2023-06-10 12:08:43.428208 libretrofuzz-3.0.7/PKG-INFO
```

### Comparing `libretrofuzz-3.0.6/LICENSE` & `libretrofuzz-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.0.6/README.rst` & `libretrofuzz-3.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.0.6/libretrofuzz/__main__.py` & `libretrofuzz-3.0.7/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from functools import partial
 from itertools import chain
 from struct import unpack
 import json
 import os
 import sys
 import io
-import regex
 import zlib
 import fnmatch
 import collections
 import shutil
 import unicodedata
 import asyncio
 import subprocess
@@ -42,14 +41,17 @@
 from bs4 import BeautifulSoup
 from questionary import Style, select
 from httpx import RequestError, HTTPStatusError, Client, AsyncClient
 from tqdm import trange, tqdm
 from typer.colors import YELLOW, RED, BLUE, GREEN
 from typer import style, echo, run, Exit, Argument, Option
 from prompt_toolkit.input import create_input
+import regex
+
+regex.DEFAULT_VERSION = regex.VERSION1
 
 # stop showing the variables - a library installed this behind my back
 try:
     from rich.traceback import install
 
     install(show_locals=False)
 except ImportError:
@@ -232,32 +234,27 @@
     if label is None:
         label = uri
     # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
     escape_mask = "\033]8;{};{}\033\\{}\033]8;;\033\\"
     return escape_mask.format(parameters, uri, label)
 
 
-ppatterns = {"()": regex.compile(r"\([^)(]*\)"), "[]": regex.compile(r"\[[^][]*\]")}
-
-
-def removeparenthesis(s, open_p="(", close_p=")"):
-    nb_rep = 1
-    key = open_p + close_p
-    try:
-        pattern = ppatterns[key]
-    except:
-        pattern = regex.compile(rf"\{open_p}[^{close_p}{open_p}]*\{close_p}")
-        ppatterns[key] = pattern
-    while nb_rep:
-        (s, nb_rep) = regex.subn(pattern, "", s)
-    return s
-
-
-spatterns = {" - ": regex.compile(r".*( - .*)"), ": ": regex.compile(r".*(: .*)")}
-before_metadata = regex.compile(r"(^[^[({]*)")
+def removeparenthesis(input_str, open_p="(", close_p=")"):
+    result = ""
+    paren_level = 0
+    for ch in input_str:
+        if ch == open_p:
+            paren_level += 1
+        elif (ch == close_p) and paren_level:
+            paren_level -= 1
+        elif not paren_level:
+            result += ch
+    if paren_level != 0:
+        error(f"'{input_str}' has a unclosed parenthesis")
+    return result
 
 
 def replacemany(our_str, to_be_replaced, replace_with):
     for nextchar in to_be_replaced:
         our_str = our_str.replace(nextchar, replace_with)
     return our_str
 
@@ -324,39 +321,44 @@
 # ---------------------------------------------------------------
 # word splitter regex, wont even attempt to explain how and why
 camelcase_pattern = regex.compile(
     r"((?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|(?<=[0-9])(?=[A-Z][a-z])|(?<=[a-zA-Z])(?=[0-9]))"
 )
 # number sequences that start with 0
 zero_lead_pattern = regex.compile(r"([^\d])0+([1-9])")
-# all symbols
-all_symbols_pattern = regex.compile(r"(\p{P})")
+# all symbols except some used later
+almost_symbols_pattern = regex.compile(r"([\p{P}--',])")
 
 
 def normalizer(nometa, hack, t):
     if nometa:
         t = removeparenthesis(t, "(", ")")
     if not hack:
         t = removeparenthesis(t, "[", "]")
     # replace the default character representing illegal chars
     # in the libretro database by space
     t = t.replace("_", " ")
     # remove any number of leading 0s that ends in a digit
     t = regex.sub(zero_lead_pattern, r"\1\2", t)
-    # split subtitles. The second is forbidden in server names
+    # split subtitles. ': ' is forbidden in server names
     # but may occur in the local name. Do this before camelcase
     # split because its hard to do a regex that allows splitting
     # Word-Word or Word:Word without creating new subtitle
+    # and removing articles from subtitles is helpful anyway
     subtitles = t.split(" - ")
     if len(subtitles) == 1:
         subtitles = t.split(": ")
     new_t = []
     for i, st in enumerate(subtitles):
+        # remove all symbols, except, ',' and '''
+        # this needs to be here for all the names
+        # to be operating on the same base for definite articles
+        st = regex.sub(almost_symbols_pattern, "", st)
         # CamelCaseNames for local labels are common when there are no spaces
-        # do this to normalize definite articles
+        # do this to normalize for definite articles
         st = " ".join([a for s in regex.split(camelcase_pattern, st) if s and (a := s.strip())])
         # normalize case
         st = st.lower()
         # beginning and end definite articles in several european languages (people move them)
         # make sure we're only removing the start and end forms with spaces
         st = removefirst(st, ", the")
         st = removeprefix(st, "the ")
@@ -385,20 +387,20 @@
         st = removeprefix(st, "os ")
         st = removefirst(st, ", as")
         st = removeprefix(st, "as ")
         st = removefirst(st, ", o")
         st = removeprefix(st, "o ")
         st = removefirst(st, ", a")
         st = removeprefix(st, "a ")
+        # finally get rid of the rest
+        st = replacemany(st, ",'", "")
         # if a remote name has ' and ' instead of ' _ ' to replace ' & ' make it work
         st = st.replace(" and ", " ")
         # and why not
         st = st.replace(" the ", " ")
-        # remove all symbols
-        st = regex.sub(all_symbols_pattern, "", st)
         # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
         # If both str tested have roman numerals no harm done if XXIV gets turned into 204.
         st = st.replace("xviii", "18")
         st = st.replace("xvii", "17")
         st = st.replace("xvi", "16")
         st = st.replace("xiii", "13")
         st = st.replace("xii", "12")
@@ -989,19 +991,18 @@
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
 
         # to simplify this code, the forbidden characters are replaced twice, on the string
         # that is going to be the filename and the string copy that is going to be matched.
         nameaux = name
-
         #'before' has priority over subtitle removal
         if before:
             # Ignore metadata and get the string before it
-            name_without_meta = regex.search(before_metadata, nameaux)
+            name_without_meta = regex.search(r"(^[^\[({]*)", nameaux)
             if name_without_meta:
                 before_index = name_without_meta.group(1).find(before)
                 if before_index != -1:
                     nameaux = nameaux[0:before_index]
 
         # only the local names should have forbidden characters
         # this is the character libretro server uses to replace
```

### Comparing `libretrofuzz-3.0.6/pyproject.toml` & `libretrofuzz-3.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.0.6"
+version = "3.0.7"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.0.6/setup.py` & `libretrofuzz-3.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.0.6',
+    'version': '3.0.7',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.0.6/PKG-INFO` & `libretrofuzz-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.0.6
+Version: 3.0.7
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

