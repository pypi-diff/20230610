# Comparing `tmp/mybar-0.7.tar.gz` & `tmp/mybar-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybar-0.7.tar", last modified: Tue Jun  6 10:38:21 2023, max compression
+gzip compressed data, was "mybar-0.7.1.tar", last modified: Sat Jun 10 06:43:51 2023, max compression
```

## Comparing `mybar-0.7.tar` & `mybar-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-06 10:38:21.409394 mybar-0.7/
--rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.7/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-06-06 10:38:21.409394 mybar-0.7/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.7/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-06 10:38:21.409394 mybar-0.7/mybar/
--rw-r--r--   0 sam       (1000) sam       (1000)      599 2023-06-06 10:20:26.000000 mybar-0.7/mybar/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-06-01 10:53:22.000000 mybar-0.7/mybar/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-05-30 09:20:33.000000 mybar-0.7/mybar/_setups.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3846 2023-05-31 09:01:05.000000 mybar-0.7/mybar/_types.py
--rw-r--r--   0 sam       (1000) sam       (1000)    46651 2023-06-06 10:30:53.000000 mybar-0.7/mybar/bar.py
--rw-r--r--   0 sam       (1000) sam       (1000)    12944 2023-06-06 10:17:47.000000 mybar-0.7/mybar/cli.py
--rw-r--r--   0 sam       (1000) sam       (1000)      861 2023-06-02 05:55:18.000000 mybar-0.7/mybar/constants.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2112 2023-05-29 11:58:23.000000 mybar-0.7/mybar/defaults.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3439 2023-06-02 11:18:30.000000 mybar-0.7/mybar/errors.py
--rw-r--r--   0 sam       (1000) sam       (1000)    28629 2023-06-06 09:58:42.000000 mybar-0.7/mybar/field.py
--rw-r--r--   0 sam       (1000) sam       (1000)    15856 2023-05-31 09:45:55.000000 mybar-0.7/mybar/field_funcs.py
--rw-r--r--   0 sam       (1000) sam       (1000)    25593 2023-05-30 10:50:38.000000 mybar-0.7/mybar/formatting.py
--rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-05-31 11:58:31.000000 mybar-0.7/mybar/log.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.7/mybar/sync.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1929 2023-05-30 10:32:04.000000 mybar-0.7/mybar/templates.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5685 2023-05-29 15:02:35.000000 mybar-0.7/mybar/utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-06 10:38:21.409394 mybar-0.7/mybar.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      468 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.7/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.7/requirements.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      890 2023-06-06 10:38:21.409394 mybar-0.7/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-10 06:43:51.853762 mybar-0.7.1/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.7.1/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-10 06:43:51.853762 mybar-0.7.1/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.7.1/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-10 06:43:51.853762 mybar-0.7.1/mybar/
+-rw-r--r--   0 sam       (1000) sam       (1000)      601 2023-06-10 06:41:32.000000 mybar-0.7.1/mybar/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-06-01 10:53:22.000000 mybar-0.7.1/mybar/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-05-30 09:20:33.000000 mybar-0.7.1/mybar/_setups.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3846 2023-05-31 09:01:05.000000 mybar-0.7.1/mybar/_types.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    46651 2023-06-06 10:30:53.000000 mybar-0.7.1/mybar/bar.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    12944 2023-06-10 06:37:43.000000 mybar-0.7.1/mybar/cli.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      861 2023-06-02 05:55:18.000000 mybar-0.7.1/mybar/constants.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2112 2023-05-29 11:58:23.000000 mybar-0.7.1/mybar/defaults.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3439 2023-06-02 11:18:30.000000 mybar-0.7.1/mybar/errors.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    28629 2023-06-06 09:58:42.000000 mybar-0.7.1/mybar/field.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13999 2023-06-06 11:33:06.000000 mybar-0.7.1/mybar/field_funcs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    28082 2023-06-06 12:01:35.000000 mybar-0.7.1/mybar/formatting.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-05-31 11:58:31.000000 mybar-0.7.1/mybar/log.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.7.1/mybar/sync.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1929 2023-05-30 10:32:04.000000 mybar-0.7.1/mybar/templates.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5685 2023-05-29 15:02:35.000000 mybar-0.7.1/mybar/utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-10 06:43:51.853762 mybar-0.7.1/mybar.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      468 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.7.1/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.7.1/requirements.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      892 2023-06-10 06:43:51.857095 mybar-0.7.1/setup.cfg
```

### Comparing `mybar-0.7/LICENSE` & `mybar-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mybar-0.7/PKG-INFO` & `mybar-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.7
+Version: 0.7.1
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.7/mybar/__init__.py` & `mybar-0.7.1/mybar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 :copyright: (c) 2021-present by LonelyAbsol.
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'mybar'
 __description__ = "An async status bar with a highly customizable API."
 __url__ = "https://github.com/lonelyabsol/mybar"
-__version__ = '0.7'
+__version__ = '0.7.1'
 __author__ = "LonelyAbsol"
 __license__ = 'MIT'
 __copyright__ = "Copyright (c) 2021-present LonelyAbsol"
 
 
 from .constants import *
 from . import utils
```

### Comparing `mybar-0.7/mybar/_setups.py` & `mybar-0.7.1/mybar/_setups.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/_types.py` & `mybar-0.7.1/mybar/_types.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/bar.py` & `mybar-0.7.1/mybar/bar.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/cli.py` & `mybar-0.7.1/mybar/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,16 +239,16 @@
             '--options', '-o',
             action='extend',
             nargs='+',
             metavar=("'FIELD1.OPTION=VAL'", "'FIELD2.OPTION=VAL'"),
             dest='field_options',
             help=(
                 "Set arbitrary options for discrete Fields using"
-                " dot-attribute syntax.",
-            )
+                " dot-attribute syntax."
+            ),
         )
 
         self.add_argument(
             '-r', '--refresh',
             type=float,
             dest='refresh_rate',
             help=(
```

### Comparing `mybar-0.7/mybar/constants.py` & `mybar-0.7.1/mybar/constants.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/defaults.py` & `mybar-0.7.1/mybar/defaults.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/errors.py` & `mybar-0.7.1/mybar/errors.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/field.py` & `mybar-0.7.1/mybar/field.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/field_funcs.py` & `mybar-0.7.1/mybar/field_funcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from datetime import datetime
 from string import Formatter
 
 # if not embedded system:
 import psutil
 
 from .errors import *
-from .formatting import ElapsedTime, ConditionalFormatStr
+from .formatting import ElapsedTime, ConditionalFormatStr, format_uptime
 from .utils import join_options
 from ._types import (
     Contents,
     DiskMeasure,
     FormatStr,
     POWERS_OF_1024,
     MetricSymbol,
@@ -451,72 +451,7 @@
 
     if dynamic:
         out = format_uptime(secs, **setupvars)
         return out
 
     return fmt.format_map(setupvars['namespace'])
 
-
-def format_uptime(
-    secs: int,
-    sep: str,
-    namespace: dict[str],
-    groups,
-    *args, **kwargs
-) -> str:
-    '''Format a dict of numbers according to a format string by parsing
-    fields delineated by a separator.
-    '''
-    newgroups = []
-    for i, group in enumerate(groups):
-        if not group:
-            # Just an extraneous separator.
-            newgroups.append(())
-            continue
-
-        newgroup = []
-        
-        for maybe_field in group:
-            # Skip groups that should appear blank:
-            if (val := namespace.get(maybe_field[1])
-                ) == 0:
-                break
-
-            buf = ""
-
-            match maybe_field:
-                case [lit, None, None, None]:
-                    # A trailing literal.
-                    buf += lit
-
-                case [lit, field, spec, conv]:
-                    # A veritable format string field!
-                    # Add the text right before the field:
-                    if lit is not None:
-                        buf += lit
-
-                    # Format the value if necessary:
-                    if spec:
-                        buf += format(val, spec)
-                    else:
-                        try:
-                            # Round floats by default:
-                            buf += str(round(val))
-                        except TypeError:
-                            buf += str(val)
-
-                case _:
-                    raise ValueError(
-                        f"\n"
-                        f"Invalid structure in tuple\n"
-                        f"  {i} {maybe_field}:\n"
-                        f"  {spam!r}"
-                    )
-
-            if buf:
-                newgroup.append(buf)
-        if newgroup:
-            newgroups.append(newgroup)
-
-    # Join everything.
-    return sep.join(''.join(g) for g in newgroups)
-
```

### Comparing `mybar-0.7/mybar/formatting.py` & `mybar-0.7.1/mybar/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from ._types import (
     Duration,
     FormatStr,
     FormatterLiteral,
     FormatterFname,
     FormatterFormatSpec,
     FormatterConversion,
+    Duration
 )
 
 from collections.abc import Callable, Container, Hashable, Iterable
 from typing import Any, NamedTuple, NoReturn, Self, TypeAlias
 
 
 class FormatStringError(ValueError):
@@ -783,7 +784,89 @@
             return meme_hidden
 
         def __repr__(self) -> str:
             return repr(self._safe())
 
     conversions_to_secs = _Special_Obfuscating_Dict(conversions_to_secs)
 
+
+def format_uptime(
+    secs: int,
+    sep: str,
+    namespace: dict[Duration, int],
+    groups: tuple[tuple[FormatterFieldSig]],
+    *args,
+    **kwargs
+) -> str:
+    '''
+    Format a dict of numbers according to a format string by parsing
+    fields delineated by a separator.
+
+    :param secs: Total elapsed time in seconds (unused)
+    :type secs: :class:`int`
+
+    :param sep: A string that separates groups of text based on division
+        of time
+    :type sep: :class:`str`
+
+    :param namespace: A mapping of time unit names to :class:`int`
+    :type namespace: dict[:class:`Unit`, :class:`int`]
+
+    :param groups: A format string broken up by
+        :func:`_setups.setup_uptime` into tuples of
+        :class:`FormatterFieldSig` based on the locations of `separator`
+    :type groups: tuple[tuple[:class:`FormatterFieldSig`]]
+    '''
+    newgroups = []
+    for i, group in enumerate(groups):
+        if not group:
+            # Just an extraneous separator.
+            newgroups.append(())
+            continue
+
+        newgroup = []
+
+        for maybe_field in group:
+            # Skip groups that should appear blank:
+            if (val := namespace.get(maybe_field[1])
+                ) == 0:
+                break
+
+            buf = ""
+
+            match maybe_field:
+                case [lit, None, None, None]:
+                    # A trailing literal.
+                    buf += lit
+
+                case [lit, field, spec, conv]:
+                    # A veritable format string field!
+                    # Add the text right before the field:
+                    if lit is not None:
+                        buf += lit
+
+                    # Format the value if necessary:
+                    if spec:
+                        buf += format(val, spec)
+                    else:
+                        try:
+                            # Round floats by default:
+                            buf += str(round(val))
+                        except TypeError:
+                            buf += str(val)
+
+                case _:
+                    raise ValueError(
+                        f"\n"
+                        f"Invalid structure in tuple\n"
+                        f"  {i} {maybe_field}:\n"
+                        f"  {spam!r}"
+                    )
+
+            if buf:
+                newgroup.append(buf)
+        if newgroup:
+            newgroups.append(newgroup)
+
+    # Join everything.
+    return sep.join(''.join(g) for g in newgroups)
+
```

### Comparing `mybar-0.7/mybar/sync.py` & `mybar-0.7.1/mybar/sync.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/templates.py` & `mybar-0.7.1/mybar/templates.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar/utils.py` & `mybar-0.7.1/mybar/utils.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7/mybar.egg-info/PKG-INFO` & `mybar-0.7.1/mybar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.7
+Version: 0.7.1
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.7/setup.cfg` & `mybar-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mybar
-version = 0.7
+version = 0.7.1
 description = An async status bar with a highly customizable API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = lonelyabsol
 url = https://github.com/lonelyabsol/mybar
 project_urls = 
 	GitHub: repo = https://github.com/lonelyabsol/mybar
```

