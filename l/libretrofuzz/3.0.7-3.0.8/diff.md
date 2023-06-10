# Comparing `tmp/libretrofuzz-3.0.7.tar.gz` & `tmp/libretrofuzz-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.0.7.tar", max compression
+gzip compressed data, was "libretrofuzz-3.0.8.tar", max compression
```

## Comparing `libretrofuzz-3.0.7.tar` & `libretrofuzz-3.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/LICENSE
--rw-r--r--   0        0        0     7682 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/README.rst
--rw-r--r--   0        0        0       22 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    54358 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-10 12:08:31.042414 libretrofuzz-3.0.7/pyproject.toml
--rw-r--r--   0        0        0     8859 2023-06-10 12:08:43.427276 libretrofuzz-3.0.7/setup.py
--rw-r--r--   0        0        0     8870 2023-06-10 12:08:43.428208 libretrofuzz-3.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-10 17:26:38.503949 libretrofuzz-3.0.8/LICENSE
+-rw-r--r--   0        0        0     7682 2023-06-10 17:26:38.503949 libretrofuzz-3.0.8/README.rst
+-rw-r--r--   0        0        0       22 2023-06-10 17:26:38.503949 libretrofuzz-3.0.8/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    53143 2023-06-10 17:26:38.503949 libretrofuzz-3.0.8/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-10 17:26:38.503949 libretrofuzz-3.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8859 2023-06-10 17:26:49.411842 libretrofuzz-3.0.8/setup.py
+-rw-r--r--   0        0        0     8870 2023-06-10 17:26:49.412775 libretrofuzz-3.0.8/PKG-INFO
```

### Comparing `libretrofuzz-3.0.7/LICENSE` & `libretrofuzz-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.0.7/README.rst` & `libretrofuzz-3.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.0.7/libretrofuzz/__main__.py` & `libretrofuzz-3.0.8/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,57 +280,57 @@
 
 
 # -------------------------------------------------------------------
 # The heart of the program, what orders titles to be 'more similar'
 # or less to the local labels (after the normalization)
 # -------------------------------------------------------------------
 class TitleScorer(object):
-    def __init__(self):
+    def __init__(self, subtitles):
         # rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way)
         # so it uses internal api to prevent a possible early exit at == 100
         self._RF_ScorerPy = {
             "get_scorer_flags": lambda **kwargs: {
                 "optimal_score": MAX_SCORE,
                 "worst_score": 0,
                 "flags": (1 << 6),
             }
         }
+        self.subtitles = subtitles
+
+    def check_full_match(self, name, other_name):
+        candidates = []
+        other_subs = self.subtitles[other_name]
+        for sub in other_subs:
+            if name == sub:
+                candidates.append(200 - len(other_subs) + 1)
+            else:
+                len_ratio = min(len(name), len(sub)) / max(len(name), len(sub))
+                heuristic = len(os.path.commonprefix([name, sub])) * len_ratio
+                candidates.append(fuzz.WRatio(name, sub) + heuristic)
+        len_ratio = min(len(name), len(other_name)) / max(len(name), len(other_name))
+        heuristic = len(os.path.commonprefix([name, other_name])) * len_ratio
+        candidates.append(fuzz.WRatio(name, other_name) + heuristic)
+        return max(candidates)
 
     def __call__(self, s1, s2, processor=None, score_cutoff=None):
-        # if a short title is completely contained in another
-        # token_set_ratio gives that 100. Add the length ratio
-        # which will give the rate of 'similar length'
-        len_ratio = min(len(s1), len(s2)) / max(len(s1), len(s2))
-
-        # add a heuristic to give primacy to larger start of string similarity
-        # multiplied by the length similarity, so at low length ratio
-        # you get less than at high.
-        heuristic = len(os.path.commonprefix([s1, s2])) * len_ratio
-
-        # score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
-        # 1. the caller of this, extract passes the 'current best score' as score_cutoff
-        # 2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
-        # 3. 'current best score' includes the prefix, which this call can't include in 2.
-        similarity = fuzz.token_set_ratio(s1, s2, processor=None, score_cutoff=0)
-        # print(similarity + len_ratio + hs_prefix)
-        return min(MAX_SCORE - 1, similarity + heuristic)
+        return self.check_full_match(s1, s2)
 
 
 # ---------------------------------------------------------------
 # Normalization functions, part of the functions that change both
 # local labels and remote names to be more similar to compare
 # ---------------------------------------------------------------
 # word splitter regex, wont even attempt to explain how and why
 camelcase_pattern = regex.compile(
     r"((?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|(?<=[0-9])(?=[A-Z][a-z])|(?<=[a-zA-Z])(?=[0-9]))"
 )
 # number sequences that start with 0
 zero_lead_pattern = regex.compile(r"([^\d])0+([1-9])")
 # all symbols except some used later
-almost_symbols_pattern = regex.compile(r"([\p{P}--',])")
+almost_symbols_pattern = regex.compile(r"([[:punct:]--',])")
 
 
 def normalizer(nometa, hack, t):
     if nometa:
         t = removeparenthesis(t, "(", ")")
     if not hack:
         t = removeparenthesis(t, "[", "]")
@@ -343,15 +343,14 @@
     # but may occur in the local name. Do this before camelcase
     # split because its hard to do a regex that allows splitting
     # Word-Word or Word:Word without creating new subtitle
     # and removing articles from subtitles is helpful anyway
     subtitles = t.split(" - ")
     if len(subtitles) == 1:
         subtitles = t.split(": ")
-    new_t = []
     for i, st in enumerate(subtitles):
         # remove all symbols, except, ',' and '''
         # this needs to be here for all the names
         # to be operating on the same base for definite articles
         st = regex.sub(almost_symbols_pattern, "", st)
         # CamelCaseNames for local labels are common when there are no spaces
         # do this to normalize for definite articles
@@ -417,35 +416,17 @@
         st = st.replace("iv", "4")
         st = st.replace("v", "5")
         st = st.replace("ix", "9")
         st = st.replace("x", "10")
         st = st.replace("i", "1")
         # remove diacritics (not to asian languages diacritics, only for 2 to 1 character combinations)
         st = "".join([c for c in unicodedata.normalize("NFKD", st) if not unicodedata.combining(c)])
-        # remove spaces for the strings. but keep the index/main string with spaces
-        # rapidfuzz algorithms needs them to tokenize
-        st = st.strip().split()
-        new_t.append(" ".join(st))
-        subtitles[i] = "".join(st)
-    return " ".join(new_t), subtitles
-
-
-def check_full_match(name_subs, subtitlemap, namemap):
-    # A hack to take care of those that are either exactly equal
-    # or are exactly equal to one and only one subtitle
-    result = []
-    nameaux_nospaces = "".join(name_subs)
-    for key, ns_list in subtitlemap.items():
-        if "".join(ns_list) == nameaux_nospaces:
-            result.append((namemap[key], MAX_SCORE, key))
-        elif len(ns_list) > 1:
-            for sub in ns_list:
-                if sub == nameaux_nospaces:
-                    result.append((namemap[key], MAX_SCORE, key))
-    return result
+        st = " ".join(st.strip().split())
+        subtitles[i] = st
+    return " ".join(subtitles), subtitles
 
 
 # ---------------------------------------------------------------------------------
 # Initalization functions, since there are two main programs so the code is reused
 # ---------------------------------------------------------------------------------
 class RzipReader(object):
     """used to abstract the libretro compressed playlist format"""
@@ -962,32 +943,32 @@
     short_names = os.getenv("SHORT")
     short_names = True if short_names and short_names != "0" else False
     strfy_runtime = partial(strfy, score, short_names, nub_verbose)
     norm = partial(normalizer, nometa, hack)
     failure = 0
     success = 0
 
-    title_scorer = TitleScorer()
     # we choose the highest similarity of all 3 directories,
     # since no mixed matches are allowed
     # (until you call again without --no-merge anyway)
     remote_names = set()
     remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
     # preprocess data for speed and to make
     # exact matches (for total name or subtitle)
     # not involved in the fuzz function.
     # turn into a dict, original key and
-    # (normalized value, [normalized value nospaces,... possible subtitles nospace])
+    # (normalized value, [possible subtitles normalized nospace])
     subtitle = dict()
     mappings = dict()
     for x in remote_names:
         normstr, lst = norm(x)
-        subtitle[x] = lst
+        subtitle[normstr] = lst
         mappings[x] = normstr
     remote_names = mappings
+    title_scorer = TitleScorer(subtitle)
 
     for name, destination in names:
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
@@ -1006,24 +987,22 @@
 
         # only the local names should have forbidden characters
         # this is the character libretro server uses to replace
         name = regex.sub(forbidden, "_", name)
         nameaux = regex.sub(forbidden, "_", nameaux)
 
         # unlike the server thumbnails, normalization wasn't done yet
-        (nameaux, nameaux_subs) = norm(nameaux)
-        # this checks if the name has a full match among
-        # the normalized names or the normalized subtitles
-        result = check_full_match(nameaux_subs, subtitle, remote_names)
-        if not result:
-            # operate on cache (to speed up by not applying normalization every iteration)
-            # normalization can make it so that the winner has the same score as the runner up(s)
-            # so to make sure we catch at least two candidates for cases where that happens
-            # it's a improvement because sometimes server thumbnail types have case letter typos
-            result = process.extract(nameaux, remote_names, scorer=title_scorer, limit=verbose or 2)
+        (nameaux, namesubs) = norm(nameaux)
+        if nameaux not in subtitle:
+            subtitle[nameaux] = namesubs
+
+        # normalization can make it so that the winner has the same score as the runner up(s)
+        # so to make sure we catch at least two candidates for cases where that happens
+        # it's a improvement because sometimes server thumbnail types have case letter typos
+        result = process.extract(nameaux, remote_names, scorer=title_scorer, limit=verbose or 2)
         _, max_score, _ = (result and result[0]) or (None, -1, None)
         winners = [x for x in result if x[1] == max_score and x[1] >= score]
         show = result if verbose else winners
         name_format = style((nameaux if short_names else name) + ": ", bold=True)
         if winners:
             allow = True
             # these parent directories were created when reading the playlist
```

### Comparing `libretrofuzz-3.0.7/pyproject.toml` & `libretrofuzz-3.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.0.7"
+version = "3.0.8"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.0.7/setup.py` & `libretrofuzz-3.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.0.7',
+    'version': '3.0.8',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.0.7/PKG-INFO` & `libretrofuzz-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.0.7
+Version: 3.0.8
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

