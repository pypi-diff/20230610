# Comparing `tmp/rechtspraak_citations_extractor-1.0.4.tar.gz` & `tmp/rechtspraak_citations_extractor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_citations_extractor-1.0.4.tar", last modified: Sat Jun  3 12:36:40 2023, max compression
+gzip compressed data, was "rechtspraak_citations_extractor-1.0.5.tar", last modified: Sat Jun 10 19:17:21 2023, max compression
```

## Comparing `rechtspraak_citations_extractor-1.0.4.tar` & `rechtspraak_citations_extractor-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:36:40.884020 rechtspraak_citations_extractor-1.0.4/
--rw-rw-rw-   0        0        0     4818 2023-06-03 12:36:40.883020 rechtspraak_citations_extractor-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 12:36:40.872660 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/
--rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/__init__.py
--rw-rw-rw-   0        0        0    13293 2023-06-03 12:36:33.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/citations_extractor.py
--rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:36:40.880821 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/
--rw-rw-rw-   0        0        0     4818 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 12:36:40.884020 rechtspraak_citations_extractor-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-06-03 12:36:33.000000 rechtspraak_citations_extractor-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:17:21.842878 rechtspraak_citations_extractor-1.0.5/
+-rw-rw-rw-   0        0        0     4818 2023-06-10 19:17:21.840878 rechtspraak_citations_extractor-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 19:17:21.830878 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor/
+-rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor/__init__.py
+-rw-rw-rw-   0        0        0    13391 2023-06-10 19:17:14.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor/citations_extractor.py
+-rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:17:21.838878 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor.egg-info/
+-rw-rw-rw-   0        0        0     4818 2023-06-10 19:17:21.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-10 19:17:21.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 19:17:21.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-10 19:17:21.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-10 19:17:21.000000 rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 19:17:21.842878 rechtspraak_citations_extractor-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-06-10 19:17:14.000000 rechtspraak_citations_extractor-1.0.5/setup.py
```

### Comparing `rechtspraak_citations_extractor-1.0.4/PKG-INFO` & `rechtspraak_citations_extractor-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak_citations_extractor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.4
+Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.5
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.4/README.md` & `rechtspraak_citations_extractor-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/citations_extractor.py` & `rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor/citations_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import urllib.request
 import rdflib
 import threading
 import json
 import pandas as pd
 from dotenv import load_dotenv
 from requests.auth import HTTPBasicAuth
-
+from tqdm import tqdm
 load_dotenv()
 
 LIDO_ENDPOINT = "http://linkeddata.overheid.nl/service/get-links"
 
 target_ecli = 'target_ecli'
 label = 'label'
 type = 'type'
@@ -131,15 +131,15 @@
             total_legislations.extend(legislation_citations)
     df_incoming = pd.DataFrame(total_incoming)
     df_outgoing = pd.DataFrame(total_outgoing)
     df_legislations = pd.DataFrame(total_legislations)
     return df_incoming, df_outgoing, df_legislations
 
 
-def citations_multithread_single(big_incoming, big_outgoing, big_legislations, ecli, username, password, current_index):
+def citations_multithread_single(big_incoming, big_outgoing, big_legislations, ecli, username, password, current_index,bar):
     incoming_df = pd.Series([], dtype='string')
     outgoing_df = pd.Series([], dtype='string')
     legislations_df = pd.Series([], dtype='string')
     for i, ecli in enumerate(ecli):
         index = current_index + i
         case_citations_incoming, case_citations_outgoing, legislation_citations = find_citations_for_case(
             remove_spaces_from_ecli(ecli), case_citations_fieldnames, legislation_citations_fieldnames, username,
@@ -149,14 +149,15 @@
             incoming_df[index] = encoded
         if case_citations_outgoing:
             encoded = json.dumps(case_citations_outgoing)
             outgoing_df[index] = encoded
         if legislation_citations:
             encoded = json.dumps(legislation_citations)
             legislations_df[index] = encoded
+        bar.update(1)
     big_incoming.append(incoming_df)
     big_outgoing.append(outgoing_df)
     big_legislations.append(legislations_df)
 
 
 def add_column_frow_list(data, name, list):
     column = pd.Series([], dtype='string')
@@ -170,18 +171,19 @@
     ecli = dataframe['ecli'].dropna().reset_index(drop=True)
     length = ecli.size
     at_once_threads = int(length / threads)
     big_incoming = []
     big_outgoing = []
     big_legislations = []
     threads = []
+    bar = tqdm(total=length, colour="GREEN")
     for i in range(0, length, at_once_threads):
         curr_ecli = ecli[i:(i + at_once_threads)]
         t = threading.Thread(target=citations_multithread_single,
-                             args=[big_incoming, big_outgoing, big_legislations, curr_ecli, username, password, i])
+                             args=[big_incoming, big_outgoing, big_legislations, curr_ecli, username, password, i,bar])
         threads.append(t)
     for t in threads:
         t.start()
     for t in threads:
         t.join()
     add_column_frow_list(dataframe, 'citations_incoming', big_incoming)
     add_column_frow_list(dataframe, 'citations_outgoing', big_outgoing)
```

### Comparing `rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/PKG-INFO` & `rechtspraak_citations_extractor-1.0.5/rechtspraak_citations_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak-citations-extractor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.4
+Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.5
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.4/setup.py` & `rechtspraak_citations_extractor-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_citations_extractor',
     packages=find_packages(include=['rechtspraak_citations_extractor']),
-    version='1.0.4',
+    version='1.0.5',
     description='Library for extracting rechtspraak citations via LIDO',
     author='LawTech Lab',
     license='MIT',
-    install_requires=['requests>=2.26.0', 'python_dotenv==0.15.0', 'pandas >=1.2.5','urllib3>=1.26.12','lxml>=4.6.3'],
+    install_requires=['requests>=2.26.0', 'python_dotenv==0.15.0', 'pandas >=1.2.5','urllib3>=1.26.12','lxml>=4.6.3','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'citations', 'rechtspraak citations', 'RS citations'],
     long_description=long_descr,
     long_description_content_type='text/markdown',
     project_urls={
         "Bug Tracker": "https://github.com/maastrichtlawtech/extraction_libraries",
         "Build Source": "https://github.com/maastrichtlawtech/extraction_libraries",
```

