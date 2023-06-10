# Comparing `tmp/compactify-1.tar.gz` & `tmp/compactify-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compactify-1.tar", last modified: Sat Jun 10 12:26:46 2023, max compression
+gzip compressed data, was "compactify-2.tar", last modified: Sat Jun 10 13:28:46 2023, max compression
```

## Comparing `compactify-1.tar` & `compactify-2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 12:26:46.338384 compactify-1/
--rw-r--r--   0 olle       (501) staff       (20)     1069 2023-06-10 11:50:40.000000 compactify-1/LICENSE
--rw-r--r--   0 olle       (501) staff       (20)     1876 2023-06-10 12:26:46.338246 compactify-1/PKG-INFO
--rw-r--r--   0 olle       (501) staff       (20)      282 2023-06-10 10:16:28.000000 compactify-1/README.md
-drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 12:26:46.337129 compactify-1/compactify/
--rw-r--r--   0 olle       (501) staff       (20)       62 2023-06-10 12:02:11.000000 compactify-1/compactify/__init__.py
--rwxr-xr-x   0 olle       (501) staff       (20)      129 2023-06-10 12:02:11.000000 compactify-1/compactify/__main__.py
--rw-r--r--   0 olle       (501) staff       (20)     5421 2023-06-10 12:13:52.000000 compactify-1/compactify/core.py
--rw-r--r--   0 olle       (501) staff       (20)     1009 2023-06-10 12:02:11.000000 compactify-1/compactify/logs.py
--rwxr-xr-x   0 olle       (501) staff       (20)     2153 2023-06-10 12:13:10.000000 compactify-1/compactify/main.py
-drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 12:26:46.337909 compactify-1/compactify.egg-info/
--rw-r--r--   0 olle       (501) staff       (20)     1876 2023-06-10 12:26:46.000000 compactify-1/compactify.egg-info/PKG-INFO
--rw-r--r--   0 olle       (501) staff       (20)      331 2023-06-10 12:26:46.000000 compactify-1/compactify.egg-info/SOURCES.txt
--rw-r--r--   0 olle       (501) staff       (20)        1 2023-06-10 12:26:46.000000 compactify-1/compactify.egg-info/dependency_links.txt
--rw-r--r--   0 olle       (501) staff       (20)       56 2023-06-10 12:26:46.000000 compactify-1/compactify.egg-info/entry_points.txt
--rw-r--r--   0 olle       (501) staff       (20)       11 2023-06-10 12:26:46.000000 compactify-1/compactify.egg-info/top_level.txt
--rw-r--r--   0 olle       (501) staff       (20)      625 2023-06-10 12:11:39.000000 compactify-1/pyproject.toml
--rw-r--r--   0 olle       (501) staff       (20)       38 2023-06-10 12:26:46.338422 compactify-1/setup.cfg
-drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 12:26:46.338025 compactify-1/tests/
--rw-r--r--   0 olle       (501) staff       (20)     2161 2023-06-10 12:02:11.000000 compactify-1/tests/testing_infra.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 13:28:46.047509 compactify-2/
+-rw-r--r--   0 olle       (501) staff       (20)     1069 2023-06-10 11:50:40.000000 compactify-2/LICENSE
+-rw-r--r--   0 olle       (501) staff       (20)     1876 2023-06-10 13:28:46.047313 compactify-2/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)      282 2023-06-10 10:16:28.000000 compactify-2/README.md
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 13:28:46.045745 compactify-2/compactify/
+-rw-r--r--   0 olle       (501) staff       (20)       62 2023-06-10 12:02:11.000000 compactify-2/compactify/__init__.py
+-rwxr-xr-x   0 olle       (501) staff       (20)      129 2023-06-10 12:02:11.000000 compactify-2/compactify/__main__.py
+-rw-r--r--   0 olle       (501) staff       (20)     5519 2023-06-10 13:24:24.000000 compactify-2/compactify/core.py
+-rw-r--r--   0 olle       (501) staff       (20)     1009 2023-06-10 12:02:11.000000 compactify-2/compactify/logs.py
+-rwxr-xr-x   0 olle       (501) staff       (20)     2153 2023-06-10 12:13:10.000000 compactify-2/compactify/main.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 13:28:46.046813 compactify-2/compactify.egg-info/
+-rw-r--r--   0 olle       (501) staff       (20)     1876 2023-06-10 13:28:46.000000 compactify-2/compactify.egg-info/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)      331 2023-06-10 13:28:46.000000 compactify-2/compactify.egg-info/SOURCES.txt
+-rw-r--r--   0 olle       (501) staff       (20)        1 2023-06-10 13:28:46.000000 compactify-2/compactify.egg-info/dependency_links.txt
+-rw-r--r--   0 olle       (501) staff       (20)       56 2023-06-10 13:28:46.000000 compactify-2/compactify.egg-info/entry_points.txt
+-rw-r--r--   0 olle       (501) staff       (20)       11 2023-06-10 13:28:46.000000 compactify-2/compactify.egg-info/top_level.txt
+-rw-r--r--   0 olle       (501) staff       (20)      625 2023-06-10 12:31:30.000000 compactify-2/pyproject.toml
+-rw-r--r--   0 olle       (501) staff       (20)       38 2023-06-10 13:28:46.047568 compactify-2/setup.cfg
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2023-06-10 13:28:46.047016 compactify-2/tests/
+-rw-r--r--   0 olle       (501) staff       (20)     2161 2023-06-10 12:02:11.000000 compactify-2/tests/testing_infra.py
```

### Comparing `compactify-1/LICENSE` & `compactify-2/LICENSE`

 * *Files identical despite different names*

### Comparing `compactify-1/PKG-INFO` & `compactify-2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compactify
-Version: 1
+Version: 2
 Summary: Make Python code more compact
 Author: Olle Lindgren
 Author-email: olle.ln@outlook.com
 License: MIT License
         
         Copyright (c) 2023 OlleLindgren
```

### Comparing `compactify-1/compactify/core.py` & `compactify-2/compactify/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import ast
 import re
 from pathlib import Path
 from typing import Sequence
 
+from compactify import logs as logger
+
 
 def _group_matching_lines(
     lines: Sequence[str], pattern: str, min_group_size: int = 2
 ) -> Sequence[Sequence[int]]:
     """
     Given a list of lines and a regex pattern, return a sorted list of groups of sorted line numbers
     where each group contains at least min_group_size consecutive lines matching the pattern.
@@ -22,30 +24,30 @@
 
 
 def _merge_lines(lines: Sequence[str], group: Sequence[int]) -> None:
     """
     Merge the lines at the given indices into one line.
     """
     lines_subset = [lines[i] for i in group]
-    indent = min(len(line) - len(line.lstrip()) for line in lines_subset)
+    indent = min((len(line) - len(line.lstrip()) for line in lines_subset if line.strip()), default=0)
     indent_character = lines_subset[0][0]  # Won't be whitespace if indent==0, but that's fine
     new_line = indent * indent_character + re.sub(r"\s", "", "".join(lines_subset))
     for i in sorted(group, reverse=True):
         lines.pop(i)
 
     lines.insert(min(group), new_line)
 
 
 def collapse_rparen_lines(lines: Sequence[str]) -> None:
     """
     For all consecutive lines matching rparen_pattern, collapse them into one line,
     remove all whitespace, and indent as much as the least indented line.
     """
-    rparen_only_pattern = r"[\]\)\},]"
-    rparen_or_ws_pattern = r"[\]\)\},\s]"
+    rparen_only_pattern = r"[\]\)\},:]"
+    rparen_or_ws_pattern = r"[\]\)\},:\s]"
     rparen_pattern = r"^\s*" + rparen_only_pattern + rparen_or_ws_pattern + r"*$"
 
     for group in reversed(_group_matching_lines(lines, rparen_pattern)):
         _merge_lines(lines, group)
 
 
 def collapse_lparen_lines(lines: Sequence[str]) -> None:
@@ -82,18 +84,21 @@
         return
 
     indents = [
         len(line) - len(line.lstrip()) for line in lines
     ]
     best_indents = [indents[0]]
     for i, indent in enumerate(indents[1:], start=1):
-        # if re.match(r"[\]\)\}]", (lines[i].lstrip() + " ")[0]):
-        #     best_indents.append(min(indent, indents[i-1]))
-        # else:
-        best_indents.append(min(indent, indents[i-1] + 4))
+        previous_indent = 0
+        for j in range(i - 1, -1, -1):
+            if lines[j].strip():
+                previous_indent = indents[j]
+                break
+
+        best_indents.append(min(indent, previous_indent + 4))
 
     deindents = [0 for _ in lines]
 
     for i, line, indent, best_indent in zip(
         range(len(lines)),
         lines,
         indents,
```

### Comparing `compactify-1/compactify/logs.py` & `compactify-2/compactify/logs.py`

 * *Files identical despite different names*

### Comparing `compactify-1/compactify/main.py` & `compactify-2/compactify/main.py`

 * *Files identical despite different names*

### Comparing `compactify-1/compactify.egg-info/PKG-INFO` & `compactify-2/compactify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compactify
-Version: 1
+Version: 2
 Summary: Make Python code more compact
 Author: Olle Lindgren
 Author-email: olle.ln@outlook.com
 License: MIT License
         
         Copyright (c) 2023 OlleLindgren
```

### Comparing `compactify-1/pyproject.toml` & `compactify-2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "compactify"
-version = "1"
+version = "2"
 description = "Make Python code more compact"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {email = "olle.ln@outlook.com"},
     {name = "Olle Lindgren"}
```

### Comparing `compactify-1/tests/testing_infra.py` & `compactify-2/tests/testing_infra.py`

 * *Files identical despite different names*

