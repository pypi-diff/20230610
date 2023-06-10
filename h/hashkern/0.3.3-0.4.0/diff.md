# Comparing `tmp/hashkern-0.3.3.tar.gz` & `tmp/hashkern-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashkern-0.3.3.tar", last modified: Thu May 25 21:59:40 2023, max compression
+gzip compressed data, was "hashkern-0.4.0.tar", last modified: Sat Jun 10 17:55:40 2023, max compression
```

## Comparing `hashkern-0.3.3.tar` & `hashkern-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    11344 2023-01-13 23:42:17.000000 hashkern-0.3.3/LICENSE
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14841 2023-05-25 21:59:40.606595 hashkern-0.3.3/PKG-INFO
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14107 2023-05-25 21:38:34.000000 hashkern-0.3.3/README.md
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       38 2023-05-25 21:59:40.606595 hashkern-0.3.3/setup.cfg
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     1231 2023-05-25 21:59:10.000000 hashkern-0.3.3/setup.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.602595 hashkern-0.3.3/src/
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      296 2023-05-25 21:58:21.000000 hashkern-0.3.3/src/hash/__init__.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/cli/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       23 2023-01-14 12:45:56.000000 hashkern-0.3.3/src/hash/cli/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5912 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/cli/main.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7189 2023-01-13 23:42:17.000000 hashkern-0.3.3/src/hash/dag.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     2148 2023-05-14 21:16:53.000000 hashkern-0.3.3/src/hash/errors.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/kern/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      148 2023-05-25 21:59:19.000000 hashkern-0.3.3/src/hash/kern/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    10412 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/action.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7379 2023-05-25 21:58:08.000000 hashkern-0.3.3/src/hash/kern/execute.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      931 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/hash.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3196 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/main.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    16126 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/planner.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     4181 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/secrets.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    19277 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/state.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5952 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/templates.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3461 2023-01-13 23:42:17.000000 hashkern-0.3.3/src/hash/logs.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/resources/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       69 2023-05-14 22:02:35.000000 hashkern-0.3.3/src/hash/resources/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    97796 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/resources/base.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    22702 2023-05-15 21:31:58.000000 hashkern-0.3.3/src/hash/resources/targets.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/store/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       59 2023-01-13 23:42:17.000000 hashkern-0.3.3/src/hash/store/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    28132 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/store/base.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    12523 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/utils.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hashkern.egg-info/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14841 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/PKG-INFO
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      738 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/SOURCES.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        1 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/dependency_links.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       39 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/entry_points.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      213 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/requires.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        5 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.331613 hashkern-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2023-06-10 17:55:36.000000 hashkern-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15234 2023-06-10 17:55:40.331613 hashkern-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14500 2023-06-10 17:55:36.000000 hashkern-0.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 17:55:40.331613 hashkern-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-06-10 17:55:36.000000 hashkern-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.325613 hashkern-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.326613 hashkern-0.4.0/src/hash/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.327613 hashkern-0.4.0/src/hash/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5912 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/cli/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     7189 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2148 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.329613 hashkern-0.4.0/src/hash/kern/
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10412 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     7379 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/hash.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    16126 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/planner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4181 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)    19277 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/state.py
+-rw-rw-rw-   0 root         (0) root         (0)     5952 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/kern/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.329613 hashkern-0.4.0/src/hash/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   110674 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    33455 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/resources/targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.330613 hashkern-0.4.0/src/hash/store/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/store/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28132 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/store/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12523 2023-06-10 17:55:36.000000 hashkern-0.4.0/src/hash/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 17:55:40.331613 hashkern-0.4.0/src/hashkern.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15234 2023-06-10 17:55:40.000000 hashkern-0.4.0/src/hashkern.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-10 17:55:40.000000 hashkern-0.4.0/src/hashkern.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 17:55:40.000000 hashkern-0.4.0/src/hashkern.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-10 17:55:40.000000 hashkern-0.4.0/src/hashkern.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-10 17:55:40.000000 hashkern-0.4.0/src/hashkern.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-10 17:55:40.000000 hashkern-0.4.0/src/hashkern.egg-info/top_level.txt
```

### Comparing `hashkern-0.3.3/LICENSE` & `hashkern-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/PKG-INFO` & `hashkern-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: hashkern
-Version: 0.3.3
-Summary: A tool for managing resources in a mono repository
-Author: Mouhsen Ibrahim
-Author-email: mouhsen.ibrahim@gmail.com
-Project-URL: Documentation, https://hash-kern.readthedocs.io/en/latest/index.html
-Project-URL: Source, https://gitlab.com/hash-platform/hashkern
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Hash kern
 
 Hash kern is the core of the Hash platform, it allows you to define your resources in your Mono Repository and
 it can be used to manage building, testing, publishing, and deploying those resources to your own environments,
 Hash kern uses yaml files to define resources and their kinds along with the environments used in your project.
 It allows you also to specify dependencies between resources and in many cases it can automatically detect
 them. It uses a backend store for storing the state of your resources which include the hash of the resource's
@@ -53,27 +34,28 @@
 ```bash
 pip install hashkern
 ```
 
 Then you can use the CLI like this
 
 ```bash
-> hashc
-usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] {build,test,publish,deploy} ...
+> haks
+usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] [--plan PLAN] {build,test,publish,deploy,hash,render,clear,version} ...
 
 A tool to build resources based on their hash and type
 
 positional arguments:
-  {build,test,publish,deploy}
+  {build,test,publish,deploy,hash,render,clear,version}
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   --storage STORAGE     The storage system used default is Local File
   --config CONFIG       The configuration file default is config.ini
   --env ENV             An environment to run the action in it
+  --plan PLAN           Only do a plan and save it to this file
 ```
 
 ### Install from source
 
 Install the required packages to clone the code, create virtual env and run the tests with make
 
 ```bash
@@ -122,35 +104,37 @@
 ```
 
 Print the help for the client with this command
 
 ```bash
 > python src/client/main.py
 
-usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] {build,test,publish,deploy} ...
+usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] [--plan PLAN] {build,test,publish,deploy,hash,render,clear,version} ...
 
 A tool to build resources based on their hash and type
 
 positional arguments:
-  {build,test,publish,deploy}
+  {build,test,publish,deploy,hash,render,clear,version}
 
 optional arguments:
   -h, --help            show this help message and exit
   --storage STORAGE     The storage system used default is Local File
   --config CONFIG       The configuration file default is config.ini
   --env ENV             An environment to run the action in it
+  --plan PLAN           Only do a plan and save it to this file
 ```
 
 The client takes three options:
 
 * `--storage` this one is used to select a storage backend for the state, the options for storage backend are in the config file.
 * `--config` this option is used to select a config file for storage backends, it is an INI file, its default value is `config.ini`
 * `--env` this option is used to select the environment name where the action will be executed, its default value is `None`, this
   value is acceptabe for some actions on some resources and it is not acceptable for some other actions, the environment
   must exist in the repository otherwise we get an error.
+* `--plan` this option is used to only run the plan and save it to the file specified in the option, it defaults to false.
 
 The format for config file is as follows:
 
 ```ini
 [LocalFile]
 output = hash_test/storage
 organization = hashio
```

### Comparing `hashkern-0.3.3/README.md` & `hashkern-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: hashkern
+Version: 0.4.0
+Summary: A tool for managing resources in a mono repository
+Author: Mouhsen Ibrahim
+Author-email: mouhsen.ibrahim@gmail.com
+Project-URL: Documentation, https://hash-kern.readthedocs.io/en/latest/index.html
+Project-URL: Source, https://gitlab.com/hash-platform/hashkern
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Hash kern
 
 Hash kern is the core of the Hash platform, it allows you to define your resources in your Mono Repository and
 it can be used to manage building, testing, publishing, and deploying those resources to your own environments,
 Hash kern uses yaml files to define resources and their kinds along with the environments used in your project.
 It allows you also to specify dependencies between resources and in many cases it can automatically detect
 them. It uses a backend store for storing the state of your resources which include the hash of the resource's
@@ -34,27 +53,28 @@
 ```bash
 pip install hashkern
 ```
 
 Then you can use the CLI like this
 
 ```bash
-> hashc
-usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] {build,test,publish,deploy} ...
+> haks
+usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] [--plan PLAN] {build,test,publish,deploy,hash,render,clear,version} ...
 
 A tool to build resources based on their hash and type
 
 positional arguments:
-  {build,test,publish,deploy}
+  {build,test,publish,deploy,hash,render,clear,version}
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   --storage STORAGE     The storage system used default is Local File
   --config CONFIG       The configuration file default is config.ini
   --env ENV             An environment to run the action in it
+  --plan PLAN           Only do a plan and save it to this file
 ```
 
 ### Install from source
 
 Install the required packages to clone the code, create virtual env and run the tests with make
 
 ```bash
@@ -103,35 +123,37 @@
 ```
 
 Print the help for the client with this command
 
 ```bash
 > python src/client/main.py
 
-usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] {build,test,publish,deploy} ...
+usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] [--plan PLAN] {build,test,publish,deploy,hash,render,clear,version} ...
 
 A tool to build resources based on their hash and type
 
 positional arguments:
-  {build,test,publish,deploy}
+  {build,test,publish,deploy,hash,render,clear,version}
 
 optional arguments:
   -h, --help            show this help message and exit
   --storage STORAGE     The storage system used default is Local File
   --config CONFIG       The configuration file default is config.ini
   --env ENV             An environment to run the action in it
+  --plan PLAN           Only do a plan and save it to this file
 ```
 
 The client takes three options:
 
 * `--storage` this one is used to select a storage backend for the state, the options for storage backend are in the config file.
 * `--config` this option is used to select a config file for storage backends, it is an INI file, its default value is `config.ini`
 * `--env` this option is used to select the environment name where the action will be executed, its default value is `None`, this
   value is acceptabe for some actions on some resources and it is not acceptable for some other actions, the environment
   must exist in the repository otherwise we get an error.
+* `--plan` this option is used to only run the plan and save it to the file specified in the option, it defaults to false.
 
 The format for config file is as follows:
 
 ```ini
 [LocalFile]
 output = hash_test/storage
 organization = hashio
```

### Comparing `hashkern-0.3.3/setup.py` & `hashkern-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         return f.read().splitlines()
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name="hashkern",
-    version="0.3.3",
+    version="0.4.0",
     author="Mouhsen Ibrahim",
     author_email="mouhsen.ibrahim@gmail.com",
     description="A tool for managing resources in a mono repository",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `hashkern-0.3.3/src/hash/cli/main.py` & `hashkern-0.4.0/src/hash/cli/main.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/dag.py` & `hashkern-0.4.0/src/hash/dag.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/errors.py` & `hashkern-0.4.0/src/hash/errors.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/action.py` & `hashkern-0.4.0/src/hash/kern/action.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/execute.py` & `hashkern-0.4.0/src/hash/kern/execute.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/hash.py` & `hashkern-0.4.0/src/hash/kern/hash.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/main.py` & `hashkern-0.4.0/src/hash/kern/main.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/planner.py` & `hashkern-0.4.0/src/hash/kern/planner.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/secrets.py` & `hashkern-0.4.0/src/hash/kern/secrets.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/state.py` & `hashkern-0.4.0/src/hash/kern/state.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/kern/templates.py` & `hashkern-0.4.0/src/hash/kern/templates.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/logs.py` & `hashkern-0.4.0/src/hash/logs.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/resources/base.py` & `hashkern-0.4.0/src/hash/resources/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,21 +43,27 @@
 
     @hookspec
     def get_ignores(self):
         pass
 
 
 class FileDownloadVerify(object):
-    def __init__(self, url: str) -> None:
+    def __init__(self, url: str, cpu_arch=None, os_name=None) -> None:
         utils.check_type(
             url, str, Exception, False, f"url must be string found {type(url)}"
         )
         self.__url = url
-        self.__os_name = platform.system().lower()
-        self.__cpu_arch = platform.processor().lower()
+        if cpu_arch is None:
+            self.__cpu_arch = platform.processor().lower()
+        else:
+            self.__cpu_arch = cpu_arch
+        if os_name is None:
+            self.__os_name = platform.system().lower()
+        else:
+            self.__os_name = os_name
 
     def __verify_checksum(self, file: str, checksum: str):
         utils.check_type(
             checksum,
             str,
             Exception,
             False,
@@ -98,15 +104,15 @@
             try:
                 self.__verify_checksum(path, checksum)
                 return
             except errors.ChecksumError:
                 pass
         response = requests.get(
             self.__url.format(
-                version=version, os_name=self.__os_name, cpu_arch=self.__cpu_arch
+                version=version, cpu_arch=self.__cpu_arch, os_name=self.__os_name
             ),
             stream=True,
         )
         with open(path, "wb") as f:
             for chunk in response.iter_content(chunk_size=512):
                 f.write(chunk)
         self.__verify_checksum(path, checksum)
@@ -1004,14 +1010,21 @@
                 env.getName(),
                 state.get("hash", ""),
                 "file",
                 os.path.join(self.getPath(), "tfplan"),
             )
         ]
         normal_outputs, sensitive_outputs = self.get_outputs(self.getPath())
+        if not self.getSpec("store_sensitive_outputs_in_secrets"):
+            return {
+                "status": "plan generated",
+                "artifacts": artifacts,
+                "globals": {**normal_outputs, **sensitive_outputs},
+                "version": self.__get_version(),
+            }
         return {
             "status": "plan generated",
             "artifacts": artifacts,
             "globals": normal_outputs,
             "secrets": sensitive_outputs,
             "version": self.__get_version(),
         }
@@ -1098,14 +1111,20 @@
                     vars += f" -var {var_name}={var_value}"
             deploy_command += vars
         try:
             self.execute(
                 deploy_command, self.getPath(), self.getSpec("apply_timeout", 300)
             )
             normal_outputs, sensitive_outputs = self.get_outputs(self.getPath())
+            if not self.getSpec("store_sensitive_outputs_in_secrets"):
+                return {
+                    "status": "plan applied",
+                    "globals": {**normal_outputs, **sensitive_outputs},
+                    "version": self.__get_version(),
+                }
             return {
                 "status": "plan applied",
                 "globals": normal_outputs,
                 "secrets": sensitive_outputs,
                 "version": self.__get_version(),
             }
         except FileNotFoundError as e:
@@ -1306,14 +1325,38 @@
             raise errors.ResourceBuildError("Cannot find kustomize in PATH")
         except subprocess.CalledProcessError as e:
             raise errors.ResourceBuildError(e.stderr.decode("UTF-8"))
         path = os.path.join(path, file)
         with open(path, "w") as f:
             f.write(p.stdout.decode("UTF-8"))
 
+    def re_action(self, action: str, state: dict, env: EnvResource) -> bool:
+        if action == "deploy" and env is not None:
+            target = env.getTarget("K8STarget")
+            if target:
+                artifacts = (
+                    state.get("envs", {})
+                    .get(env.getName(), {})
+                    .get("build", {})
+                    .get("artifacts", [])
+                )
+                for artifact in artifacts:
+                    if artifact.getId() != "manifests":
+                        continue
+                    config = {
+                        "path": self.getPath(),
+                        "manifests_path": artifact.getData(),
+                        "diff": True,
+                    }
+                    try:
+                        return target.action("test", config)
+                    except errors.ResourceError as e:
+                        raise errors.ResourceTestError(str(e))
+        return False
+
     @hookimpl
     def action(self, name, state, env):
         self.check_kubectl()
         if name == "build":
             return self.build(state, env)
         elif name == "test":
             return self.test(state, env)
@@ -1355,14 +1398,15 @@
                     manifest.get("metadata", {}).get("namespace") is not None
                     and force_namespace
                 ):
                     manifest["metadata"]["namespace"] = namespace
                 elif manifest.get("metadata", {}).get("namespace") is None:
                     manifest["metadata"]["namespace"] = namespace
                 new_manifests.append(manifest)
+
         with open(path, "w") as f:
             yaml.safe_dump_all(new_manifests, f)
         env_variables = self.getSpec("envs", {})
         for name, value in env_variables.items():
             os.environ[name] = value
         try:
             command = f"cat {path} | envsubst"
@@ -1372,15 +1416,18 @@
         except subprocess.CalledProcessError as e:
             raise errors.ResourceBuildError(
                 f"An error when filling env variables in manifests: {p.stderr.decode('UTF-8')}"
             )
         artifact = self.create_artifact(
             "manifests", "build", env.getName(), state.get("hash", ""), "file", path
         )
-        return {"msg": "manifests generated", "artifacts": [artifact]}
+        return {
+            "msg": "manifests generated",
+            "artifacts": [artifact],
+        }
 
     @classmethod
     def runTests(
         cls,
         target: Target,
         path: str,
         artifacts: list,
@@ -1424,32 +1471,71 @@
                 }
                 try:
                     target.action("test", config)
                 except errors.ResourceError as e:
                     raise errors.ResourceTestError(str(e))
 
     @classmethod
-    def applyManifests(cls, env: EnvResource, path: str, artifacts: list, kubectl: str):
+    def applyManifests(
+        cls,
+        env: EnvResource,
+        path: str,
+        artifacts: list,
+        kubectl: str,
+        manifests_applied_in_state=[],
+    ):
         if env is None:
             raise errors.ResourceDeployError("You need an env to apply k8s manifests")
         target = env.getTarget("K8STarget")
         if target is None:
             raise errors.ResourceDeployError(
                 f"No K8S target found in env {env.getName()}"
             )
+        applied_manifests = []
         for artifact in artifacts:
             config = {
                 "path": path,
                 "kubectl": kubectl,
                 "manifests_path": artifact.getData(),
             }
             try:
                 target.action("deploy", config)
             except errors.ResourceError as e:
                 raise errors.ResourceDeployError(str(e))
+            with open(artifact.getData(), "r") as f:
+                data = yaml.load_all(f, Loader=yaml.SafeLoader)
+                for manifest in data:
+                    applied_manifests.append(
+                        manifest.get("apiVersion", "")
+                        + ":"
+                        + manifest.get("kind", "")
+                        + ":"
+                        + manifest.get("metadata", {}).get("name", "")
+                        + ":"
+                        + manifest.get("metadata", {}).get("namespace", "")
+                    )
+        for manifest in manifests_applied_in_state:
+            if manifest not in applied_manifests:
+                manifest_parts = manifest.split(":")
+                if len(manifest_parts) != 4:
+                    raise errors.ResourceDeployError(
+                        f"saved manifest name in state ${manifest} is wrongly formatted"
+                    )
+                config = {
+                    "path": path,
+                    "kubectl": kubectl,
+                    "resource_kind": manifest_parts[1],
+                    "resource_name": manifest_parts[2],
+                    "resource_namespace": manifest_parts[3],
+                }
+                try:
+                    target.action("delete", config)
+                except errors.ResourceError as e:
+                    raise errors.ResourceDeployError(str(e))
+        return applied_manifests
 
     def test(self, state: dict, env: EnvResource):
         if env is None:
             raise errors.ResourceTestError(
                 "Testing a kustomize resource requires an env"
             )
         else:
@@ -1459,15 +1545,15 @@
                 raise errors.ResourceTestError(
                     f"No target of kind K8STarget in env {env}"
                 )
         namespace = self.getSpec("namespace", env.getName())
         try:
             config = {"path": self.getPath(), "namespace": namespace}
             target.action("create_namespace", config)
-        except subprocess.CalledProcessError:
+        except errors.ResourceError:
             pass
         self.runTests(
             target,
             self.getPath(),
             artifacts,
             env,
             self.__kubectl,
@@ -1479,16 +1565,30 @@
     def deploy(self, state: dict, env: EnvResource):
         if env is None:
             raise errors.ResourceTestError(
                 "Deploying a kustomize resource requires an env"
             )
         else:
             artifacts = state["envs"][env.getName()]["build"].get("artifacts", [])
-        self.applyManifests(env, self.getPath(), artifacts, self.__kubectl)
-        return {"msg": "kustomize applied without errors"}
+        manifests_applied_in_state = []
+        if self.getSpec("remove_deleted_resources", False):
+            manifests_applied_in_state = (
+                state.get("local", {})
+                .get(env.getName(), {})
+                .get("deploy", {})
+                .get("manifests", [])
+            )
+        applied_manifests = self.applyManifests(
+            env, self.getPath(), artifacts, self.__kubectl, manifests_applied_in_state
+        )
+
+        return {
+            "msg": "kustomize applied without errors",
+            "local": {"manifests": applied_manifests},
+        }
 
 
 # Docker resource
 
 
 class DockerImageResource(Resource):
     @classmethod
@@ -1512,20 +1612,53 @@
         super().__init__(file)
         if self.getKind() != "DockerImage":
             raise errors.ResourceConfigError("This is not a DockerImage resource")
         self.name = self.getMetadata("name")
 
     @classmethod
     def DockerBuild(cls, path, image_name, docker_file="Dockerfile"):
-        build_command = f"docker build -t {image_name} . -f {docker_file}"
+        build_command = f"docker build -t {image_name} . -f {docker_file} --iidfile dockerimage.id --metadata-file dockerimage.metadata"
+        imageid_path = os.path.join(path, "dockerimage.id")
+        imagemeta_path = os.path.join(path, "dockerimage.metadata")
         try:
             cls.execute(build_command, path)
-            return {"error": False, "msg": "built docker image"}
+            with open(imageid_path, "r") as f:
+                imageid = f.read().strip()
+            with open(imagemeta_path, "r") as f:
+                imagemeta = json.load(f)
+            return {
+                "error": False,
+                "msg": "built docker image",
+                "image_digest": imageid,
+                "image_metadata": imagemeta,
+            }
         except subprocess.CalledProcessError as e:
             raise errors.ResourceBuildError(e.stderr.decode("UTF-8"))
+        finally:
+            if os.path.exists(imageid_path):
+                os.remove(imageid_path)
+            if os.path.exists(imagemeta_path):
+                os.remove(imagemeta_path)
+
+    @hookimpl
+    def re_action(self, action: str, state: dict, env: EnvResource) -> bool:
+        if action in ["build", "test", "deploy"]:  # TODO process deploy action
+            return False
+        if env is None:
+            raise errors.ResourceError(
+                "publishing docker image resource requires an env"
+            )
+        target = env.getTarget("DockerRegistryTarget")
+        if target is None:
+            raise errors.ResourceError(
+                f"env {env.getName()} has no Docker Registry resource"
+            )
+        image_name = self.build_image_name(self, state)
+        config = {"image_name": image_name, "path": self.getPath()}
+        return not target.action("inspect", config)["found"]
 
     @hookimpl
     def action(self, name, state, env):
         if name == "build":
             return self.build(state, env)
         elif name == "test":
             return self.test(state, env)
@@ -1610,38 +1743,47 @@
         return {"error": False, "msg": "tested docker image"}
 
     def publish(self, state: dict, env: EnvResource):
         if env is None:
             raise errors.ResourcePublishError(
                 "Cannot publish Docker resource without an env"
             )
-        artifacts = state["envs"][env.getName()]["build"].get("artifacts", [])
         image_name = self.build_image_name(self, state)
         config = {
             "path": self.getPath(),
             "image_name": image_name,
             "docker_file": self.getSpec("docker_file", "Dockerfile"),
             "image_file": os.path.join(self.getPath(), "docker.build"),
         }
         target = env.getTarget("DockerRegistryTarget")
         if target is None:
             raise errors.ResourceDeployError(
                 f"No Docker Registry target found in env {env.getName()}"
             )
-        image_url = target.action("publish", config)
+        image_data = target.action("publish", config)
+        image_url = image_data["image_url"]
+        image_url_digest = image_data["image_url_digest"]
         return {
             "artifacts": [
                 self.create_artifact(
                     "image_url",
                     "publish",
                     env.getName(),
                     state.get("hash", ""),
                     "url",
                     image_url,
-                )
+                ),
+                self.create_artifact(
+                    "image_url_digest",
+                    "publish",
+                    env.getName(),
+                    state.get("hash", ""),
+                    "url",
+                    image_url_digest,
+                ),
             ]
         }
 
     def deploy(self, state: dict, env: EnvResource):
         if env is None:
             raise errors.ResourceDeployError(
                 "Cannot deploy Docker resource without an env"
@@ -1754,15 +1896,16 @@
 
 class MicroService(object):
     @classmethod
     def build(cls, res, state, target, env: EnvResource):
         docker_path = os.path.join(res.getPath(), res.getSpec("docker_path", "."))
         image_name = DockerImageResource.build_image_name(res, state)
         config = {"image_name": image_name, "path": res.getPath()}
-        image_url = target.action("publish", config)
+        image_data = target.action("publish", config)
+        image_url = image_data.get("image_url")
         k8s_path = os.path.join(res.getPath(), res.getSpec("k8s_path", "k8s"))
         KustomizeResource.generate(k8s_path, "manifests.yaml", env)
         k8s_file = os.path.join(k8s_path, "manifests.yaml")
         try:
             with open(k8s_file, "r") as f:
                 if f.read() == "" and not res.getSpec("allow_empty_manifests", True):
                     raise errors.ResourceBuildError(
@@ -2107,15 +2250,15 @@
             self.__go, self.__golangci_lint, self.getPath()
         )
         if deploy_target == "kubernetes":
             namespace = self.getSpec("namespace", env.getName())
             try:
                 config = {"path": self.getPath(), "namespace": namespace}
                 target.action("create_namespace", config)
-            except subprocess.CalledProcessError:
+            except errors.ResourceError:
                 pass
             MicroService.test(self, target, artifacts, env)
         return {"_golangci_lint": golang_ci_lint_env_data}
 
     def deploy(self, state: dict, env):
         # deploy k8s manifests only
         if env is None:
@@ -2168,14 +2311,22 @@
             go_mod_path = self.getSpace().get_base()
         else:
             go_mod_path = os.path.join(self.getPath(), go_mod_path)
         h = kern.Hash().hash(go_mod_path, ["go.mod", "go.sum"])
         go_mod_hash = result.get("build", {}).get("_go_mod_hash")
         if go_mod_hash != h:
             return True
+        # check if docker image is still in registry
+        if action == "build" and env is not None:
+            image_name = DockerImageResource.build_image_name(self, state)
+            config = {"image_name": image_name, "path": self.getPath()}
+            target = env.getTarget("DockerRegistryTarget")
+            if target:
+                if target.action("inspect", config)["found"] is False:
+                    return True
         if action == "deploy" and env is not None:
             target = env.getTarget("K8STarget")
             if target:
                 artifacts = (
                     state.get("envs", {})
                     .get(env.getName(), {})
                     .get("build", {})
@@ -2204,26 +2355,162 @@
             if version != go_version:
                 return True
         except subprocess.CalledProcessError as e:
             raise errors.ResourceBuildError(e)
         return False
 
 
+class IstioCtl(object):
+    def __init__(self, version: str, path: str, checksum=None) -> None:
+        self.__version = version
+        self.__cli = os.path.join(path, f"istioctl-{version}")
+        os_name = platform.system().lower()
+        cpu_arch = platform.processor().lower()
+        if cpu_arch == "x86_64":
+            cpu_arch = "amd64"
+        self.fdv = FileDownloadVerify(
+            "https://github.com/istio/istio/releases/download/{version}/istioctl-{version}-{os_name}-{cpu_arch}.tar.gz",
+            cpu_arch=cpu_arch,
+        )
+        self.__checksums = {
+            "amd64": {
+                "1.17.2": "c2dfaf0cf832ccc7236aac51c672b74429a1f801e32bc8f4bc24ca54dec38653",
+                "1.17.1": "8c81017cabe3961e11e9a0b33afd24844fc099127df3d090edbdef0753cc819b",
+                "1.17.0": "b1aa886329657e3219679081f43c14c6d24ebc5b8ab0def1970e0e5f8cc22237",
+                "1.16.5": "85387fccd7c0cac436d7d97609a54e8ca5b3cecffc38f530dbd70f3f84eb9165",
+                "1.16.4": "99a98c6721afae9665064a6f0ff6e2ca493ba86550b3b5091b58077d60371d3e",
+                "1.16.3": "7a412d0c430aedbde4067ca1c4202b8bf995b76011e7e807b07a4b9917713736",
+                "1.16.2": "b47f090ce8383e5c03913ff2f6fd8fc994fe3aee3844cce730d435bfa5deff0c",
+                "1.16.1": "752b3104a4894793fa7acff53e2a3354e3baf716e70506e6c6a82dbb0cbd2bf7",
+                "1.16.0": "c4ad9b40d19c70238e6b48019b3b1f1c5c8de3d1253d61e7899f4a3d300f869d",
+                "1.15.7": "7afbfb098508e20d373b2cae569a90be7faede3a95107f680fa2a829cd143606",
+                "1.15.6": "41cfb4a00d4a0e3fffb6e58fcde1ca8f81657a50dc774872e546dfc095b0a8bf",
+                "1.15.5": "613170bd9560b58b0c0ee764eed94139861da45250d4c61719b06206a2cd44bf",
+                "1.15.4": "b89064522144d4a8506aa15ea86391a3a2f991eec6ce50d732f2a8efe8016206",
+                "1.15.3": "c99d6850aa33690809fd8decf0d34bf8b6e72ff95595cc2111b0a704e08399e1",
+                "1.15.2": "1b3692822b942b418aff8b83f8790875e56e939da8d90a00c31865f5f79e6afc",
+                "1.15.1": "b32e05d678fd518e7de2a0c129fb70cca7c1265c80c7791216134269a3233752",
+                "1.15.0": "e0069e99d43038735bfd8c7f8b69cd8c1edd3a1a27eeb858282d04faab1a8777",
+                "1.14.6": "8f5a811ca1b05f4d594b13b87b5d196146b57990b93ae32f200e0d2056969db6",
+                "1.14.5": "bd6175584a064829ab58cf736d6160b3c506fe0f31fb8e3268c3690087f3a73e",
+                "1.14.4": "73c0b5fd8c7990a8f55a7defbbd8c264cf53e2c6499309b0bf0aef913353ba4f",
+                "1.14.3": "4d629e4d51ad002fb2a019f27f72a9a5d362b364f63e3e43b4aecd20d7c32266",
+                "1.14.2": "c7efb763b5f88ba1d4dd10f955a56f6eec54e1696eaca3412d403af6af48f395",
+                "1.14.1": "6fc691fdec5299a5855b3d85c14778d5b31544fab9b08b55c2bbab2484169dbd",
+                "1.14.0": "1b666afca48f5f662f556365af07e0c45e5bc3cd40605513db92870d1032a8a0",
+                "1.13.9": "711d6e67bd8def09caf7e062f5b53f2045e661b33bc77c8c751b4f106d82eac9",
+                "1.13.8": "977400c70e8f3fae572759f379d0af32e90d878b55b84fd129bb82a13de6f3c7",
+                "1.13.7": "7e9e6fd806e4b6c5525f1b8402b22010063c2efb699dc282eb7e6ffe235ffebe",
+                "1.13.6": "c9402458b7c20ab10b8a46d9d428ad065e6ff16e2e1ded7fa5f606fac20deebd",
+                "1.13.5": "89f1cdcc64ed63132ea63459d630cd9d63b285909e6bf093cf3c92abf3f7b117",
+                "1.13.4": "9f8a0b35a62ca3c979e19ee878f4b516a9a8dec47357e0cf1d0bf5529998ac65",
+                "1.13.3": "f6d20c16691e8466233214278b50c4e07797cc30792eeb9402f95974872618fc",
+                "1.13.2": "e674a04a7c4fc95bbcd17576fdd89758971dd4f5f51ed95e0914d02ab7a40d60",
+                "1.13.1": "4fcb905302802cf12ce5999f3784f5c72c6b70423fa8ba29161da07a09f938c7",
+                "1.13.0": "2444d60b0fb6168ce047a639ef0071d249caf79965b4489670bfd32ee97c3c58",
+            }
+        }
+        file_name = os.path.join(
+            path, "istioctl-{version}-" + os_name + "-" + cpu_arch + ".tar.gz"
+        )
+        if checksum is None:
+            checksum = self.__checksums.get(cpu_arch, {}).get(self.__version, "")
+        self.fdv.prepare(
+            self.__version,
+            checksum,
+            file_name,
+            self.__cli,
+            True,
+        )
+        self.__cli = os.path.join(self.__cli, "istioctl")
+
+    def install(self, args: str):
+        install_command = f"{self.__cli} {args} install -y"
+        Resource.execute(install_command, ".")
+
+    def verify_install(self, args: str):
+        verify_install_command = f"{self.__cli} verify-install"
+        Resource.execute(verify_install_command, ".")
+
+
+class IstioResource(Resource):
+    @hookimpl
+    def init(self, file):
+        super().__init__(file)
+        if self.getKind() != "Istio":
+            raise errors.ResourceConfigError("This is not a Istio resource")
+        self.name = self.getMetadata("name")
+
+    @hookimpl
+    def re_action(self, action: str, state: dict, env: EnvResource) -> bool:
+        if action != "deploy":
+            return False
+        if env is None:
+            raise errors.ResourceError(
+                "IstioResource needs an environment to run actions"
+            )
+        target = env.getTarget("K8STarget")
+        if target is None:
+            raise errors.ResourceError(
+                f"IstioResource needs a K8STarget in environment {env.getName()}"
+            )
+        version = self.getSpec("version", "1.17.2")
+        config = {
+            "path": self.getPath(),
+            "istioctl": IstioCtl(
+                version, self.getSpace().get_hash_dir(), self.getSpec("checksum")
+            ),
+        }
+        return target.action("istioctl_verify-install", config)
+
+    @hookimpl
+    def action(self, name: str, state: dict, env: EnvResource):
+        if env is None:
+            raise errors.ResourceError(
+                "IstioResource needs an environment to run actions"
+            )
+        target = env.getTarget("K8STarget")
+        if target is None:
+            raise errors.ResourceError(
+                f"IstioResource needs a K8STarget in environment {env.getName()}"
+            )
+        if name == "deploy":
+            return self.deploy(state, env, target)
+
+    def deploy(self, state: dict, env: EnvResource, target: Target):
+        version = self.getSpec("version", "1.17.2")
+        istio = {
+            "profile": self.getSpec("profile", "default"),
+            "config_file": os.path.join(self.getPath(), self.getSpec("config_file"))
+            if self.getSpec("config_file")
+            else None,
+            "revision": self.getSpec("revision"),
+        }
+        config = {
+            "path": self.getPath(),
+            "istioctl": IstioCtl(version, self.getSpace().get_hash_dir()),
+            "istio": istio,
+        }
+        target.action("istioctl_install", config)
+        return {"local": {"version": version}}
+
+
 def get_plugin_manager():
     pm = pluggy.PluginManager("hash-resource")
     pm.add_hookspecs(ResourceSpec)
     pm.load_setuptools_entrypoints("hash-resource")
     pm.register(FakeResource, "FakeResource")
     pm.register(EnvResource, "EnvResource")
     pm.register(ProjectResource, "ProjectResource")
     pm.register(TerraformResource, "TerraformResource")
     pm.register(KustomizeResource, "KustomizeResource")
     pm.register(DockerImageResource, "DockerImageResource")
     pm.register(GoServiceResource, "GoServiceResource")
     pm.register(GoMicroServiceResource, "GoMicroServiceResource")
+    pm.register(IstioResource, "IstioResource")
     return pm
 
 
 def get_resource(file: str):
     """
     Retrun the specific resource object of the resource file
     passed as an argument
```

### Comparing `hashkern-0.3.3/src/hash/resources/targets.py` & `hashkern-0.4.0/src/hash/resources/targets.py`

 * *Files 27% similar despite different names*

```diff
@@ -53,352 +53,620 @@
     def init(self, config: dict, space) -> None:
         self._init(config)
         if self.kind != "K8STarget":
             raise errors.TargetConfigError(
                 f"This target is not of kind K8S, it is of kind {self.kind}"
             )
         self.__space = space
+        self.certificate_ca = None
+        self.certificate = None
+        self.client_key = None
+        self.kube_config = None
 
-    @hookimpl
-    def action(self, name: str, config: dict):
-        if name != "deploy" and name != "test" and name != "create_namespace":
-            raise errors.TargetActionError(
-                f"Cannot run action {name} with target of type K8S"
-            )
-        kubectl_binary = config.get("kubectl", "kubectl")
+    def remove_temp_files(self):
+        if self.certificate_ca:
+            try:
+                os.remove(self.certificate_ca)
+            except Exception:
+                pass
+        if self.certificate:
+            try:
+                os.remove(self.certificate)
+            except Exception:
+                pass
+        if self.client_key:
+            try:
+                os.remove(self.client_key)
+            except Exception:
+                pass
+        if self.kube_config:
+            try:
+                os.remove(self.kube_config)
+            except Exception:
+                pass
+
+    def authenticate_istioctl(self) -> str:
         context = self.spec.get("context")
-        k8s_certificate_ca = self.spec.get("k8s_certificate_ca")
-        if k8s_certificate_ca:
+        kube_config = self.spec.get("kube_config")
+        if context or kube_config:
+            return self.authenticate_istioctl_context(context, kube_config)
+
+    def authenticate_istioctl_context(self, context, kube_config) -> str:
+        istioctl_args = ""
+        if context:
+            istioctl_args += f" --context=${context} "
+        if kube_config:
             try:
-                open(k8s_certificate_ca, "r")
+                open(kube_config, "r")
             except FileNotFoundError:
-                t = k8s_certificate_ca
-                k8s_certificate_ca = tempfile.mkstemp(text=True)
-                with open(k8s_certificate_ca[1], "w") as f:
+                t = kube_config
+                kube_config = tempfile.mkstemp(text=True)
+                with open(kube_config[1], "w") as f:
                     f.write(t)
-                k8s_certificate_ca = k8s_certificate_ca[1]
+                self.kube_config = kube_config[1]
+                istioctl_args += f" --kubeconfig {self.kube_config} "
             except OSError as e:
-                if e.errno == 36:  # File name too long
-                    t = k8s_certificate_ca
-                    k8s_certificate_ca = tempfile.mkstemp(text=True)
-                    with open(k8s_certificate_ca[1], "w") as f:
+                if e.errno == 36:
+                    t = kube_config
+                    kube_config = tempfile.mkstemp(text=True)
+                    with open(kube_config[1], "w") as f:
                         f.write(t)
-                    k8s_certificate_ca = k8s_certificate_ca[1]
+                    self.kube_config = kube_config[1]
+                    istioctl_args += f" --kubeconfig {self.kube_config} "
                 else:
-                    pass  # TODO: raise error
-        k8s_certificate = self.spec.get("k8s_certificate")
-        if k8s_certificate:
+                    pass
+        return istioctl_args
+
+    def authenticate_kubectl(self) -> str:
+        """
+        Authenticate kubectl binary using the method specified in specs
+
+        First try to use `contex` and `kube_config` files, if not defined then
+        try to use direct k8s authentication using token, API server endpoint and token.
+        If not defined then try using GKE specs and if not defined then try using
+        AKS specs.
+        """
+        context = self.spec.get("context")
+        kube_config = self.spec.get("kube_config")
+        if context or kube_config:
+            return self.authenticate_kubectl_context(context, kube_config)
+        k8s = self.spec.get("k8s", {})
+        if k8s and type(k8s) == dict:
+            return self.authenticate_kubectl_k8s(k8s)
+        gke = self.spec.get("gke", {})
+        if gke and type(gke) == dict:
+            return self.authenticate_kubectl_gke(gke)
+        aks = self.spec.get("aks", {})
+        if aks and type(aks) == dict:
+            return self.authenticate_kubectl_aks(aks)
+
+    def authenticate_kubectl_context(self, context, kube_config) -> str:
+        kubectl_args = ""
+        if context:
+            kubectl_args += f" --context=${context} "
+        if kube_config:
             try:
-                open(k8s_certificate, "r")
+                open(kube_config, "r")
             except FileNotFoundError:
-                t = k8s_certificate
-                k8s_certificate = tempfile.mkstemp(text=True)
-                with open(k8s_certificate[1], "w") as f:
+                t = kube_config
+                kube_config = tempfile.mkstemp(text=True)
+                with open(kube_config[1], "w") as f:
                     f.write(t)
-                k8s_certificate = k8s_certificate[1]
+                self.kube_config = kube_config[1]
             except OSError as e:
                 if e.errno == 36:
-                    t = k8s_certificate
-                    k8s_certificate = tempfile.mkstemp(text=True)
-                    with open(k8s_certificate[1], "w") as f:
+                    t = kube_config
+                    kube_config = tempfile.mkstemp(text=True)
+                    with open(kube_config[1], "w") as f:
                         f.write(t)
-                    k8s_certificate = k8s_certificate[1]
+                    self.kube_config = kube_config[1]
                 else:
                     pass
-        k8s_client_key = self.spec.get("k8s_client_key")
-        if k8s_client_key:
+
+        if self.kube_config:
+            os.environ["KUBECONFIG"] = self.kube_config
+        return kubectl_args
+
+    def authenticate_kubectl_k8s(self, k8s: dict) -> str:
+        kubectl_args = ""
+        certificate_ca = k8s.get("certificate_ca")
+        if certificate_ca:
             try:
-                open(k8s_client_key, "r")
+                open(certificate_ca, "r")
             except FileNotFoundError:
-                t = k8s_client_key
-                k8s_client_key = tempfile.mkstemp(text=True)
-                with open(k8s_client_key[1], "w") as f:
+                t = certificate_ca
+                certificate_ca = tempfile.mkstemp(text=True)
+                with open(certificate_ca[1], "w") as f:
                     f.write(t)
-                k8s_client_key = k8s_client_key[1]
+                self.certificate_ca = certificate_ca[1]
+            except OSError as e:
+                if e.errno == 36:  # File name too long
+                    t = certificate_ca
+                    certificate_ca = tempfile.mkstemp(text=True)
+                    with open(certificate_ca[1], "w") as f:
+                        f.write(t)
+                    self.certificate_ca = certificate_ca[1]
+                else:
+                    pass  # TODO: raise error
+        certificate = k8s.get("certificate")
+        if certificate:
+            try:
+                open(certificate, "r")
+            except FileNotFoundError:
+                t = certificate
+                certificate = tempfile.mkstemp(text=True)
+                with open(certificate[1], "w") as f:
+                    f.write(t)
+                self.certificate = certificate[1]
             except OSError as e:
                 if e.errno == 36:
-                    t = k8s_client_key
-                    k8s_client_key = tempfile.mkstemp(text=True)
-                    with open(k8s_client_key[1], "w") as f:
+                    t = certificate
+                    certificate = tempfile.mkstemp(text=True)
+                    with open(certificate[1], "w") as f:
                         f.write(t)
-                    k8s_client_key = k8s_client_key[1]
+                    self.certificate = certificate[1]
                 else:
                     pass
-        k8s_kube_config = self.spec.get("k8s_kube_config")
-        if k8s_kube_config:
+        client_key = k8s.get("client_key")
+        if client_key:
             try:
-                open(k8s_kube_config, "r")
+                open(client_key, "r")
             except FileNotFoundError:
-                t = k8s_kube_config
-                k8s_kube_config = tempfile.mkstemp(text=True)
-                with open(k8s_kube_config[1], "w") as f:
+                t = client_key
+                client_key = tempfile.mkstemp(text=True)
+                with open(client_key[1], "w") as f:
                     f.write(t)
-                k8s_kube_config = k8s_kube_config[1]
+                self.client_key = client_key[1]
             except OSError as e:
                 if e.errno == 36:
-                    t = k8s_kube_config
-                    k8s_kube_config = tempfile.mkstemp(text=True)
-                    with open(k8s_kube_config[1], "w") as f:
+                    t = client_key
+                    client_key = tempfile.mkstemp(text=True)
+                    with open(client_key[1], "w") as f:
                         f.write(t)
-                    k8s_kube_config = k8s_kube_config[1]
+                    self.client_key = client_key[1]
                 else:
                     pass
-        server = self.spec.get("server")
-        token = self.spec.get("token")
-        config_kind = config.get("kind", "Kustomize")
-        kubectl_args = ""
-        path = config.get("path")
-        if path is None:
-            raise errors.ResourcePublishError(
-                "You need to specify path for command execution"
-            )
-        use_gcloud = False
-        if self.spec.get("use_gcloud") == True:
-            use_gcloud = True
-            cluster_name = self.spec.get("cluster_name")
-            if cluster_name is None:
-                raise errors.ActionError(
-                    "use_gcloud is set to True but cluster_name is not set"
-                )
-            project_name = self.spec.get("project_name")
-            if project_name is None:
-                raise errors.ActionError(
-                    "use_gcloud is set to True but project_name is not set"
-                )
-            cluster_region = self.spec.get("cluster_region")
-            if cluster_region is None:
-                cluster_zone = self.spec.get("cluster_zone")
-                if cluster_zone is None:
-                    raise errors.ActionError(
-                        "neither cluster_region nor cluster_zone is set"
-                    )
-                try:
-                    gcloud_command = f"gcloud container clusters get-credentials {cluster_name} --zone {cluster_zone} --project {project_name}"
-                    os.environ["KUBECONFIG"] = os.path.join(
-                        self.__space.get_hash_dir(),
-                        f"{cluster_name}-{project_name}-config",
-                    )
-                    resources.Resource.execute(gcloud_command, path)
-                except CalledProcessError as e:
-                    raise errors.ActionError(e)
-            else:
-                try:
-                    gcloud_command = f"gcloud container clusters get-credentials {cluster_name} --region {cluster_region} --project {project_name}"
-                    os.environ["KUBECONFIG"] = os.path.join(
-                        self.__space.get_hash_dir(),
-                        f"{cluster_name}-{project_name}-config",
-                    )
-                    resources.Resource.execute(gcloud_command, path)
-                except CalledProcessError as e:
-                    raise errors.ActionError(e)
-        use_az = False
-        if self.spec.get("use_az") == True:
-            use_az = True
-            cluster_name = self.spec.get("cluster_name")
-            if cluster_name is None:
-                raise errors.ActionError(
-                    "use_az is set to True but cluster_name is not set"
-                )
-            subscription_id = self.spec.get("subscription_id")
-            if subscription_id is None:
-                raise errors.ActionError(
-                    "use_az is set to True but subscription_id is not set"
-                )
-            resource_group = self.spec.get("resource_group")
-            if resource_group is None:
-                raise errors.ActionError(
-                    "use_az is set to True but resource_group is not set"
+        server = k8s.get("server")
+        token = k8s.get("token")
+        if certificate_ca and certificate and client_key:
+            kubectl_args = f" --certificate-authority={certificate_ca} --client-certificate={certificate} --client-key={client_key} "
+        if server:
+            kubectl_args += f" --server={server} "
+        if token:
+            kubectl_args += f" --token={token} "
+        return kubectl_args
+
+    def authenticate_kubectl_gke(self, gke: dict) -> str:
+        cluster_name = gke.get("cluster_name")
+        if cluster_name is None:
+            raise errors.ActionError("gke is set but gke.cluster_name is not set")
+        project_id = gke.get("project_id")
+        if project_id is None:
+            raise errors.ActionError("gke is set but gke.project_id is not set")
+        region = gke.get("region")
+        if region is None:
+            zone = gke.get("zone")
+            if zone is None:
+                raise errors.ActionError("neither region nor zone is set under gke")
+            try:
+                gcloud_command = f"gcloud container clusters get-credentials {cluster_name} --zone {zone} --project {project_id}"
+                os.environ["KUBECONFIG"] = os.path.join(
+                    self.__space.get_hash_dir(),
+                    f"{cluster_name}-{zone}-{project_id}-config",
                 )
+                resources.Resource.execute(gcloud_command, ".")
+            except CalledProcessError as e:
+                raise errors.ActionError(e)
+        else:
             try:
-                az_command = f"az aks get-credentials --name {cluster_name} --resource-group {resource_group} --subscription {subscription_id} --overwrite-existing"
+                gcloud_command = f"gcloud container clusters get-credentials {cluster_name} --region {region} --project {project_id}"
                 os.environ["KUBECONFIG"] = os.path.join(
                     self.__space.get_hash_dir(),
-                    f"{cluster_name}-{resource_group}-{subscription_id}-config",
+                    f"{cluster_name}-{region}-{project_id}-config",
                 )
-                resources.Resource.execute(az_command, path)
+                resources.Resource.execute(gcloud_command, ".")
             except CalledProcessError as e:
                 raise errors.ActionError(e)
-        if not use_gcloud and not use_az:
-            if context:
-                kubectl_args = f" --context={context} "
-            else:
-                if k8s_certificate_ca and k8s_certificate and k8s_client_key:
-                    kubectl_args = f" --certificate-authority={k8s_certificate_ca} --client-certificate={k8s_certificate} --client-key={k8s_client_key} "
-                if server:
-                    kubectl_args += f" --server={server} "
-                if token:
-                    kubectl_args += f" --token={token} "
-                if k8s_kube_config:
-                    kubectl_args += f" --kubeconfig={k8s_kube_config} "
-        if config_kind not in ["Kustomize", "DockerImage"]:
-            raise errors.ResourceDeployError(
-                "Config kind must be either 'Kustomize' or 'DockerImage'"
+        return ""
+
+    def authenticate_kubectl_aks(self, aks: dict) -> str:
+        cluster_name = aks.get("cluster_name")
+        if cluster_name is None:
+            raise errors.ActionError("aks is set but aks.cluster_name is not set")
+        subscription_id = aks.get("subscription_id")
+        if subscription_id is None:
+            raise errors.ActionError("aks is set but aks.subscription_id is not set")
+        resource_group = aks.get("resource_group")
+        if resource_group is None:
+            raise errors.ActionError("aksis set but aks.resource_group is not set")
+        try:
+            az_command = f"az aks get-credentials --name {cluster_name} --resource-group {resource_group} --subscription {subscription_id} --overwrite-existing"
+            os.environ["KUBECONFIG"] = os.path.join(
+                self.__space.get_hash_dir(),
+                f"{cluster_name}-{resource_group}-{subscription_id}-config",
             )
-        port = config.get("port")
-        if port:
-            kubectl_args += f"--port={port}"
-        service_account = config.get("service_account")
-        if service_account:
-            kubectl_args += f"--serviceaccount={service_account}"
-        if config_kind == "Kustomize" and name != "create_namespace":
-            manifests_path = config.get("manifests_path")
-            if manifests_path is None:
-                raise errors.ResourceError(f"No manifests path supplied for K8S target")
-            if name == "deploy":
-                kubectl_command = (
-                    f"{kubectl_binary} apply {kubectl_args} -f {manifests_path}"
-                )
-            elif name == "test" and config.get("diff") is not True:
-                kubectl_command = f"{kubectl_binary} apply {kubectl_args} --dry-run=server -f {manifests_path}"
-            elif name == "test" and config.get("diff") is True:
-                kubectl_command = (
-                    f"{kubectl_binary} diff {kubectl_args} -f {manifests_path}"
-                )
-        elif config_kind == "DockerImage":
-            image_url = config.get("image_url")
-            if image_url is None:
-                raise errors.ResourceError("No image URL supplied for K8S target")
-            pod_name = config.get("pod_name", name)
+            resources.Resource.execute(az_command, ".")
+        except CalledProcessError as e:
+            raise errors.ActionError(e)
+        return ""
+
+    def process_kustomize(self, name: str, config: dict, kubectl_args: str):
+        kubectl_binary = config.get("kubectl", "kubectl")
+        manifests_path = config.get("manifests_path")
+        if manifests_path is None:
+            raise errors.ResourceError(f"No manifests path supplied for K8S target")
+        if name == "deploy":
             kubectl_command = (
-                f"{kubectl_binary} run {kubectl_args} --image={image_url} {pod_name}"
+                f"{kubectl_binary} apply {kubectl_args} -f {manifests_path}"
             )
-        if name == "create_namespace":
-            namespace = config.get("namespace")
-            if namespace is None:
-                raise errors.ResourceError(
-                    "k8s target: create_namespace is reqested but no namespace name is provided"
-                )
+        elif name == "test" and config.get("diff") is not True:
+            kubectl_command = f"{kubectl_binary} apply {kubectl_args} --dry-run=server -f {manifests_path}"
+        elif name == "test" and config.get("diff") is True:
             kubectl_command = (
-                f"{kubectl_binary} create namespace {kubectl_args} {namespace}"
+                f"{kubectl_binary} diff {kubectl_args} -f {manifests_path}"
             )
         try:
-            resources.Resource.execute(kubectl_command, path)
+            resources.Resource.execute(kubectl_command, config.get("path"))
         except CalledProcessError as e:
             if config.get("diff") is True and e.returncode == 1:
                 return True
-            if name == "create_namespace":
-                raise e
             raise errors.ResourceError(e.stderr.decode("UTF-8"))
         finally:
-            if k8s_certificate_ca:
-                try:
-                    os.remove(k8s_certificate_ca)
-                except Exception:
-                    pass
-            if k8s_certificate:
-                try:
-                    os.remove(k8s_certificate)
-                except Exception:
-                    pass
-            if k8s_client_key:
-                try:
-                    os.remove(k8s_client_key)
-                except Exception:
-                    pass
-            if k8s_kube_config:
-                try:
-                    os.remove(k8s_kube_config)
-                except Exception:
-                    pass
+            self.remove_temp_files()
+
+    def process_docker_image(self, name: str, config: dict, kubectl_args: str):
+        kubectl_binary = config.get("kubectl", "kubectl")
+        port = config.get("port")
+        if port:
+            kubectl_args += f"--port={port}"
+        image_url = config.get("image_url")
+        if image_url is None:
+            raise errors.ResourceError("No image_url supplied for K8S target")
+        pod_name = config.get("pod_name")
+        if pod_name is None:
+            raise errors.ResourceError("No pod_name supplied for K8S target")
+        kubectl_command = (
+            f"{kubectl_binary} run {kubectl_args} --image={image_url} {pod_name}"
+        )
+        try:
+            resources.Resource.execute(kubectl_command, config.get("path"))
+        except CalledProcessError as e:
+            raise errors.ResourceError(e.stderr.decode("UTF-8"))
+        finally:
+            self.remove_temp_files()
+
+    def process_create_namespace(self, config: dict, kubectl_args: str):
+        kubectl_binary = config.get("kubectl", "kubectl")
+        namespace = config.get("namespace")
+        if namespace is None:
+            raise errors.ResourceError(
+                "k8s target: create_namespace is reqested but no namespace name is provided"
+            )
+        kubectl_command = (
+            f"{kubectl_binary} create namespace {kubectl_args} {namespace}"
+        )
+        try:
+            resources.Resource.execute(kubectl_command, config.get("path"))
+        except CalledProcessError as e:
+            raise errors.ResourceError(e.stderr.decode("UTF-8"))
+        finally:
+            self.remove_temp_files()
+
+    def process_delete(self, config: dict, kubectl_args: str):
+        kubectl_binary = config.get("kubectl", "kubectl")
+        resource_name = config.get("resource_name")
+        if resource_name is None:
+            raise errors.ResourceError(
+                "k8s target: delete is reqested but no resource_name is provided"
+            )
+        resource_kind = config.get("resource_kind")
+        if resource_kind is None:
+            raise errors.ResourceError(
+                "k8s target: delete is reqested but no resource_kind is provided"
+            )
+        resource_namespace = config.get("resource_namespace")
+        if (
+            resource_kind != "Namespace"
+            and not resource_kind.startswith("Cluster")
+            and not resource_namespace
+        ):
+            raise errors.ResourceError(
+                f"k8s target: delete is reqested but no resource_namespace is provided and resource_kind is {resource_kind}"
+            )
+        kubectl_command = (
+            f"{kubectl_binary} delete {kubectl_args} {resource_kind} {resource_name}"
+        )
+        if resource_namespace:
+            kubectl_command += f" -n {resource_namespace}"
+        try:
+            resources.Resource.execute(kubectl_command, config.get("path"))
+        except CalledProcessError as e:
+            raise errors.ResourceError(e.stderr.decode("UTF-8"))
+        finally:
+            self.remove_temp_files()
+
+    def process_istioctl_install(self, config: dict, istioctl_args: str):
+        istioctl = config.get("istioctl")
+        if istioctl is None or type(istioctl) != resources.IstioCtl:
+            raise errors.ResourceError(
+                "config['istioctl'] should be an instance of resources.IstioCtl"
+            )
+        istio = config.get("istio", {})
+        istio_profile = istio.get("profile")
+        if istio_profile:
+            istioctl_args += f" --set profile={istio_profile}"
+        istio_config_file = istio.get("config_file")
+        if istio_config_file:
+            istioctl_args += f" -f {istio_config_file} "
+        revision = istio.get("revision")
+        if revision:
+            istioctl_args += f" -r {revision} "
+        try:
+            istioctl.install(istioctl_args)
+        except CalledProcessError as e:
+            raise errors.ResourceError(e.stderr.decode("UTF-8"))
+        finally:
+            self.remove_temp_files()
+
+    def process_istioctl_verify_install(self, config: dict, istioctl_args: str):
+        istioctl = config.get("istioctl")
+        if istioctl is None or type(istioctl) != resources.IstioCtl:
+            raise errors.ResourceError(
+                "config['istioctl'] should be an instance of resources.IstioCtl"
+            )
+        try:
+            istioctl.verify_install(istioctl_args)
+        except CalledProcessError as e:
+            if e.returncode == 1:
+                return True
+            raise errors.ResourceError(e.stderr.decode("UTF-8"))
+        finally:
+            self.remove_temp_files()
+        return False
+
+    def check_config(self, config: dict):
+        if config.get("path") is None:
+            raise errors.ResourcePublishError(
+                "You need to specify path for command execution"
+            )
+        if config.get("kind", "Kustomize") not in ["Kustomize", "DockerImage"]:
+            raise errors.ResourceDeployError(
+                "Config kind must be either 'Kustomize' or 'DockerImage'"
+            )
+
+    @hookimpl
+    def action(self, name: str, config: dict):
+        if name not in [
+            "deploy",
+            "test",
+            "create_namespace",
+            "delete",
+            "istioctl_install",
+            "istioctl_verify-install",
+        ]:
+            raise errors.TargetActionError(
+                f"Cannot run action {name} with target of type K8S"
+            )
+        kubectl_args = self.authenticate_kubectl()
+        self.check_config(config)
+        config_kind = config.get("kind", "Kustomize")
+        service_account = config.get("service_account")
+        if service_account:
+            kubectl_args += f"--serviceaccount={service_account}"
+        if name == "create_namespace":
+            return self.process_create_namespace(config, kubectl_args)
+        elif name == "delete":
+            return self.process_delete(config, kubectl_args)
+        elif name == "istioctl_install":
+            istioctl_args = self.authenticate_istioctl()
+            return self.process_istioctl_install(config, istioctl_args)
+        elif name == "istioctl_verify-install":
+            istioctl_args = self.authenticate_istioctl()
+            return self.process_istioctl_verify_install(config, istioctl_args)
+        if config_kind == "Kustomize":
+            return self.process_kustomize(name, config, kubectl_args)
+        elif config_kind == "DockerImage":
+            return self.process_docker_image(name, config, kubectl_args)
 
 
 class DockerRegistryTarget(Target):
     @hookimpl
     def init(self, config: dict, space) -> None:
         self._init(config)
         if self.kind != "DockerRegistryTarget":
             raise errors.TargetConfigError(
                 f"This target is not of kind DockerRegistry, it is of kind {self.kind}"
             )
         self.__space = space
+        self.docker_config_dir = None
 
-    @hookimpl
-    def action(self, name: str, config: dict):
-        if name != "publish":
-            raise errors.TargetActionError(
-                f"Cannot run action {name} with target of type Docker Registry"
-            )
+    def authenticate_docker(self):
         registry_url = self.spec.get("registry_url")
         if registry_url is None:
             raise errors.ResourcePublishError("No registry_url in target")
-        docker_config_dir = None
-        credHelpers = self.spec.get("credHelpers")
-        if credHelpers:
-            docker_config_dir = tempfile.mkdtemp()
-            with open(os.path.join(docker_config_dir, "config.json"), "w") as f:
-                out = {"credHelpers": credHelpers}
-                json.dump(out, f)
-        docker_config = self.spec.get("docker_config")
+
+        docker = self.spec.get("docker", {})
+        if docker and type(docker) == dict:
+            return self.authenticate_docker_config(docker)
+        gcr = self.spec.get("gcr", {})
+        if gcr and type(gcr) == dict:
+            return self.authenticate_docker_gcr(gcr)
+        acr = self.spec.get("acr", {})
+        if acr and type(acr) == dict:
+            return self.authenticate_docker_acr(acr)
+
+    def authenticate_docker_config(self, docker: dict):
+        docker_config = docker.get("config")
         if docker_config:
-            docker_config_dir = tempfile.mkdtemp()
-            with open(os.path.join(docker_config_dir, "config.json"), "w") as f:
+            self.docker_config_dir = tempfile.mkdtemp()
+            with open(os.path.join(self.docker_config_dir, "config.json"), "w") as f:
                 f.write(docker_config)
-        config_kind = config.get("kind", "DockerFile")
-        if config_kind not in ["DockerFile", "DockerImage"]:
-            raise errors.ResourcePublishError(
-                "target connfig kind must be either 'DockerFile' or 'DockerImage'"
-            )
-        service_account = self.spec.get("service_account")
-        login_command = None
+        else:
+            credHelpers = docker.get("credHelpers")
+            if credHelpers:
+                self.docker_config_dir = tempfile.mkdtemp()
+                with open(
+                    os.path.join(self.docker_config_dir, "config.json"), "w"
+                ) as f:
+                    out = {"credHelpers": credHelpers}
+                    json.dump(out, f)
+        if self.docker_config_dir:
+            os.environ["DOCKER_CONFIG"] = self.docker_config_dir
+
+    def authenticate_docker_gcr(self, gcr: dict):
+        service_account = gcr.get("service_account")
+        registry_url = self.spec.get("registry_url")
+        registry_host = registry_url.split("/")[0]
+        login_command = f"gcloud auth print-access-token | docker login -u oauth2accesstoken --password-stdin https://{registry_host}"
+        self.docker_config_dir = os.path.join(
+            self.__space.get_hash_dir(),
+            f"{registry_host}-local-docker-config",
+        )
         if service_account:
-            registry_host = registry_url.split("/")[0]
+            self.docker_config_dir = os.path.join(
+                self.__space.get_hash_dir(),
+                f"{registry_host}-{service_account}-docker-config",
+            )
             login_command = f"gcloud auth print-access-token --impersonate-service-account {service_account} | docker login -u oauth2accesstoken --password-stdin https://{registry_host}"
-        use_az = self.spec.get("use_az")
-        if use_az == True:
-            registry_name = self.spec.get("registry_name")
-            if registry_name is None:
-                raise errors.ActionError("use_az is True but registry_name is not set")
-            subscription_id = self.spec.get("subscription_id")
-            if subscription_id is None:
-                raise errors.ActionError(
-                    "use_az is True but subscription_id is not set"
-                )
-            login_command = (
-                f"az acr login --subscription {subscription_id} --name {registry_name}"
+        try:
+            os.makedirs(self.docker_config_dir, exist_ok=True)
+            os.environ["DOCKER_CONFIG"] = self.docker_config_dir
+            resources.Resource.execute(login_command, ".")
+        except CalledProcessError as e:
+            raise errors.ResourcePublishError(e.stderr.decode("UTF-8"))
+
+    def authenticate_docker_acr(self, acr: dict):
+        registry_name = acr.get("registry_name")
+        if registry_name is None:
+            raise errors.ActionError("acr is set but acr.registry_name is not set")
+        subscription_id = acr.get("subscription_id")
+        if subscription_id is None:
+            raise errors.ActionError("acr is set but acr.subscription_id is not set")
+        login_command = (
+            f"az acr login --subscription {subscription_id} --name {registry_name}"
+        )
+        self.docker_config_dir = os.path.join(
+            self.__space.get_hash_dir(),
+            f"{registry_name}-{subscription_id}-docker-config",
+        )
+        try:
+            os.makedirs(self.docker_config_dir, exist_ok=True)
+            os.environ["DOCKER_CONFIG"] = self.docker_config_dir
+            resources.Resource.execute(login_command, ".")
+        except CalledProcessError as e:
+            raise errors.ResourcePublishError(e.stderr.decode("UTF-8"))
+
+    def check_config(self, config: dict):
+        if config.get("path") is None:
+            raise errors.ResourcePublishError(
+                "You need to specify path for command execution"
             )
-        if config_kind == "DockerFile":
-            image_name = config.get("image_name")
-            if image_name is None:
-                raise errors.ResourcePublishError("You need to specify image name")
-            image_file = config.get("image_file")
-            docker_file = config.get("docker_file", "Dockerfile")
-            docker_file_path = config.get("docker_file_path", ".")
-            image_url = f"{registry_url}/{image_name}"
-            tag_command = None
-            if docker_config_dir:
-                if image_file:
-                    build_command = f"docker image load -i {image_file}"
-                    tag_command = f"docker tag {image_name} {image_url}"
-                else:
-                    build_command = f"docker --config={docker_config_dir} build -t {image_url} {docker_file_path} -f {docker_file}"
-                publish_command = (
-                    f"docker --config={docker_config_dir} push {image_url}"
-                )
+        if config.get("kind", "DockerFile") not in ["DockerFile", "DockerImage"]:
+            raise errors.ResourceDeployError(
+                "Config kind must be either 'DockerFile' or 'DockerImage'"
+            )
+
+    def process_docker_file(self, config: dict):
+        image_name = config.get("image_name")
+        if image_name is None:
+            raise errors.ResourcePublishError("You need to specify image name")
+        registry_url = self.spec.get("registry_url")
+        path = config.get("path")
+        docker_file = config.get("docker_file", "Dockerfile")
+        docker_file_path = config.get("docker_file_path", path)
+        image_url = f"{registry_url}/{image_name}"
+        build_command = (
+            f"docker build -t {image_url} {docker_file_path} -f {docker_file}"
+        )
+        publish_command = f"docker push {image_url}"
+        inspect_command = "docker inspect --format='{{.RepoDigests}}' " + image_url
+        try:
+            resources.Resource.execute(build_command, path)
+            resources.Resource.execute(publish_command, path)
+            p = resources.Resource.execute(inspect_command, path)
+            image_digest = p.stdout.decode("UTF-8").replace("[", "").replace("]", "")
+            image_digests = image_digest.split(" ")
+            docker_image_name = image_name.split(":")[0]
+            image_digest = ""
+            if len(image_digests) == 1:
+                if len(image_digests[0].split("@")) <= 1:
+                    raise errors.ResourceError(
+                        f"images digest {image_digests[0]} has no @"
+                    )
+                image_digest = image_digests[0].split("@")[1].strip()
             else:
-                if image_file:
-                    build_command = f"docker image load -i {image_file}"
-                    tag_command = f"docker tag {image_name} {image_url}"
-                else:
-                    build_command = f"docker build -t {image_url} {docker_file_path} -f {docker_file}"
-                publish_command = f"docker push {image_url}"
-            path = config.get("path")
-            if path is None:
-                raise errors.ResourcePublishError(
-                    "You need to specify path for command execution"
+                for digest in image_digests:
+                    if len(digest.split("@")) <= 1:
+                        raise errors.ResourceError(f"images digest {digest} has no @")
+                    host_part = digest.split("@")[0]
+                    if host_part == f"{registry_url}/{docker_image_name}":
+                        image_digest = digest.split("@")[1].strip()
+            if image_digest == "":
+                raise errors.ResourceError(
+                    f"Cannot find image digest for image {image_url} in {image_digests}"
                 )
-            try:
-                if login_command:
-                    resources.Resource.execute(login_command, path)
-                resources.Resource.execute(build_command, path)
-                if tag_command:
-                    resources.Resource.execute(tag_command, path)
-                resources.Resource.execute(publish_command, path)
-                return image_url
-            except CalledProcessError as e:
-                raise errors.ResourcePublishError(e.stderr.decode("UTF-8"))
+            image_url_digest = f"{registry_url}/{docker_image_name}@{image_digest}"
+            return {"image_url": image_url, "image_url_digest": image_url_digest}
+        except CalledProcessError as e:
+            raise errors.ResourcePublishError(e.stderr.decode("UTF-8"))
+
+    def process_docker_image(self, config):
+        image_name = config.get("image_name")
+        if image_name is None:
+            raise errors.ResourcePublishError("You need to specify image name")
+        registry_url = self.spec.get("registry_url")
+        image_file = config.get("image_file")
+        image_url = f"{registry_url}/{image_name}"
+        build_command = f"docker image load -i {image_file}"
+        tag_command = f"docker tag {image_name} {image_url}"
+        publish_command = f"docker push {image_url}"
+        path = config.get("path")
+        try:
+            resources.Resource.execute(build_command, path)
+            resources.Resource.execute(tag_command, path)
+            resources.Resource.execute(publish_command, path)
+            return image_url
+        except CalledProcessError as e:
+            raise errors.ResourcePublishError(e.stderr.decode("UTF-8"))
+
+    def process_inspect(self, config):
+        image_name = config.get("image_name")
+        if image_name is None:
+            raise errors.ResourcePublishError("You need to specify image name")
+        registry_url = self.spec.get("registry_url")
+        image_url = f"{registry_url}/{image_name}"
+        inspect_command = f"docker manifest inspect {image_url}"
+        path = config.get("path")
+        try:
+            p = resources.Resource.execute(inspect_command, path)
+            data = json.loads(p.stdout.decode("UTF-8"))
+            return {"found": True, "data": data}
+        except CalledProcessError as e:
+            if e.returncode == 1:
+                return {"found": False, "data": {}}
+            raise errors.ResourceError(
+                f"Error inpsecting docker image {image_url} : {e.stderr.decode('utf-8')}"
+            )
+
+    @hookimpl
+    def action(self, name: str, config: dict):
+        if name not in ["publish", "inspect"]:
+            raise errors.TargetActionError(
+                f"Cannot run action {name} with target of type Docker Registry"
+            )
+        self.authenticate_docker()
+        self.check_config(config)
+        if name == "inspect":
+            return self.process_inspect(config)
+        else:
+            config_kind = config.get("kind", "DockerFile")
+            if config_kind == "DockerFile":
+                return self.process_docker_file(config)
+            elif config_kind == "DockerImage":
+                return self.process_docker_image(config)
 
 
 class DOFunctionTarget(Target):
     def __verify_function(
         self, package_name: str, function_name: str, config: dict
     ) -> bool:
         packages = config.get("packages", [])
```

### Comparing `hashkern-0.3.3/src/hash/store/base.py` & `hashkern-0.4.0/src/hash/store/base.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hash/utils.py` & `hashkern-0.4.0/src/hash/utils.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.3/src/hashkern.egg-info/PKG-INFO` & `hashkern-0.4.0/src/hashkern.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashkern
-Version: 0.3.3
+Version: 0.4.0
 Summary: A tool for managing resources in a mono repository
 Author: Mouhsen Ibrahim
 Author-email: mouhsen.ibrahim@gmail.com
 Project-URL: Documentation, https://hash-kern.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://gitlab.com/hash-platform/hashkern
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -53,27 +53,28 @@
 ```bash
 pip install hashkern
 ```
 
 Then you can use the CLI like this
 
 ```bash
-> hashc
-usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] {build,test,publish,deploy} ...
+> haks
+usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] [--plan PLAN] {build,test,publish,deploy,hash,render,clear,version} ...
 
 A tool to build resources based on their hash and type
 
 positional arguments:
-  {build,test,publish,deploy}
+  {build,test,publish,deploy,hash,render,clear,version}
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   --storage STORAGE     The storage system used default is Local File
   --config CONFIG       The configuration file default is config.ini
   --env ENV             An environment to run the action in it
+  --plan PLAN           Only do a plan and save it to this file
 ```
 
 ### Install from source
 
 Install the required packages to clone the code, create virtual env and run the tests with make
 
 ```bash
@@ -122,35 +123,37 @@
 ```
 
 Print the help for the client with this command
 
 ```bash
 > python src/client/main.py
 
-usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] {build,test,publish,deploy} ...
+usage: hash [-h] [--storage STORAGE] [--config CONFIG] [--env ENV] [--plan PLAN] {build,test,publish,deploy,hash,render,clear,version} ...
 
 A tool to build resources based on their hash and type
 
 positional arguments:
-  {build,test,publish,deploy}
+  {build,test,publish,deploy,hash,render,clear,version}
 
 optional arguments:
   -h, --help            show this help message and exit
   --storage STORAGE     The storage system used default is Local File
   --config CONFIG       The configuration file default is config.ini
   --env ENV             An environment to run the action in it
+  --plan PLAN           Only do a plan and save it to this file
 ```
 
 The client takes three options:
 
 * `--storage` this one is used to select a storage backend for the state, the options for storage backend are in the config file.
 * `--config` this option is used to select a config file for storage backends, it is an INI file, its default value is `config.ini`
 * `--env` this option is used to select the environment name where the action will be executed, its default value is `None`, this
   value is acceptabe for some actions on some resources and it is not acceptable for some other actions, the environment
   must exist in the repository otherwise we get an error.
+* `--plan` this option is used to only run the plan and save it to the file specified in the option, it defaults to false.
 
 The format for config file is as follows:
 
 ```ini
 [LocalFile]
 output = hash_test/storage
 organization = hashio
```

### Comparing `hashkern-0.3.3/src/hashkern.egg-info/SOURCES.txt` & `hashkern-0.4.0/src/hashkern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

