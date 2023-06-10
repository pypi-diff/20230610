# Comparing `tmp/maadstml-3.24.tar.gz` & `tmp/maadstml-3.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.24.tar", last modified: Mon Jun  5 23:52:28 2023, max compression
+gzip compressed data, was "maadstml-3.25.tar", last modified: Sat Jun 10 20:00:22 2023, max compression
```

## Comparing `maadstml-3.24.tar` & `maadstml-3.25.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 23:52:28.488510 maadstml-3.24/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.24/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.24/MANIFEST.in
--rw-rw-rw-   0        0        0   171433 2023-06-05 23:52:28.488510 maadstml-3.24/PKG-INFO
--rw-rw-rw-   0        0        0   170836 2023-06-05 23:48:59.000000 maadstml-3.24/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 23:52:28.472869 maadstml-3.24/maadstml/
--rw-rw-rw-   0        0        0     2084 2023-02-19 21:08:01.000000 maadstml-3.24/maadstml/__init__.py
--rw-rw-rw-   0        0        0    64739 2023-02-19 21:07:09.000000 maadstml-3.24/maadstml/sendfiles.py
-drwxrwxrwx   0        0        0        0 2023-06-05 23:52:28.488510 maadstml-3.24/maadstml.egg-info/
--rw-rw-rw-   0        0        0   171433 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 23:52:28.000000 maadstml-3.24/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:04.000000 maadstml-3.24/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 23:52:28.488510 maadstml-3.24/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-05 23:51:33.000000 maadstml-3.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:00:22.092486 maadstml-3.25/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.25/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.25/MANIFEST.in
+-rw-rw-rw-   0        0        0   171897 2023-06-10 20:00:22.092486 maadstml-3.25/PKG-INFO
+-rw-rw-rw-   0        0        0   171300 2023-06-10 19:59:31.000000 maadstml-3.25/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 20:00:22.061183 maadstml-3.25/maadstml/
+-rw-rw-rw-   0        0        0     2121 2023-06-10 19:55:10.000000 maadstml-3.25/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.25/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    65114 2023-06-10 19:54:10.000000 maadstml-3.25/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.25/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:00:22.092486 maadstml-3.25/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   171897 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-10 20:00:22.000000 maadstml-3.25/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 20:00:21.000000 maadstml-3.25/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2021-02-05 16:13:04.000000 maadstml-3.25/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 20:00:22.092486 maadstml-3.25/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-10 19:55:28.000000 maadstml-3.25/setup.py
```

### Comparing `maadstml-3.24/LICENSE.txt` & `maadstml-3.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.24/PKG-INFO` & `maadstml-3.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.24
+Version: 3.25
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -241,14 +241,17 @@
     distance.  It is a very useful function if you want to determine common behaviours between devices, patients, or other entities.
 	Users can also setup email alerts if specific clusters are found.
 
 - **vipersearchanomaly**
   - Perform advanced analysis for user search.  This function is useful if you want to monitor what people are searching for, and determine
     if the searches are anamolous and differ from the peer group of "normal" search behaviour.
 
+- **vipernlp**
+  - Perform advanced natural language summary of PDFs.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4501,7 +4504,25 @@
 - You can specify the name of the source brokers.
 
 *servicenameto* : string, optional
 
 - You can specify the name of the destination brokers.
 
 *rollbackoffset*: ignored
+
+**36. maadstml.vipernlp(filename,maxsummarywords,maxkeywords)**
+
+**Parameters:**	Perform NLP summarization of PDFs
+
+*filename* : string, required
+
+- Filename of PDF to summarize.
+
+*maxsummarywords* : int, required
+       
+- Maximum amount of words in the summary.
+
+*maxkeywords* : int, required
+
+- Maximum amount of keywords to extract.
+
+RETURNS: JSON string of summary.
```

### Comparing `maadstml-3.24/README.md` & `maadstml-3.25/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,17 @@
     distance.  It is a very useful function if you want to determine common behaviours between devices, patients, or other entities.
 	Users can also setup email alerts if specific clusters are found.
 
 - **vipersearchanomaly**
   - Perform advanced analysis for user search.  This function is useful if you want to monitor what people are searching for, and determine
     if the searches are anamolous and differ from the peer group of "normal" search behaviour.
 
+- **vipernlp**
+  - Perform advanced natural language summary of PDFs.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4489,7 +4492,25 @@
 - You can specify the name of the source brokers.
 
 *servicenameto* : string, optional
 
 - You can specify the name of the destination brokers.
 
 *rollbackoffset*: ignored
+
+**36. maadstml.vipernlp(filename,maxsummarywords,maxkeywords)**
+
+**Parameters:**	Perform NLP summarization of PDFs
+
+*filename* : string, required
+
+- Filename of PDF to summarize.
+
+*maxsummarywords* : int, required
+       
+- Maximum amount of words in the summary.
+
+*maxkeywords* : int, required
+
+- Maximum amount of keywords to extract.
+
+RETURNS: JSON string of summary.
```

### Comparing `maadstml-3.24/maadstml/__init__.py` & `maadstml-3.25/maadstml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,8 +71,11 @@
 from .sendfiles import viperanomalypredictbatch
 
 from .sendfiles import areyoubusy
 from .sendfiles import vipermirrorbrokers
 
 from .sendfiles import viperhpdepredictprocess
 
+from .sendfiles import vipernlp
+
+
 name = "maadstml"
```

### Comparing `maadstml-3.24/maadstml/sendfiles.py` & `maadstml-3.25/maadstml/sendfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import asyncio
 import validators
 from urllib.parse import urljoin
 from urllib.parse import urlsplit
 import aiohttp
 from aiohttp import ClientSession,ClientTimeout
 import async_timeout
+import readpdf
 
 
 connectionerror=""
 
 loop = asyncio.get_event_loop()
 
 def cancelalltasks():
@@ -1060,14 +1061,24 @@
 
     val=loop.run_until_complete(tcp_echo_clientviper(value, loop,host,port,microserviceid))
     if connectionerror:
          return connectionerror
 
     return val
 
+def vipernlp(filename,fvalue,keys):
+    if filename=="":
+         return "Please enter host,port,vipertoken,groupname,groupid"
+    if fvalue > 10000:
+        return "Summary count too high. Must be  < 10000"
+    if keys > 100:
+        return "Keyword count too high. Must be  < 100"
+        
+    return readpdf.startpdfreading(filename,300,10)
+    
 def areyoubusy(host,port=-999,microserviceid=''):
     global connectionerror
 
     if (len(host)==0 or port==-999 ):
          return "Please enter host,port"
     value=("areyoubusy")
```

### Comparing `maadstml-3.24/maadstml.egg-info/PKG-INFO` & `maadstml-3.25/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.24
+Version: 3.25
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -241,14 +241,17 @@
     distance.  It is a very useful function if you want to determine common behaviours between devices, patients, or other entities.
 	Users can also setup email alerts if specific clusters are found.
 
 - **vipersearchanomaly**
   - Perform advanced analysis for user search.  This function is useful if you want to monitor what people are searching for, and determine
     if the searches are anamolous and differ from the peer group of "normal" search behaviour.
 
+- **vipernlp**
+  - Perform advanced natural language summary of PDFs.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4501,7 +4504,25 @@
 - You can specify the name of the source brokers.
 
 *servicenameto* : string, optional
 
 - You can specify the name of the destination brokers.
 
 *rollbackoffset*: ignored
+
+**36. maadstml.vipernlp(filename,maxsummarywords,maxkeywords)**
+
+**Parameters:**	Perform NLP summarization of PDFs
+
+*filename* : string, required
+
+- Filename of PDF to summarize.
+
+*maxsummarywords* : int, required
+       
+- Maximum amount of words in the summary.
+
+*maxkeywords* : int, required
+
+- Maximum amount of keywords to extract.
+
+RETURNS: JSON string of summary.
```

### Comparing `maadstml-3.24/setup.py` & `maadstml-3.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.24',
+    version='3.25',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

