# Comparing `tmp/libretrofuzz-3.0.4.tar.gz` & `tmp/libretrofuzz-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.0.4.tar", max compression
+gzip compressed data, was "libretrofuzz-3.0.6.tar", max compression
```

## Comparing `libretrofuzz-3.0.4.tar` & `libretrofuzz-3.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-09 09:53:51.009614 libretrofuzz-3.0.4/LICENSE
--rw-r--r--   0        0        0     8014 2023-06-09 09:53:51.009614 libretrofuzz-3.0.4/README.rst
--rw-r--r--   0        0        0       22 2023-06-09 09:53:51.009614 libretrofuzz-3.0.4/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    54744 2023-06-09 09:53:51.009614 libretrofuzz-3.0.4/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-09 09:53:51.009614 libretrofuzz-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     9194 2023-06-09 09:54:03.482013 libretrofuzz-3.0.4/setup.py
--rw-r--r--   0        0        0     9202 2023-06-09 09:54:03.483170 libretrofuzz-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/LICENSE
+-rw-r--r--   0        0        0     7682 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/README.rst
+-rw-r--r--   0        0        0       22 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    54164 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-10 04:49:21.932704 libretrofuzz-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8859 2023-06-10 04:49:32.177276 libretrofuzz-3.0.6/setup.py
+-rw-r--r--   0        0        0     8870 2023-06-10 04:49:32.178208 libretrofuzz-3.0.6/PKG-INFO
```

### Comparing `libretrofuzz-3.0.4/LICENSE` & `libretrofuzz-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.0.4/README.rst` & `libretrofuzz-3.0.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 If you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.
 
 Besides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.
 
 If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
 
 Example:
- | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``
- | then
- | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``
+ | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``
 
  The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.
 
 Note that the system name you download from doesn't have to be the same as the playlist name.
 
 If the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.
 
@@ -29,18 +27,18 @@
  ``libretro-fuzz --no-meta --no-merge``
 
  After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.
  Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.
 
 Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.
 
-False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
+False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
 
 Example:
-  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``
+  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``
 
   The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
 To debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.
 
 libretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]
   :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.
@@ -61,15 +59,14 @@
                         | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
   --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
-  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
   --verbose N           | Show length N list: score, name, emoji hyperlinks.
                         | [x>=1]
```

### Comparing `libretrofuzz-3.0.4/libretrofuzz/__main__.py` & `libretrofuzz-3.0.6/libretrofuzz/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -252,30 +252,14 @@
     return s
 
 
 spatterns = {" - ": regex.compile(r".*( - .*)"), ": ": regex.compile(r".*(: .*)")}
 before_metadata = regex.compile(r"(^[^[({]*)")
 
 
-def nosubtitle_aux(t, subtitle_marker=" - "):
-    # last subtitle marker and everything there until the
-    # end, last because i noticed that 'subsubtitles' exist
-    # for instance, ultima 7 - part 1|2 - subtitle
-    try:
-        pattern = spatterns[subtitle_marker]
-    except:
-        pattern = regex.compile(rf".*({subtitle_marker}.*)")
-        spatterns[subtitle_marker] = pattern
-    name_without_meta = regex.search(before_metadata, t)
-    subtitle = regex.search(pattern, name_without_meta.group(1) if name_without_meta else t)
-    if subtitle:
-        t = t[0 : subtitle.start(1)] + " " + t[subtitle.end(1) :]
-    return t
-
-
 def replacemany(our_str, to_be_replaced, replace_with):
     for nextchar in to_be_replaced:
         our_str = our_str.replace(nextchar, replace_with)
     return our_str
 
 
 def removefirst(name: str, suf: str):
@@ -311,134 +295,155 @@
                 "optimal_score": MAX_SCORE,
                 "worst_score": 0,
                 "flags": (1 << 6),
             }
         }
 
     def __call__(self, s1, s2, processor=None, score_cutoff=None):
-        # names are whitespace and case normalized, but they keep spaces
-        # for token_set_ratio. But still test this case, since it's common
-        if s1 == s2 or "".join(s1.split()) == "".join(s2.split()):
-            return MAX_SCORE
-
-        # since many games do not have images, they get caught up
-        # on a short title being completely contained in another
+        # if a short title is completely contained in another
         # token_set_ratio gives that 100. Add the length ratio
-        # which will give slight primacy to 'similar length' strings'
+        # which will give the rate of 'similar length'
         len_ratio = min(len(s1), len(s2)) / max(len(s1), len(s2))
-        # common prefix heuristic to give priority to longer similar names
-        # helps on cases where the first game in a series was winning sequels
-        # is counter productive in some cases where the series name comes first
-        hs_prefix = len(os.path.commonprefix([s1, s2]))
+
+        # add a heuristic to give primacy to larger start of string similarity
+        # multiplied by the length similarity, so at low length ratio
+        # you get less than at high.
+        heuristic = len(os.path.commonprefix([s1, s2])) * len_ratio
 
         # score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
         # 1. the caller of this, extract passes the 'current best score' as score_cutoff
         # 2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
         # 3. 'current best score' includes the prefix, which this call can't include in 2.
         similarity = fuzz.token_set_ratio(s1, s2, processor=None, score_cutoff=0)
         # print(similarity + len_ratio + hs_prefix)
-        return min(MAX_SCORE - 1, similarity + len_ratio + hs_prefix)
+        return min(MAX_SCORE - 1, similarity + heuristic)
 
 
 # ---------------------------------------------------------------
 # Normalization functions, part of the functions that change both
 # local labels and remote names to be more similar to compare
 # ---------------------------------------------------------------
-camelcase_pattern = regex.compile(r"(\p{Lu}\p{Ll}+(?>(?:(?:'s)|(?:'em))?))")
-# number sequences in the middle (not start or end) of a string that start with 0
+# word splitter regex, wont even attempt to explain how and why
+camelcase_pattern = regex.compile(
+    r"((?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|(?<=[0-9])(?=[A-Z][a-z])|(?<=[a-zA-Z])(?=[0-9]))"
+)
+# number sequences that start with 0
 zero_lead_pattern = regex.compile(r"([^\d])0+([1-9])")
+# all symbols
+all_symbols_pattern = regex.compile(r"(\p{P})")
 
 
-def normalizer(t, nometa, hack):
+def normalizer(nometa, hack, t):
     if nometa:
         t = removeparenthesis(t, "(", ")")
     if not hack:
         t = removeparenthesis(t, "[", "]")
-    # change all common ascci symbol characters we aren't going to use after this (, and ')
-    t = replacemany(t, '_()[]{}-.!?#"', "")
-    # strips just because the user may have made a mistake naming the source
-    # (or the replacement above introduce boundary spaces)
-    t = t.strip()
-    # remove any number leading 0, except at the end or the start of the string
-    # where it is likely a important part of the name, not a file manager sort workaround
+    # replace the default character representing illegal chars
+    # in the libretro database by space
+    t = t.replace("_", " ")
+    # remove any number of leading 0s that ends in a digit
     t = regex.sub(zero_lead_pattern, r"\1\2", t)
-    # CamelCaseNames for local labels are common when there are no spaces, split them
-    # do this to normalize definite articles in normalization with spaces only (minimizes changes)
-    # print(regex.split(camelcase_pattern, t))
-    t = " ".join([s.strip() for s in regex.split(camelcase_pattern, t) if s and s.strip()])
-    # normalize case
-    t = t.lower()
-    # beginning and end definite articles in several european languages (people move them)
-    # make sure we're only removing the start and end forms with spaces
-    t = removefirst(t, ", the")
-    t = removeprefix(t, "the ")
-    t = removefirst(t, ", los")
-    t = removeprefix(t, "los ")
-    t = removefirst(t, ", las")
-    t = removeprefix(t, "las ")
-    t = removefirst(t, ", les")
-    t = removeprefix(t, "les ")
-    t = removefirst(t, ", le")
-    t = removeprefix(t, "le ")
-    t = removefirst(t, ", la")
-    t = removeprefix(t, "la ")
-    t = removefirst(t, ", l'")
-    # L' sometimes ommits the space so always remove L' at the start even without space
-    t = removeprefix(t, "l'")  # if there is a extra space the next join will remove it
-    t = removefirst(t, ", der")
-    t = removeprefix(t, "der ")
-    t = removefirst(t, ", die")
-    t = removeprefix(t, "die ")
-    t = removefirst(t, ", das")
-    t = removeprefix(t, "das ")
-    t = removefirst(t, ", el")
-    t = removeprefix(t, "el ")
-    t = removefirst(t, ", os")
-    t = removeprefix(t, "os ")
-    t = removefirst(t, ", as")
-    t = removeprefix(t, "as ")
-    t = removefirst(t, ", o")
-    t = removeprefix(t, "o ")
-    t = removefirst(t, ", a")
-    t = removeprefix(t, "a ")
-    # remove the symbols used in the definite article normalization and word splitting
-    t = replacemany(t, ",'“”\"", "")
-    # this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
-    #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
-    t = t.replace(" and ", " ")
-    # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
-    # If both str tested have roman numerals no harm done if XXIV gets turned into 204.
-    t = t.replace("xviii", "18")
-    t = t.replace("xvii", "17")
-    t = t.replace("xvi", "16")
-    t = t.replace("xiii", "13")
-    t = t.replace("xii", "12")
-    t = t.replace("xiv", "14")
-    t = t.replace("xv", "15")
-    t = t.replace("xix", "19")
-    t = t.replace("xx", "20")
-    t = t.replace("xi", "11")
-    t = t.replace("viii", "8")
-    t = t.replace("vii", "7")
-    t = t.replace("vi", "6")
-    t = t.replace("iii", "3")
-    t = t.replace("ii", "2")
-    t = t.replace("iv", "4")
-    t = t.replace("v", "5")
-    t = t.replace("ix", "9")
-    t = t.replace("x", "10")
-    t = t.replace("i", "1")
-    # remove diacritics (not to asian languages diacritics, only for 2 to 1 character combinations)
-    t = "".join([c for c in unicodedata.normalize("NFKD", t) if not unicodedata.combining(c)])
-    # normalize spaces (don't remove them for other later score methods to be able to reorder tokens)
-    return " ".join(t.split())
-
-
-def nosubtitle_normalizer(t, nometa, hack):
-    return normalizer(nosubtitle_aux(t), nometa, hack)
+    # split subtitles. The second is forbidden in server names
+    # but may occur in the local name. Do this before camelcase
+    # split because its hard to do a regex that allows splitting
+    # Word-Word or Word:Word without creating new subtitle
+    subtitles = t.split(" - ")
+    if len(subtitles) == 1:
+        subtitles = t.split(": ")
+    new_t = []
+    for i, st in enumerate(subtitles):
+        # CamelCaseNames for local labels are common when there are no spaces
+        # do this to normalize definite articles
+        st = " ".join([a for s in regex.split(camelcase_pattern, st) if s and (a := s.strip())])
+        # normalize case
+        st = st.lower()
+        # beginning and end definite articles in several european languages (people move them)
+        # make sure we're only removing the start and end forms with spaces
+        st = removefirst(st, ", the")
+        st = removeprefix(st, "the ")
+        st = removefirst(st, ", los")
+        st = removeprefix(st, "los ")
+        st = removefirst(st, ", las")
+        st = removeprefix(st, "las ")
+        st = removefirst(st, ", les")
+        st = removeprefix(st, "les ")
+        st = removefirst(st, ", le")
+        st = removeprefix(st, "le ")
+        st = removefirst(st, ", la")
+        st = removeprefix(st, "la ")
+        st = removefirst(st, ", l'")
+        # L' sometimes ommits the space so always remove L' at the start even without space
+        st = removeprefix(st, "l'")  # if there is a extra space the next strip will remove it
+        st = removefirst(st, ", der")
+        st = removeprefix(st, "der ")
+        st = removefirst(st, ", die")
+        st = removeprefix(st, "die ")
+        st = removefirst(st, ", das")
+        st = removeprefix(st, "das ")
+        st = removefirst(st, ", el")
+        st = removeprefix(st, "el ")
+        st = removefirst(st, ", os")
+        st = removeprefix(st, "os ")
+        st = removefirst(st, ", as")
+        st = removeprefix(st, "as ")
+        st = removefirst(st, ", o")
+        st = removeprefix(st, "o ")
+        st = removefirst(st, ", a")
+        st = removeprefix(st, "a ")
+        # if a remote name has ' and ' instead of ' _ ' to replace ' & ' make it work
+        st = st.replace(" and ", " ")
+        # and why not
+        st = st.replace(" the ", " ")
+        # remove all symbols
+        st = regex.sub(all_symbols_pattern, "", st)
+        # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
+        # If both str tested have roman numerals no harm done if XXIV gets turned into 204.
+        st = st.replace("xviii", "18")
+        st = st.replace("xvii", "17")
+        st = st.replace("xvi", "16")
+        st = st.replace("xiii", "13")
+        st = st.replace("xii", "12")
+        st = st.replace("xiv", "14")
+        st = st.replace("xv", "15")
+        st = st.replace("xix", "19")
+        st = st.replace("xx", "20")
+        st = st.replace("xi", "11")
+        st = st.replace("viii", "8")
+        st = st.replace("vii", "7")
+        st = st.replace("vi", "6")
+        st = st.replace("iii", "3")
+        st = st.replace("ii", "2")
+        st = st.replace("iv", "4")
+        st = st.replace("v", "5")
+        st = st.replace("ix", "9")
+        st = st.replace("x", "10")
+        st = st.replace("i", "1")
+        # remove diacritics (not to asian languages diacritics, only for 2 to 1 character combinations)
+        st = "".join([c for c in unicodedata.normalize("NFKD", st) if not unicodedata.combining(c)])
+        # remove spaces for the strings. but keep the index/main string with spaces
+        # rapidfuzz algorithms needs them to tokenize
+        st = st.strip().split()
+        new_t.append(" ".join(st))
+        subtitles[i] = "".join(st)
+    return " ".join(new_t), subtitles
+
+
+def check_full_match(name_subs, subtitlemap, namemap):
+    # A hack to take care of those that are either exactly equal
+    # or are exactly equal to one and only one subtitle
+    result = []
+    nameaux_nospaces = "".join(name_subs)
+    for key, ns_list in subtitlemap.items():
+        if "".join(ns_list) == nameaux_nospaces:
+            result.append((namemap[key], MAX_SCORE, key))
+        elif len(ns_list) > 1:
+            for sub in ns_list:
+                if sub == nameaux_nospaces:
+                    result.append((namemap[key], MAX_SCORE, key))
+    return result
 
 
 # ---------------------------------------------------------------------------------
 # Initalization functions, since there are two main programs so the code is reused
 # ---------------------------------------------------------------------------------
 class RzipReader(object):
     """used to abstract the libretro compressed playlist format"""
@@ -660,19 +665,14 @@
     nofail: bool = Option(False, "--no-fail", help="Download any score. Equivalent to --score 0."),
     noimage: bool = Option(False, "--no-image", help="Don't show images even with chafa installed."),
     nomerge: bool = Option(
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
     ),
-    nosubtitle: bool = Option(
-        False,
-        "--no-subtitle",
-        help="Ignores text after last ' - ' or ': '. ':' can't occur in server names, so if the server has 'Name_ subtitle.png' and not 'Name - subtitle.png' (uncommon), this option doesn't help.",
-    ),
     nometa: bool = Option(
         False,
         "--no-meta",
         help="Ignores () delimited metadata and may cause false positives. Forced with --before.",
     ),
     hack: bool = Option(
         False,
@@ -748,15 +748,14 @@
                         filters,
                         score,
                         noimage,
                         nomerge,
                         nofail,
                         nometa,
                         hack,
-                        nosubtitle,
                         verbose,
                         nub_verbose,
                         before,
                         tmpdir,
                         thumbnails_dir,
                         client,
                     )
@@ -807,19 +806,14 @@
     nofail: bool = Option(False, "--no-fail", help="Download any score. Equivalent to --score 0."),
     noimage: bool = Option(False, "--no-image", help="Don't show images even with chafa installed."),
     nomerge: bool = Option(
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
     ),
-    nosubtitle: bool = Option(
-        False,
-        "--no-subtitle",
-        help="Ignores text after last ' - ' or ': '. ':' can't occur in server names, so if the server has 'Name_ subtitle.png' and not 'Name - subtitle.png' (uncommon), this option doesn't help.",
-    ),
     nometa: bool = Option(
         False,
         "--no-meta",
         help="Ignores () delimited metadata and may cause false positives. Forced with --before.",
     ),
     hack: bool = Option(
         False,
@@ -873,15 +867,14 @@
                                 filters,
                                 score,
                                 noimage,
                                 nomerge,
                                 nofail,
                                 nometa,
                                 hack,
-                                nosubtitle,
                                 verbose,
                                 nub_verbose,
                                 before,
                                 tmpdir,
                                 thumbnails_dir,
                                 client,
                             )
@@ -938,15 +931,14 @@
     filters: Optional[List[str]],
     score: int,
     noimage: bool,
     nomerge: bool,
     nofail: bool,
     nometa: bool,
     hack: bool,
-    nosubtitle: bool,
     verbose: Optional[int],
     nub_verbose: bool,
     before: Optional[str],
     tmpdir: Path,
     thumbnails_dir: Path,
     client: AsyncClient,
 ):
@@ -964,25 +956,37 @@
         score = 0
 
     # build the function that will be called to print data,
     # filling in some fixed arguments
     short_names = os.getenv("SHORT")
     short_names = True if short_names and short_names != "0" else False
     strfy_runtime = partial(strfy, score, short_names, nub_verbose)
+    norm = partial(normalizer, nometa, hack)
+    failure = 0
+    success = 0
 
-    # preprocess data so it's not redone every loop iteration.
     title_scorer = TitleScorer()
-    # normalize with or without subtitles, besides the
-    # remote_names this is used on the iterated local names later
-    norm = nosubtitle_normalizer if nosubtitle else normalizer
-    # we choose the highest similarity of all 3 directories, since no mixed matches are allowed
+    # we choose the highest similarity of all 3 directories,
+    # since no mixed matches are allowed
+    # (until you call again without --no-merge anyway)
     remote_names = set()
     remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
-    # turn into a set, original key and normalized value.
-    remote_names = {x: norm(x, nometa, hack) for x in remote_names}
+    # preprocess data for speed and to make
+    # exact matches (for total name or subtitle)
+    # not involved in the fuzz function.
+    # turn into a dict, original key and
+    # (normalized value, [normalized value nospaces,... possible subtitles nospace])
+    subtitle = dict()
+    mappings = dict()
+    for x in remote_names:
+        normstr, lst = norm(x)
+        subtitle[x] = lst
+        mappings[x] = normstr
+    remote_names = mappings
+
     for name, destination in names:
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
 
@@ -995,37 +999,30 @@
             # Ignore metadata and get the string before it
             name_without_meta = regex.search(before_metadata, nameaux)
             if name_without_meta:
                 before_index = name_without_meta.group(1).find(before)
                 if before_index != -1:
                     nameaux = nameaux[0:before_index]
 
-        # there is a second form of subtitles, which doesn't appear in the thumbnail server
-        # but can appear in linux game names. It uses the colon character, which is forbidden
-        # in windows. Note that this means that if the servername has 'Name_ subtitle.png',
-        # not 'Name - subtitle.png' it has little chance of a match, but that's rarer than opposite.
-        # not to mention that this only applies if the user signals 'no-subtitle',
-        # which presumably means they tried without it - which does match.
-        if nosubtitle:
-            nameaux = nosubtitle_aux(nameaux, ": ")
-
         # only the local names should have forbidden characters
+        # this is the character libretro server uses to replace
         name = regex.sub(forbidden, "_", name)
         nameaux = regex.sub(forbidden, "_", nameaux)
 
         # unlike the server thumbnails, normalization wasn't done yet
-        nameaux = norm(nameaux, nometa, hack)
-
-        # operate on cache (to speed up by not applying normalization every iteration)
-        # normalization can make it so that the winner has the same score as the runner up(s)
-        # so to make sure we catch at least two candidates for cases where that happens
-        # it's a improvement because sometimes server thumbnail types have case letter typos
-        result = process.extract(
-            nameaux, remote_names, scorer=title_scorer, processor=None, limit=verbose or 2, score_cutoff=None
-        )
+        (nameaux, nameaux_subs) = norm(nameaux)
+        # this checks if the name has a full match among
+        # the normalized names or the normalized subtitles
+        result = check_full_match(nameaux_subs, subtitle, remote_names)
+        if not result:
+            # operate on cache (to speed up by not applying normalization every iteration)
+            # normalization can make it so that the winner has the same score as the runner up(s)
+            # so to make sure we catch at least two candidates for cases where that happens
+            # it's a improvement because sometimes server thumbnail types have case letter typos
+            result = process.extract(nameaux, remote_names, scorer=title_scorer, limit=verbose or 2)
         _, max_score, _ = (result and result[0]) or (None, -1, None)
         winners = [x for x in result if x[1] == max_score and x[1] >= score]
         show = result if verbose else winners
         name_format = style((nameaux if short_names else name) + ": ", bold=True)
         if winners:
             allow = True
             # these parent directories were created when reading the playlist
@@ -1111,48 +1108,52 @@
                     if downloaded_once:
                         for old, new in downloaded_dict.values():
                             if new.exists():
                                 shutil.move(new, old)
                         name_format = name_format + ", ".join((strfy_runtime(x, urls) for x in show))
                         success_format = f'{style("Success",   fg=GREEN, bold=True)}: {name_format}'
                         echo(success_format)
+                        success += 1
                 except StopProgram as e:
                     name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
                     skipped_format = f'{style("Skipped",     fg=(135,135,135), bold=True)}: {name_format}'
                     echo(skipped_format)
                     raise e
                 except StopDownload:
                     name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
                     skipped_format = f'{style("Skipped",     fg=(135,135,135), bold=True)}: {name_format}'
                     echo(skipped_format)
         else:
+            failure += 1
             if verbose:
                 name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
                 failure_format = f'{style("Failure",     fg=RED, bold=True)}: {name_format}'
                 echo(failure_format)
             # same idea as above can't be unified because
             # the above delete needs to be after downloads
             # but before displaying the image
             if filters:
                 for dirname in Thumbs._fields:
                     Path(thumbnails_dir, destination, dirname, name + ".png").unlink(missing_ok=True)
+    echo(f"{success}/{len(names)} successes {failure}/{len(names)} failures")
 
 
 async def printwait(wait: Optional[float], waiting_format: str):
     count = int(wait / 0.1)
     with handleContinueDownload():
         for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, leave=False):
             checkDownload()
             await asyncio.sleep(0.1)
 
 
 def strfy(required_score, short_names, nub_verbose, r, urlsdict=None):
     thumb_norm, thumb_score, thumb_name = r
     score_color = RED if thumb_score < required_score else GREEN
-    score_text = style(f"{int(thumb_score)}", fg=f"{score_color}", bold=True)
+    # thumb_score = thumb_score if short_names else int(thumb_score)
+    score_text = style(f"{thumb_score}", fg=f"{score_color}", bold=True)
     if nub_verbose:
         return f"{score_text} {thumb_norm}"
     elif urlsdict:
         url1 = urlsdict.get((Thumbs._fields[0], r), None)
         url2 = urlsdict.get((Thumbs._fields[1], r), None)
         url3 = urlsdict.get((Thumbs._fields[2], r), None)
     else:
@@ -1284,10 +1285,10 @@
 
 
 def fuzzall():
     run(mainfuzzall)
 
 
 if __name__ == "__main__":
-    print(globals()[sys.argv[1]](*sys.argv[2:]))
-    # error("Please run libretro-fuzz or libretro-fuzzall instead of running the script directly")
-    # raise Exit(code=1)
+    # print(globals()[sys.argv[1]](*sys.argv[2:]))
+    error("Please run libretro-fuzz or libretro-fuzzall instead of running the script directly")
+    raise Exit(code=1)
```

### Comparing `libretrofuzz-3.0.4/pyproject.toml` & `libretrofuzz-3.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.0.4"
+version = "3.0.6"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.0.4/setup.py` & `libretrofuzz-3.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.0.4',
+    'version': '3.0.6',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-3.0.4/PKG-INFO` & `libretrofuzz-3.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.0.4
+Version: 3.0.6
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -40,17 +40,15 @@
 If you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.
 
 Besides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.
 
 If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
 
 Example:
- | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``
- | then
- | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``
+ | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``
 
  The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.
 
 Note that the system name you download from doesn't have to be the same as the playlist name.
 
 If the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.
 
@@ -58,18 +56,18 @@
  ``libretro-fuzz --no-meta --no-merge``
 
  After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.
  Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.
 
 Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.
 
-False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
+False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
 
 Example:
-  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``
+  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``
 
   The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
 To debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.
 
 libretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]
   :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.
@@ -90,15 +88,14 @@
                         | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
   --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
-  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
   --verbose N           | Show length N list: score, name, emoji hyperlinks.
                         | [x>=1]
```

