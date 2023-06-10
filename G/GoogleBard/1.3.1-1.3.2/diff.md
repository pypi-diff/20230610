# Comparing `tmp/GoogleBard-1.3.1.tar.gz` & `tmp/GoogleBard-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.3.1.tar", last modified: Fri Jun  9 10:19:34 2023, max compression
+gzip compressed data, was "GoogleBard-1.3.2.tar", last modified: Sat Jun 10 01:54:32 2023, max compression
```

## Comparing `GoogleBard-1.3.1.tar` & `GoogleBard-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.440179 GoogleBard-1.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:54:32.301902 GoogleBard-1.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.3.1/LICENSE` & `GoogleBard-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.3.1/PKG-INFO` & `GoogleBard-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.3.1
+Version: 1.3.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.3.1/README.md` & `GoogleBard-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.3.1/setup.py` & `GoogleBard-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.3.1",
+    version="1.3.2",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.3.1/src/Bard.py` & `GoogleBard-1.3.2/src/Bard.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         if not self.session_id or self.session_id[-1] != ".":
             raise Exception(
                 "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value.",
             )
         resp = await self.session.get(
             "https://bard.google.com/",
             timeout=10,
+            follow_redirects=True,
         )
         if resp.status_code != 200:
             raise Exception(
                 f"Response code not 200. Response Status is {resp.status_code}",
             )
         SNlM0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
         if not SNlM0e:
```

### Comparing `GoogleBard-1.3.1/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.3.2/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.3.1
+Version: 1.3.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

