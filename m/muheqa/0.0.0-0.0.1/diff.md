# Comparing `tmp/muheqa-0.0.0.tar.gz` & `tmp/muheqa-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muheqa-0.0.0.tar", last modified: Sat Jun 10 17:57:32 2023, max compression
+gzip compressed data, was "muheqa-0.0.1.tar", last modified: Sat Jun 10 17:45:00 2023, max compression
```

## Comparing `muheqa-0.0.0.tar` & `muheqa-0.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.156185 muheqa-0.0.0/
--rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.0/LICENSE
--rw-r--r--   0 cbadenes   (501) staff       (20)     1077 2023-06-10 17:57:32.156052 muheqa-0.0.0/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      544 2023-06-10 17:56:37.000000 muheqa-0.0.0/README.md
--rw-r--r--   0 cbadenes   (501) staff       (20)      796 2023-06-10 17:56:01.000000 muheqa-0.0.0/pyproject.toml
--rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-10 17:57:32.156228 muheqa-0.0.0/setup.cfg
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.152543 muheqa-0.0.0/src/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.153144 muheqa-0.0.0/src/muheqa/
--rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.0/src/muheqa/__init__.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.153961 muheqa-0.0.0/src/muheqa/answer/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.154112 muheqa-0.0.0/src/muheqa/answer/analysis/
--rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.0/src/muheqa/answer/analysis/classifier.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.0/src/muheqa/answer/composer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.154226 muheqa-0.0.0/src/muheqa/answer/generation/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.0/src/muheqa/answer/generation/model.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.0/src/muheqa/connection.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      145 2023-06-10 17:08:51.000000 muheqa-0.0.0/src/muheqa/connector.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.154382 muheqa-0.0.0/src/muheqa/evidence/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.154517 muheqa-0.0.0/src/muheqa/evidence/candidates/
--rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.0/src/muheqa/evidence/candidates/ranking.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.0/src/muheqa/evidence/discoverer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.154650 muheqa-0.0.0/src/muheqa/evidence/documents/
--rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.0/src/muheqa/evidence/documents/splitter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.154802 muheqa-0.0.0/src/muheqa/evidence/responses/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1364 2023-06-09 14:48:51.000000 muheqa-0.0.0/src/muheqa/evidence/responses/retriever.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.0/src/muheqa/logformatter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.154923 muheqa-0.0.0/src/muheqa/summary/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.155255 muheqa-0.0.0/src/muheqa/summary/keywords/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.0/src/muheqa/summary/keywords/concept.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.0/src/muheqa/summary/keywords/discovery.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.0/src/muheqa/summary/keywords/entity.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.155727 muheqa-0.0.0/src/muheqa/summary/resources/
--rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.0/src/muheqa/summary/resources/d4c.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     6296 2023-06-09 14:46:22.000000 muheqa-0.0.0/src/muheqa/summary/resources/dbpedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-09 14:59:33.000000 muheqa-0.0.0/src/muheqa/summary/resources/graph.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-09 14:47:38.000000 muheqa-0.0.0/src/muheqa/summary/resources/wikipedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.0/src/muheqa/summary/summarizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.155850 muheqa-0.0.0/src/muheqa/summary/texts/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.0/src/muheqa/summary/texts/verbalizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:57:32.153794 muheqa-0.0.0/src/muheqa.egg-info/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1077 2023-06-10 17:57:32.000000 muheqa-0.0.0/src/muheqa.egg-info/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      930 2023-06-10 17:57:32.000000 muheqa-0.0.0/src/muheqa.egg-info/SOURCES.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-10 17:57:32.000000 muheqa-0.0.0/src/muheqa.egg-info/dependency_links.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-10 17:57:32.000000 muheqa-0.0.0/src/muheqa.egg-info/requires.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       14 2023-06-10 17:57:32.000000 muheqa-0.0.0/src/muheqa.egg-info/top_level.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)      207 2023-06-10 17:08:16.000000 muheqa-0.0.0/src/sample.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.234853 muheqa-0.0.1/
+-rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.1/LICENSE
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1111 2023-06-10 17:45:00.234716 muheqa-0.0.1/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      578 2023-06-10 17:16:58.000000 muheqa-0.0.1/README.md
+-rw-r--r--   0 cbadenes   (501) staff       (20)      792 2023-06-10 17:43:30.000000 muheqa-0.0.1/pyproject.toml
+-rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-10 17:45:00.234895 muheqa-0.0.1/setup.cfg
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.231497 muheqa-0.0.1/src/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.231955 muheqa-0.0.1/src/muheqa/
+-rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.1/src/muheqa/__init__.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.232693 muheqa-0.0.1/src/muheqa/answer/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.232819 muheqa-0.0.1/src/muheqa/answer/analysis/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.1/src/muheqa/answer/analysis/classifier.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.1/src/muheqa/answer/composer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.232960 muheqa-0.0.1/src/muheqa/answer/generation/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.1/src/muheqa/answer/generation/model.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.1/src/muheqa/connection.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      145 2023-06-10 17:08:51.000000 muheqa-0.0.1/src/muheqa/connector.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.233062 muheqa-0.0.1/src/muheqa/evidence/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.233176 muheqa-0.0.1/src/muheqa/evidence/candidates/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.1/src/muheqa/evidence/candidates/ranking.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.1/src/muheqa/evidence/discoverer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.233296 muheqa-0.0.1/src/muheqa/evidence/documents/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.1/src/muheqa/evidence/documents/splitter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.233399 muheqa-0.0.1/src/muheqa/evidence/responses/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1364 2023-06-09 14:48:51.000000 muheqa-0.0.1/src/muheqa/evidence/responses/retriever.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.1/src/muheqa/logformatter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.233512 muheqa-0.0.1/src/muheqa/summary/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.233919 muheqa-0.0.1/src/muheqa/summary/keywords/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.1/src/muheqa/summary/keywords/concept.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.1/src/muheqa/summary/keywords/discovery.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.1/src/muheqa/summary/keywords/entity.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.234407 muheqa-0.0.1/src/muheqa/summary/resources/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.1/src/muheqa/summary/resources/d4c.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     6296 2023-06-09 14:46:22.000000 muheqa-0.0.1/src/muheqa/summary/resources/dbpedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-09 14:59:33.000000 muheqa-0.0.1/src/muheqa/summary/resources/graph.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-09 14:47:38.000000 muheqa-0.0.1/src/muheqa/summary/resources/wikipedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.1/src/muheqa/summary/summarizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.234516 muheqa-0.0.1/src/muheqa/summary/texts/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.1/src/muheqa/summary/texts/verbalizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 17:45:00.232552 muheqa-0.0.1/src/muheqa.egg-info/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1111 2023-06-10 17:45:00.000000 muheqa-0.0.1/src/muheqa.egg-info/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      930 2023-06-10 17:45:00.000000 muheqa-0.0.1/src/muheqa.egg-info/SOURCES.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-10 17:45:00.000000 muheqa-0.0.1/src/muheqa.egg-info/dependency_links.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-10 17:45:00.000000 muheqa-0.0.1/src/muheqa.egg-info/requires.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       14 2023-06-10 17:45:00.000000 muheqa-0.0.1/src/muheqa.egg-info/top_level.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)      207 2023-06-10 17:08:16.000000 muheqa-0.0.1/src/sample.py
```

### Comparing `muheqa-0.0.0/LICENSE` & `muheqa-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/PKG-INFO` & `muheqa-0.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.0
+Version: 0.0.1
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Multiple and Heterogeneous Question-Answering (MuHeQA) system
+# muheqa-core
+multiple and heterogeneous question-answering system
+
 
 ## Quick Start!
 
-Install the `muheqa` package:
+Open a new [Google Colab](https://colab.research.google.com/) notebook and install the `muheqa` package:
 ````python
-pip install muheqa
+!pip install -i https://test.pypi.org/simple/ muheqa
 ````
 
 Create a new connection to Wikidata, or DBpedia, or D4C (Drugs4Covid):
-*(the first time it may take a few minutes to download the required models)*
 ````python
 import muheqa.connector as mhqa
 
 wikidata = mhqa.connect(wikidata=True)
 ````
 
-And finally, make a question in natural language!:
+Finally, make a question in natural language!:
 ````python
 response = wikidata.query("Who is the father of Barack Obama")
 print("Response:",response)
 ````
```

### Comparing `muheqa-0.0.0/README.md` & `muheqa-0.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Multiple and Heterogeneous Question-Answering (MuHeQA) system
+# muheqa-core
+multiple and heterogeneous question-answering system
+
 
 ## Quick Start!
 
-Install the `muheqa` package:
+Open a new [Google Colab](https://colab.research.google.com/) notebook and install the `muheqa` package:
 ````python
-pip install muheqa
+!pip install -i https://test.pypi.org/simple/ muheqa
 ````
 
 Create a new connection to Wikidata, or DBpedia, or D4C (Drugs4Covid):
-*(the first time it may take a few minutes to download the required models)*
 ````python
 import muheqa.connector as mhqa
 
 wikidata = mhqa.connect(wikidata=True)
 ````
 
-And finally, make a question in natural language!:
+Finally, make a question in natural language!:
 ````python
 response = wikidata.query("Who is the father of Barack Obama")
 print("Response:",response)
 ````
```

### Comparing `muheqa-0.0.0/pyproject.toml` & `muheqa-0.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     "sentence-transformers",
     "sparqlwrapper"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "muheqa"
+version = "0.0.1"
 authors = [
   { name="Carlos Badenes-Olmedo", email="carlos.badenes@upm.es" },
 ]
 description = "Multiple and Heterogeneous Question-Answering"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,12 +24,11 @@
 ]
 dependencies = [
     "sparqlwrapper",
     "flair",
     "unidecode",
     "sentence-transformers"
 ]
-dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/librairy/muheqa-core"
 "Bug Tracker" = "https://github.com/librairy/muheqa-core/issues"
```

### Comparing `muheqa-0.0.0/src/muheqa/answer/analysis/classifier.py` & `muheqa-0.0.1/src/muheqa/answer/analysis/classifier.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/answer/composer.py` & `muheqa-0.0.1/src/muheqa/answer/composer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/answer/generation/model.py` & `muheqa-0.0.1/src/muheqa/answer/generation/model.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/connection.py` & `muheqa-0.0.1/src/muheqa/connection.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/evidence/candidates/ranking.py` & `muheqa-0.0.1/src/muheqa/evidence/candidates/ranking.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/evidence/discoverer.py` & `muheqa-0.0.1/src/muheqa/evidence/discoverer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/evidence/documents/splitter.py` & `muheqa-0.0.1/src/muheqa/evidence/documents/splitter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/evidence/responses/retriever.py` & `muheqa-0.0.1/src/muheqa/evidence/responses/retriever.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/logformatter.py` & `muheqa-0.0.1/src/muheqa/logformatter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/keywords/concept.py` & `muheqa-0.0.1/src/muheqa/summary/keywords/concept.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/keywords/discovery.py` & `muheqa-0.0.1/src/muheqa/summary/keywords/discovery.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/keywords/entity.py` & `muheqa-0.0.1/src/muheqa/summary/keywords/entity.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/resources/d4c.py` & `muheqa-0.0.1/src/muheqa/summary/resources/d4c.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/resources/dbpedia.py` & `muheqa-0.0.1/src/muheqa/summary/resources/dbpedia.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/resources/graph.py` & `muheqa-0.0.1/src/muheqa/summary/resources/graph.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/resources/wikipedia.py` & `muheqa-0.0.1/src/muheqa/summary/resources/wikipedia.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/summarizer.py` & `muheqa-0.0.1/src/muheqa/summary/summarizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa/summary/texts/verbalizer.py` & `muheqa-0.0.1/src/muheqa/summary/texts/verbalizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.0/src/muheqa.egg-info/PKG-INFO` & `muheqa-0.0.1/src/muheqa.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.0
+Version: 0.0.1
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Multiple and Heterogeneous Question-Answering (MuHeQA) system
+# muheqa-core
+multiple and heterogeneous question-answering system
+
 
 ## Quick Start!
 
-Install the `muheqa` package:
+Open a new [Google Colab](https://colab.research.google.com/) notebook and install the `muheqa` package:
 ````python
-pip install muheqa
+!pip install -i https://test.pypi.org/simple/ muheqa
 ````
 
 Create a new connection to Wikidata, or DBpedia, or D4C (Drugs4Covid):
-*(the first time it may take a few minutes to download the required models)*
 ````python
 import muheqa.connector as mhqa
 
 wikidata = mhqa.connect(wikidata=True)
 ````
 
-And finally, make a question in natural language!:
+Finally, make a question in natural language!:
 ````python
 response = wikidata.query("Who is the father of Barack Obama")
 print("Response:",response)
 ````
```

### Comparing `muheqa-0.0.0/src/muheqa.egg-info/SOURCES.txt` & `muheqa-0.0.1/src/muheqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

