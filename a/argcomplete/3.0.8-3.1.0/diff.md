# Comparing `tmp/argcomplete-3.0.8.tar.gz` & `tmp/argcomplete-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argcomplete-3.0.8.tar", last modified: Sun Apr 23 21:45:39 2023, max compression
+gzip compressed data, was "argcomplete-3.1.0.tar", last modified: Sat Jun 10 20:52:29 2023, max compression
```

## Comparing `argcomplete-3.0.8.tar` & `argcomplete-3.1.0.tar`

### file list

```diff
@@ -1,51 +1,71 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.244956 argcomplete-3.0.8/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       35 2021-06-26 14:08:42.000000 argcomplete-3.0.8/Authors.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    12542 2023-04-23 21:45:09.000000 argcomplete-3.0.8/Changes.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10174 2021-06-26 14:08:42.000000 argcomplete-3.0.8/LICENSE.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       79 2021-06-26 14:08:42.000000 argcomplete-3.0.8/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      387 2023-03-21 01:42:51.000000 argcomplete-3.0.8/NOTICE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16463 2023-04-23 21:45:39.245201 argcomplete-3.0.8/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14856 2023-04-23 21:34:49.000000 argcomplete-3.0.8/README.rst
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.228992 argcomplete-3.0.8/argcomplete/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      693 2023-03-21 01:39:54.000000 argcomplete-3.0.8/argcomplete/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2140 2023-03-04 23:22:21.000000 argcomplete-3.0.8/argcomplete/_check_console_script.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2600 2023-03-17 18:26:27.000000 argcomplete-3.0.8/argcomplete/_check_module.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.233792 argcomplete-3.0.8/argcomplete/bash_completion.d/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5422 2023-03-29 02:42:12.000000 argcomplete-3.0.8/argcomplete/bash_completion.d/python-argcomplete
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3980 2023-03-29 02:42:12.000000 argcomplete-3.0.8/argcomplete/completers.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      112 2023-03-19 19:40:27.000000 argcomplete-3.0.8/argcomplete/exceptions.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    26975 2023-03-29 02:42:12.000000 argcomplete-3.0.8/argcomplete/finders.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      866 2023-03-19 19:40:27.000000 argcomplete-3.0.8/argcomplete/io.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2131 2023-03-21 01:39:33.000000 argcomplete-3.0.8/argcomplete/lexers.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.235956 argcomplete-3.0.8/argcomplete/packages/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-19 19:40:27.000000 argcomplete-3.0.8/argcomplete/packages/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15846 2023-03-19 19:40:27.000000 argcomplete-3.0.8/argcomplete/packages/_argparse.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    12766 2023-03-19 19:40:27.000000 argcomplete-3.0.8/argcomplete/packages/_shlex.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-17 19:10:26.000000 argcomplete-3.0.8/argcomplete/py.typed
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7012 2023-04-23 21:34:49.000000 argcomplete-3.0.8/argcomplete/shell_integration.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.232278 argcomplete-3.0.8/argcomplete.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16463 2023-04-23 21:45:39.000000 argcomplete-3.0.8/argcomplete.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1059 2023-04-23 21:45:39.000000 argcomplete-3.0.8/argcomplete.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-04-23 21:45:39.000000 argcomplete-3.0.8/argcomplete.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-04-23 21:45:19.000000 argcomplete-3.0.8/argcomplete.egg-info/not-zip-safe
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      153 2023-04-23 21:45:39.000000 argcomplete-3.0.8/argcomplete.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       12 2023-04-23 21:45:39.000000 argcomplete-3.0.8/argcomplete.egg-info/top_level.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      371 2023-04-04 02:41:07.000000 argcomplete-3.0.8/pyproject.toml
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.237830 argcomplete-3.0.8/scripts/
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     3374 2023-03-22 00:11:35.000000 argcomplete-3.0.8/scripts/activate-global-python-argcomplete
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2609 2023-03-19 19:40:27.000000 argcomplete-3.0.8/scripts/python-argcomplete-check-easy-install-script
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1997 2023-04-23 21:34:49.000000 argcomplete-3.0.8/scripts/register-python-argcomplete
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      143 2023-04-23 21:45:39.245985 argcomplete-3.0.8/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2403 2023-04-23 21:44:59.000000 argcomplete-3.0.8/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.241655 argcomplete-3.0.8/test/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-26 14:08:42.000000 argcomplete-3.0.8/test/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       31 2023-03-04 23:22:21.000000 argcomplete-3.0.8/test/inputrc
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1765 2023-03-04 23:22:21.000000 argcomplete-3.0.8/test/prog
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    59360 2023-04-23 21:44:19.000000 argcomplete-3.0.8/test/test.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3183 2023-03-17 17:41:01.000000 argcomplete-3.0.8/test/test_contrib_shells.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.243813 argcomplete-3.0.8/test/test_package/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-04 23:22:21.000000 argcomplete-3.0.8/test/test_package/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      299 2023-03-04 23:22:21.000000 argcomplete-3.0.8/test/test_package/setup.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       94 2023-03-04 23:22:21.000000 argcomplete-3.0.8/test/test_package/test_module.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:45:39.244498 argcomplete-3.0.8/test/test_package/test_package/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      289 2023-03-04 23:22:21.000000 argcomplete-3.0.8/test/test_package/test_package/__init__.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866948 argcomplete-3.1.0/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.857466 argcomplete-3.1.0/.github/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       18 2022-08-21 15:59:43.000000 argcomplete-3.1.0/.github/FUNDING.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.857724 argcomplete-3.1.0/.github/workflows/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      924 2023-04-22 14:28:37.000000 argcomplete-3.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      474 2023-03-18 19:32:22.000000 argcomplete-3.1.0/.gitignore
+-rw-r--r--   0 kislyuk    (501) staff       (20)       35 2016-06-14 14:20:26.000000 argcomplete-3.1.0/Authors.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)    12880 2023-06-10 20:52:11.000000 argcomplete-3.1.0/Changes.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10174 2016-06-14 14:20:26.000000 argcomplete-3.1.0/LICENSE.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)       79 2022-08-21 15:59:43.000000 argcomplete-3.1.0/MANIFEST.in
+-rw-r--r--   0 kislyuk    (501) staff       (20)      766 2023-05-07 04:23:05.000000 argcomplete-3.1.0/Makefile
+-rw-r--r--   0 kislyuk    (501) staff       (20)      387 2023-03-21 02:49:58.000000 argcomplete-3.1.0/NOTICE
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16334 2023-06-10 20:52:29.867092 argcomplete-3.1.0/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)    14690 2023-06-10 20:45:18.000000 argcomplete-3.1.0/README.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)      705 2023-03-05 19:47:13.000000 argcomplete-3.1.0/SECURITY.md
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.860163 argcomplete-3.1.0/argcomplete/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      693 2023-03-21 02:49:58.000000 argcomplete-3.1.0/argcomplete/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2719 2023-06-10 20:45:18.000000 argcomplete-3.1.0/argcomplete/_check_console_script.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2600 2023-03-18 19:32:22.000000 argcomplete-3.1.0/argcomplete/_check_module.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861117 argcomplete-3.1.0/argcomplete/bash_completion.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8165 2023-06-10 20:45:18.000000 argcomplete-3.1.0/argcomplete/bash_completion.d/_python-argcomplete
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3980 2023-03-26 15:30:13.000000 argcomplete-3.1.0/argcomplete/completers.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      112 2023-03-19 18:35:55.000000 argcomplete-3.1.0/argcomplete/exceptions.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    26975 2023-03-26 15:30:13.000000 argcomplete-3.1.0/argcomplete/finders.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      866 2023-03-19 18:46:34.000000 argcomplete-3.1.0/argcomplete/io.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2131 2023-03-21 02:49:58.000000 argcomplete-3.1.0/argcomplete/lexers.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861555 argcomplete-3.1.0/argcomplete/packages/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-19 10:11:13.000000 argcomplete-3.1.0/argcomplete/packages/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    15846 2023-03-19 18:59:55.000000 argcomplete-3.1.0/argcomplete/packages/_argparse.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    12766 2023-03-18 19:32:22.000000 argcomplete-3.1.0/argcomplete/packages/_shlex.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-18 19:32:22.000000 argcomplete-3.1.0/argcomplete/py.typed
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7012 2023-04-22 14:28:37.000000 argcomplete-3.1.0/argcomplete/shell_integration.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861020 argcomplete-3.1.0/argcomplete.egg-info/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16334 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1323 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-06-10 20:52:19.000000 argcomplete-3.1.0/argcomplete.egg-info/not-zip-safe
+-rw-r--r--   0 kislyuk    (501) staff       (20)       96 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/requires.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)       12 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/top_level.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2214 2023-06-10 20:45:18.000000 argcomplete-3.1.0/common.mk
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861786 argcomplete-3.1.0/contrib/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2888 2023-04-22 14:28:37.000000 argcomplete-3.1.0/contrib/README.rst
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.863021 argcomplete-3.1.0/docs/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       56 2023-05-06 23:05:14.000000 argcomplete-3.1.0/docs/changelog.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1162 2023-05-07 04:24:09.000000 argcomplete-3.1.0/docs/conf.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.863337 argcomplete-3.1.0/docs/examples/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      721 2022-09-14 03:21:59.000000 argcomplete-3.1.0/docs/examples/describe_github_user.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    14171 2022-08-21 15:59:43.000000 argcomplete-3.1.0/docs/fish_help_string.png
+-rw-r--r--   0 kislyuk    (501) staff       (20)      293 2023-05-06 23:04:09.000000 argcomplete-3.1.0/docs/index.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)        8 2023-05-06 23:03:19.000000 argcomplete-3.1.0/docs/toc.html
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2083 2023-06-10 20:45:18.000000 argcomplete-3.1.0/pyproject.toml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.863855 argcomplete-3.1.0/scripts/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     4710 2023-06-10 20:45:18.000000 argcomplete-3.1.0/scripts/activate-global-python-argcomplete
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     2608 2023-06-10 20:45:18.000000 argcomplete-3.1.0/scripts/python-argcomplete-check-easy-install-script
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1997 2023-04-22 14:28:37.000000 argcomplete-3.1.0/scripts/register-python-argcomplete
+-rw-r--r--   0 kislyuk    (501) staff       (20)      143 2023-06-10 20:52:29.867442 argcomplete-3.1.0/setup.cfg
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      408 2023-06-10 20:45:18.000000 argcomplete-3.1.0/setup.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866106 argcomplete-3.1.0/test/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:26.000000 argcomplete-3.1.0/test/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      139 2016-06-16 15:02:13.000000 argcomplete-3.1.0/test/__init__.pyc
+-rw-r--r--   0 kislyuk    (501) staff       (20)       31 2023-03-05 19:47:13.000000 argcomplete-3.1.0/test/inputrc
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1764 2023-06-10 20:45:18.000000 argcomplete-3.1.0/test/prog
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)    59360 2023-05-06 22:57:27.000000 argcomplete-3.1.0/test/test.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    31570 2016-10-16 02:47:39.000000 argcomplete-3.1.0/test/test.pyc
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3183 2023-03-18 19:32:22.000000 argcomplete-3.1.0/test/test_contrib_shells.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866590 argcomplete-3.1.0/test/test_package/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-05 19:47:13.000000 argcomplete-3.1.0/test/test_package/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      299 2022-09-14 03:21:59.000000 argcomplete-3.1.0/test/test_package/setup.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)       94 2022-09-14 03:21:59.000000 argcomplete-3.1.0/test/test_package/test_module.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866822 argcomplete-3.1.0/test/test_package/test_package/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      289 2022-09-14 03:21:59.000000 argcomplete-3.1.0/test/test_package/test_package/__init__.py
```

### Comparing `argcomplete-3.0.8/Changes.rst` & `argcomplete-3.1.0/Changes.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Changes for v3.1.0 (2023-06-10)
+===============================
+
+-  setup.py -> pyproject.toml migration start (#427)
+
+-  Improve user install logic in activate-global-python-argcomplete
+   (#437)
+
+-  Ensure Python 3.7 compatibility in check_console_script (#436)
+
+-  ZSH implementation fixes (#431, #433)
+
+-  Documentation improvements
+
 Changes for v3.0.8 (2023-04-23)
 ===============================
 
 -  Test suite shell wrapper: Accept OSError on exit
 
 Changes for v3.0.7 (2023-04-23)
 ===============================
```

### Comparing `argcomplete-3.0.8/LICENSE.rst` & `argcomplete-3.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/PKG-INFO` & `argcomplete-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.0.8
+Version: 3.1.0
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
@@ -28,14 +28,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.rst
 License-File: NOTICE
 
 argcomplete - Bash/zsh tab completion for argparse
 ==================================================
 *Tab complete all the things!*
@@ -54,15 +55,15 @@
 Installation
 ------------
 ::
 
     pip install argcomplete
     activate-global-python-argcomplete
 
-On Linux, you will need to run the second command with ``sudo``. See `Activating global completion`_ below for details.
+See `Activating global completion`_ below for details about the second step.
 
 Refresh your shell environment (start a new shell).
 
 Synopsis
 --------
 Add the ``PYTHON_ARGCOMPLETE_OK`` marker and a call to ``argcomplete.autocomplete()`` to your Python application as
 follows:
@@ -246,17 +247,16 @@
 
 Global completion
 -----------------
 In global completion mode, you don't have to register each argcomplete-capable executable separately. Instead, the shell
 will look for the string **PYTHON_ARGCOMPLETE_OK** in the first 1024 bytes of any executable that it's running
 completion for, and if it's found, follow the rest of the argcomplete protocol as described above.
 
-Additionally, completion is activated for scripts run as ``python <script>`` and ``python -m <module>``.
-This also works for alternate Python versions (e.g. ``python3`` and ``pypy``), as long as that version of Python has
-argcomplete installed.
+Additionally, completion is activated for scripts run as ``python <script>`` and ``python -m <module>``. If you're using
+multiple Python versions on the same system, the version being used to run the script must have argcomplete installed.
 
 .. admonition:: Bash version compatibility
 
  When using bash, global completion requires bash support for ``complete -D``, which was introduced in bash 4.2. Since
  Mac OS ships with an outdated version of Bash (3.2), you can either use zsh or install a newer version of bash using
  `Homebrew <http://brew.sh/>`_ (``brew install bash`` - you will also need to add ``/usr/local/bin/bash`` to
  ``/etc/shells``, and run ``chsh`` to change your shell). You can check the version of the running copy of bash with
@@ -271,20 +271,18 @@
 registration roules apply: namely, the script name is passed directly to ``complete``, meaning it is only tab completed
 when invoked exactly as it was registered. In the above example, ``my-python-app`` must be on the path, and the user
 must be attempting to complete it by that name. The above line alone would **not** allow you to complete
 ``./my-python-app``, or ``/path/to/my-python-app``.
 
 Activating global completion
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The script ``activate-global-python-argcomplete`` will try to install the global completion script
-``bash_completion.d/python-argcomplete`` (`see on GitHub`_) into an appropriate location on your system for both bash
-and zsh (``/etc/bash_completion.d`` and ``/usr/local/share/zsh/site-functions``). On Linux, you will need to run the
-script with sudo: ``sudo activate-global-python-argcomplete``, or run the script with ``--help`` to see other options.
-
-.. _`see on GitHub`: https://github.com/kislyuk/argcomplete/blob/master/argcomplete/bash_completion.d/python-argcomplete
+The script ``activate-global-python-argcomplete`` installs the global completion script
+`bash_completion.d/_python-argcomplete <https://github.com/kislyuk/argcomplete/blob/master/argcomplete/bash_completion.d/_python-argcomplete>`_
+into an appropriate location on your system for both bash and zsh. The specific location depends on your platform and
+whether you installed argcomplete system-wide using ``sudo`` or locally (into your user's home directory).
 
 Zsh Support
 -----------
 Argcomplete supports zsh. On top of plain completions like in bash, zsh allows you to see argparse help strings as
 completion descriptions. All shellcode included with argcomplete is compatible with both bash and zsh, so the same
 completer commands ``activate-global-python-argcomplete`` and ``eval "$(register-python-argcomplete my-python-app)"``
 work for zsh as well.
```

### Comparing `argcomplete-3.0.8/README.rst` & `argcomplete-3.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Installation
 ------------
 ::
 
     pip install argcomplete
     activate-global-python-argcomplete
 
-On Linux, you will need to run the second command with ``sudo``. See `Activating global completion`_ below for details.
+See `Activating global completion`_ below for details about the second step.
 
 Refresh your shell environment (start a new shell).
 
 Synopsis
 --------
 Add the ``PYTHON_ARGCOMPLETE_OK`` marker and a call to ``argcomplete.autocomplete()`` to your Python application as
 follows:
@@ -208,17 +208,16 @@
 
 Global completion
 -----------------
 In global completion mode, you don't have to register each argcomplete-capable executable separately. Instead, the shell
 will look for the string **PYTHON_ARGCOMPLETE_OK** in the first 1024 bytes of any executable that it's running
 completion for, and if it's found, follow the rest of the argcomplete protocol as described above.
 
-Additionally, completion is activated for scripts run as ``python <script>`` and ``python -m <module>``.
-This also works for alternate Python versions (e.g. ``python3`` and ``pypy``), as long as that version of Python has
-argcomplete installed.
+Additionally, completion is activated for scripts run as ``python <script>`` and ``python -m <module>``. If you're using
+multiple Python versions on the same system, the version being used to run the script must have argcomplete installed.
 
 .. admonition:: Bash version compatibility
 
  When using bash, global completion requires bash support for ``complete -D``, which was introduced in bash 4.2. Since
  Mac OS ships with an outdated version of Bash (3.2), you can either use zsh or install a newer version of bash using
  `Homebrew <http://brew.sh/>`_ (``brew install bash`` - you will also need to add ``/usr/local/bin/bash`` to
  ``/etc/shells``, and run ``chsh`` to change your shell). You can check the version of the running copy of bash with
@@ -233,20 +232,18 @@
 registration roules apply: namely, the script name is passed directly to ``complete``, meaning it is only tab completed
 when invoked exactly as it was registered. In the above example, ``my-python-app`` must be on the path, and the user
 must be attempting to complete it by that name. The above line alone would **not** allow you to complete
 ``./my-python-app``, or ``/path/to/my-python-app``.
 
 Activating global completion
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The script ``activate-global-python-argcomplete`` will try to install the global completion script
-``bash_completion.d/python-argcomplete`` (`see on GitHub`_) into an appropriate location on your system for both bash
-and zsh (``/etc/bash_completion.d`` and ``/usr/local/share/zsh/site-functions``). On Linux, you will need to run the
-script with sudo: ``sudo activate-global-python-argcomplete``, or run the script with ``--help`` to see other options.
-
-.. _`see on GitHub`: https://github.com/kislyuk/argcomplete/blob/master/argcomplete/bash_completion.d/python-argcomplete
+The script ``activate-global-python-argcomplete`` installs the global completion script
+`bash_completion.d/_python-argcomplete <https://github.com/kislyuk/argcomplete/blob/master/argcomplete/bash_completion.d/_python-argcomplete>`_
+into an appropriate location on your system for both bash and zsh. The specific location depends on your platform and
+whether you installed argcomplete system-wide using ``sudo`` or locally (into your user's home directory).
 
 Zsh Support
 -----------
 Argcomplete supports zsh. On top of plain completions like in bash, zsh allows you to see argparse help strings as
 completion descriptions. All shellcode included with argcomplete is compatible with both bash and zsh, so the same
 completer commands ``activate-global-python-argcomplete`` and ``eval "$(register-python-argcomplete my-python-app)"``
 work for zsh as well.
```

### Comparing `argcomplete-3.0.8/argcomplete/__init__.py` & `argcomplete-3.1.0/argcomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/_check_console_script.py` & `argcomplete-3.1.0/argcomplete/_check_console_script.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,28 +12,43 @@
 Intended to be invoked by argcomplete's global completion function.
 """
 import os
 import sys
 
 try:
     from importlib.metadata import entry_points as importlib_entry_points
+    from importlib.metadata import EntryPoint
+    use_entry_points_backport = False
 except ImportError:
     from importlib_metadata import entry_points as importlib_entry_points  # type:ignore
+    from importlib_metadata import EntryPoint # type:ignore
+    use_entry_points_backport = True
 
 from ._check_module import ArgcompleteMarkerNotFound, find
+from typing import Iterable
 
 
 def main():
     # Argument is the full path to the console script.
     script_path = sys.argv[1]
 
     # Find the module and function names that correspond to this
     # assuming it is actually a console script.
     name = os.path.basename(script_path)
-    entry_points = [ep for ep in importlib_entry_points()["console_scripts"] if ep.name == name]
+
+    entry_points : Iterable[EntryPoint] = importlib_entry_points() # type:ignore
+
+    # The importlib_metadata backport returns a tuple of entry point objects
+    # whereas the official library returns a SelectableGroups object
+    if not use_entry_points_backport:
+        entry_points = entry_points["console_scripts"] # type:ignore
+
+    entry_points = [ep for ep in entry_points \
+            if ep.name == name and ep.group == "console_scripts" ] # type:ignore
+
     if not entry_points:
         raise ArgcompleteMarkerNotFound("no entry point found matching script")
     entry_point = entry_points[0]
     module_name, function_name = entry_point.value.split(":", 1)
 
     # Check this looks like the script we really expected.
     with open(script_path) as f:
```

### Comparing `argcomplete-3.0.8/argcomplete/_check_module.py` & `argcomplete-3.1.0/argcomplete/_check_module.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/completers.py` & `argcomplete-3.1.0/argcomplete/completers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/finders.py` & `argcomplete-3.1.0/argcomplete/finders.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/io.py` & `argcomplete-3.1.0/argcomplete/io.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/lexers.py` & `argcomplete-3.1.0/argcomplete/lexers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/packages/_argparse.py` & `argcomplete-3.1.0/argcomplete/packages/_argparse.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/packages/_shlex.py` & `argcomplete-3.1.0/argcomplete/packages/_shlex.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete/shell_integration.py` & `argcomplete-3.1.0/argcomplete/shell_integration.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/argcomplete.egg-info/PKG-INFO` & `argcomplete-3.1.0/argcomplete.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.0.8
+Version: 3.1.0
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
@@ -28,14 +28,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.rst
 License-File: NOTICE
 
 argcomplete - Bash/zsh tab completion for argparse
 ==================================================
 *Tab complete all the things!*
@@ -54,15 +55,15 @@
 Installation
 ------------
 ::
 
     pip install argcomplete
     activate-global-python-argcomplete
 
-On Linux, you will need to run the second command with ``sudo``. See `Activating global completion`_ below for details.
+See `Activating global completion`_ below for details about the second step.
 
 Refresh your shell environment (start a new shell).
 
 Synopsis
 --------
 Add the ``PYTHON_ARGCOMPLETE_OK`` marker and a call to ``argcomplete.autocomplete()`` to your Python application as
 follows:
@@ -246,17 +247,16 @@
 
 Global completion
 -----------------
 In global completion mode, you don't have to register each argcomplete-capable executable separately. Instead, the shell
 will look for the string **PYTHON_ARGCOMPLETE_OK** in the first 1024 bytes of any executable that it's running
 completion for, and if it's found, follow the rest of the argcomplete protocol as described above.
 
-Additionally, completion is activated for scripts run as ``python <script>`` and ``python -m <module>``.
-This also works for alternate Python versions (e.g. ``python3`` and ``pypy``), as long as that version of Python has
-argcomplete installed.
+Additionally, completion is activated for scripts run as ``python <script>`` and ``python -m <module>``. If you're using
+multiple Python versions on the same system, the version being used to run the script must have argcomplete installed.
 
 .. admonition:: Bash version compatibility
 
  When using bash, global completion requires bash support for ``complete -D``, which was introduced in bash 4.2. Since
  Mac OS ships with an outdated version of Bash (3.2), you can either use zsh or install a newer version of bash using
  `Homebrew <http://brew.sh/>`_ (``brew install bash`` - you will also need to add ``/usr/local/bin/bash`` to
  ``/etc/shells``, and run ``chsh`` to change your shell). You can check the version of the running copy of bash with
@@ -271,20 +271,18 @@
 registration roules apply: namely, the script name is passed directly to ``complete``, meaning it is only tab completed
 when invoked exactly as it was registered. In the above example, ``my-python-app`` must be on the path, and the user
 must be attempting to complete it by that name. The above line alone would **not** allow you to complete
 ``./my-python-app``, or ``/path/to/my-python-app``.
 
 Activating global completion
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The script ``activate-global-python-argcomplete`` will try to install the global completion script
-``bash_completion.d/python-argcomplete`` (`see on GitHub`_) into an appropriate location on your system for both bash
-and zsh (``/etc/bash_completion.d`` and ``/usr/local/share/zsh/site-functions``). On Linux, you will need to run the
-script with sudo: ``sudo activate-global-python-argcomplete``, or run the script with ``--help`` to see other options.
-
-.. _`see on GitHub`: https://github.com/kislyuk/argcomplete/blob/master/argcomplete/bash_completion.d/python-argcomplete
+The script ``activate-global-python-argcomplete`` installs the global completion script
+`bash_completion.d/_python-argcomplete <https://github.com/kislyuk/argcomplete/blob/master/argcomplete/bash_completion.d/_python-argcomplete>`_
+into an appropriate location on your system for both bash and zsh. The specific location depends on your platform and
+whether you installed argcomplete system-wide using ``sudo`` or locally (into your user's home directory).
 
 Zsh Support
 -----------
 Argcomplete supports zsh. On top of plain completions like in bash, zsh allows you to see argparse help strings as
 completion descriptions. All shellcode included with argcomplete is compatible with both bash and zsh, so the same
 completer commands ``activate-global-python-argcomplete`` and ``eval "$(register-python-argcomplete my-python-app)"``
 work for zsh as well.
```

### Comparing `argcomplete-3.0.8/scripts/python-argcomplete-check-easy-install-script` & `argcomplete-3.1.0/scripts/python-argcomplete-check-easy-install-script`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright 2012-2023, Andrey Kislyuk and argcomplete contributors.
 # Licensed under the Apache License. See https://github.com/kislyuk/argcomplete for more info.
 
 """
 This script is part of the Python argcomplete package (https://github.com/kislyuk/argcomplete).
 It is used to check if an EASY-INSTALL-SCRIPT wrapper redirects to a script that contains the string
```

### Comparing `argcomplete-3.0.8/scripts/register-python-argcomplete` & `argcomplete-3.1.0/scripts/register-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/test/prog` & `argcomplete-3.1.0/test/prog`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # PYTHON_ARGCOMPLETE_OK
 """Test script used by test.TestBash."""
 
 import argparse
 import os
 import sys
```

### Comparing `argcomplete-3.0.8/test/test.py` & `argcomplete-3.1.0/test/test.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.8/test/test_contrib_shells.py` & `argcomplete-3.1.0/test/test_contrib_shells.py`

 * *Files identical despite different names*

