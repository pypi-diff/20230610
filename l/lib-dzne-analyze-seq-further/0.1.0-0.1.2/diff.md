# Comparing `tmp/lib-dzne-analyze-seq-further-0.1.0.tar.gz` & `tmp/lib-dzne-analyze-seq-further-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-analyze-seq-further-0.1.0.tar", last modified: Sun Mar  5 21:27:24 2023, max compression
+gzip compressed data, was "lib-dzne-analyze-seq-further-0.1.2.tar", last modified: Sat Jun 10 15:07:30 2023, max compression
```

## Comparing `lib-dzne-analyze-seq-further-0.1.0.tar` & `lib-dzne-analyze-seq-further-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-05 21:27:24.763702 lib-dzne-analyze-seq-further-0.1.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-analyze-seq-further-0.1.0/LICENSE
--rw-r--r--   0 base      (1001) base      (1001)       56 2023-03-01 20:28:52.000000 lib-dzne-analyze-seq-further-0.1.0/MANIFEST.in
--rw-rw-r--   0 base      (1001) base      (1001)     1478 2023-03-05 21:27:24.763702 lib-dzne-analyze-seq-further-0.1.0/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      551 2023-03-05 21:26:56.000000 lib-dzne-analyze-seq-further-0.1.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-03-05 21:27:24.763702 lib-dzne-analyze-seq-further-0.1.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-05 21:27:24.763702 lib-dzne-analyze-seq-further-0.1.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-05 21:27:24.763702 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further/
--rw-rw-r--   0 base      (1001) base      (1001)        2 2023-03-05 21:26:02.000000 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)     1180 2023-03-05 21:25:44.000000 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further/regions.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-05 21:27:24.763702 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1478 2023-03-05 21:27:24.000000 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      412 2023-03-05 21:27:24.000000 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-03-05 21:27:24.000000 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       41 2023-03-05 21:27:24.000000 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       29 2023-03-05 21:27:24.000000 lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-10 15:07:30.672774 lib-dzne-analyze-seq-further-0.1.2/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-analyze-seq-further-0.1.2/LICENSE
+-rw-r--r--   0 base      (1001) base      (1001)       56 2023-03-01 20:28:52.000000 lib-dzne-analyze-seq-further-0.1.2/MANIFEST.in
+-rw-rw-r--   0 base      (1001) base      (1001)     1478 2023-06-10 15:07:30.672774 lib-dzne-analyze-seq-further-0.1.2/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       31 2023-06-10 15:01:44.000000 lib-dzne-analyze-seq-further-0.1.2/README.md
+-rw-r--r--   0 base      (1001) base      (1001)      551 2023-06-10 15:05:08.000000 lib-dzne-analyze-seq-further-0.1.2/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-10 15:07:30.672774 lib-dzne-analyze-seq-further-0.1.2/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-10 15:07:30.672774 lib-dzne-analyze-seq-further-0.1.2/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-10 15:07:30.672774 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further/
+-rw-rw-r--   0 base      (1001) base      (1001)        2 2023-03-18 23:05:52.000000 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further/__init__.py
+-rw-rw-r--   0 base      (1001) base      (1001)     1161 2023-06-10 15:03:38.000000 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further/regions.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-10 15:07:30.672774 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1478 2023-06-10 15:07:30.000000 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      422 2023-06-10 15:07:30.000000 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-10 15:07:30.000000 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       41 2023-06-10 15:07:30.000000 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       29 2023-06-10 15:07:30.000000 lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further.egg-info/top_level.txt
```

### Comparing `lib-dzne-analyze-seq-further-0.1.0/LICENSE` & `lib-dzne-analyze-seq-further-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-analyze-seq-further-0.1.0/PKG-INFO` & `lib-dzne-analyze-seq-further-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-analyze-seq-further
-Version: 0.1.0
+Version: 0.1.2
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-analyze-seq-further-0.1.0/pyproject.toml` & `lib-dzne-analyze-seq-further-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-analyze-seq-further"
-version = "0.1.0"
+version = "0.1.2"
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ['BASE', 'brain', 'antibody']
 dependencies = [
-    'lib-dzne-data>=0.1.2',
+    'lib-dzne-math>=0.2.3',
     'lib-dzne-seq>=0.1.1',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further/regions.py` & `lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further/regions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-import lib_dzne_seq
-import lib_dzne_data
+import lib_dzne_math.na as _na
+import lib_dzne_seq as _seq
+
 
 def main(*, seq, sub_region_table, alignment_table):
     infos = [
         (sub_region_table, 'start', 'end'),
         (alignment_table, 'from', 'to'),
     ]
     previous_end = 0
     ans = dict()
     regions = list()
     for y in range(1, 4):
         for x in ('fr', 'cdr'):
             regions.append(f"{x}{y}")
     for reg in regions:
         for table, a, b in infos:
-            if lib_dzne_data.isna(table):
+            if _na.isna(table):
                 continue
             start = None
             end = None
             for index, (row,) in table.items():
                 if index.startswith(reg):
                     start = row.get(a)
                     end = row.get(b)
                     break
-            if lib_dzne_data.isna(start, end):
+            if _na.isna(start, end):
                 continue
             ans[reg] = dict()
             if not (previous_end <= start - 1 <= end):
                 raise ValueError()
             previous_end = end
-            if lib_dzne_data.isna(seq):
+            if _na.isna(seq):
                 continue
-            ans[reg] = lib_dzne_seq.data(
+            ans[reg] = _seq.data(
                 seq=seq,
                 go=start-1,
                 end=end,
             )
             break
     return ans
```

### Comparing `lib-dzne-analyze-seq-further-0.1.0/src/lib_dzne_analyze_seq_further.egg-info/PKG-INFO` & `lib-dzne-analyze-seq-further-0.1.2/src/lib_dzne_analyze_seq_further.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-analyze-seq-further
-Version: 0.1.0
+Version: 0.1.2
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

