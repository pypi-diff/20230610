# Comparing `tmp/pyaikit-1.0.2.tar.gz` & `tmp/pyaikit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyaikit-1.0.2.tar", last modified: Sat Jun 10 12:34:27 2023, max compression
+gzip compressed data, was "dist\pyaikit-1.0.3.tar", last modified: Sat Jun 10 13:42:07 2023, max compression
```

## Comparing `pyaikit-1.0.2.tar` & `pyaikit-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:34:27.000000 pyaikit-1.0.2/
--rw-rw-rw-   0        0        0     3240 2023-06-10 12:34:27.000000 pyaikit-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 12:34:27.000000 pyaikit-1.0.2/pyaikit/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:20:37.000000 pyaikit-1.0.2/pyaikit/__init__.py
--rw-rw-rw-   0        0        0      750 2023-06-04 08:19:53.000000 pyaikit-1.0.2/pyaikit/authentication.py
--rw-rw-rw-   0        0        0     1155 2023-06-10 11:55:09.000000 pyaikit-1.0.2/pyaikit/example.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:34:27.000000 pyaikit-1.0.2/pyaikit/sentiment_analysis/
--rw-rw-rw-   0        0        0     6743 2023-06-05 17:19:55.000000 pyaikit-1.0.2/pyaikit/sentiment_analysis/sentiment_analyzer.py
--rw-rw-rw-   0        0        0     3624 2023-06-10 12:33:34.000000 pyaikit-1.0.2/pyaikit/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:34:27.000000 pyaikit-1.0.2/pyaikit/text_generation/
--rw-rw-rw-   0        0        0     1574 2023-06-10 10:03:48.000000 pyaikit-1.0.2/pyaikit/text_generation/text_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:34:27.000000 pyaikit-1.0.2/pyaikit/text_summerization/
--rw-rw-rw-   0        0        0     4761 2023-06-07 04:21:23.000000 pyaikit-1.0.2/pyaikit/text_summerization/text_summerizer.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:34:27.000000 pyaikit-1.0.2/pyaikit/translation/
--rw-rw-rw-   0        0        0     1546 2023-06-10 09:50:21.000000 pyaikit-1.0.2/pyaikit/translation/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:34:27.000000 pyaikit-1.0.2/pyaikit.egg-info/
--rw-rw-rw-   0        0        0     3240 2023-06-10 12:34:26.000000 pyaikit-1.0.2/pyaikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-06-10 12:34:27.000000 pyaikit-1.0.2/pyaikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:34:26.000000 pyaikit-1.0.2/pyaikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:34:26.000000 pyaikit-1.0.2/pyaikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0      106 2023-06-10 12:34:26.000000 pyaikit-1.0.2/pyaikit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:34:27.000000 pyaikit-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3624 2023-06-10 12:33:57.000000 pyaikit-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/
+-rw-rw-rw-   0        0        0     5720 2023-06-10 13:42:07.000000 pyaikit-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4977 2023-06-10 12:49:12.000000 pyaikit-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:20:37.000000 pyaikit-1.0.3/pyaikit/__init__.py
+-rw-rw-rw-   0        0        0      750 2023-06-04 08:19:53.000000 pyaikit-1.0.3/pyaikit/authentication.py
+-rw-rw-rw-   0        0        0     1155 2023-06-10 11:55:09.000000 pyaikit-1.0.3/pyaikit/example.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/sentiment_analysis/
+-rw-rw-rw-   0        0        0     6743 2023-06-05 17:19:55.000000 pyaikit-1.0.3/pyaikit/sentiment_analysis/sentiment_analyzer.py
+-rw-rw-rw-   0        0        0     1177 2023-06-10 13:42:00.000000 pyaikit-1.0.3/pyaikit/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/text_generation/
+-rw-rw-rw-   0        0        0     1574 2023-06-10 10:03:48.000000 pyaikit-1.0.3/pyaikit/text_generation/text_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/text_summerization/
+-rw-rw-rw-   0        0        0     4761 2023-06-07 04:21:23.000000 pyaikit-1.0.3/pyaikit/text_summerization/text_summerizer.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/translation/
+-rw-rw-rw-   0        0        0     1546 2023-06-10 09:50:21.000000 pyaikit-1.0.3/pyaikit/translation/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/
+-rw-rw-rw-   0        0        0     5720 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      106 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:42:07.000000 pyaikit-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-06-10 13:41:57.000000 pyaikit-1.0.3/setup.py
```

### Comparing `pyaikit-1.0.2/pyaikit/authentication.py` & `pyaikit-1.0.3/pyaikit/authentication.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.2/pyaikit/example.py` & `pyaikit-1.0.3/pyaikit/example.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.2/pyaikit/sentiment_analysis/sentiment_analyzer.py` & `pyaikit-1.0.3/pyaikit/sentiment_analysis/sentiment_analyzer.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.2/pyaikit/text_generation/text_generator.py` & `pyaikit-1.0.3/pyaikit/text_generation/text_generator.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.2/pyaikit/text_summerization/text_summerizer.py` & `pyaikit-1.0.3/pyaikit/text_summerization/text_summerizer.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.2/pyaikit/translation/translator.py` & `pyaikit-1.0.3/pyaikit/translation/translator.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.2/pyaikit.egg-info/SOURCES.txt` & `pyaikit-1.0.3/pyaikit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 pyaikit/__init__.py
 pyaikit/authentication.py
 pyaikit/example.py
 pyaikit/setup.py
 pyaikit.egg-info/PKG-INFO
 pyaikit.egg-info/SOURCES.txt
```

