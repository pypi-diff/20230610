# Comparing `tmp/py_fumen_util-0.1.0.tar.gz` & `tmp/py_fumen_util-0.2.0.tar.gz`

## Comparing `py_fumen_util-0.1.0.tar` & `py_fumen_util-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/__init__.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/__main__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/fumen_combiner.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/fumen_locker.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/fumen_splitter.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/glue_fumen.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/grayout_all.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/grayout_last.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/mirror_fumen.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/remove_comment.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/unglue_fumen.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/LICENSE
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/README.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/__init__.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/__main__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/fumen_combiner.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/fumen_locker.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/fumen_splitter.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/glue_fumen.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/grayout_all.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/grayout_last.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/mirror_fumen.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/remove_comment.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/unglue_fumen.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/README.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/PKG-INFO
```

### Comparing `py_fumen_util-0.1.0/src/py_fumen_util/__main__.py` & `py_fumen_util-0.2.0/src/py_fumen_util/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # -*- coding:utf-8 -*-
 
+import argparse
 import sys
 
 from py_fumen_py import *
 from .fumen_combiner import fumen_combiner
 from .fumen_locker import fumen_locker
 from .fumen_splitter import fumen_splitter
 from .glue_fumen import glue_fumen
 from .grayout_all import grayout_all_fumen
 from .grayout_last import grayout_fumen
 from .mirror_fumen import mirror_fumen
 from .remove_comment import remove_comment
 from .unglue_fumen import unglue_fumen
 
-def usage(dummy_arg=None):
+_command_function_map = {
+    'combine': fumen_combiner,
+    'concat' : fumen_combiner,
+    'join': fumen_combiner,
+    'split': fumen_splitter,
+    'glue': glue_fumen,
+    'decompile': glue_fumen,
+    'unglue': unglue_fumen,
+    'compile': unglue_fumen,
+    'gray': grayout_fumen,
+    'grey': grayout_fumen,
+    'grayall': grayout_all_fumen,
+    'greyall': grayout_all_fumen,
+    'lock': fumen_locker,
+    'mirror': mirror_fumen,
+    'flip': mirror_fumen,
+    'uncomment': remove_comment,
+}
+
+def usage():
     return [
-        'Usage:',
-        'python3 -m py_fumen_util command fumen_code [fumen_code...]',
-        'Commands (case-insensitive):',
+        'commands (case-insensitive):',
         '    Combine:   Combine multiple Fumens into one',
         '               Alias: Concat, Join',
         '    Split:     Split each page into a Fumen',
         '',
         '    Glue:      Glue each Fumen page into tetromino placements',
         '               Alias: Decompile',
         '    Unglue:    Unglue Fumen placements into one page',
@@ -35,39 +53,47 @@
         '    Lock:      Lock the last page of each Fumen and append a new page',
         '    Mirror:    Mirror Fumen pages',
         '               Alias: Flip',
         '    Uncomment: Uncomment Fumen pages',
     ]
 
 if __name__ == '__main__':
-    if len(sys.argv) > 2:
-        command = sys.argv[1].casefold()
-        fumen_codes = ' '.join(sys.argv[2:]).split()
-
-        command_function = {
-            'combine': fumen_combiner,
-            'concat' : fumen_combiner,
-            'join': fumen_combiner,
-            'split': fumen_splitter,
-            'glue': glue_fumen,
-            'decompile': glue_fumen,
-            'unglue': unglue_fumen,
-            'compile': unglue_fumen,
-            'gray': grayout_fumen,
-            'grey': grayout_fumen,
-            'grayall': grayout_all_fumen,
-            'greyall': grayout_all_fumen,
-            'lock': fumen_locker,
-            'mirror': mirror_fumen,
-            'flip': mirror_fumen,
-            'uncomment': remove_comment,
-        }.get(command, usage)
-    else:
-        command_function = usage
-        fumen_codes = None
-
-    try:
-        for line in command_function(fumen_codes):
-            print(line)
-    except Exception as e:
-        print(e)
-        usage()
+    argparser = argparse.ArgumentParser(
+        description='Tetris Fumen utilies in Python.',
+        prog='python3 -m py_fumen_util'
+    )
+    argparser.add_argument(
+        'command',
+        type=str,
+        nargs='+',
+        help='Command(s) to execute on the Fumen(s).'
+    )
+    argparser.add_argument(
+        'file',
+        type=str,
+        help='File with Fumen strings, separated with whitespace and/or linebreak. Use "-" to read from standard input.'
+    )
+
+    args = argparser.parse_args(sys.argv[1:])
+    commands = args.command
+    fumen_file = sys.stdin if args.file == '-' else open(args.file, 'r')
+    fumen_codes = fumen_file.read().split()
+    fumen_file.close()
+
+    for command in commands:
+        command_function = _command_function_map.get(command.casefold(), None)
+        try:
+            fumen_codes = command_function(fumen_codes)
+        except Exception as e:
+            if command_function:
+                print(e)
+            else:
+                print(f'"{command}" is not a valid command.')
+            print()
+            argparser.print_help()
+            print()
+            for line in usage():
+                print(line)
+            exit()
+
+    for line in fumen_codes:
+        print(line)
```

### Comparing `py_fumen_util-0.1.0/src/py_fumen_util/fumen_splitter.py` & `py_fumen_util-0.2.0/src/py_fumen_util/fumen_splitter.py`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/src/py_fumen_util/glue_fumen.py` & `py_fumen_util-0.2.0/src/py_fumen_util/glue_fumen.py`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/src/py_fumen_util/grayout_all.py` & `py_fumen_util-0.2.0/src/py_fumen_util/grayout_all.py`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/src/py_fumen_util/grayout_last.py` & `py_fumen_util-0.2.0/src/py_fumen_util/grayout_last.py`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/src/py_fumen_util/mirror_fumen.py` & `py_fumen_util-0.2.0/src/py_fumen_util/mirror_fumen.py`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/src/py_fumen_util/unglue_fumen.py` & `py_fumen_util-0.2.0/src/py_fumen_util/unglue_fumen.py`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/.gitignore` & `py_fumen_util-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/LICENSE` & `py_fumen_util-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.1.0/README.md` & `py_fumen_util-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 # py-fumen-util
 Python implementation of [swng's FumenUtil](https://github.com/swng/FumenUtil), using [py-fumen-py](https://github.com/OctupusTea/py-fumen-py)
 
 ## Dependency
 - `py-fumen-py`: Python implementation of knewjade's `tetris-fumen` node module
 
+## Installation
+
+```bash
+python3 -m pip install py-fumen-util
+```
+
 ## Usage
 
 ```bash
-python3 -m py_fumen_util command fumen_code [fumen_code...]
+python3 -m py_fumen_util command [commmand...] file
 ```
 
+- `command`: Command(s) to execute on the Fumen(s).
+- `file`: File with Fumen strings, separated with whitespace and/or linebreak. Use "-" to read from standard input.
+
 ### Commands
 
 Commands are case-insensitive.
 
 |Command|Description|Alias|
 |:-|:-|:-|
 |Combine|Combine multiple Fumens into one|Concat, Join|
```

### Comparing `py_fumen_util-0.1.0/pyproject.toml` & `py_fumen_util-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_fumen_util"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
 	{ name="Octupus Tea" },
 ]
 description = "Python implementation of the JavaScript package 'FumenUtil'"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

