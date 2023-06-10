# Comparing `tmp/relint-3.0.0.tar.gz` & `tmp/relint-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relint-3.0.0.tar", last modified: Thu Mar  9 10:34:26 2023, max compression
+gzip compressed data, was "relint-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `relint-3.0.0.tar` & `relint-3.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-03-09 10:34:05.630016 relint-3.0.0/LICENSE
--rw-r--r--   0        0        0     2226 2023-03-09 10:34:05.630016 relint-3.0.0/README.md
--rw-r--r--   0        0        0     1652 2023-03-09 10:34:05.630016 relint-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      151 2023-03-09 10:34:05.630016 relint-3.0.0/relint/__init__.py
--rw-r--r--   0        0        0     2930 2023-03-09 10:34:05.630016 relint-3.0.0/relint/__main__.py
--rw-r--r--   0        0        0      160 2023-03-09 10:34:26.815119 relint-3.0.0/relint/_version.py
--rw-r--r--   0        0        0     1363 2023-03-09 10:34:05.630016 relint-3.0.0/relint/config.py
--rw-r--r--   0        0        0       94 2023-03-09 10:34:05.630016 relint-3.0.0/relint/exceptions.py
--rw-r--r--   0        0        0     5724 2023-03-09 10:34:05.630016 relint-3.0.0/relint/parse.py
--rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 relint-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-10 07:40:16.909062 relint-3.1.0/LICENSE
+-rw-r--r--   0        0        0     2226 2023-06-10 07:40:16.909062 relint-3.1.0/README.md
+-rw-r--r--   0        0        0     1652 2023-06-10 07:40:16.909062 relint-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-06-10 07:40:16.913062 relint-3.1.0/relint/__init__.py
+-rw-r--r--   0        0        0     2930 2023-06-10 07:40:16.913062 relint-3.1.0/relint/__main__.py
+-rw-r--r--   0        0        0      160 2023-06-10 07:40:34.721350 relint-3.1.0/relint/_version.py
+-rw-r--r--   0        0        0     1363 2023-06-10 07:40:16.913062 relint-3.1.0/relint/config.py
+-rw-r--r--   0        0        0       94 2023-06-10 07:40:16.913062 relint-3.1.0/relint/exceptions.py
+-rw-r--r--   0        0        0     6013 2023-06-10 07:40:16.913062 relint-3.1.0/relint/parse.py
+-rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 relint-3.1.0/PKG-INFO
```

### Comparing `relint-3.0.0/LICENSE` & `relint-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `relint-3.0.0/README.md` & `relint-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `relint-3.0.0/pyproject.toml` & `relint-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `relint-3.0.0/relint/__main__.py` & `relint-3.1.0/relint/__main__.py`

 * *Files identical despite different names*

### Comparing `relint-3.0.0/relint/config.py` & `relint-3.1.0/relint/config.py`

 * *Files identical despite different names*

### Comparing `relint-3.0.0/relint/parse.py` & `relint-3.1.0/relint/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,58 +99,67 @@
 
         start_line_no = match.string[: match.start()].count("\n") + 1
         end_line_no = match.string[: match.end()].count("\n") + 1
 
         if args.summarize:
             match_groups[test].append(f"{filename}:{start_line_no}")
         else:
-            hint = Panel(
-                Markdown(test.hint, justify="left"),
-                title="Hint:",
-                title_align="left",
-                padding=(0, 2),
-            )
+            message_bits = []
 
-            if args.code_padding == -1:
-                message = hint
-            else:
+            if args.code_padding != -1:
                 lexer = Syntax.guess_lexer(filename)
-                syntax = Syntax(
-                    match.string,
-                    lexer=lexer,
-                    line_numbers=True,
-                    line_range=(
-                        start_line_no - args.code_padding,
-                        end_line_no + args.code_padding,
-                    ),
-                    highlight_lines=range(start_line_no, end_line_no + 1),
+                message_bits.append(
+                    Syntax(
+                        match.string,
+                        lexer=lexer,
+                        line_numbers=True,
+                        line_range=(
+                            start_line_no - args.code_padding,
+                            end_line_no + args.code_padding,
+                        ),
+                        highlight_lines=range(start_line_no, end_line_no + 1),
+                    )
+                )
+
+            if test.hint:
+                message_bits.append(
+                    Panel(
+                        Markdown(test.hint, justify="left"),
+                        title="Hint:",
+                        title_align="left",
+                        padding=(0, 2),
+                    )
                 )
-                message = Group(syntax, hint)
 
             messages.append(
                 Panel(
-                    message,
+                    Group(*message_bits),
                     title=f"{'Error' if test.error else 'Warning'}: {test.name}",
                     title_align="left",
                     subtitle=f"{filename}:{start_line_no}",
                     subtitle_align="left",
                     border_style="bold red" if test.error else "yellow",
                     padding=(0, 2),
                 )
             )
 
     if args.summarize:
         for test, filenames in match_groups.items():
-            hint = Panel(
-                Markdown(test.hint, justify="left"),
-                title="Hint:",
-                title_align="left",
-                padding=(0, 2),
-            )
-            group = Group(Group(*filenames), hint)
+            group = Group(*filenames)
+            if test.hint:
+                group = Group(
+                    group,
+                    Panel(
+                        Markdown(test.hint, justify="left"),
+                        title="Hint:",
+                        title_align="left",
+                        padding=(0, 2),
+                    ),
+                )
+
             messages.append(
                 Panel(
                     group,
                     title=f"{'Error' if test.error else 'Warning'}: {test.name}",
                     title_align="left",
                     subtitle=f"{len(filenames)} occurrence(s)",
                     subtitle_align="left",
```

### Comparing `relint-3.0.0/PKG-INFO` & `relint-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relint
-Version: 3.0.0
+Version: 3.1.0
 Summary: Write your own linting rules using regular expressions.
 Keywords: regex,linter
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

