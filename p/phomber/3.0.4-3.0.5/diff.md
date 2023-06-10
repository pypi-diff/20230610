# Comparing `tmp/phomber-3.0.4-py3.9.egg` & `tmp/phomber-3.0.5-py3.9.egg`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 52607 bytes, number of entries: 13
--rw-r--r--  2.0 unx     5447 b- defN 23-Jun-10 19:27 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      275 b- defN 23-Jun-10 19:27 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 19:27 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       50 b- defN 23-Jun-10 19:27 EGG-INFO/entry_points.txt
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-10 19:27 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-10 19:27 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 19:27 EGG-INFO/zip-safe
+Zip file size: 52586 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     5404 b- defN 23-Jun-10 19:38 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-10 19:38 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 19:38 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-10 19:38 EGG-INFO/entry_points.txt
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-10 19:38 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-10 19:38 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 19:38 EGG-INFO/zip-safe
 -rw-r--r--  2.0 unx        0 b- defN 23-May-21 17:02 phomber/__init__.py
 -rw-r--r--  2.0 unx    68998 b- defN 23-Jun-03 16:45 phomber/phomber.py
 -rw-r--r--  2.0 unx    68998 b- defN 23-Jun-03 15:51 phomber/phomberv3.0.2_beta.py
--rw-r--r--  2.0 unx      139 b- defN 23-Jun-10 19:27 phomber/__pycache__/__init__.cpython-39.pyc
--rw-r--r--  2.0 unx    40416 b- defN 23-Jun-10 19:27 phomber/__pycache__/phomber.cpython-39.pyc
--rw-r--r--  2.0 unx    40427 b- defN 23-Jun-10 19:27 phomber/__pycache__/phomberv3.0.2_beta.cpython-39.pyc
-13 files, 224836 bytes uncompressed, 50887 bytes compressed:  77.4%
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-10 19:38 phomber/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx    40416 b- defN 23-Jun-10 19:38 phomber/__pycache__/phomber.cpython-39.pyc
+-rw-r--r--  2.0 unx    40427 b- defN 23-Jun-10 19:38 phomber/__pycache__/phomberv3.0.2_beta.cpython-39.pyc
+13 files, 224793 bytes uncompressed, 50866 bytes compressed:  77.4%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomber
-Version: 3.0.4
+Version: 3.0.5
 Summary: `PH0MBER` a simple yet powerful osint framework for reconnaissance and information gathering
 Home-page: https://github.com/s41r4j/phomber
 Author: s41r4j
 License: UNKNOWN
 Description: <p align=center>
                  <img src='.images/phomber_logo.png'>
         </p>
@@ -20,15 +20,15 @@
                  <a href='https://www.python.org/'><img src="https://img.shields.io/badge/Python-3-blue.svg?style=flat&logo=python"></a>
                  <a href='LICENSE'><img src="https://img.shields.io/badge/License-GPL%20v3.0-brightgreen.svg"></a>
                  <a href=''><img src="https://img.shields.io/badge/Disclaimer-With great power comes great responsibility-red.svg?logo=hackaday"></a>
         </p>
               
         <br>
         
-        <h1 align=center>PH0MBER: osint framework [3.0.4 (beta)]</h1>
+        <h1 align=center>PH0MBER: osint framework [3.0.5 (beta)]</h1>
         
         
         
         <br>
         
         ## What is PH0MBER?
         
@@ -117,11 +117,10 @@
         - `PH0MBER` is back with all new features and user interface
         - `v3` has osint tools with no _api key_ requirement
         - Currently this `v3.0-beta` is for testing, try using & report bugs
         ```
         
 Keywords: python,hacking,pentesting,phomber,reverse lookup,osint,framework
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: phomber Version: 3.0.4 Summary: `PH0MBER` a simple
+Metadata-Version: 2.1 Name: phomber Version: 3.0.5 Summary: `PH0MBER` a simple
 yet powerful osint framework for reconnaissance and information gathering Home-
 page: https://github.com/s41r4j/phomber Author: s41r4j License: UNKNOWN
 Description:
                           [.images/phomber_logo.png]
 ``` An open source infomation grathering & reconnaissance framework! ```
   [https://img.shields.io/badge/Etical_Hacking-OSINT-yellow.svg?logo=sharp]
 [https://img.shields.io/badge/Version-v3.0-orange.svg?logo=vectorworks] [https:
   //img.shields.io/badge/Python-3-blue.svg?style=flat&logo=python] [https://
       img.shields.io/badge/License-GPL%20v3.0-brightgreen.svg] [https://
  img.shields.io/badge/Disclaimer-With great power comes great responsibility-
                             red.svg?logo=hackaday]
 
-             ****** PH0MBER: osint framework [3.0.4 (beta)] ******
+             ****** PH0MBER: osint framework [3.0.5 (beta)] ******
 
 ## What is PH0MBER? - `PH0MBER` is a tool which is used to gather information
 about a target which is publicly available - Previously `PH0MBER` was a tool
 which was used to gather information about a phone number, but now it has been
 upgraded to a _framework_ with many _scanners_
 
 ## Install & Usage: A Quick Guide ### Installation: - __git clone__ ``` git
@@ -43,10 +43,10 @@
 silent mode by using `-s`/`--silent` flag - You can also use `Ctrl+C` to exit -
 Descriptions ending with `*` needs internet connection
 
 ### NOTES: ``` - `PH0MBER` is back with all new features and user interface -
 `v3` has osint tools with no _api key_ requirement - Currently this `v3.0-beta`
 is for testing, try using & report bugs ``` Keywords:
 python,hacking,pentesting,phomber,reverse lookup,osint,framework Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Programming
-Language :: Python Classifier: License :: OSI Approved :: GNU General Public
-License v3 (GPLv3) Description-Content-Type: text/markdown
+UNKNOWN Classifier: Programming Language :: Python Classifier: License :: OSI
+Approved :: GNU General Public License v3 (GPLv3) Description-Content-Type:
+text/markdown
```

