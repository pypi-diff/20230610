# Comparing `tmp/PoolFlow-0.0.4.tar.gz` & `tmp/PoolFlow-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PoolFlow-0.0.4.tar", last modified: Sat Jun 10 14:31:47 2023, max compression
+gzip compressed data, was "PoolFlow-0.0.5.tar", last modified: Sat Jun 10 14:33:03 2023, max compression
```

## Comparing `PoolFlow-0.0.4.tar` & `PoolFlow-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 14:31:47.659595 PoolFlow-0.0.4/
--rw-rw-rw-   0        0        0     1620 2023-06-10 14:31:47.658595 PoolFlow-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 14:31:47.651089 PoolFlow-0.0.4/PoolFlow/
--rw-rw-rw-   0        0        0       81 2022-09-07 08:06:49.000000 PoolFlow-0.0.4/PoolFlow/__init__.py
--rw-rw-rw-   0        0        0    13971 2023-06-10 13:44:35.000000 PoolFlow-0.0.4/PoolFlow/dynamic_pool.py
--rw-rw-rw-   0        0        0     3091 2023-06-10 14:12:38.000000 PoolFlow-0.0.4/PoolFlow/server_pool.py
--rw-rw-rw-   0        0        0    11450 2023-06-10 13:44:35.000000 PoolFlow-0.0.4/PoolFlow/static_pool.py
-drwxrwxrwx   0        0        0        0 2023-06-10 14:31:47.657595 PoolFlow-0.0.4/PoolFlow/tests/
--rw-rw-rw-   0        0        0       22 2022-09-07 09:55:01.000000 PoolFlow-0.0.4/PoolFlow/tests/__init__.py
--rw-rw-rw-   0        0        0      868 2022-09-07 09:49:55.000000 PoolFlow-0.0.4/PoolFlow/tests/test_.py
-drwxrwxrwx   0        0        0        0 2023-06-10 14:31:47.658595 PoolFlow-0.0.4/PoolFlow/utilities/
--rw-rw-rw-   0        0        0       31 2022-09-07 09:37:10.000000 PoolFlow-0.0.4/PoolFlow/utilities/__init__.py
--rw-rw-rw-   0        0        0     8940 2023-06-10 13:49:57.000000 PoolFlow-0.0.4/PoolFlow/utilities/pool_utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-10 14:31:47.656595 PoolFlow-0.0.4/PoolFlow.egg-info/
--rw-rw-rw-   0        0        0     1620 2023-06-10 14:31:47.000000 PoolFlow-0.0.4/PoolFlow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-06-10 14:31:47.000000 PoolFlow-0.0.4/PoolFlow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 14:31:47.000000 PoolFlow-0.0.4/PoolFlow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 14:24:15.000000 PoolFlow-0.0.4/PoolFlow.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2023-06-10 14:31:47.000000 PoolFlow-0.0.4/PoolFlow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 14:31:47.000000 PoolFlow-0.0.4/PoolFlow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1347 2023-06-10 14:20:23.000000 PoolFlow-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 14:31:47.659595 PoolFlow-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-06-10 14:31:40.000000 PoolFlow-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 14:33:03.281032 PoolFlow-0.0.5/
+-rw-rw-rw-   0        0        0     1567 2023-06-10 14:33:03.281032 PoolFlow-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 14:33:03.273032 PoolFlow-0.0.5/PoolFlow/
+-rw-rw-rw-   0        0        0       81 2022-09-07 08:06:49.000000 PoolFlow-0.0.5/PoolFlow/__init__.py
+-rw-rw-rw-   0        0        0    13971 2023-06-10 13:44:35.000000 PoolFlow-0.0.5/PoolFlow/dynamic_pool.py
+-rw-rw-rw-   0        0        0     3091 2023-06-10 14:12:38.000000 PoolFlow-0.0.5/PoolFlow/server_pool.py
+-rw-rw-rw-   0        0        0    11450 2023-06-10 13:44:35.000000 PoolFlow-0.0.5/PoolFlow/static_pool.py
+drwxrwxrwx   0        0        0        0 2023-06-10 14:33:03.279032 PoolFlow-0.0.5/PoolFlow/tests/
+-rw-rw-rw-   0        0        0       22 2022-09-07 09:55:01.000000 PoolFlow-0.0.5/PoolFlow/tests/__init__.py
+-rw-rw-rw-   0        0        0      868 2022-09-07 09:49:55.000000 PoolFlow-0.0.5/PoolFlow/tests/test_.py
+drwxrwxrwx   0        0        0        0 2023-06-10 14:33:03.280032 PoolFlow-0.0.5/PoolFlow/utilities/
+-rw-rw-rw-   0        0        0       31 2022-09-07 09:37:10.000000 PoolFlow-0.0.5/PoolFlow/utilities/__init__.py
+-rw-rw-rw-   0        0        0     8940 2023-06-10 13:49:57.000000 PoolFlow-0.0.5/PoolFlow/utilities/pool_utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-10 14:33:03.279032 PoolFlow-0.0.5/PoolFlow.egg-info/
+-rw-rw-rw-   0        0        0     1567 2023-06-10 14:33:03.000000 PoolFlow-0.0.5/PoolFlow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-06-10 14:33:03.000000 PoolFlow-0.0.5/PoolFlow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 14:33:03.000000 PoolFlow-0.0.5/PoolFlow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-10 14:24:15.000000 PoolFlow-0.0.5/PoolFlow.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2023-06-10 14:33:03.000000 PoolFlow-0.0.5/PoolFlow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 14:33:03.000000 PoolFlow-0.0.5/PoolFlow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1294 2023-06-10 14:32:27.000000 PoolFlow-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 14:33:03.281032 PoolFlow-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      830 2023-06-10 14:32:41.000000 PoolFlow-0.0.5/setup.py
```

### Comparing `PoolFlow-0.0.4/PKG-INFO` & `PoolFlow-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 Metadata-Version: 2.1
 Name: PoolFlow
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple process management library
 Home-page: https://victorgarric.github.io/PoolFlow/
 Author: Victor Garric
 Author-email: victor.garric@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # PoolFlow
 
-<center>
+
 
 **A simple process management library**
 
-</center>
+
 
 ## Introduction
 
 **PoolFlow** provides simple objects to manage the execution of a variety of tasks and 
 its memory usage. The main objective of **PoolFlow** is to perform a lot of scientific calculations
  and manage their successive executions through the subprocess library.
 
 ## Schematic principle
 
 The way **PoolFlow** works could be synthesized by the following diagram. A list of jobs is 
 given and the `pool` object manage the available virtual memory, considering the maximum estimated
 cost of the job given by the user.
 
-<center>
+
 
 ``` mermaid
 graph LR
 A[Job with<br>given cost]-->|Set of parameters|B{Pool};
 B-->C[Estimated usage<br>memory];
 C-->|Not enough<br>memory|B;
 C-->|Memory available<br>and allocated|D[Job is<br>launched];
 D-->|Job is done<br>memory est released|B;
 
 ```
-</center>
+
 
 ## Installing 
 The only external package **SourceFlow** depends on is `rich`. Install it directly via `pip`:
 
-<center>
 
 `pip install PoolFlow`
 
-</center>
+
 
 ## [Documentation](https://victorgarric.github.io/PoolFlow/)
 
 
 ## Warning and known issues
 
 **PoolFlow** uses management resources via `resource` native package. Due to the way `resource` work, some limitation
```

### Comparing `PoolFlow-0.0.4/PoolFlow/dynamic_pool.py` & `PoolFlow-0.0.5/PoolFlow/dynamic_pool.py`

 * *Files identical despite different names*

### Comparing `PoolFlow-0.0.4/PoolFlow/server_pool.py` & `PoolFlow-0.0.5/PoolFlow/server_pool.py`

 * *Files identical despite different names*

### Comparing `PoolFlow-0.0.4/PoolFlow/static_pool.py` & `PoolFlow-0.0.5/PoolFlow/static_pool.py`

 * *Files identical despite different names*

### Comparing `PoolFlow-0.0.4/PoolFlow/tests/test_.py` & `PoolFlow-0.0.5/PoolFlow/tests/test_.py`

 * *Files identical despite different names*

### Comparing `PoolFlow-0.0.4/PoolFlow/utilities/pool_utilities.py` & `PoolFlow-0.0.5/PoolFlow/utilities/pool_utilities.py`

 * *Files identical despite different names*

### Comparing `PoolFlow-0.0.4/PoolFlow.egg-info/PKG-INFO` & `PoolFlow-0.0.5/PoolFlow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 Metadata-Version: 2.1
 Name: PoolFlow
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple process management library
 Home-page: https://victorgarric.github.io/PoolFlow/
 Author: Victor Garric
 Author-email: victor.garric@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # PoolFlow
 
-<center>
+
 
 **A simple process management library**
 
-</center>
+
 
 ## Introduction
 
 **PoolFlow** provides simple objects to manage the execution of a variety of tasks and 
 its memory usage. The main objective of **PoolFlow** is to perform a lot of scientific calculations
  and manage their successive executions through the subprocess library.
 
 ## Schematic principle
 
 The way **PoolFlow** works could be synthesized by the following diagram. A list of jobs is 
 given and the `pool` object manage the available virtual memory, considering the maximum estimated
 cost of the job given by the user.
 
-<center>
+
 
 ``` mermaid
 graph LR
 A[Job with<br>given cost]-->|Set of parameters|B{Pool};
 B-->C[Estimated usage<br>memory];
 C-->|Not enough<br>memory|B;
 C-->|Memory available<br>and allocated|D[Job is<br>launched];
 D-->|Job is done<br>memory est released|B;
 
 ```
-</center>
+
 
 ## Installing 
 The only external package **SourceFlow** depends on is `rich`. Install it directly via `pip`:
 
-<center>
 
 `pip install PoolFlow`
 
-</center>
+
 
 ## [Documentation](https://victorgarric.github.io/PoolFlow/)
 
 
 ## Warning and known issues
 
 **PoolFlow** uses management resources via `resource` native package. Due to the way `resource` work, some limitation
```

### Comparing `PoolFlow-0.0.4/README.md` & `PoolFlow-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # PoolFlow
 
-<center>
+
 
 **A simple process management library**
 
-</center>
+
 
 ## Introduction
 
 **PoolFlow** provides simple objects to manage the execution of a variety of tasks and 
 its memory usage. The main objective of **PoolFlow** is to perform a lot of scientific calculations
  and manage their successive executions through the subprocess library.
 
 ## Schematic principle
 
 The way **PoolFlow** works could be synthesized by the following diagram. A list of jobs is 
 given and the `pool` object manage the available virtual memory, considering the maximum estimated
 cost of the job given by the user.
 
-<center>
+
 
 ``` mermaid
 graph LR
 A[Job with<br>given cost]-->|Set of parameters|B{Pool};
 B-->C[Estimated usage<br>memory];
 C-->|Not enough<br>memory|B;
 C-->|Memory available<br>and allocated|D[Job is<br>launched];
 D-->|Job is done<br>memory est released|B;
 
 ```
-</center>
+
 
 ## Installing 
 The only external package **SourceFlow** depends on is `rich`. Install it directly via `pip`:
 
-<center>
 
 `pip install PoolFlow`
 
-</center>
+
 
 ## [Documentation](https://victorgarric.github.io/PoolFlow/)
 
 
 ## Warning and known issues
 
 **PoolFlow** uses management resources via `resource` native package. Due to the way `resource` work, some limitation
```

### Comparing `PoolFlow-0.0.4/setup.py` & `PoolFlow-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='PoolFlow',
-      version='0.0.4',
+      version='0.0.5',
       description='A simple process management library',
       url='https://victorgarric.github.io/PoolFlow/',
       license='MIT',
       long_description=README,
       long_description_content_type="text/markdown",
       author='Victor Garric',
       packages=setuptools.find_packages(),
```

