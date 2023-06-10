# Comparing `tmp/html_report_line_profiler-0.0.1.tar.gz` & `tmp/html_report_line_profiler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_report_line_profiler-0.0.1.tar", last modified: Fri Jun  9 22:49:36 2023, max compression
+gzip compressed data, was "html_report_line_profiler-0.0.2.tar", last modified: Sat Jun 10 16:32:59 2023, max compression
```

## Comparing `html_report_line_profiler-0.0.1.tar` & `html_report_line_profiler-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-09 22:49:36.250918 html_report_line_profiler-0.0.1/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2365 2023-06-09 22:49:36.250918 html_report_line_profiler-0.0.1/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2009 2023-06-08 16:29:02.000000 html_report_line_profiler-0.0.1/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-09 22:49:36.234919 html_report_line_profiler-0.0.1/html_report_line_profiler/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      648 2023-06-09 22:37:23.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      448 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/__version__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-09 22:49:36.250918 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1267 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3437 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_extract_profiled_data.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1295 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_extract_tools.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      845 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_extract_with_mask.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      588 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_find_profiled_files.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1931 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_find_test_functions.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3038 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_generate_html_page.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_generate_page_index.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      369 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_generate_tools.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4123 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1772 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_tool_find.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2311 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_tools_profile.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      349 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/setup_profiler.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1159 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/html_report_line_profiler/teardown_profiler.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-09 22:49:36.238919 html_report_line_profiler-0.0.1/html_report_line_profiler.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2365 2023-06-09 22:49:36.000000 html_report_line_profiler-0.0.1/html_report_line_profiler.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1221 2023-06-09 22:49:36.000000 html_report_line_profiler-0.0.1/html_report_line_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-09 22:49:36.000000 html_report_line_profiler-0.0.1/html_report_line_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       26 2023-06-09 22:49:36.000000 html_report_line_profiler-0.0.1/html_report_line_profiler.egg-info/top_level.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)      195 2023-06-09 22:49:36.254918 html_report_line_profiler-0.0.1/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5417 2023-06-09 22:48:47.000000 html_report_line_profiler-0.0.1/setup.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-09 22:49:36.250918 html_report_line_profiler-0.0.1/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      376 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.1/tests/test.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.743239 html_report_line_profiler-0.0.2/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2877 2023-06-10 16:32:59.743239 html_report_line_profiler-0.0.2/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2009 2023-06-08 16:29:02.000000 html_report_line_profiler-0.0.2/README.md
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.719239 html_report_line_profiler-0.0.2/html_report_line_profiler/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      656 2023-06-10 16:30:42.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      504 2023-06-10 13:35:09.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/__version__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.739239 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      110 2023-06-10 16:17:34.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3437 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_profiled_data.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1295 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_tools.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      845 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_with_mask.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      588 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_profiled_files.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1931 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_test_functions.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3173 2023-06-09 23:31:14.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_html_page.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_page_index.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      467 2023-06-10 00:30:04.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_tools.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4294 2023-06-10 15:53:03.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1772 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tool_find.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2819 2023-06-10 15:54:13.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tools_profile.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1406 2023-06-10 16:31:54.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/generate_html_report_fct.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.739239 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      886 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/page.html
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2107 2023-06-10 15:51:42.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/style.css
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      551 2023-06-09 23:17:13.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/setup_profiler.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1264 2023-06-09 23:34:14.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/teardown_profiler.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.727239 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2877 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1510 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       46 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       26 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.715239 html_report_line_profiler-0.0.2/scripts/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      768 2023-06-10 16:29:39.000000 html_report_line_profiler-0.0.2/scripts/profiler_html_report.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      167 2023-06-10 16:32:59.743239 html_report_line_profiler-0.0.2/setup.cfg
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7052 2023-06-10 16:27:40.000000 html_report_line_profiler-0.0.2/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.739239 html_report_line_profiler-0.0.2/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      376 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/tests/test.py
```

### Comparing `html_report_line_profiler-0.0.1/PKG-INFO` & `html_report_line_profiler-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: html_report_line_profiler
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate an HTML report for line_parser
 Home-page: https://1sixunhuit.frama.io/html_report_line_profiler
 Author: Pierre
 Author-email: pierre@exemple.com
 License: AGPL 3
-Keywords: dotenv,.env,toolkit,parse dates
-Requires-Python: <4,>=3.9
+Keywords: ['profiling','profiler','line_profiler','html','report']
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Environment :: Console
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Natural Language :: French
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
+Provides-Extra: doc
+Provides-Extra: test
+Provides-Extra: upload
 
 # Utilisation :
 
 A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
 
 Dans :
 ```
```

### Comparing `html_report_line_profiler-0.0.1/README.md` & `html_report_line_profiler-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/__init__.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Generate html pages from line_parser profiler
 """
 
-from .generate_html_report import generate_html_report
+from .generate_html_report import generate_html_report_fct
 from .setup_profiler import setUp_profiler
 from .teardown_profiler import tearDown_profiler
 
 from .__version__ import (
     __author__,
     __author_email__,
     __copyright__,
@@ -20,11 +20,11 @@
 # requirements are in requirements.txt
 
 
 __all__ = [
     '__author__', '__author_email__',
     '__copyright__', '__description__', '__license__',
     '__title__', '__version__', '__pkg_name__',
-    "generate_html_report",
+    "generate_html_report_fct",
     "setUp_profiler",
     "tearDown_profiler"
 ]
```

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/__init__.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/generate_html_report_fct.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from ._find_test_functions import find_test_functions, testfunctions_to_dict
 from ._find_profiled_files import find_profiled_files
 
 from ._profilefile2htmlfile import functions2profilfile
 
 from ..__version__ import __pkg_name__
-def generate_html_report(the_dir:str="./", out_dir=None, build_tree:bool=True):
+
+def generate_html_report_fct(the_dir:str="./", out_dir=None, build_tree:bool=True):
     """
 :param str the_dir: Name of the directory
 :param str out_dir: Name of the out directory for html pages
 :param bool build_tree: Build a tree : /out_dir/module/function/test.html
 """
 
     if out_dir is None:
@@ -26,15 +27,22 @@
 
     list_mod = []
     total_time_mod = 0.0
 
     a = functions2profilfile(ordered_files, list_prof, ext=".dat", out_dir=out_dir, build_tree=build_tree)
 
     # Copie du fichier css
-    with open(f"../{__pkg_name__}/template/style.css", "r") as f:
+    template_css = os.path.abspath(
+        os.path.join(
+            os.path.dirname(__file__),
+            "template",
+            "style.css"
+        )
+    )
+    with open(template_css, "r") as f:
         css = f.read()
     # endWith
     with open(os.path.join(out_dir, "style.css"), "w") as f:
         f.write(css)
     # endWith
 
     # Creer index des fichiers du module :
```

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_extract_profiled_data.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_profiled_data.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_extract_tools.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_tools.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_extract_with_mask.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_with_mask.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_find_profiled_files.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_profiled_files.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_find_test_functions.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_test_functions.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_generate_html_page.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_html_page.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,16 +56,22 @@
                 <td class="time">{time}</td>
                 <td class="per-hit">{per_hit}</td>
                 <td class="percentage">{time_percentage}</td>
                 <td class="line-content">{line_content}</td>
             </tr>
         '''
     # endFor
-
-    with open(f"../{__pkg_name__}/template/page.html", "r") as f:
+    template_html = os.path.abspath(
+        os.path.join(
+            os.path.dirname(__file__),
+            "template",
+            "page.html"
+        )
+    )
+    with open(template_html, "r") as f:
         page = f.read()
     # endWith
 
 
     page = page.replace(":HEADER:", f"<div id='header'>{str(header)}</div>" if header else "")
     page = page.replace(
         ":TIME_UNIT:",
```

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_generate_page_index.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_page_index.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 
-from ._tools_profile import extract_profpath, profilefile2htmlfile, html2file
+from ._tools_profile import extract_profpath, profilefile2htmlfile, html2file,  names_file_class_fct2path
 from ._generate_html_page import generate_html_page
 from ..__version__ import __pkg_name__
 
 
 def functions2profilfile(ordered_files, list_prof, ext=".dat", out_dir="./", build_tree:bool=True):
 
     if ext[0] == "." and len(ext)>1:
@@ -25,15 +25,16 @@
         for class_name, d_class in d_file.items():
 
             total_time_fct = 0.0
             list_fct = []
 
             for each_fct in d_class["functions"]:
 
-                basename = f"{class_name}_{each_fct['name']}.{ext}"
+                basename = f"{file_name}_{class_name}_{each_fct['name']}.{ext}"
+
                 path_prof = extract_profpath(
                     basename=basename,
                     list_prof=list_prof,
                     rangelen_listprof=rl_listprof
                 )
 
                 if not path_prof:
@@ -42,14 +43,15 @@
 
                 each_fct["profile_in"] = path_prof
 
                 path_html, total_time = profilefile2htmlfile(
                     file_in=path_prof,
                     ext_in=".dat",
                     out_dir=out_dir,
+                    fct_name=each_fct['name'],
                     class_name=class_name,
                     file_name=file_name,
                     build_tree=build_tree
                 )
 
                 total_time_fct +=  float(str(total_time).strip().split(" ")[0])
 
@@ -70,44 +72,48 @@
             #
             # fonction1
             # - test1
             # - test2
 
             datas = {"timer unit":None,
                      "total time": total_time_fct,
-                     "file":f"{file_name}"  ,# nom du fichier source module/function.py
-                     "function":class_name, # nom de la classe
+                     "file":f"{file_name}",  # nom du fichier source module/function.py
+                     "function":class_name,  # nom de la classe
                      "report":list_fct
                      }
 
             total_time_mod +=  float(str(datas["total time"]).strip().split(" ")[0])
 
             html = generate_html_page(
                 datas,
                 path_css=out_dir,
                 header=f"<h1>INDEX : {class_name}</h1>"
             )
 
             basename = f'index.html'
 
             dirout1 = "/".join([e for e in out_dir.split("/") if e])
+            path_html_dir = names_file_class_fct2path(
+                base_path=out_dir,
+                file_name=file_name,
+                class_name=class_name,
+                fct_name=None,
+                build_tree=build_tree
+            )
 
             index_class_html = html2file(
                 html,
                 basename=basename,
-                out_dir=dirout1,
-                mod_name=class_name,
-                fct_name=None,
-                build_tree=build_tree
+                path=path_html_dir,
             )
 
             index_page.append(
                 {
                     "line": 0,
-                    "line content":f"<a href={os.path.abspath(index_class_html)}>{class_name}</a>"
+                    "line content":f"<a href={os.path.abspath(index_class_html)}>{file_name}.py: {class_name}</a>"
                     }
                 )
 
             sys.stdout.write(f"write file> {os.path.abspath(index_class_html)}\n")
         # endFor classname
     # endFor filename
 
@@ -127,14 +133,11 @@
 
 
     basename = f'index.html'
 
     html_page = html2file(
         html,
         basename=basename,
-        out_dir=out_dir,
-        mod_name=None,
-        fct_name=None,
-        build_tree=build_tree
+        path=out_dir
     )
     sys.stdout.write(f"write file> {os.path.abspath(html_page)}\n")
 #
```

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_tool_find.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tool_find.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/generate_html_report/_tools_profile.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tools_profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,115 @@
 import sys
 import os
 
 from ._extract_profiled_data import extract_profiled_data
 from ._generate_html_page import generate_html_page
 from ._extract_with_mask  import extractWithMask
 
+
+def names_file_class_fct2path(
+        base_path: str = "./",
+        file_name: str = None,
+        class_name: str = None,
+        fct_name: str = None,
+        build_tree: bool = True
+):
+
+    if build_tree:
+
+        ldirname = [
+            file_name.replace("/", "_").replace(".", "_") if file_name is not None else "",
+            class_name.replace("/", "_").replace(".", "_") if class_name is not None else ""
+        ]
+
+        dirname = "_".join([e for e in ldirname if e]).lower()
+        path = os.path.join(base_path, dirname)
+
+    else:
+
+        path = base_path
+
+    #endIf
+
+    # Creer le dossier si n'existe pas et ecrire le fichier
+    os.makedirs(path, exist_ok=True)
+
+    return os.path.abspath(path)
+#
+
 def profilefile2htmlfile(
         file_in:str="file.dat",
         ext_in:str=".dat",
         out_dir:str="./",
-        class_name:str="class_name",
         file_name:str="file_name",
+        class_name:str="class_name",
+        fct_name:str="function_name",
         build_tree:bool=True
         ):
 
     datas = extract_profiled_data(file_name=file_in)
 
+    datas["function"] = f"{file_name}.py: {class_name}: {fct_name}: {datas['function']}"
     html = generate_html_page(datas, path_css=out_dir)
 
-    basename_html = os.path.basename(file_in).replace(ext_in, ".html")
+    #basename_html = os.path.basename(file_in).replace(ext_in, ".html")
+    basename_html = f"{fct_name}.html".lower()
+
+    path_html_dir = names_file_class_fct2path(
+        base_path=out_dir,
+        file_name=file_name,
+        class_name=class_name,
+        fct_name=fct_name,
+        build_tree=build_tree
+    )
 
     path_html = html2file(
         html,
         basename=basename_html,
-        out_dir=out_dir,
-        mod_name=class_name,
-        fct_name=file_name,
-        build_tree=build_tree
+        path=path_html_dir
     )
 
     sys.stdout.write(f"write file> {os.path.abspath(path_html)}\n")
 
     return path_html, datas["total time"]
 #
 
 def extract_profpath(basename, list_prof, rangelen_listprof):
-    mask = [basename == os.path.basename(e) for e in list_prof]
+    basenamelow = basename.lower()
+    mask = [basenamelow == os.path.basename(e).lower() for e in list_prof]
 
     fileprof = extractWithMask(
         the_list=list_prof,
         the_mask=mask,
         rangelen_list=rangelen_listprof
     )
 
     if len(fileprof) == 1:
         return fileprof[0]
     elif len(fileprof) > 1:
-        print("unexpected, trop : ", fileprof)
-        print()
-        return  fileprof[0]
+        sys.stderr.write(f">unexpected, trop : {fileprof}\n\n")
+        return fileprof[0]
     # endIf
+
     return ""
 #
 
 
-def html2file(html, basename="out.html", out_dir="./", mod_name:str=None, fct_name:str=None, build_tree:bool=True):
+def html2file(html, basename="out.html", path="./"):
     """Write HTML file from string (html)
 
 :param str html: HTML content
-:param basename: Name of the html file
-:param mod_name: Name of the module
-:param fct_name: Name of the function
-:param bool build_tree: Build the tree directories
+:param str basename: Name of the html file
+:param str path: Path of the html file
 
 :return: the path to the html file
 :rtypes: str
 """
 
-    if build_tree:
-
-        path = os.path.join(
-            out_dir,
-            (mod_name.replace("/", "_").replace(".", "_") if mod_name is not None else ""),
-            (fct_name.replace("/", "_").replace(".", "_") if fct_name is not None else "")
-        )
-
-    else:
-
-        path = out_dir
-
-    #endIf
-
-    # Creer le dossier si n'existe pas et ecrire le fichier
-    os.makedirs(path, exist_ok=True)
     path_html = os.path.join(path, basename)
+
     with open(path_html, "w") as f:
         f.write(html)
     #endWith
+
     return path_html
 #end
```

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler/teardown_profiler.py` & `html_report_line_profiler-0.0.2/html_report_line_profiler/teardown_profiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import os
 import io
 
 #
 # class_name_t = class_name.lower().replace('test',"")
 # class_name_t = class_name_t if not class_name_t[0] == "_" else class_name_t[1:]
 # proffile_basename = os.path.join(dirout, f"{class_name_t}_{test_method_name}")
-def tearDown_profiler(proffile_basename="file", output_folder="./profile"):
+#
+def tearDown_profiler(profiler, proffile_basename="file", output_folder="./profile", delete_profiling_env:bool=False):
+    if profiler is None:
+        return
+    #
     # Code executé après chaque test
     #del self.my_class_instance
-    self.profiler.disable_by_count()
+    output_folder = os.path.abspath(output_folder)
+    profiler.disable_by_count()
     os.makedirs(output_folder, exist_ok=True)  # Creer si necessaire le dossier
 
-    test_method_name = self._testMethodName
-
     binary_file = f"{proffile_basename}.lprof"
-    output_folder = "./profile/"
     outfile = os.path.join(output_folder, binary_file)
-    self.profiler.dump_stats(outfile)
+    profiler.dump_stats(outfile)
     print(f">> WRITE {outfile}")
     #
 
-    text_file = f"{proffile_basename}.lprof"
+    text_file = f"{proffile_basename}.dat"
     output_stream = io.StringIO()
-    self.profiler.print_stats(stream=output_stream)
+    profiler.print_stats(stream=output_stream)
     stats_output = output_stream.getvalue()
 
-    with open(text_file, "w") as f:
+    with open(os.path.join(output_folder, text_file), "w") as f:
         f.write(stats_output)
     #
 
     print(f">> WRITE {text_file}")
 
-    self.profiler.print_stats()
-    if self.delete_profiling_env:
+    profiler.print_stats()
+    if delete_profiling_env and os.environ.get("PROFILING", False):
         del os.environ["PROFILING"]
     #
 #
```

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler.egg-info/PKG-INFO` & `html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: html-report-line-profiler
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate an HTML report for line_parser
 Home-page: https://1sixunhuit.frama.io/html_report_line_profiler
 Author: Pierre
 Author-email: pierre@exemple.com
 License: AGPL 3
-Keywords: dotenv,.env,toolkit,parse dates
-Requires-Python: <4,>=3.9
+Keywords: ['profiling','profiler','line_profiler','html','report']
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Environment :: Console
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Natural Language :: French
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
+Provides-Extra: doc
+Provides-Extra: test
+Provides-Extra: upload
 
 # Utilisation :
 
 A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
 
 Dans :
 ```
```

### Comparing `html_report_line_profiler-0.0.1/html_report_line_profiler.egg-info/SOURCES.txt` & `html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 README.md
 setup.cfg
 setup.py
+./scripts/profiler_html_report.py
 html_report_line_profiler/__init__.py
 html_report_line_profiler/__version__.py
 html_report_line_profiler/setup_profiler.py
 html_report_line_profiler/teardown_profiler.py
 html_report_line_profiler.egg-info/PKG-INFO
 html_report_line_profiler.egg-info/SOURCES.txt
 html_report_line_profiler.egg-info/dependency_links.txt
+html_report_line_profiler.egg-info/requires.txt
 html_report_line_profiler.egg-info/top_level.txt
 html_report_line_profiler/generate_html_report/__init__.py
 html_report_line_profiler/generate_html_report/_extract_profiled_data.py
 html_report_line_profiler/generate_html_report/_extract_tools.py
 html_report_line_profiler/generate_html_report/_extract_with_mask.py
 html_report_line_profiler/generate_html_report/_find_profiled_files.py
 html_report_line_profiler/generate_html_report/_find_test_functions.py
 html_report_line_profiler/generate_html_report/_generate_html_page.py
 html_report_line_profiler/generate_html_report/_generate_page_index.py
 html_report_line_profiler/generate_html_report/_generate_tools.py
 html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
 html_report_line_profiler/generate_html_report/_tool_find.py
 html_report_line_profiler/generate_html_report/_tools_profile.py
+html_report_line_profiler/generate_html_report/generate_html_report_fct.py
+html_report_line_profiler/generate_html_report/template/page.html
+html_report_line_profiler/generate_html_report/template/style.css
 tests/test.py
```

### Comparing `html_report_line_profiler-0.0.1/setup.py` & `html_report_line_profiler-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup
 import os
 import sys
+import glob
 
 # Variables ##########################################
 package_name = "html_report_line_profiler"
+packages = [package_name,f"{package_name}.generate_html_report"]
 # packages = Components of the package to add
-packages = [package_name, f"{package_name}.generate_html_report"]
+# package_dir = []  # pour importer des librairies par exemple, mais ne s'appelle pas comme des modules
 url_page = "https://1sixunhuit.frama.io"
 url_git = "https://framagit.org"
-package_data = {'template': ['page.html', 'style.css']}  # non py files
+package_data = {package_name: ['generate_html_report/template/page.html', 'generate_html_report/template/style.css']}  # non py files
 # #####################################################
 #
 # THEN : DO NOT MODIFY
 # --------------------
 # #####################################################
 
 def parse_version(path:str='./modulename/__version__.py'):
@@ -20,15 +22,16 @@
     with open(path, "r") as f:
         exec(f.read(), about)
     #endWith
     return about
 #endDef
 
 def parse_requirements(path:str='./requirements.txt'):
-    """    Parser le fichier requirements.txt
+    """
+    Parser le fichier requirements.txt
 
 - Nommer les categories de modules pour separer l'indispensable au package de ceux pour le deploiement et la doc
 - Les tags qui ne sont pas indiques ici seront consideres comme principaux
 > # tag
 > package == X.Y.Z
 
 - Pour creer une nouvelle categorie :
@@ -131,14 +134,23 @@
     packages = [line.split(' ')[0] for line in packages_lines]
     extras_require = {k:[e for e in v if e] for k,v in extras_pkg.items() if k}
 
     return packages, extras_require
 #endDef
 
 
+def find_scripts(script_dir="./scripts"):
+
+    if os.path.exists(script_dir):
+        return [e for e in glob.glob(os.path.join(script_dir, "*.py"))] # .replace(".py", "")
+    #endIf
+
+    return []
+#
+
 if __name__ == '__main__':
 
     try:
         import sphinx
     except ImportError:
         sphinxInstalled=False
     else:
@@ -166,24 +178,66 @@
     ## Creation de variables
     url = f'{url_page}/{about["__git_name__"]}'
     project_urls = {
         'Source Code': f'{url_git}/{about["__git_group__"]}/{about["__git_name__"]}',
     }
 
     # Setup ..........................................................
-    setup(
-        name = str(about["__pkg_name__"]),
-        version = str(about["__version__"]),
-        license = str(about["__license__"]),
-        copyright = str(about["__copyright__"]),
-        url = url,
-        project_url = project_urls,
-        author = str(about["__author__"]),
-        author_email = str(about["__author_email__"]),
-        description = str(about["__description__"]),
-        keywords=str(about["__keywords__"]),
-        packages=packages+packages_requirements,
-        extras_require=extras_require,
-        package_data=package_data,
-    )
+    setupkw = {}
+
+    # Metadata
+    setupkw["name"] = str(about["__pkg_name__"])
+    setupkw["version"] = str(about["__version__"])
+    setupkw["license"] = str(about["__license__"])
+    setupkw["copyright"] = str(about["__copyright__"])
+    setupkw["url"] = url
+    setupkw["project_url"] = project_urls
+    setupkw["author"] = str(about["__author__"])
+    setupkw["author_email"] = str(about["__author_email__"])
+    setupkw["description"] = str(about["__description__"])
+    setupkw["keywords"]=str(about["__keywords__"])
+
+    # Content
+    setupkw["packages"]=packages #*package_dir]
+    try:
+        setupkw["packages_dir"]=package_dir
+    except NameError:
+        setupkw["packages_dir"]=[]
+        print(">>> NO PKG DIR")
+    #
+    try:
+        setupkw["package_data"]=package_data
+    except NameError:
+        setupkw["package_data"]=[]
+        print(">>> NO PKG DATA")
+    #
+    try:
+        setupkw["scripts"]=find_scripts()
+        #find_scripts()  # generate env/bin/scriptname.py
+    except NameError:
+        setupkw["scripts"]=[]
+        print(">>> NO SCRIPT")
+    #
+
+    # Requirements :
+    setupkw["python_requires"]=str(about["__python_requires__"])
+    setupkw["install_requires"]=packages_requirements
+    setupkw["extras_require"]=extras_require
+
+    # Classifiers: cf https://pypi.org/classifiers/
+    setupkw["classifiers"]=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.9",
+        "Environment :: Console",
+        "Operating System :: POSIX :: Linux",
+        "Natural Language :: French",
+        "Natural Language :: English",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
+        "Operating System :: OS Independent",
+    ]
+
+    # No entry point, use scripts
+
+    setup(**setupkw)
 
 #endIf
```

