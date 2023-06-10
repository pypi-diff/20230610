# Comparing `tmp/html_report_line_profiler-0.1.0.tar.gz` & `tmp/html_report_line_profiler-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_report_line_profiler-0.1.0.tar", last modified: Sat Jun 10 17:52:32 2023, max compression
+gzip compressed data, was "html_report_line_profiler-0.1.1a0.tar", last modified: Sat Jun 10 21:22:47 2023, max compression
```

## Comparing `html_report_line_profiler-0.1.0.tar` & `html_report_line_profiler-0.1.1a0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     2205 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.259280 html_report_line_profiler-0.1.0/html_report_line_profiler/
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3437 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_profiled_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_with_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_profiled_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_test_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3693 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_html_page.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_page_index.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4323 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1772 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tool_find.py
--rw-rw-rw-   0 root         (0) root         (0)     2870 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tools_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/generate_html_report_fct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/page.html
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/style.css
--rw-rw-rw-   0 root         (0) root         (0)     1912 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/html_report_line_profiler/unittest_ext_profiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2205 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1456 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      212 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-10 17:52:32.000000 html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:52:32.259280 html_report_line_profiler-0.1.0/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/scripts/profiler_html_report.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-10 17:52:32.263280 html_report_line_profiler-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     7052 2023-06-10 17:40:40.000000 html_report_line_profiler-0.1.0/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 21:22:47.109130 html_report_line_profiler-0.1.1a0/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2980 2023-06-10 21:22:47.109130 html_report_line_profiler-0.1.1a0/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1551 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/README.md
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 21:22:47.089131 html_report_line_profiler-0.1.1a0/html_report_line_profiler/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      671 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      505 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/__version__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 21:22:47.105130 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      110 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3437 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_profiled_data.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1295 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_tools.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      845 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_with_mask.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      588 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_find_profiled_files.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1931 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_find_test_functions.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3676 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_generate_html_page.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_generate_page_index.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      467 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_generate_tools.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4308 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1772 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_tool_find.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2886 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_tools_profile.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1406 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/generate_html_report_fct.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 21:22:47.109130 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/template/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      886 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/template/page.html
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2107 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/template/style.css
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1912 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler/unittest_ext_profiler.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 21:22:47.093131 html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2980 2023-06-10 21:22:47.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1470 2023-06-10 21:22:47.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-10 21:22:47.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      212 2023-06-10 21:22:47.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       26 2023-06-10 21:22:47.000000 html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 21:22:47.089131 html_report_line_profiler-0.1.1a0/scripts/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      886 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/scripts/profiler_html_report.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      167 2023-06-10 21:22:47.113130 html_report_line_profiler-0.1.1a0/setup.cfg
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7052 2023-06-10 21:22:36.000000 html_report_line_profiler-0.1.1a0/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-10 21:22:47.109130 html_report_line_profiler-0.1.1a0/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      376 2023-06-09 22:29:57.000000 html_report_line_profiler-0.1.1a0/tests/test.py
```

### Comparing `html_report_line_profiler-0.1.0/PKG-INFO` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 Metadata-Version: 2.1
-Name: html_report_line_profiler
-Version: 0.1.0
+Name: html-report-line-profiler
+Version: 0.1.1a0
 Summary: Generate an HTML report for line_parser
 Home-page: https://1sixunhuit.frama.io/html_report_line_profiler
 Author: Pierre
 Author-email: pierre@exemple.com
 License: AGPL 3
+Description: # Intro
+        
+        Basé sur https://github.com/pyutils/line_profiler, fork de https://github.com/rkern/line_profiler
+        
+        
+        # TODO
+        - [ ] Several classes in one file : bug...
+        - [ ] Badges de la page d'accueil de la doc a changer
+        
+        # Utilisation dans les tests unitaires :
+        
+        A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
+        
+        Dans :
+        ```
+        [...]
+        
+        import html_report_line_profiler as hr
+        
+        
+        class Test_CeciEstUnTest(unittest.TestCase):
+            def setUp(self):
+                # Code execute avant chaque test
+                [...] # ce que l'on veut
+        
+                # Profiler :
+                self.profiler, self.delete_profiling_env = hr.setUp_profiler(castList)
+        
+            #endDef
+        
+            # ...
+        
+            def tearDown(self):
+                # Code executé après chaque test
+                # Terminer le profiler en premier
+        
+                # Create basename
+                hr.proffile_basename = classname2basename(
+                    file_name = __file__,
+                    class_name = self.__class__.__name__,
+                    method_name = self._testMethodName
+                )
+        
+                # Launch the profiler out
+                hr.tearDown_profiler(
+                    profiler=self.profiler,
+                    proffile_basename=proffile_basename,
+                    output_folder=output_folder,
+                    delete_profiling_env=self.delete_profiling_env
+                )
+                #
+        	# [...] # Les autres commandes
+            #endDef
+        #endClass
+        ```
+        
+        
+        # Rapport HTML
+        Pour lancer ensuite le post-traitement (rapport html) :
+        ```
+        $ profiler_html_report.py
+        ```
+        
+        Remarques
+        
+        * `-d = --input-dir` (default : './profile')
+        * `-o = --output-dir` (default : './profile_html')
 Keywords: ['profiling','profiler','line_profiler','html','report']
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: French
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: upload
-
-# Utilisation dans les tests unitaires :
-
-A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
-
-Dans :
-```
-[...]
-
-import html_report_line_profiler as hr
-
-
-class Test_CeciEstUnTest(unittest.TestCase):
-    def setUp(self):
-        # Code execute avant chaque test
-        [...] # ce que l'on veut
-
-        # Profiler :
-        self.profiler, self.delete_profiling_env = hr.setUp_profiler(castList)
-
-    #endDef
-
-    # ...
-
-    def tearDown(self):
-        # Code executé après chaque test
-        # Terminer le profiler en premier
-
-        # Create basename
-        hr.proffile_basename = classname2basename(
-            file_name = __file__,
-            class_name = self.__class__.__name__,
-            method_name = self._testMethodName
-        )
-
-        # Launch the profiler out
-        hr.tearDown_profiler(
-            profiler=self.profiler,
-            proffile_basename=proffile_basename,
-            output_folder=output_folder,
-            delete_profiling_env=self.delete_profiling_env
-        )
-        #
-	# [...] # Les autres commandes
-    #endDef
-#endClass
-```
-
-
-# Rapport HTML
-Pour lancer ensuite le post-traitement (rapport html) :
-```
-$ profiler_html_report.py
-```
-
-Remarques
-
-* `-d = --input-dir` (default : './profile')
-* `-o = --output-dir` (default : './profile_html')
```

### Comparing `html_report_line_profiler-0.1.0/README.md` & `html_report_line_profiler-0.1.1a0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# Intro
+
+Basé sur https://github.com/pyutils/line_profiler, fork de https://github.com/rkern/line_profiler
+
+
+# TODO
+- [ ] Several classes in one file : bug...
+- [ ] Badges de la page d'accueil de la doc a changer
+
 # Utilisation dans les tests unitaires :
 
 A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
 
 Dans :
 ```
 [...]
```

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/__init__.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_profiled_data.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_profiled_data.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_tools.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_tools.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_extract_with_mask.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_with_mask.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_profiled_files.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_find_profiled_files.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_find_test_functions.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_find_test_functions.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_html_page.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_generate_html_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,13 +124,13 @@
         ":CONTENT:",
         str(html)
         if html is not None
         else ''
     )
 
     if path_css:
-        page = page.replace("./style.css", os.path.abspath(os.path.join(path_css, "style.css")))
+        page = page.replace("./style.css", os.path.join(path_css, "style.css"))
     # endIf
 
     return page
```

#### html2text {}

```diff
@@ -34,9 +34,9 @@
 unit'])_if_'timer_unit'_in_data.keys()_and_data['timer_unit']_is_not_None_else
 ''_)_page_=_page.replace(_":TOTAL_TIME:",_str(data['total_time'])_if_'total
 time'_in_data.keys()_and_data['total_time']_is_not_None_else_''_)_page_=
 page.replace(_":FILE:",_str(data['file'])_if_'file'_in_data.keys()_and_data
 ['file']_is_not_None_else_''_)_page_=_page.replace(_":FUNCTION:",_str(data
 ['function'])_if_'function'_in_data.keys()_and_data['function']_is_not_None
 else_''_)_page_=_page.replace(_":CONTENT:",_str(html)_if_html_is_not_None_else
-''_)_if_path_css:_page_=_page.replace("./style.css",_os.path.abspath
-(os.path.join(path_css,_"style.css")))_#_endIf_return_page
+''_)_if_path_css:_page_=_page.replace("./style.css",_os.path.join(path_css,
+"style.css"))_#_endIf_return_page
```

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_generate_page_index.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_generate_page_index.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 
     for file_name, d_file in ordered_files.items():
 
         total_time_mod = 0.0
 
         for class_name, d_class in d_file.items():
 
+            path_html_dir = names_file_class_fct2path(
+                base_path=out_dir,
+                file_name=file_name,
+                class_name=class_name,
+                fct_name=None,
+                build_tree=build_tree
+            )
+
             total_time_fct = 0.0
             list_fct = []
 
             for each_fct in d_class["functions"]:
 
                 basename = f"{file_name}_{class_name}_{each_fct['name']}.{ext}"
 
@@ -55,15 +63,15 @@
 
                 total_time_fct +=  float(str(total_time).strip().split(" ")[0])
 
                 list_fct.append(
                     {
                         "line": 0, "hits": 1, "per hit": None, "% time": None,
                         "time": total_time,
-                        "line content":f"<a href={os.path.abspath(path_html)}>{os.path.basename(path_html)}</a>"
+                        "line content":f"<a href={os.path.relpath(path_html, path_html_dir)}>{os.path.basename(path_html)}</a>"
                     }
                 )
             # endFor each_fct
 
             for elt in list_fct:
                 elt["% time"] = float(str(elt["time"]).strip().split(" ")[0]) / total_time_fct * 100.0
             # endFor
@@ -81,39 +89,30 @@
                      "report":list_fct
                      }
 
             total_time_mod +=  float(str(datas["total time"]).strip().split(" ")[0])
 
             html = generate_html_page(
                 datas,
-                path_css=out_dir,
+                path_css=os.path.relpath(out_dir, path_html_dir),
                 header=f"<h1>INDEX : {class_name}</h1>"
             )
 
             basename = f'index.html'
 
-            dirout1 = "/".join([e for e in out_dir.split("/") if e])
-            path_html_dir = names_file_class_fct2path(
-                base_path=out_dir,
-                file_name=file_name,
-                class_name=class_name,
-                fct_name=None,
-                build_tree=build_tree
-            )
-
             index_class_html = html2file(
                 html,
                 basename=basename,
                 path=path_html_dir
             )
 
             index_page.append(
                 {
                     "line": 0,
-                    "line content":f"<a href={os.path.abspath(index_class_html)}>{file_name}.py: {class_name}</a>"
+                    "line content":f"<a href={os.path.relpath(index_class_html, out_dir)}>{file_name}.py: {class_name}</a>"
                     }
                 )
 
             sys.stdout.write(f"write file> {os.path.abspath(index_class_html)}\n")
         # endFor classname
     # endFor filename
 
@@ -123,15 +122,15 @@
              "function":None, # nom de la classe
              "report":index_page
              }
 
 
     html = generate_html_page(
         datas,
-        path_css=out_dir,
+        path_css="./" ,
         header=f"<h1>INDEX</h1>",
         not_above_index=True
     )
 
 
     basename = f'index.html'
```

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tool_find.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_tool_find.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/_tools_profile.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_tools_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         path = base_path
 
     #endIf
 
     # Creer le dossier si n'existe pas et ecrire le fichier
     os.makedirs(path, exist_ok=True)
 
-    return os.path.abspath(path)
+    return path
 #
 
 def profilefile2htmlfile(
         file_in:str="file.dat",
         ext_in:str=".dat",
         out_dir:str="./",
         file_name:str="file_name",
@@ -45,31 +45,32 @@
         fct_name:str="function_name",
         build_tree:bool=True
         ):
 
     datas = extract_profiled_data(file_name=file_in)
 
     datas["function"] = f"{file_name}.py: {class_name}: {fct_name}: {datas['function']}"
-    html = generate_html_page(
-        datas,
-        path_css=out_dir,
-        index_same_dir=True
-    )
-
-    #basename_html = os.path.basename(file_in).replace(ext_in, ".html")
-    basename_html = f"{fct_name}.html".lower()
 
     path_html_dir = names_file_class_fct2path(
         base_path=out_dir,
         file_name=file_name,
         class_name=class_name,
         fct_name=fct_name,
         build_tree=build_tree
     )
 
+    html = generate_html_page(
+        datas,
+        path_css=os.path.relpath(out_dir, path_html_dir),
+        index_same_dir=True
+    )
+
+    #basename_html = os.path.basename(file_in).replace(ext_in, ".html")
+    basename_html = f"{fct_name}.html".lower()
+
     path_html = html2file(
         html,
         basename=basename_html,
         path=path_html_dir
     )
 
     sys.stdout.write(f"write file> {os.path.abspath(path_html)}\n")
```

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/generate_html_report_fct.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/generate_html_report_fct.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/page.html` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/template/page.html`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/generate_html_report/template/style.css` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/template/style.css`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler/unittest_ext_profiler.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/unittest_ext_profiler.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/PKG-INFO` & `html_report_line_profiler-0.1.1a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 Metadata-Version: 2.1
-Name: html-report-line-profiler
-Version: 0.1.0
+Name: html_report_line_profiler
+Version: 0.1.1a0
 Summary: Generate an HTML report for line_parser
 Home-page: https://1sixunhuit.frama.io/html_report_line_profiler
 Author: Pierre
 Author-email: pierre@exemple.com
 License: AGPL 3
+Description: # Intro
+        
+        Basé sur https://github.com/pyutils/line_profiler, fork de https://github.com/rkern/line_profiler
+        
+        
+        # TODO
+        - [ ] Several classes in one file : bug...
+        - [ ] Badges de la page d'accueil de la doc a changer
+        
+        # Utilisation dans les tests unitaires :
+        
+        A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
+        
+        Dans :
+        ```
+        [...]
+        
+        import html_report_line_profiler as hr
+        
+        
+        class Test_CeciEstUnTest(unittest.TestCase):
+            def setUp(self):
+                # Code execute avant chaque test
+                [...] # ce que l'on veut
+        
+                # Profiler :
+                self.profiler, self.delete_profiling_env = hr.setUp_profiler(castList)
+        
+            #endDef
+        
+            # ...
+        
+            def tearDown(self):
+                # Code executé après chaque test
+                # Terminer le profiler en premier
+        
+                # Create basename
+                hr.proffile_basename = classname2basename(
+                    file_name = __file__,
+                    class_name = self.__class__.__name__,
+                    method_name = self._testMethodName
+                )
+        
+                # Launch the profiler out
+                hr.tearDown_profiler(
+                    profiler=self.profiler,
+                    proffile_basename=proffile_basename,
+                    output_folder=output_folder,
+                    delete_profiling_env=self.delete_profiling_env
+                )
+                #
+        	# [...] # Les autres commandes
+            #endDef
+        #endClass
+        ```
+        
+        
+        # Rapport HTML
+        Pour lancer ensuite le post-traitement (rapport html) :
+        ```
+        $ profiler_html_report.py
+        ```
+        
+        Remarques
+        
+        * `-d = --input-dir` (default : './profile')
+        * `-o = --output-dir` (default : './profile_html')
 Keywords: ['profiling','profiler','line_profiler','html','report']
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: French
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: upload
-
-# Utilisation dans les tests unitaires :
-
-A ajouter a un test unittaire unittest, et à lancer avec $ coverage run -m unittest test_str.py 
-
-Dans :
-```
-[...]
-
-import html_report_line_profiler as hr
-
-
-class Test_CeciEstUnTest(unittest.TestCase):
-    def setUp(self):
-        # Code execute avant chaque test
-        [...] # ce que l'on veut
-
-        # Profiler :
-        self.profiler, self.delete_profiling_env = hr.setUp_profiler(castList)
-
-    #endDef
-
-    # ...
-
-    def tearDown(self):
-        # Code executé après chaque test
-        # Terminer le profiler en premier
-
-        # Create basename
-        hr.proffile_basename = classname2basename(
-            file_name = __file__,
-            class_name = self.__class__.__name__,
-            method_name = self._testMethodName
-        )
-
-        # Launch the profiler out
-        hr.tearDown_profiler(
-            profiler=self.profiler,
-            proffile_basename=proffile_basename,
-            output_folder=output_folder,
-            delete_profiling_env=self.delete_profiling_env
-        )
-        #
-	# [...] # Les autres commandes
-    #endDef
-#endClass
-```
-
-
-# Rapport HTML
-Pour lancer ensuite le post-traitement (rapport html) :
-```
-$ profiler_html_report.py
-```
-
-Remarques
-
-* `-d = --input-dir` (default : './profile')
-* `-o = --output-dir` (default : './profile_html')
```

### Comparing `html_report_line_profiler-0.1.0/html_report_line_profiler.egg-info/SOURCES.txt` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 html_report_line_profiler/generate_html_report/_generate_page_index.py
 html_report_line_profiler/generate_html_report/_generate_tools.py
 html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
 html_report_line_profiler/generate_html_report/_tool_find.py
 html_report_line_profiler/generate_html_report/_tools_profile.py
 html_report_line_profiler/generate_html_report/generate_html_report_fct.py
 html_report_line_profiler/generate_html_report/template/page.html
-html_report_line_profiler/generate_html_report/template/style.css
+html_report_line_profiler/generate_html_report/template/style.css
+tests/test.py
```

### Comparing `html_report_line_profiler-0.1.0/scripts/profiler_html_report.py` & `html_report_line_profiler-0.1.1a0/scripts/profiler_html_report.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 #!python3
 import sys
 import optparse
 
-from html_report_line_profiler import generate_html_report_fct
-
+try:
+    from html_report_line_profiler import generate_html_report_fct
+except:
+    sys.path.insert(0, "../")
+    from html_report_line_profiler import generate_html_report_fct
+#end
 
 def main(args=None):
     parser=optparse.OptionParser()
     parser.add_option("-d", "--input-dir", help="Input directory", type=str)
     parser.add_option("-o", "--output-dir", type=str)
 
     args, _ = parser.parse_args() # instantiate parser
```

### Comparing `html_report_line_profiler-0.1.0/setup.py` & `html_report_line_profiler-0.1.1a0/setup.py`

 * *Files identical despite different names*

