# Comparing `tmp/html_report_line_profiler-0.0.2.tar.gz` & `tmp/html_report_line_profiler-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_report_line_profiler-0.0.2.tar", last modified: Sat Jun 10 16:32:59 2023, max compression
+gzip compressed data, was "html_report_line_profiler-0.1.0.tar", last modified: Sat Jun 10 17:52:32 2023, max compression
```

## Comparing `html_report_line_profiler-0.0.2.tar` & `html_report_line_profiler-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.743239 html_report_line_profiler-0.0.2/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2877 2023-06-10 16:32:59.743239 html_report_line_profiler-0.0.2/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2009 2023-06-08 16:29:02.000000 html_report_line_profiler-0.0.2/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.719239 html_report_line_profiler-0.0.2/html_report_line_profiler/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      656 2023-06-10 16:30:42.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      504 2023-06-10 13:35:09.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/__version__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.739239 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      110 2023-06-10 16:17:34.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3437 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_profiled_data.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1295 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_tools.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      845 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_with_mask.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      588 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_profiled_files.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1931 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_test_functions.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3173 2023-06-09 23:31:14.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_html_page.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_page_index.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      467 2023-06-10 00:30:04.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_tools.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4294 2023-06-10 15:53:03.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1772 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tool_find.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2819 2023-06-10 15:54:13.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tools_profile.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1406 2023-06-10 16:31:54.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/generate_html_report_fct.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.739239 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      886 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/page.html
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2107 2023-06-10 15:51:42.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/style.css
--rw-r--r--   0 pierre    (1000) pierre    (1000)      551 2023-06-09 23:17:13.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/setup_profiler.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1264 2023-06-09 23:34:14.000000 html_report_line_profiler-0.0.2/html_report_line_profiler/teardown_profiler.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.727239 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2877 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1510 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       46 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       26 2023-06-10 16:32:59.000000 html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/top_level.txt
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.715239 html_report_line_profiler-0.0.2/scripts/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      768 2023-06-10 16:29:39.000000 html_report_line_profiler-0.0.2/scripts/profiler_html_report.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      167 2023-06-10 16:32:59.743239 html_report_line_profiler-0.0.2/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7052 2023-06-10 16:27:40.000000 html_report_line_profiler-0.0.2/setup.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 16:32:59.739239 html_report_line_profiler-0.0.2/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      376 2023-06-09 22:29:57.000000 html_report_line_profiler-0.0.2/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.259280 html_report_line_profiler-0.1.0/html_report_line_profiler/
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3437 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_profiled_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_with_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_profiled_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_test_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3693 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_html_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_page_index.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4323 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1772 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tool_find.py
+-rw-rw-rw-   0 root         (0) root         (0)     2870 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tools_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/generate_html_report_fct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/page.html
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/style.css
+-rw-rw-rw-   0 root         (0) root         (0)     1912 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/unittest_ext_profiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.259280 html_report_line_profiler-0.1.0/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/scripts/profiler_html_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     7052 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/setup.py
```

### Comparing `html_report_line_profiler-0.0.2/PKG-INFO` & `html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: html_report_line_profiler
-Version: 0.0.2
+Name: html-report-line-profiler
+Version: 0.1.0
 Summary: Generate an HTML report for line_parser
 Home-page: https://1sixunhuit.frama.io/html_report_line_profiler
 Author: Pierre
 Author-email: pierre@exemple.com
 License: AGPL 3
 Keywords: ['profiling','profiler','line_profiler','html','report']
 Classifier: Development Status :: 3 - Alpha
@@ -18,69 +18,65 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: upload
 
-# Utilisation :
+# Utilisation dans les tests unitaires :
 
 A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
 
 Dans :
 ```
+[...]
+
+import html_report_line_profiler as hr
+
+
 class Test_CeciEstUnTest(unittest.TestCase):
     def setUp(self):
         # Code execute avant chaque test
         [...] # ce que l'on veut
 
         # Profiler :
-        if os.environ.get("PROFILING", False).lower() == "time":
-            os.environ["PROFILING"] = "1"
-            self.delete_profiling_env = True
-
-            self.profiler = LineProfiler()
-            self.profiler.add_function(str2digit)
-            self.profiler.enable_by_count()
-        #endIf
+        self.profiler, self.delete_profiling_env = hr.setUp_profiler(castList)
+
     #endDef
 
     # ...
 
     def tearDown(self):
         # Code executé après chaque test
         # Terminer le profiler en premier
-        if os.environ.get("PROFILING", False).lower() == "time":
-            output_folder = "./profile_time/"
-            self.profiler.disable_by_count()
-            os.makedirs(output_folder, exist_ok=True)  # Creer si necessaire le dossier
-
-            test_method_name = self._testMethodName
-            class_name = self.__class__.__name__
-
-            # Ecriture du fichier .lprof
-            filename = f"{class_name}_{test_method_name}.lprof".replace("Test_","")
-            outfile = os.path.join(output_folder, filename)
-            self.profiler.dump_stats(outfile)
-            print(f">> WRITE {outfile}")
-
-            # Ecriture du fichier texte
-            outfile = outfile.replace(".lprof", ".dat")
-            output_stream = io.StringIO()
-            self.profiler.print_stats(stream=output_stream)
-            stats_output = output_stream.getvalue()
-            with open(outfile, "w") as f:
-                f.write(stats_output)
- 	    #
-            print(f">> WRITE {outfile}")
-
-            # Affichage a l'ecran
-            self.profiler.print_stats()
-	    
-	    # Supprimer la variable d'environnement
-            if self.delete_profiling_env:
-                del os.environ["PROFILING"]
-	    #
+
+        # Create basename
+        hr.proffile_basename = classname2basename(
+            file_name = __file__,
+            class_name = self.__class__.__name__,
+            method_name = self._testMethodName
+        )
+
+        # Launch the profiler out
+        hr.tearDown_profiler(
+            profiler=self.profiler,
+            proffile_basename=proffile_basename,
+            output_folder=output_folder,
+            delete_profiling_env=self.delete_profiling_env
+        )
         #
 	# [...] # Les autres commandes
     #endDef
 #endClass
+```
+
+
+# Rapport HTML
+Pour lancer ensuite le post-traitement (rapport html) :
+```
+$ profiler_html_report.py
+```
+
+Remarques
+
+* `-d = --input-dir` (default : './profile')
+* `-o = --output-dir` (default : './profile_html')
```

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/__init__.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Generate html pages from line_parser profiler
 """
 
 from .generate_html_report import generate_html_report_fct
-from .setup_profiler import setUp_profiler
-from .teardown_profiler import tearDown_profiler
+from .unittest_ext_profiler import setUp_profiler, tearDown_profiler, names2basename
 
 from .__version__ import (
     __author__,
     __author_email__,
     __copyright__,
     __description__,
     __license__,
@@ -22,9 +21,10 @@
 
 __all__ = [
     '__author__', '__author_email__',
     '__copyright__', '__description__', '__license__',
     '__title__', '__version__', '__pkg_name__',
     "generate_html_report_fct",
     "setUp_profiler",
-    "tearDown_profiler"
+    "tearDown_profiler",
+    "names2basename"
 ]
```

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_profiled_data.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_profiled_data.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_tools.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_tools.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_extract_with_mask.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_with_mask.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_profiled_files.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_profiled_files.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_find_test_functions.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_test_functions.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_html_page.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_html_page.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,199 +1,231 @@
 00000000: 696d 706f 7274 206f 730a 0a66 726f 6d20  import os..from 
 00000010: 2e5f 6765 6e65 7261 7465 5f74 6f6f 6c73  ._generate_tools
 00000020: 2069 6d70 6f72 7420 6765 745f 696e 7465   import get_inte
 00000030: 7276 616c 0a66 726f 6d20 2e2e 5f5f 7665  rval.from ..__ve
 00000040: 7273 696f 6e5f 5f20 696d 706f 7274 205f  rsion__ import _
 00000050: 5f70 6b67 5f6e 616d 655f 5f0a 0a64 6566  _pkg_name__..def
 00000060: 2067 656e 6572 6174 655f 6874 6d6c 5f70   generate_html_p
-00000070: 6167 6528 6461 7461 2c20 7061 7468 5f63  age(data, path_c
-00000080: 7373 3a73 7472 3d22 222c 2068 6561 6465  ss:str="", heade
-00000090: 723a 7374 723d 2222 293a 0a20 2020 2022  r:str=""):.    "
-000000a0: 2222 436f 6e76 6572 7420 6469 6374 2063  ""Convert dict c
-000000b0: 7265 6174 6520 7769 7468 203a 6675 6e63  reate with :func
-000000c0: 3a60 6578 7472 6163 745f 7072 6f66 696c  :`extract_profil
-000000d0: 655f 6461 7461 6020 746f 2061 6e20 4854  e_data` to an HT
-000000e0: 4d4c 2070 6167 650a 0a3a 7061 7261 6d20  ML page..:param 
-000000f0: 6469 6374 2064 6174 613a 207b 2774 696d  dict data: {'tim
-00000100: 6572 2075 6e69 7427 2c20 2774 6f74 616c  er unit', 'total
-00000110: 2074 696d 6527 2c20 2766 696c 6527 2c20   time', 'file', 
-00000120: 2766 756e 6374 696f 6e27 2c20 2772 6570  'function', 'rep
-00000130: 6f72 7427 3a20 5b20 7b6c 696e 652c 2068  ort': [ {line, h
-00000140: 6974 732c 2070 6572 2068 6974 2c20 2520  its, per hit, % 
-00000150: 7469 6d65 2c20 6c69 6e65 2063 6f6e 7465  time, line conte
-00000160: 6e74 7d2c 202e 2e2e 5d7d 0a3a 7061 7261  nt}, ...]}.:para
-00000170: 6d20 7374 7220 7061 7468 5f63 7373 3a20  m str path_css: 
-00000180: 7061 7468 2066 6f72 2074 6865 2063 7373  path for the css
-00000190: 2066 696c 650a 3a70 6172 616d 2073 7472   file.:param str
-000001a0: 2068 6561 6465 723a 2041 6464 2068 6561   header: Add hea
-000001b0: 6465 720a 0a3a 7265 7475 726e 3a20 4854  der..:return: HT
-000001c0: 4d4c 2063 6f6e 7465 6e74 0a3a 7274 7970  ML content.:rtyp
-000001d0: 6573 3a20 7374 720a 2222 220a 2020 2020  es: str.""".    
-000001e0: 6874 6d6c 203d 2022 220a 0a20 2020 2066  html = ""..    f
-000001f0: 6f72 206c 696e 655f 6461 7461 2069 6e20  or line_data in 
-00000200: 6461 7461 5b27 7265 706f 7274 275d 3a0a  data['report']:.
-00000210: 0a20 2020 2020 2020 206c 696e 6520 3d20  .        line = 
-00000220: 6c69 6e65 5f64 6174 615b 276c 696e 6527  line_data['line'
-00000230: 5d0a 0a20 2020 2020 2020 2069 6620 2768  ]..        if 'h
-00000240: 6974 7327 2069 6e20 6c69 6e65 5f64 6174  its' in line_dat
-00000250: 612e 6b65 7973 2829 2061 6e64 206c 696e  a.keys() and lin
-00000260: 655f 6461 7461 5b27 6869 7473 275d 2069  e_data['hits'] i
-00000270: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00000280: 2020 2020 2020 2020 6869 7473 203d 206c          hits = l
-00000290: 696e 655f 6461 7461 5b27 6869 7473 275d  ine_data['hits']
-000002a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000002b0: 2020 2020 2020 2020 2020 2068 6974 7320             hits 
-000002c0: 3d20 2727 0a20 2020 2020 2020 2023 0a0a  = ''.        #..
-000002d0: 2020 2020 2020 2020 6966 2027 7469 6d65          if 'time
-000002e0: 2720 696e 206c 696e 655f 6461 7461 2e6b  ' in line_data.k
-000002f0: 6579 7328 2920 616e 6420 6c69 6e65 5f64  eys() and line_d
-00000300: 6174 615b 2774 696d 6527 5d20 6973 206e  ata['time'] is n
-00000310: 6f74 204e 6f6e 6520 3a0a 2020 2020 2020  ot None :.      
-00000320: 2020 2020 2020 7469 6d65 203d 206c 696e        time = lin
-00000330: 655f 6461 7461 5b27 7469 6d65 275d 0a20  e_data['time']. 
-00000340: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000350: 2020 2020 2020 2020 2074 696d 6520 3d20           time = 
-00000360: 2727 0a20 2020 2020 2020 2023 0a0a 2020  ''.        #..  
-00000370: 2020 2020 2020 6966 2027 7065 7220 6869        if 'per hi
-00000380: 7427 2069 6e20 6c69 6e65 5f64 6174 612e  t' in line_data.
-00000390: 6b65 7973 2829 2061 6e64 206c 696e 655f  keys() and line_
-000003a0: 6461 7461 5b27 7065 7220 6869 7427 5d20  data['per hit'] 
-000003b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000003c0: 2020 2020 2020 2020 2070 6572 5f68 6974           per_hit
-000003d0: 203d 206c 696e 655f 6461 7461 5b27 7065   = line_data['pe
-000003e0: 7220 6869 7427 5d0a 2020 2020 2020 2020  r hit'].        
-000003f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00000400: 2020 7065 725f 6869 7420 3d20 2727 0a20    per_hit = ''. 
-00000410: 2020 2020 2020 2023 0a0a 2020 2020 2020         #..      
-00000420: 2020 6966 2027 2520 7469 6d65 2720 696e    if '% time' in
-00000430: 206c 696e 655f 6461 7461 2e6b 6579 7328   line_data.keys(
-00000440: 2920 616e 6420 6c69 6e65 5f64 6174 615b  ) and line_data[
-00000450: 2725 2074 696d 6527 5d20 6973 206e 6f74  '% time'] is not
-00000460: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00000470: 2020 2074 696d 655f 7065 7263 656e 7461     time_percenta
-00000480: 6765 203d 206c 696e 655f 6461 7461 5b27  ge = line_data['
-00000490: 2520 7469 6d65 275d 0a20 2020 2020 2020  % time'].       
-000004a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000004b0: 2020 2074 696d 655f 7065 7263 656e 7461     time_percenta
-000004c0: 6765 203d 2027 270a 2020 2020 2020 2020  ge = ''.        
-000004d0: 230a 0a20 2020 2020 2020 2069 6620 276c  #..        if 'l
-000004e0: 696e 6520 636f 6e74 656e 7427 2069 6e20  ine content' in 
-000004f0: 6c69 6e65 5f64 6174 612e 6b65 7973 2829  line_data.keys()
-00000500: 2061 6e64 206c 696e 655f 6461 7461 5b27   and line_data['
-00000510: 6c69 6e65 2063 6f6e 7465 6e74 275d 2069  line content'] i
-00000520: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00000530: 2020 2020 2020 2020 6c69 6e65 5f63 6f6e          line_con
-00000540: 7465 6e74 203d 206c 696e 655f 6461 7461  tent = line_data
-00000550: 5b27 6c69 6e65 2063 6f6e 7465 6e74 275d  ['line content']
-00000560: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00000570: 2020 2020 2020 2020 2020 206c 696e 655f             line_
-00000580: 636f 6e74 656e 7420 3d20 2727 0a20 2020  content = ''.   
-00000590: 2020 2020 2023 0a0a 2020 2020 2020 2020       #..        
-000005a0: 6874 6d6c 202b 3d20 6627 2727 0a20 2020  html += f'''.   
-000005b0: 2020 2020 2020 2020 203c 7472 2063 6c61           <tr cla
-000005c0: 7373 3d22 7b67 6574 5f69 6e74 6572 7661  ss="{get_interva
-000005d0: 6c28 7469 6d65 5f70 6572 6365 6e74 6167  l(time_percentag
-000005e0: 6529 7d22 3e0a 2020 2020 2020 2020 2020  e)}">.          
-000005f0: 2020 2020 2020 3c74 6420 636c 6173 733d        <td class=
-00000600: 226c 696e 652d 6e75 6d62 6572 223e 7b6c  "line-number">{l
-00000610: 696e 657d 3c2f 7464 3e0a 2020 2020 2020  ine}</td>.      
-00000620: 2020 2020 2020 2020 2020 3c74 6420 636c            <td cl
-00000630: 6173 733d 2268 6974 7322 3e7b 6869 7473  ass="hits">{hits
-00000640: 7d3c 2f74 643e 0a20 2020 2020 2020 2020  }</td>.         
-00000650: 2020 2020 2020 203c 7464 2063 6c61 7373         <td class
-00000660: 3d22 7469 6d65 223e 7b74 696d 657d 3c2f  ="time">{time}</
-00000670: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
-00000680: 2020 2020 3c74 6420 636c 6173 733d 2270      <td class="p
-00000690: 6572 2d68 6974 223e 7b70 6572 5f68 6974  er-hit">{per_hit
-000006a0: 7d3c 2f74 643e 0a20 2020 2020 2020 2020  }</td>.         
-000006b0: 2020 2020 2020 203c 7464 2063 6c61 7373         <td class
-000006c0: 3d22 7065 7263 656e 7461 6765 223e 7b74  ="percentage">{t
-000006d0: 696d 655f 7065 7263 656e 7461 6765 7d3c  ime_percentage}<
-000006e0: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
-000006f0: 2020 2020 203c 7464 2063 6c61 7373 3d22       <td class="
-00000700: 6c69 6e65 2d63 6f6e 7465 6e74 223e 7b6c  line-content">{l
-00000710: 696e 655f 636f 6e74 656e 747d 3c2f 7464  ine_content}</td
-00000720: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-00000730: 7472 3e0a 2020 2020 2020 2020 2727 270a  tr>.        '''.
-00000740: 2020 2020 2320 656e 6446 6f72 0a20 2020      # endFor.   
-00000750: 2074 656d 706c 6174 655f 6874 6d6c 203d   template_html =
-00000760: 206f 732e 7061 7468 2e61 6273 7061 7468   os.path.abspath
-00000770: 280a 2020 2020 2020 2020 6f73 2e70 6174  (.        os.pat
-00000780: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
-00000790: 2020 2020 6f73 2e70 6174 682e 6469 726e      os.path.dirn
-000007a0: 616d 6528 5f5f 6669 6c65 5f5f 292c 0a20  ame(__file__),. 
-000007b0: 2020 2020 2020 2020 2020 2022 7465 6d70             "temp
-000007c0: 6c61 7465 222c 0a20 2020 2020 2020 2020  late",.         
-000007d0: 2020 2022 7061 6765 2e68 746d 6c22 0a20     "page.html". 
-000007e0: 2020 2020 2020 2029 0a20 2020 2029 0a20         ).    ). 
-000007f0: 2020 2077 6974 6820 6f70 656e 2874 656d     with open(tem
-00000800: 706c 6174 655f 6874 6d6c 2c20 2272 2229  plate_html, "r")
-00000810: 2061 7320 663a 0a20 2020 2020 2020 2070   as f:.        p
-00000820: 6167 6520 3d20 662e 7265 6164 2829 0a20  age = f.read(). 
-00000830: 2020 2023 2065 6e64 5769 7468 0a0a 0a20     # endWith... 
-00000840: 2020 2070 6167 6520 3d20 7061 6765 2e72     page = page.r
-00000850: 6570 6c61 6365 2822 3a48 4541 4445 523a  eplace(":HEADER:
-00000860: 222c 2066 223c 6469 7620 6964 3d27 6865  ", f"<div id='he
-00000870: 6164 6572 273e 7b73 7472 2868 6561 6465  ader'>{str(heade
-00000880: 7229 7d3c 2f64 6976 3e22 2069 6620 6865  r)}</div>" if he
-00000890: 6164 6572 2065 6c73 6520 2222 290a 2020  ader else "").  
-000008a0: 2020 7061 6765 203d 2070 6167 652e 7265    page = page.re
-000008b0: 706c 6163 6528 0a20 2020 2020 2020 2022  place(.        "
-000008c0: 3a54 494d 455f 554e 4954 3a22 2c0a 2020  :TIME_UNIT:",.  
-000008d0: 2020 2020 2020 7374 7228 6461 7461 5b27        str(data['
-000008e0: 7469 6d65 7220 756e 6974 275d 290a 2020  timer unit']).  
-000008f0: 2020 2020 2020 6966 2027 7469 6d65 7220        if 'timer 
-00000900: 756e 6974 2720 696e 2064 6174 612e 6b65  unit' in data.ke
-00000910: 7973 2829 2061 6e64 0a20 2020 2020 2020  ys() and.       
-00000920: 2064 6174 615b 2774 696d 6572 2075 6e69   data['timer uni
-00000930: 7427 5d20 6973 206e 6f74 204e 6f6e 650a  t'] is not None.
-00000940: 2020 2020 2020 2020 656c 7365 2027 270a          else ''.
-00000950: 2020 2020 290a 2020 2020 7061 6765 203d      ).    page =
-00000960: 2070 6167 652e 7265 706c 6163 6528 0a20   page.replace(. 
-00000970: 2020 2020 2020 2022 3a54 4f54 414c 5f54         ":TOTAL_T
-00000980: 494d 453a 222c 0a20 2020 2020 2020 2073  IME:",.        s
-00000990: 7472 2864 6174 615b 2774 6f74 616c 2074  tr(data['total t
-000009a0: 696d 6527 5d29 0a20 2020 2020 2020 2069  ime']).        i
-000009b0: 6620 2774 6f74 616c 2074 696d 6527 2069  f 'total time' i
-000009c0: 6e20 6461 7461 2e6b 6579 7328 2920 616e  n data.keys() an
-000009d0: 640a 2020 2020 2020 2020 6461 7461 5b27  d.        data['
-000009e0: 746f 7461 6c20 7469 6d65 275d 2069 7320  total time'] is 
-000009f0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-00000a00: 2065 6c73 6520 2727 0a20 2020 2029 0a20   else ''.    ). 
-00000a10: 2020 2070 6167 6520 3d20 7061 6765 2e72     page = page.r
-00000a20: 6570 6c61 6365 280a 2020 2020 2020 2020  eplace(.        
-00000a30: 223a 4649 4c45 3a22 2c0a 2020 2020 2020  ":FILE:",.      
-00000a40: 2020 7374 7228 6461 7461 5b27 6669 6c65    str(data['file
-00000a50: 275d 290a 2020 2020 2020 2020 6966 2027  ']).        if '
-00000a60: 6669 6c65 2720 696e 2064 6174 612e 6b65  file' in data.ke
-00000a70: 7973 2829 2061 6e64 0a20 2020 2020 2020  ys() and.       
-00000a80: 2064 6174 615b 2766 696c 6527 5d20 6973   data['file'] is
-00000a90: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-00000aa0: 2020 656c 7365 2027 270a 2020 2020 290a    else ''.    ).
-00000ab0: 2020 2020 7061 6765 203d 2070 6167 652e      page = page.
-00000ac0: 7265 706c 6163 6528 0a20 2020 2020 2020  replace(.       
-00000ad0: 2022 3a46 554e 4354 494f 4e3a 222c 0a20   ":FUNCTION:",. 
-00000ae0: 2020 2020 2020 2073 7472 2864 6174 615b         str(data[
-00000af0: 2766 756e 6374 696f 6e27 5d29 0a20 2020  'function']).   
-00000b00: 2020 2020 2069 6620 2766 756e 6374 696f       if 'functio
-00000b10: 6e27 2069 6e20 6461 7461 2e6b 6579 7328  n' in data.keys(
-00000b20: 2920 616e 640a 2020 2020 2020 2020 6461  ) and.        da
-00000b30: 7461 5b27 6675 6e63 7469 6f6e 275d 2069  ta['function'] i
-00000b40: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00000b50: 2020 2065 6c73 6520 2727 0a20 2020 2029     else ''.    )
-00000b60: 0a20 2020 2070 6167 6520 3d20 7061 6765  .    page = page
-00000b70: 2e72 6570 6c61 6365 280a 2020 2020 2020  .replace(.      
-00000b80: 2020 223a 434f 4e54 454e 543a 222c 0a20    ":CONTENT:",. 
-00000b90: 2020 2020 2020 2073 7472 2868 746d 6c29         str(html)
-00000ba0: 0a20 2020 2020 2020 2069 6620 6874 6d6c  .        if html
-00000bb0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00000bc0: 2020 2020 2065 6c73 6520 2727 0a20 2020       else ''.   
-00000bd0: 2029 0a0a 2020 2020 6966 2070 6174 685f   )..    if path_
-00000be0: 6373 733a 0a20 2020 2020 2020 2070 6167  css:.        pag
-00000bf0: 6520 3d20 7061 6765 2e72 6570 6c61 6365  e = page.replace
-00000c00: 2822 2e2f 7374 796c 652e 6373 7322 2c20  ("./style.css", 
-00000c10: 6f73 2e70 6174 682e 6162 7370 6174 6828  os.path.abspath(
-00000c20: 6f73 2e70 6174 682e 6a6f 696e 2870 6174  os.path.join(pat
-00000c30: 685f 6373 732c 2022 7374 796c 652e 6373  h_css, "style.cs
-00000c40: 7322 2929 290a 2020 2020 2320 656e 6449  s"))).    # endI
-00000c50: 660a 0a20 2020 2072 6574 7572 6e20 7061  f..    return pa
-00000c60: 6765 0a0a 0a                             ge...
+00000070: 6167 6528 0a20 2020 2020 2020 2064 6174  age(.        dat
+00000080: 612c 0a20 2020 2020 2020 2070 6174 685f  a,.        path_
+00000090: 6373 733a 7374 723d 2222 2c0a 2020 2020  css:str="",.    
+000000a0: 2020 2020 6865 6164 6572 3a73 7472 3d22      header:str="
+000000b0: 222c 0a20 2020 2020 2020 2069 6e64 6578  ",.        index
+000000c0: 5f73 616d 655f 6469 723a 626f 6f6c 203d  _same_dir:bool =
+000000d0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+000000e0: 6e6f 745f 6162 6f76 655f 696e 6465 783a  not_above_index:
+000000f0: 2062 6f6f 6c20 3d20 4661 6c73 650a 293a   bool = False.):
+00000100: 0a20 2020 2022 2222 436f 6e76 6572 7420  .    """Convert 
+00000110: 6469 6374 2063 7265 6174 6520 7769 7468  dict create with
+00000120: 203a 6675 6e63 3a60 6578 7472 6163 745f   :func:`extract_
+00000130: 7072 6f66 696c 655f 6461 7461 6020 746f  profile_data` to
+00000140: 2061 6e20 4854 4d4c 2070 6167 650a 0a3a   an HTML page..:
+00000150: 7061 7261 6d20 6469 6374 2064 6174 613a  param dict data:
+00000160: 207b 2774 696d 6572 2075 6e69 7427 2c20   {'timer unit', 
+00000170: 2774 6f74 616c 2074 696d 6527 2c20 2766  'total time', 'f
+00000180: 696c 6527 2c20 2766 756e 6374 696f 6e27  ile', 'function'
+00000190: 2c20 2772 6570 6f72 7427 3a20 5b20 7b6c  , 'report': [ {l
+000001a0: 696e 652c 2068 6974 732c 2070 6572 2068  ine, hits, per h
+000001b0: 6974 2c20 2520 7469 6d65 2c20 6c69 6e65  it, % time, line
+000001c0: 2063 6f6e 7465 6e74 7d2c 202e 2e2e 5d7d   content}, ...]}
+000001d0: 0a3a 7061 7261 6d20 7374 7220 7061 7468  .:param str path
+000001e0: 5f63 7373 3a20 7061 7468 2066 6f72 2074  _css: path for t
+000001f0: 6865 2063 7373 2066 696c 650a 3a70 6172  he css file.:par
+00000200: 616d 2073 7472 2068 6561 6465 723a 2041  am str header: A
+00000210: 6464 2068 6561 6465 720a 3a70 6172 616d  dd header.:param
+00000220: 2062 6f6f 6c20 696e 6465 785f 7361 6d65   bool index_same
+00000230: 5f64 6972 3a20 496e 6465 7820 6973 2069  _dir: Index is i
+00000240: 6e20 7468 6520 7361 6d65 2064 6972 6563  n the same direc
+00000250: 746f 7279 2028 7072 696f 7269 7479 206f  tory (priority o
+00000260: 6e20 6e6f 745f 6162 6f76 655f 696e 6465  n not_above_inde
+00000270: 7829 0a3a 7061 7261 6d20 626f 6f6c 206e  x).:param bool n
+00000280: 6f74 5f61 626f 7665 5f69 6e64 6578 3a20  ot_above_index: 
+00000290: 4e6f 7420 696e 6465 782e 6874 6d6c 2061  Not index.html a
+000002a0: 626f 7665 0a0a 3a72 6574 7572 6e3a 2048  bove..:return: H
+000002b0: 544d 4c20 636f 6e74 656e 740a 3a72 7479  TML content.:rty
+000002c0: 7065 733a 2073 7472 0a22 2222 0a20 2020  pes: str.""".   
+000002d0: 2068 746d 6c20 3d20 2222 0a0a 2020 2020   html = ""..    
+000002e0: 666f 7220 6c69 6e65 5f64 6174 6120 696e  for line_data in
+000002f0: 2064 6174 615b 2772 6570 6f72 7427 5d3a   data['report']:
+00000300: 0a0a 2020 2020 2020 2020 6c69 6e65 203d  ..        line =
+00000310: 206c 696e 655f 6461 7461 5b27 6c69 6e65   line_data['line
+00000320: 275d 0a0a 2020 2020 2020 2020 6966 2027  ']..        if '
+00000330: 6869 7473 2720 696e 206c 696e 655f 6461  hits' in line_da
+00000340: 7461 2e6b 6579 7328 2920 616e 6420 6c69  ta.keys() and li
+00000350: 6e65 5f64 6174 615b 2768 6974 7327 5d20  ne_data['hits'] 
+00000360: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00000370: 2020 2020 2020 2020 2068 6974 7320 3d20           hits = 
+00000380: 6c69 6e65 5f64 6174 615b 2768 6974 7327  line_data['hits'
+00000390: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+000003a0: 2020 2020 2020 2020 2020 2020 6869 7473              hits
+000003b0: 203d 2027 270a 2020 2020 2020 2020 230a   = ''.        #.
+000003c0: 0a20 2020 2020 2020 2069 6620 2774 696d  .        if 'tim
+000003d0: 6527 2069 6e20 6c69 6e65 5f64 6174 612e  e' in line_data.
+000003e0: 6b65 7973 2829 2061 6e64 206c 696e 655f  keys() and line_
+000003f0: 6461 7461 5b27 7469 6d65 275d 2069 7320  data['time'] is 
+00000400: 6e6f 7420 4e6f 6e65 203a 0a20 2020 2020  not None :.     
+00000410: 2020 2020 2020 2074 696d 6520 3d20 6c69         time = li
+00000420: 6e65 5f64 6174 615b 2774 696d 6527 5d0a  ne_data['time'].
+00000430: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000440: 2020 2020 2020 2020 2020 7469 6d65 203d            time =
+00000450: 2027 270a 2020 2020 2020 2020 230a 0a20   ''.        #.. 
+00000460: 2020 2020 2020 2069 6620 2770 6572 2068         if 'per h
+00000470: 6974 2720 696e 206c 696e 655f 6461 7461  it' in line_data
+00000480: 2e6b 6579 7328 2920 616e 6420 6c69 6e65  .keys() and line
+00000490: 5f64 6174 615b 2770 6572 2068 6974 275d  _data['per hit']
+000004a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000004b0: 2020 2020 2020 2020 2020 7065 725f 6869            per_hi
+000004c0: 7420 3d20 6c69 6e65 5f64 6174 615b 2770  t = line_data['p
+000004d0: 6572 2068 6974 275d 0a20 2020 2020 2020  er hit'].       
+000004e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000004f0: 2020 2070 6572 5f68 6974 203d 2027 270a     per_hit = ''.
+00000500: 2020 2020 2020 2020 230a 0a20 2020 2020          #..     
+00000510: 2020 2069 6620 2725 2074 696d 6527 2069     if '% time' i
+00000520: 6e20 6c69 6e65 5f64 6174 612e 6b65 7973  n line_data.keys
+00000530: 2829 2061 6e64 206c 696e 655f 6461 7461  () and line_data
+00000540: 5b27 2520 7469 6d65 275d 2069 7320 6e6f  ['% time'] is no
+00000550: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00000560: 2020 2020 7469 6d65 5f70 6572 6365 6e74      time_percent
+00000570: 6167 6520 3d20 6c69 6e65 5f64 6174 615b  age = line_data[
+00000580: 2725 2074 696d 6527 5d0a 2020 2020 2020  '% time'].      
+00000590: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000005a0: 2020 2020 7469 6d65 5f70 6572 6365 6e74      time_percent
+000005b0: 6167 6520 3d20 2727 0a20 2020 2020 2020  age = ''.       
+000005c0: 2023 0a0a 2020 2020 2020 2020 6966 2027   #..        if '
+000005d0: 6c69 6e65 2063 6f6e 7465 6e74 2720 696e  line content' in
+000005e0: 206c 696e 655f 6461 7461 2e6b 6579 7328   line_data.keys(
+000005f0: 2920 616e 6420 6c69 6e65 5f64 6174 615b  ) and line_data[
+00000600: 276c 696e 6520 636f 6e74 656e 7427 5d20  'line content'] 
+00000610: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00000620: 2020 2020 2020 2020 206c 696e 655f 636f           line_co
+00000630: 6e74 656e 7420 3d20 6c69 6e65 5f64 6174  ntent = line_dat
+00000640: 615b 276c 696e 6520 636f 6e74 656e 7427  a['line content'
+00000650: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+00000660: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00000670: 5f63 6f6e 7465 6e74 203d 2027 270a 2020  _content = ''.  
+00000680: 2020 2020 2020 230a 0a20 2020 2020 2020        #..       
+00000690: 2068 746d 6c20 2b3d 2066 2727 270a 2020   html += f'''.  
+000006a0: 2020 2020 2020 2020 2020 3c74 7220 636c            <tr cl
+000006b0: 6173 733d 227b 6765 745f 696e 7465 7276  ass="{get_interv
+000006c0: 616c 2874 696d 655f 7065 7263 656e 7461  al(time_percenta
+000006d0: 6765 297d 223e 0a20 2020 2020 2020 2020  ge)}">.         
+000006e0: 2020 2020 2020 203c 7464 2063 6c61 7373         <td class
+000006f0: 3d22 6c69 6e65 2d6e 756d 6265 7222 3e7b  ="line-number">{
+00000700: 6c69 6e65 7d3c 2f74 643e 0a20 2020 2020  line}</td>.     
+00000710: 2020 2020 2020 2020 2020 203c 7464 2063             <td c
+00000720: 6c61 7373 3d22 6869 7473 223e 7b68 6974  lass="hits">{hit
+00000730: 737d 3c2f 7464 3e0a 2020 2020 2020 2020  s}</td>.        
+00000740: 2020 2020 2020 2020 3c74 6420 636c 6173          <td clas
+00000750: 733d 2274 696d 6522 3e7b 7469 6d65 7d3c  s="time">{time}<
+00000760: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+00000770: 2020 2020 203c 7464 2063 6c61 7373 3d22       <td class="
+00000780: 7065 722d 6869 7422 3e7b 7065 725f 6869  per-hit">{per_hi
+00000790: 747d 3c2f 7464 3e0a 2020 2020 2020 2020  t}</td>.        
+000007a0: 2020 2020 2020 2020 3c74 6420 636c 6173          <td clas
+000007b0: 733d 2270 6572 6365 6e74 6167 6522 3e7b  s="percentage">{
+000007c0: 7469 6d65 5f70 6572 6365 6e74 6167 657d  time_percentage}
+000007d0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+000007e0: 2020 2020 2020 3c74 6420 636c 6173 733d        <td class=
+000007f0: 226c 696e 652d 636f 6e74 656e 7422 3e7b  "line-content">{
+00000800: 6c69 6e65 5f63 6f6e 7465 6e74 7d3c 2f74  line_content}</t
+00000810: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
+00000820: 2f74 723e 0a20 2020 2020 2020 2027 2727  /tr>.        '''
+00000830: 0a20 2020 2023 2065 6e64 466f 720a 2020  .    # endFor.  
+00000840: 2020 7465 6d70 6c61 7465 5f68 746d 6c20    template_html 
+00000850: 3d20 6f73 2e70 6174 682e 6162 7370 6174  = os.path.abspat
+00000860: 6828 0a20 2020 2020 2020 206f 732e 7061  h(.        os.pa
+00000870: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
+00000880: 2020 2020 206f 732e 7061 7468 2e64 6972       os.path.dir
+00000890: 6e61 6d65 285f 5f66 696c 655f 5f29 2c0a  name(__file__),.
+000008a0: 2020 2020 2020 2020 2020 2020 2274 656d              "tem
+000008b0: 706c 6174 6522 2c0a 2020 2020 2020 2020  plate",.        
+000008c0: 2020 2020 2270 6167 652e 6874 6d6c 220a      "page.html".
+000008d0: 2020 2020 2020 2020 290a 2020 2020 290a          ).    ).
+000008e0: 2020 2020 7769 7468 206f 7065 6e28 7465      with open(te
+000008f0: 6d70 6c61 7465 5f68 746d 6c2c 2022 7222  mplate_html, "r"
+00000900: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+00000910: 7061 6765 203d 2066 2e72 6561 6428 290a  page = f.read().
+00000920: 2020 2020 2320 656e 6457 6974 680a 0a20      # endWith.. 
+00000930: 2020 2069 6620 696e 6465 785f 7361 6d65     if index_same
+00000940: 5f64 6972 3a0a 2020 2020 2020 2020 7061  _dir:.        pa
+00000950: 6765 203d 2070 6167 652e 7265 706c 6163  ge = page.replac
+00000960: 6528 0a20 2020 2020 2020 2020 2020 2027  e(.            '
+00000970: 3c61 2068 7265 663d 222e 2e2f 696e 6465  <a href="../inde
+00000980: 782e 6874 6d6c 223e 272c 0a20 2020 2020  x.html">',.     
+00000990: 2020 2020 2020 2027 3c61 2068 7265 663d         '<a href=
+000009a0: 222e 2f69 6e64 6578 2e68 746d 6c22 3e27  "./index.html">'
+000009b0: 0a20 2020 2020 2020 2029 0a20 2020 2065  .        ).    e
+000009c0: 6c69 6620 6e6f 745f 6162 6f76 655f 696e  lif not_above_in
+000009d0: 6465 783a 0a20 2020 2020 2020 2070 6167  dex:.        pag
+000009e0: 6520 3d20 7061 6765 2e72 6570 6c61 6365  e = page.replace
+000009f0: 280a 2020 2020 2020 2020 2020 2020 273c  (.            '<
+00000a00: 6120 6872 6566 3d22 2e2e 2f69 6e64 6578  a href="../index
+00000a10: 2e68 746d 6c22 3e27 2c0a 2020 2020 2020  .html">',.      
+00000a20: 2020 2020 2020 273c 6120 6872 6566 3d22        '<a href="
+00000a30: 2322 3e27 2c0a 2020 2020 2020 2020 290a  #">',.        ).
+00000a40: 2020 2020 230a 0a20 2020 2070 6167 6520      #..    page 
+00000a50: 3d20 7061 6765 2e72 6570 6c61 6365 2822  = page.replace("
+00000a60: 3a48 4541 4445 523a 222c 2066 223c 6469  :HEADER:", f"<di
+00000a70: 7620 6964 3d27 6865 6164 6572 273e 7b73  v id='header'>{s
+00000a80: 7472 2868 6561 6465 7229 7d3c 2f64 6976  tr(header)}</div
+00000a90: 3e22 2069 6620 6865 6164 6572 2065 6c73  >" if header els
+00000aa0: 6520 2222 290a 2020 2020 7061 6765 203d  e "").    page =
+00000ab0: 2070 6167 652e 7265 706c 6163 6528 0a20   page.replace(. 
+00000ac0: 2020 2020 2020 2022 3a54 494d 455f 554e         ":TIME_UN
+00000ad0: 4954 3a22 2c0a 2020 2020 2020 2020 7374  IT:",.        st
+00000ae0: 7228 6461 7461 5b27 7469 6d65 7220 756e  r(data['timer un
+00000af0: 6974 275d 290a 2020 2020 2020 2020 6966  it']).        if
+00000b00: 2027 7469 6d65 7220 756e 6974 2720 696e   'timer unit' in
+00000b10: 2064 6174 612e 6b65 7973 2829 2061 6e64   data.keys() and
+00000b20: 0a20 2020 2020 2020 2064 6174 615b 2774  .        data['t
+00000b30: 696d 6572 2075 6e69 7427 5d20 6973 206e  imer unit'] is n
+00000b40: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+00000b50: 656c 7365 2027 270a 2020 2020 290a 2020  else ''.    ).  
+00000b60: 2020 7061 6765 203d 2070 6167 652e 7265    page = page.re
+00000b70: 706c 6163 6528 0a20 2020 2020 2020 2022  place(.        "
+00000b80: 3a54 4f54 414c 5f54 494d 453a 222c 0a20  :TOTAL_TIME:",. 
+00000b90: 2020 2020 2020 2073 7472 2864 6174 615b         str(data[
+00000ba0: 2774 6f74 616c 2074 696d 6527 5d29 0a20  'total time']). 
+00000bb0: 2020 2020 2020 2069 6620 2774 6f74 616c         if 'total
+00000bc0: 2074 696d 6527 2069 6e20 6461 7461 2e6b   time' in data.k
+00000bd0: 6579 7328 2920 616e 640a 2020 2020 2020  eys() and.      
+00000be0: 2020 6461 7461 5b27 746f 7461 6c20 7469    data['total ti
+00000bf0: 6d65 275d 2069 7320 6e6f 7420 4e6f 6e65  me'] is not None
+00000c00: 0a20 2020 2020 2020 2065 6c73 6520 2727  .        else ''
+00000c10: 0a20 2020 2029 0a20 2020 2070 6167 6520  .    ).    page 
+00000c20: 3d20 7061 6765 2e72 6570 6c61 6365 280a  = page.replace(.
+00000c30: 2020 2020 2020 2020 223a 4649 4c45 3a22          ":FILE:"
+00000c40: 2c0a 2020 2020 2020 2020 7374 7228 6461  ,.        str(da
+00000c50: 7461 5b27 6669 6c65 275d 290a 2020 2020  ta['file']).    
+00000c60: 2020 2020 6966 2027 6669 6c65 2720 696e      if 'file' in
+00000c70: 2064 6174 612e 6b65 7973 2829 2061 6e64   data.keys() and
+00000c80: 0a20 2020 2020 2020 2064 6174 615b 2766  .        data['f
+00000c90: 696c 6527 5d20 6973 206e 6f74 204e 6f6e  ile'] is not Non
+00000ca0: 650a 2020 2020 2020 2020 656c 7365 2027  e.        else '
+00000cb0: 270a 2020 2020 290a 2020 2020 7061 6765  '.    ).    page
+00000cc0: 203d 2070 6167 652e 7265 706c 6163 6528   = page.replace(
+00000cd0: 0a20 2020 2020 2020 2022 3a46 554e 4354  .        ":FUNCT
+00000ce0: 494f 4e3a 222c 0a20 2020 2020 2020 2073  ION:",.        s
+00000cf0: 7472 2864 6174 615b 2766 756e 6374 696f  tr(data['functio
+00000d00: 6e27 5d29 0a20 2020 2020 2020 2069 6620  n']).        if 
+00000d10: 2766 756e 6374 696f 6e27 2069 6e20 6461  'function' in da
+00000d20: 7461 2e6b 6579 7328 2920 616e 640a 2020  ta.keys() and.  
+00000d30: 2020 2020 2020 6461 7461 5b27 6675 6e63        data['func
+00000d40: 7469 6f6e 275d 2069 7320 6e6f 7420 4e6f  tion'] is not No
+00000d50: 6e65 0a20 2020 2020 2020 2065 6c73 6520  ne.        else 
+00000d60: 2727 0a20 2020 2029 0a20 2020 2070 6167  ''.    ).    pag
+00000d70: 6520 3d20 7061 6765 2e72 6570 6c61 6365  e = page.replace
+00000d80: 280a 2020 2020 2020 2020 223a 434f 4e54  (.        ":CONT
+00000d90: 454e 543a 222c 0a20 2020 2020 2020 2073  ENT:",.        s
+00000da0: 7472 2868 746d 6c29 0a20 2020 2020 2020  tr(html).       
+00000db0: 2069 6620 6874 6d6c 2069 7320 6e6f 7420   if html is not 
+00000dc0: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
+00000dd0: 6520 2727 0a20 2020 2029 0a0a 2020 2020  e ''.    )..    
+00000de0: 6966 2070 6174 685f 6373 733a 0a20 2020  if path_css:.   
+00000df0: 2020 2020 2070 6167 6520 3d20 7061 6765       page = page
+00000e00: 2e72 6570 6c61 6365 2822 2e2f 7374 796c  .replace("./styl
+00000e10: 652e 6373 7322 2c20 6f73 2e70 6174 682e  e.css", os.path.
+00000e20: 6162 7370 6174 6828 6f73 2e70 6174 682e  abspath(os.path.
+00000e30: 6a6f 696e 2870 6174 685f 6373 732c 2022  join(path_css, "
+00000e40: 7374 796c 652e 6373 7322 2929 290a 2020  style.css"))).  
+00000e50: 2020 2320 656e 6449 660a 0a20 2020 2072    # endIf..    r
+00000e60: 6574 7572 6e20 7061 6765 0a0a 0a         eturn page...
```

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_generate_page_index.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_page_index.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 fct_name=None,
                 build_tree=build_tree
             )
 
             index_class_html = html2file(
                 html,
                 basename=basename,
-                path=path_html_dir,
+                path=path_html_dir
             )
 
             index_page.append(
                 {
                     "line": 0,
                     "line content":f"<a href={os.path.abspath(index_class_html)}>{file_name}.py: {class_name}</a>"
                     }
@@ -124,15 +124,16 @@
              "report":index_page
              }
 
 
     html = generate_html_page(
         datas,
         path_css=out_dir,
-        header=f"<h1>INDEX</h1>"
+        header=f"<h1>INDEX</h1>",
+        not_above_index=True
     )
 
 
     basename = f'index.html'
 
     html_page = html2file(
         html,
```

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tool_find.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tool_find.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/_tools_profile.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tools_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,19 @@
         fct_name:str="function_name",
         build_tree:bool=True
         ):
 
     datas = extract_profiled_data(file_name=file_in)
 
     datas["function"] = f"{file_name}.py: {class_name}: {fct_name}: {datas['function']}"
-    html = generate_html_page(datas, path_css=out_dir)
+    html = generate_html_page(
+        datas,
+        path_css=out_dir,
+        index_same_dir=True
+    )
 
     #basename_html = os.path.basename(file_in).replace(ext_in, ".html")
     basename_html = f"{fct_name}.html".lower()
 
     path_html_dir = names_file_class_fct2path(
         base_path=out_dir,
         file_name=file_name,
```

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/generate_html_report_fct.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/generate_html_report_fct.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/page.html` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/page.html`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/generate_html_report/template/style.css` & `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/style.css`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler/teardown_profiler.py` & `html_report_line_profiler-0.1.0/html_report_line_profiler/unittest_ext_profiler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,40 @@
 import os
 import io
+from line_profiler import LineProfiler
+
+def setUp_profiler(function, delete_profiling_env:bool = False):
+    """
+    :param function: nom de la fonction
+    :param bool delete_profiling_env: supprimer la variable d'environnement a la fin, si cree ici
+    """
+    if not os.environ.get("PROFILING", False):
+        os.environ["PROFILING"] = "1"
+        delete_profiling_env = True
+    #endIf
+
+    profiler = LineProfiler()
+    profiler.add_function(function)
+    profiler.enable_by_count()
+
+    return profiler, delete_profiling_env
+
+#endDef
+
+
+def names2basename(
+        file_name:str,
+        class_name:str,
+        method_name:str
+):
+    class_name_t = class_name.lower().replace('test',"")
+    class_name_t = class_name_t if not class_name_t[0] == "_" else class_name_t[1:]
+    return f"{os.path.basename(file_name).replace('.py','')}_{class_name_t}_{method_name}"
+
 
-#
-# class_name_t = class_name.lower().replace('test',"")
-# class_name_t = class_name_t if not class_name_t[0] == "_" else class_name_t[1:]
-# proffile_basename = os.path.join(dirout, f"{class_name_t}_{test_method_name}")
-#
 def tearDown_profiler(profiler, proffile_basename="file", output_folder="./profile", delete_profiling_env:bool=False):
     if profiler is None:
         return
     #
     # Code executé après chaque test
     #del self.my_class_instance
     output_folder = os.path.abspath(output_folder)
```

### Comparing `html_report_line_profiler-0.0.2/html_report_line_profiler.egg-info/SOURCES.txt` & `html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 README.md
 setup.cfg
 setup.py
 ./scripts/profiler_html_report.py
 html_report_line_profiler/__init__.py
 html_report_line_profiler/__version__.py
-html_report_line_profiler/setup_profiler.py
-html_report_line_profiler/teardown_profiler.py
+html_report_line_profiler/unittest_ext_profiler.py
 html_report_line_profiler.egg-info/PKG-INFO
 html_report_line_profiler.egg-info/SOURCES.txt
 html_report_line_profiler.egg-info/dependency_links.txt
 html_report_line_profiler.egg-info/requires.txt
 html_report_line_profiler.egg-info/top_level.txt
 html_report_line_profiler/generate_html_report/__init__.py
 html_report_line_profiler/generate_html_report/_extract_profiled_data.py
@@ -21,9 +20,8 @@
 html_report_line_profiler/generate_html_report/_generate_page_index.py
 html_report_line_profiler/generate_html_report/_generate_tools.py
 html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
 html_report_line_profiler/generate_html_report/_tool_find.py
 html_report_line_profiler/generate_html_report/_tools_profile.py
 html_report_line_profiler/generate_html_report/generate_html_report_fct.py
 html_report_line_profiler/generate_html_report/template/page.html
-html_report_line_profiler/generate_html_report/template/style.css
-tests/test.py
+html_report_line_profiler/generate_html_report/template/style.css
```

### Comparing `html_report_line_profiler-0.0.2/scripts/profiler_html_report.py` & `html_report_line_profiler-0.1.0/scripts/profiler_html_report.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.0.2/setup.py` & `html_report_line_profiler-0.1.0/setup.py`

 * *Files identical despite different names*

