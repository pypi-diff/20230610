# Comparing `tmp/html_report_line_profiler-0.1.1.tar.gz` & `tmp/html_report_line_profiler-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_report_line_profiler-0.1.1.tar", last modified: Sat Jun 10 21:45:12 2023, max compression
+gzip compressed data, was "html_report_line_profiler-0.1.1a0.tar", last modified: Sat Jun 10 21:22:47 2023, max compression
```

## Comparing `html_report_line_profiler-0.1.1.tar` & `html_report_line_profiler-0.1.1a0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:45:12.464427 html_report_line_profiler-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     3867 2023-06-10 21:45:12.464427 html_report_line_profiler-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2998 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:45:12.464427 html_report_line_profiler-0.1.1/html_report_line_profiler/
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:45:12.464427 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3437 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_extract_profiled_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_extract_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_extract_with_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_find_profiled_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_find_test_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3676 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_generate_html_page.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_generate_page_index.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_generate_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1772 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_tool_find.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_tools_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/generate_html_report_fct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:45:12.464427 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/template/
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/template/page.html
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/template/style.css
--rw-rw-rw-   0 root         (0) root         (0)     1912 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/html_report_line_profiler/unittest_ext_profiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:45:12.464427 html_report_line_profiler-0.1.1/html_report_line_profiler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3867 2023-06-10 21:45:12.000000 html_report_line_profiler-0.1.1/html_report_line_profiler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1456 2023-06-10 21:45:12.000000 html_report_line_profiler-0.1.1/html_report_line_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 21:45:12.000000 html_report_line_profiler-0.1.1/html_report_line_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-10 21:45:12.000000 html_report_line_profiler-0.1.1/html_report_line_profiler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-10 21:45:12.000000 html_report_line_profiler-0.1.1/html_report_line_profiler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:45:12.464427 html_report_line_profiler-0.1.1/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/scripts/profiler_html_report.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-10 21:45:12.468427 html_report_line_profiler-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     7052 2023-06-10 21:43:31.000000 html_report_line_profiler-0.1.1/setup.py
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

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/__init__.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_extract_profiled_data.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_profiled_data.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_extract_tools.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_tools.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_extract_with_mask.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_extract_with_mask.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_find_profiled_files.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_find_profiled_files.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_find_test_functions.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_find_test_functions.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_generate_html_page.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_generate_html_page.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_generate_page_index.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_generate_page_index.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_profilefile2htmlfile.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_tool_find.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_tool_find.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/_tools_profile.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/_tools_profile.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/generate_html_report_fct.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/generate_html_report_fct.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/template/page.html` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/template/page.html`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/generate_html_report/template/style.css` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/generate_html_report/template/style.css`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler/unittest_ext_profiler.py` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler/unittest_ext_profiler.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/html_report_line_profiler.egg-info/SOURCES.txt` & `html_report_line_profiler-0.1.1a0/html_report_line_profiler.egg-info/SOURCES.txt`

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

### Comparing `html_report_line_profiler-0.1.1/scripts/profiler_html_report.py` & `html_report_line_profiler-0.1.1a0/scripts/profiler_html_report.py`

 * *Files identical despite different names*

### Comparing `html_report_line_profiler-0.1.1/setup.py` & `html_report_line_profiler-0.1.1a0/setup.py`

 * *Files identical despite different names*

