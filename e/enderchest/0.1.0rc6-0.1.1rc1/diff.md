# Comparing `tmp/enderchest-0.1.0rc6.tar.gz` & `tmp/enderchest-0.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.0rc6.tar", last modified: Mon May 29 14:00:36 2023, max compression
+gzip compressed data, was "enderchest-0.1.1rc1.tar", last modified: Fri Jun  9 22:57:09 2023, max compression
```

## Comparing `enderchest-0.1.0rc6.tar` & `enderchest-0.1.1rc1.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    31191 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.433473 enderchest-0.1.0rc6/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/rsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    22451 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.433473 enderchest-0.1.0rc6/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31260 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29630 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27683 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.836967 enderchest-0.1.1rc1/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/versioneer.py
```

### Comparing `enderchest-0.1.0rc6/LICENSE` & `enderchest-0.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/PKG-INFO` & `enderchest-0.1.1rc1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,62 @@
-Metadata-Version: 2.1
-Name: enderchest
-Version: 0.1.0rc6
-Summary: syncing and linking for all your Minecraft instances
-Home-page: https://github.com/OpenBagTwo/EnderChest
-Author: Gili "OpenBagTwo" Barlev
-License: GPL v3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # EnderChest
 
 [![PyPI version](https://badge.fury.io/py/enderchest.svg)](https://badge.fury.io/py/enderchest)
 ![PyPI downloads](https://img.shields.io/pypi/dm/enderchest.svg)
 
 ![Linux](https://img.shields.io/badge/GNU/Linux-000000?style=flat-square&logo=linux&logoColor=white&color=eda445)
 ![SteamOS](https://img.shields.io/badge/SteamOS-3776AB.svg?style=flat-square&logo=steamdeck&logoColor=white&color=7055c3)
 ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)
 ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=flat-square&logo=apple&logoColor=white&color=434334)
+![RaspberryPi](https://img.shields.io/badge/Raspberry%20Pi-000000?style=flat-square&logo=raspberrypi&logoColor=white&color=c51a4a)
 
 [![python](https://img.shields.io/badge/Python-3.10,3.11-3776AB.svg?style=flat&logo=python&logoColor=white&color=ffdc53&labelColor=3d7aaa)](https://www.python.org)
-![coverage](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/coverage.svg)
-![lint](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/pylint.svg)
+[![coverage](https://openbagtwo.github.io/EnderChest/dev/img/coverage.svg)](https://openbagtwo.github.io/EnderChest/dev/coverage)
+[![lint](https://openbagtwo.github.io/EnderChest/dev/img/pylint.svg)](https://openbagtwo.github.io/EnderChest/dev/lint-report.txt)
 
 
 A system for managing your minecraft installations across instances and
 installations
 
 ## In a Nutshell
 
 EnderChest is a command-line utility for selectively sharing Minecraft assets
 (configurations, mods, worlds, etc.)...
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
+### A Note On Linking
+
+Starting with Minecraft 1.20, Mojang by default
+[no longer allows worlds to load if they are or if they contain symbolic links](https://help.minecraft.net/hc/en-us/articles/16165590199181).
+While it is true that an improper symlink could cause Minecraft to write data
+to a place it shouldn't, nothing in EnderChest will ever generate a symlink whose
+target is outside of your EnderChest folder _unless you place_ a symbolic link in
+your EnderChest pointing to somewhere else (which you may want to do so that your
+screenshots, for example, point to your "My Pictures" folder).
+
+If you still have concerns about symlinks or questions about how they work,
+read through
+[this guide](https://www.makeuseof.com/tag/what-is-a-symbolic-link-what-are-its-uses-makeuseof-explains/)
+or [watch this explainer](https://www.youtube.com/watch?v=mA08E59-zo8), and if
+you still have questions, feel free to
+[open an issue](https://github.com/OpenBagTwo/EnderChest/issues/new?assignees=OpenBagTwo&labels=question&title=symlink%20question).
+
 ## Installation
 
 EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
+Note that the recommended sync protocol is
+[`rsync`](https://www.digitalocean.com/community/tutorials/how-to-use-rsync-to-sync-local-and-remote-directories), and EnderChest requires
+[version 3.2 or newer](https://dev.to/al5ina5/updating-rsync-on-macos-so-you-re-not-stuck-with-14-year-old-software-1b5i).
+However, other protocols are available if a modern `rsync` is not an option for you.
+
 The latest release can be installed from PyPI via `pip`:
 
 ```bash
 $ python -m pip install --user enderchest
 ```
 
 Full installation instructions can be found on
```

### Comparing `enderchest-0.1.0rc6/README.md` & `enderchest-0.1.1rc1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,74 @@
+Metadata-Version: 2.1
+Name: enderchest
+Version: 0.1.1rc1
+Summary: syncing and linking for all your Minecraft instances
+Home-page: https://github.com/OpenBagTwo/EnderChest
+Author: Gili "OpenBagTwo" Barlev
+License: GPL v3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # EnderChest
 
 [![PyPI version](https://badge.fury.io/py/enderchest.svg)](https://badge.fury.io/py/enderchest)
 ![PyPI downloads](https://img.shields.io/pypi/dm/enderchest.svg)
 
 ![Linux](https://img.shields.io/badge/GNU/Linux-000000?style=flat-square&logo=linux&logoColor=white&color=eda445)
 ![SteamOS](https://img.shields.io/badge/SteamOS-3776AB.svg?style=flat-square&logo=steamdeck&logoColor=white&color=7055c3)
 ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)
 ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=flat-square&logo=apple&logoColor=white&color=434334)
+![RaspberryPi](https://img.shields.io/badge/Raspberry%20Pi-000000?style=flat-square&logo=raspberrypi&logoColor=white&color=c51a4a)
 
 [![python](https://img.shields.io/badge/Python-3.10,3.11-3776AB.svg?style=flat&logo=python&logoColor=white&color=ffdc53&labelColor=3d7aaa)](https://www.python.org)
-![coverage](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/coverage.svg)
-![lint](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/pylint.svg)
+[![coverage](https://openbagtwo.github.io/EnderChest/dev/img/coverage.svg)](https://openbagtwo.github.io/EnderChest/dev/coverage)
+[![lint](https://openbagtwo.github.io/EnderChest/dev/img/pylint.svg)](https://openbagtwo.github.io/EnderChest/dev/lint-report.txt)
 
 
 A system for managing your minecraft installations across instances and
 installations
 
 ## In a Nutshell
 
 EnderChest is a command-line utility for selectively sharing Minecraft assets
 (configurations, mods, worlds, etc.)...
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
+### A Note On Linking
+
+Starting with Minecraft 1.20, Mojang by default
+[no longer allows worlds to load if they are or if they contain symbolic links](https://help.minecraft.net/hc/en-us/articles/16165590199181).
+While it is true that an improper symlink could cause Minecraft to write data
+to a place it shouldn't, nothing in EnderChest will ever generate a symlink whose
+target is outside of your EnderChest folder _unless you place_ a symbolic link in
+your EnderChest pointing to somewhere else (which you may want to do so that your
+screenshots, for example, point to your "My Pictures" folder).
+
+If you still have concerns about symlinks or questions about how they work,
+read through
+[this guide](https://www.makeuseof.com/tag/what-is-a-symbolic-link-what-are-its-uses-makeuseof-explains/)
+or [watch this explainer](https://www.youtube.com/watch?v=mA08E59-zo8), and if
+you still have questions, feel free to
+[open an issue](https://github.com/OpenBagTwo/EnderChest/issues/new?assignees=OpenBagTwo&labels=question&title=symlink%20question).
+
 ## Installation
 
 EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
+Note that the recommended sync protocol is
+[`rsync`](https://www.digitalocean.com/community/tutorials/how-to-use-rsync-to-sync-local-and-remote-directories), and EnderChest requires
+[version 3.2 or newer](https://dev.to/al5ina5/updating-rsync-on-macos-so-you-re-not-stuck-with-14-year-old-software-1b5i).
+However, other protocols are available if a modern `rsync` is not an option for you.
+
 The latest release can be installed from PyPI via `pip`:
 
 ```bash
 $ python -m pip install --user enderchest
 ```
 
 Full installation instructions can be found on
```

### Comparing `enderchest-0.1.0rc6/enderchest/cli.py` & `enderchest-0.1.1rc1/enderchest/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command-line interface"""
+import inspect
 import logging
 import os
 import sys
 from argparse import ArgumentParser, RawTextHelpFormatter
 from pathlib import Path
 from typing import Any, Protocol, Sequence
 
@@ -17,70 +18,102 @@
 _shulker_aliases = ("shulker_box", "shulkerbox", "shulker")
 _remote_aliases = tuple(
     alias + plural for alias in ("enderchest", "remote") for plural in ("s", "")
 )
 _list_aliases = ("inventory", "list")
 
 
+class Action(Protocol):
+    """Common protocol for CLI actions"""
+
+    def __call__(self, minecraft_root: Path, /) -> Any:
+        ...
+
+
 def _place(
     minecraft_root: Path,
     errors: str = "prompt",
-    cleanup: bool = False,
+    keep_broken_links: bool = False,
+    keep_stale_links: bool = False,
+    keep_level: int = 0,
     stop_at_first_failure: bool = False,
     ignore_errors: bool = False,
+    absolute: bool = False,
+    relative: bool = False,
 ) -> None:
-    """Wrapper to coalesce error-handling flags"""
+    """Wrapper sort through all the various argument groups"""
 
     if stop_at_first_failure:
         errors = "abort"
     if ignore_errors:  # elif?
         errors = "ignore"
     # else: errors = errors
-    place.place_ender_chest(minecraft_root, cleanup=cleanup, error_handling=errors)
+
+    if absolute is True:
+        # technically we get this for free already
+        relative = False
+
+    if keep_level > 0:
+        keep_stale_links = True
+    if keep_level > 1:
+        keep_broken_links = True
+
+    place.place_ender_chest(
+        minecraft_root,
+        keep_broken_links=keep_broken_links,
+        keep_stale_links=keep_stale_links,
+        error_handling=errors,
+        relative=relative,
+    )
 
 
 def _craft_shulker_box(minecraft_root: Path, name: str | None = None, **kwargs):
     """Wrapper to handle the fact that name is a required argument"""
     assert name  # it's required by the parser, so this should be fine
     craft.craft_shulker_box(minecraft_root, name, **kwargs)
 
 
+def _list_instance_boxes(
+    minecraft_root: Path, instance_name: str | None = None, **kwargs
+):
+    """Wrapper to handle the fact that name is a required argument"""
+    assert instance_name  # it's required by the parser, so this should be fine
+    gather.get_shulker_boxes_matching_instance(minecraft_root, instance_name, **kwargs)
+
+
 def _list_shulker_box(
     minecraft_root: Path, shulker_box_name: str | None = None, **kwargs
 ):
     """Wrapper to handle the fact that name is a required argument"""
     assert shulker_box_name  # it's required by the parser, so this should be fine
-    gather.load_shulker_box_matches(minecraft_root, shulker_box_name, **kwargs)
+    gather.get_instances_matching_shulker_box(
+        minecraft_root, shulker_box_name, **kwargs
+    )
 
 
 def _update_ender_chest(
     minecraft_root: Path,
     official: bool | None = None,
     mmc: bool | None = None,
     **kwargs,
 ):
     """Wrapper to resolve the official vs. MultiMC flag"""
     if mmc:
         official = False
     gather.update_ender_chest(minecraft_root, official=official, **kwargs)
 
 
-def _open(minecraft_root, **kwargs):
+def _open(minecraft_root: Path, verbosity: int = 0, **kwargs):
     """Router for open verb"""
-    remote.sync_with_remotes(minecraft_root, "pull", **kwargs)
+    remote.sync_with_remotes(minecraft_root, "pull", verbosity=verbosity, **kwargs)
 
 
-def _close(minecraft_root, **kwargs):
+def _close(minecraft_root: Path, verbosity: int = 0, **kwargs):
     """Router for close verb"""
-    remote.sync_with_remotes(minecraft_root, "push", **kwargs)
-
-
-class Action(Protocol):
-    def __call__(self, minecraft_root: Path, /) -> Any:
-        ...
+    remote.sync_with_remotes(minecraft_root, "push", verbosity=verbosity, **kwargs)
 
 
 ACTIONS: tuple[tuple[tuple[str, ...], str, Action], ...] = (
     # action names (first one is canonical), action description, action method
     (
         sum(((verb, verb + " enderchest") for verb in _create_aliases), ()),
         "create and configure a new EnderChest installation",
@@ -125,24 +158,37 @@
             (),
         ),
         "list the shulker boxes inside your Enderchest",
         gather.load_shulker_boxes,
     ),
     (
         tuple(
-            f"{verb} {alias}" for verb in _list_aliases for alias in _instance_aliases
+            f"{verb} {alias}"
+            for verb in _list_aliases
+            for alias in _instance_aliases
+            if alias.endswith("s")
         ),
         "list the minecraft instances registered with your Enderchest",
         gather.load_ender_chest_instances,
     ),
     (
         tuple(
+            f"{verb} {alias}"
+            for verb in _list_aliases
+            for alias in _instance_aliases
+            if not alias.endswith("s")
+        ),
+        "list the shulker boxes that the specified instance links to",
+        _list_instance_boxes,
+    ),
+    (
+        tuple(
             f"{verb} {alias}" for verb in _list_aliases for alias in _shulker_aliases
         ),
-        "list the instances that match the specified shulker box",
+        "list the minecraft instances that match the specified shulker box",
         _list_shulker_box,
     ),
     (
         tuple(f"{verb} {alias}" for verb in _list_aliases for alias in _remote_aliases),
         "list the other EnderChest installations registered with this EnderChest",
         gather.load_ender_chest_remotes,
     ),
@@ -168,15 +214,15 @@
         The top-level argument parser responsible for routing arguments to
         specific action parsers
     action_parsers : dict of str to ArgumentParser
         The verb-specific argument parsers
     """
     descriptions: dict[str, str] = {}
     root_description: str = ""
-    for commands, description, method in ACTIONS:
+    for commands, description, _ in ACTIONS:
         descriptions[commands[0]] = description
         root_description += f"\n\t{commands[0]}\n\t\tto {description}"
 
     enderchest_parser = ArgumentParser(
         prog="enderchest",
         description=(
             f"v{get_versions()['version']}\n"
@@ -337,21 +383,39 @@
             "if there's already a shulker box with the specified name,"
             " overwrite its configuration"
         ),
     )
 
     # place options
     place_parser = action_parsers["place"]
-    place_parser.add_argument(
-        "-k",
+    cleanup = place_parser.add_argument_group()
+    cleanup.add_argument(
         "--keep-broken-links",
-        action="store_false",
-        dest="cleanup",
+        action="store_true",
         help="do not remove broken links from instances",
     )
+    cleanup.add_argument(
+        "--keep-stale-links",
+        action="store_true",
+        help=(
+            "do not remove existing links into the EnderChest,"
+            " even if the shulker box or instance spec has changed"
+        ),
+    )
+    cleanup.add_argument(
+        "-k",
+        dest="keep_level",
+        action="count",
+        default=0,
+        help=(
+            "Shorthand for the above cleanup options:"
+            " -k will --keep-stale-links,"
+            " and -kk will --keep-broken-links as well"
+        ),
+    )
     error_handling = place_parser.add_mutually_exclusive_group()
     error_handling.add_argument(
         "--stop-at-first-failure",
         "-x",
         action="store_true",
         help="stop linking at the first issue",
     )
@@ -366,15 +430,31 @@
             "ignore",
             "skip",
             "skip-instance",
             "skip-shulker-box",
             "abort",
         ),
         default="prompt",
-        help="specify how to handle linking errors (default behavior is to prompt after every error)",
+        help=(
+            "specify how to handle linking errors"
+            " (default behavior is to prompt after every error)"
+        ),
+    )
+    link_type = place_parser.add_mutually_exclusive_group()
+    link_type.add_argument(
+        "--absolute",
+        "-a",
+        action="store_true",
+        help="use absolute paths for all link targets",
+    )
+    link_type.add_argument(
+        "--relative",
+        "-r",
+        action="store_true",
+        help="use relative paths for all link targets",
     )
 
     # gather instance options
     gather_instance_parser = action_parsers[f"gather {_instance_aliases[0]}"]
     gather_instance_parser.add_argument(
         "search_paths",
         nargs="+",
@@ -411,14 +491,22 @@
         ),
     )
 
     # list instances options
 
     # list shulkers options
 
+    # list instance box options
+    list_instance_boxes_parser = action_parsers[
+        f"{_list_aliases[0]} {_instance_aliases[0]}"
+    ]
+    list_instance_boxes_parser.add_argument(
+        "instance_name", help="The name of the minecraft instance to query"
+    )
+
     # list shulker options
     list_shulker_parser = action_parsers[f"{_list_aliases[0]} {_shulker_aliases[0]}"]
     list_shulker_parser.add_argument(
         "shulker_box_name", help="The name of the shulker box to query"
     )
 
     # open / close options
@@ -488,15 +576,15 @@
         The verbosity level of the operation (in terms of log levels)
     dict
         Any additional options that will be given to the action method
 
     """
     actions: dict[str, Action] = {}
     aliases: dict[str, str] = {}
-    for commands, description, method in ACTIONS:
+    for commands, _, method in ACTIONS:
         for command in commands:
             aliases[command] = commands[0]
         actions[commands[0]] = method
 
     enderchest_parser, action_parsers = generate_parsers()
 
     _ = enderchest_parser.parse_args(argv[1:2])  # check for --help and --version
@@ -504,35 +592,41 @@
     for command in sorted(aliases.keys(), key=lambda x: -len(x)):  # longest first
         if " ".join((*argv[1:], "")).startswith(command + " "):
             action_kwargs = vars(
                 action_parsers[aliases[command]].parse_args(
                     argv[1 + len(command.split()) :]
                 )
             )
+
+            action = actions[aliases[command]]
+
             root_arg = action_kwargs.pop("root")
             root_flag = action_kwargs.pop("root_flag")
 
             verbosity = action_kwargs.pop("verbose") - action_kwargs.pop("quiet")
 
-            log_level = logging.INFO - 10 * verbosity
-            if log_level == logging.NOTSET:  # that's 0, annoyingly enough
-                log_level -= 1
+            argspec = inspect.getfullargspec(action)
+            if "verbosity" in argspec.args + argspec.kwonlyargs:
+                action_kwargs["verbosity"] = verbosity
+
+            log_level = loggers.verbosity_to_log_level(verbosity)
 
             return (
-                actions[aliases[command]],
+                action,
                 Path(root_arg or root_flag or os.getcwd()),
                 log_level,
                 action_kwargs,
             )
-    else:
-        enderchest_parser.print_help(sys.stderr)
-        sys.exit(1)
+
+    enderchest_parser.print_help(sys.stderr)
+    sys.exit(1)
 
 
 def main():
+    """CLI Entrypoint"""
     logger = logging.getLogger(__package__)
     cli_handler = logging.StreamHandler()
     cli_handler.setFormatter(loggers.CLIFormatter())
     logger.addHandler(cli_handler)
 
     action, root, log_level, kwargs = parse_args(sys.argv)
```

### Comparing `enderchest-0.1.0rc6/enderchest/craft.py` & `enderchest-0.1.1rc1/enderchest/craft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Functionality for setting up the folder structure of both chests and shulker boxes"""
-import fnmatch
 import logging
 import re
 from collections import Counter
 from pathlib import Path
 from typing import Callable, Iterable, Sequence
 from urllib.parse import ParseResult
 
@@ -16,15 +15,15 @@
     _report_shulker_boxes,
     gather_minecraft_instances,
     load_ender_chest,
     load_ender_chest_instances,
     load_ender_chest_remotes,
     load_shulker_boxes,
 )
-from .instance import InstanceSpec
+from .instance import InstanceSpec, normalize_modloader
 from .loggers import CRAFT_LOGGER
 from .prompt import NO, YES, confirm, prompt
 from .remote import fetch_remotes_from_a_remote_ender_chest
 from .shulker_box import STANDARD_LINK_FOLDERS, ShulkerBox, create_shulker_box
 
 
 def craft_ender_chest(
@@ -253,15 +252,14 @@
         )
         if not confirm(default=False):
             message = f"Aborting: {fs.ender_chest_config(minecraft_root)} exists."
             raise FileExistsError(message)
     except FileNotFoundError:
         # good! Then we don't already have an EnderChest here
         CRAFT_LOGGER.debug(f"{minecraft_root} does not already contain an EnderChest")
-        pass
 
     instances: list[InstanceSpec] = []
 
     while True:
         search_home = prompt(
             "Would you like to search your home directory for the official launcher?",
             suggestion="Y/n",
@@ -385,17 +383,16 @@
             )
             continue
         break
 
     ender_chest = EnderChest(uri, name, remotes, instances)
 
     CRAFT_LOGGER.info(
-        "\n"
-        + ender_chest.write_to_cfg()
-        + "\nPreparing to generate an EnderChest with the above configuration."
+        "\n%s\nPreparing to generate an EnderChest with the above configuration.",
+        ender_chest.write_to_cfg(),
     )
 
     if not confirm(default=True):
         raise RuntimeError("EnderChest creation aborted.")
 
     return ender_chest
 
@@ -529,16 +526,14 @@
                 ),
                 suggestion="*",
             )
             or "*"
         )
         hosts = tuple(host.strip() for host in values.split(","))
 
-        # TODO: DRY this into a dedicated function
-
         # TODO: stop wastefully reloading the cfg
         host = load_ender_chest(minecraft_root).name
 
         if not shulker_box._replace(match_criteria=(("hosts", hosts),)).matches_host(
             host
         ):
             CRAFT_LOGGER.warning(
@@ -551,17 +546,16 @@
     shulker_box = shulker_box._replace(
         priority=priority,
         match_criteria=shulker_box.match_criteria + (("hosts", hosts),),
         link_folders=link_folders,
     )
 
     CRAFT_LOGGER.info(
-        "\n"
-        + shulker_box.write_to_cfg()
-        + "Preparing to generate a shulker box with the above configuration."
+        "\n%sPreparing to generate a shulker box with the above configuration.",
+        shulker_box.write_to_cfg(),
     )
 
     if not confirm(default=True):
         raise RuntimeError("Shulker box creation aborted.")
 
     return shulker_box
 
@@ -633,16 +627,16 @@
         if len(matches) == 0:
             CRAFT_LOGGER.warning("Filters do not match any known instance.")
             default = False
         elif len(matches) == 1:
             CRAFT_LOGGER.info(f"Filters match the instance: {matches[0]}")
         else:
             CRAFT_LOGGER.info(
-                "Filters match the instances:\n"
-                + "\n".join([f"  - {name}" for name in matches])
+                "Filters match the instances:\n%s",
+                "\n".join([f"  - {name}" for name in matches]),
             )
         return tester if confirm(default=default) else None, matches
 
     while True:
         version_spec = (
             prompt(
                 (
@@ -671,43 +665,43 @@
                     ' (or multiple, e.g: "B,Q", or any using "*")'
                 ),
                 suggestion="*",
             )
             or "*"
         )
 
-        modloaders: list[str] = []
+        modloaders: set[str] = set()
         for entry in modloader.split(","):
             match entry.strip().lower():
                 case "" | "n" | "none" | "vanilla":
-                    modloaders.append("None")
+                    modloaders.update(normalize_modloader(None))
                 case "g" | "forge":
-                    modloaders.append("Forge")
+                    modloaders.update(normalize_modloader("Forge"))
                 case "b" | "fabric" | "fabric loader":
-                    modloaders.append("Fabric Loader")
+                    modloaders.update(normalize_modloader("Fabric Loader"))
                 case "q" | "quilt":
-                    modloaders.append("Quilt Loader")
+                    modloaders.update(normalize_modloader("Quilt Loader"))
                 case "l" | "liteloader":
-                    modloaders.append("LiteLoader")
+                    modloaders.update(normalize_modloader("LiteLoader"))
                 case _:
-                    modloaders.append(entry)
+                    modloaders.update(normalize_modloader(entry))
 
-        updated, matches = check_progress("modloader", modloaders)
+        updated, matches = check_progress("modloader", sorted(modloaders))
         if updated:
             shulker_box = updated
             instances = [instance for instance in instances if instance.name in matches]
             break
 
     while True:
         tag_count = Counter(sum((instance.tags for instance in instances), ()))
         # TODO: should this be most common among matches?
         example_tags: list[str] = [tag for tag, _ in tag_count.most_common(5)]
         CRAFT_LOGGER.debug(
-            "Tag counts:\n"
-            + "\n".join(f"  - {tag}: {count}" for tag, count in tag_count.items())
+            "Tag counts:\n%s",
+            "\n".join(f"  - {tag}: {count}" for tag, count in tag_count.items()),
         )
 
         if len(example_tags) == 0:
             # provide examples if the user isn't using tags
             example_tags = [
                 "vanilla-plus",
                 "multiplayer",
@@ -771,16 +765,16 @@
         CRAFT_LOGGER.warning(
             "This shulker box will be applied to all instances,"
             " including ones you create in the future."
         )
         default = False
     else:
         CRAFT_LOGGER.info(
-            "You specified the following instances:\n"
-            + "\n".join([f"  - {name}" for name in instances])
+            "You specified the following instances:\n%s",
+            "\n".join([f"  - {name}" for name in instances]),
         )
         default = True
 
     if not confirm(default=default):
         CRAFT_LOGGER.debug("Trying again to prompt for instance names")
         return _prompt_for_instance_names(shulker_box)
 
@@ -862,15 +856,16 @@
                 )
 
     choices = tuple(
         instance.name for instance in instances if instance.name in selected_instances
     )
 
     CRAFT_LOGGER.info(
-        "You selected the instances:\n" + "\n".join([f"  - {name}" for name in choices])
+        "You selected the instances:\n%s",
+        "\n".join([f"  - {name}" for name in choices]),
     )
     if not confirm(default=True):
         CRAFT_LOGGER.debug("Trying again to prompt for instance numbers")
         CRAFT_LOGGER.info("")  # just making a newline
         return _prompt_for_instance_numbers(
             shulker_box, instance_loader(), instance_loader
         )
```

### Comparing `enderchest-0.1.0rc6/enderchest/enderchest.py` & `enderchest-0.1.1rc1/enderchest/enderchest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Specification and configuration of an EnderChest"""
-import datetime as dt
-from configparser import ConfigParser, ParsingError
 from dataclasses import dataclass
-from io import StringIO
 from pathlib import Path
 from socket import gethostname
-from typing import Iterable, Sequence
+from typing import Any, Iterable
 from urllib.parse import ParseResult, urlparse
 
+from . import config as cfg
 from . import filesystem as fs
 from . import instance as i
 from . import sync
-from ._version import get_versions
 from .loggers import CRAFT_LOGGER, GATHER_LOGGER
+from .sync import path_from_uri
 
 
-@dataclass(init=False, repr=False)
+@dataclass(init=False, repr=False, eq=False)
 class EnderChest:
     """Configuration of an EnderChest
 
     Parameters
     ----------
     uri : URI or Path
         The "address" of this EnderChest, ideally as it can be accessed from other
@@ -51,30 +49,44 @@
     root : Path
         The path to this EnderChest folder
     instances : list-like of InstanceSpec
         The instances registered with this EnderChest
     remotes : list-like of (ParseResult, str) pairs
         The other EnderChest installations this EnderChest is aware of, paired
         with their aliases
-    sync_confirm_wait: bool or int
+    offer_to_update_symlink_allowlist : bool
+        By default, EnderChest will offer to create or update `allowed_symlinks.txt`
+        on any 1.20+ instances that do not already blanket allow links into
+        EnderChest. **EnderChest will never modify that or any other Minecraft
+        file without your express consent.** If you would prefer to edit these
+        files yourself (or simply not symlink your world saves), change this
+        parameter to False.
+    sync_confirm_wait : bool or int
         The default behavior when syncing EnderChests is to first perform a dry
         run of every sync operation and then wait 5 seconds before proceeding with the
         real sync. The idea is to give the user time to interrupt the sync if
         the dry run looks wrong. This can be changed by either raising or lowering
         the value of confirm, by disabling the dry-run-first behavior entirely
         (`confirm=False`) or by requiring that the user explicitly confirms
         the sync (`confirm=True`). This default behavior can also be overridden
         when actually calling the sync commands.
+    do_not_sync : list of str
+        Glob patterns of files that should not be synced between EnderChest
+        installations. By default, this list comprises `EnderChest/enderchest.cfg`,
+        any top-level folders starting with a "." (like .git) and
+        `.DS_Store` (for all you mac gamers).
     """
 
     name: str
     _uri: ParseResult
     _instances: list[i.InstanceSpec]
     _remotes: dict[str, ParseResult]
+    offer_to_update_symlink_allowlist: bool = True
     sync_confirm_wait: bool | int = 5
+    do_not_sync = ["EnderChest/enderchest.cfg", "EnderChest/.*", ".DS_Store"]
 
     def __init__(
         self,
         uri: str | ParseResult | Path,
         name: str | None = None,
         remotes: Iterable[str | ParseResult | tuple[str, str] | tuple[ParseResult, str]]
         | None = None,
@@ -114,15 +126,15 @@
         return self._uri.geturl()
 
     def __repr__(self) -> str:
         return f"EnderChest({self.uri, self.name})"
 
     @property
     def root(self) -> Path:
-        return fs.ender_chest_folder(Path(self._uri.path))
+        return fs.ender_chest_folder(path_from_uri(self._uri), check_exists=False)
 
     @property
     def instances(self) -> tuple[i.InstanceSpec, ...]:
         return tuple(self._instances)
 
     def register_instance(self, instance: i.InstanceSpec) -> i.InstanceSpec:
         """Register a new Minecraft installation
@@ -144,15 +156,15 @@
           this method will choose a new one
         - If this instance shares a path with an existing instance, it will
           replace that instance
         """
         self._instances = [
             old_instance
             for old_instance in self._instances
-            if not i.equals(Path(self._uri.path), instance, old_instance)
+            if not i.equals(path_from_uri(self._uri), instance, old_instance)
         ]
         name = instance.name
         counter = 0
         taken_names = {old_instance.name for old_instance in self._instances}
         while True:
             if name not in taken_names:
                 break
@@ -187,15 +199,15 @@
             If the provided remote is invalid
         """
         try:
             remote = remote if isinstance(remote, ParseResult) else urlparse(remote)
             alias = alias or remote.hostname
             if not alias:
                 raise AttributeError(f"{remote.geturl()} has no hostname")
-            GATHER_LOGGER.debug(f"Registering remote {remote.geturl()} ({alias})")
+            GATHER_LOGGER.debug("Registering remote %s (%s)", remote.geturl(), alias)
             self._remotes[alias] = remote
         except AttributeError as parse_problem:
             raise ValueError(f"{remote} is not a valid URI") from parse_problem
 
     @classmethod
     def from_cfg(cls, config_file: Path) -> "EnderChest":
         """Parse an EnderChest from its config file
@@ -213,53 +225,49 @@
         Raises
         ------
         ValueError
             If the config file at that location cannot be parsed
         FileNotFoundError
             If there is no config file at the specified location
         """
-        parser = ConfigParser(
-            allow_no_value=True,
-            delimiters=("=",),
-            inline_comment_prefixes=(";",),
-            interpolation=None,
-        )
-        parser.optionxform = str  # type: ignore
-        try:
-            assert parser.read(config_file)
-        except ParsingError as bad_cfg:
-            raise ValueError(f"Could not parse {config_file}") from bad_cfg
-        except AssertionError:
-            raise FileNotFoundError(f"Could not open {config_file}")
+        config = cfg.read_cfg(config_file)
 
         # All I'm gonna say is that Windows pathing is the worst
         path = urlparse(config_file.absolute().parent.parent.as_uri()).path
 
         instances: list[i.InstanceSpec] = []
         remotes: list[str | tuple[str, str]] = []
 
         scheme: str | None = None
         netloc: str | None = None
         name: str | None = None
         sync_confirm_wait: str | None = None
+        offer_to_update_symlink_allowlist: bool = True
+        do_not_sync: list[str] | None = None
 
-        for section in parser.sections():
+        for section in config.sections():
             if section == "properties":
-                scheme = parser[section].get("sync-protocol")
-                netloc = parser[section].get("address")
-                name = parser[section].get("name")
-                sync_confirm_wait = parser[section].get("sync-confirmation-time")
+                scheme = config[section].get("sync-protocol")
+                netloc = config[section].get("address")
+                name = config[section].get("name")
+                sync_confirm_wait = config[section].get("sync-confirmation-time")
+                offer_to_update_symlink_allowlist = config[section].getboolean(
+                    "offer-to-update-symlink-allowlist", True
+                )
+                if "do-not-sync" in config[section].keys():
+                    do_not_sync = cfg.parse_ini_list(
+                        config[section]["do-not-sync"] or ""
+                    )
             elif section == "remotes":
-                for remote in parser[section].items():
+                for remote in config[section].items():
                     if remote[1] is None:
                         raise ValueError("All remotes must have an alias specified")
-                    else:
-                        remotes.append((remote[1], remote[0]))
+                    remotes.append((remote[1], remote[0]))
             else:
-                instances.append(i.InstanceSpec.from_cfg(parser[section]))
+                instances.append(i.InstanceSpec.from_cfg(config[section]))
 
         scheme = scheme or sync.DEFAULT_PROTOCOL
         netloc = netloc or sync.get_default_netloc()
         uri = ParseResult(
             scheme=scheme, netloc=netloc, path=path, params="", query="", fragment=""
         )
 
@@ -274,14 +282,30 @@
                     try:
                         ender_chest.sync_confirm_wait = int(sync_confirm_wait)
                     except ValueError:
                         raise ValueError(
                             "Invalid value for sync-confirmation-time:"
                             f" {sync_confirm_wait}"
                         )
+        ender_chest.offer_to_update_symlink_allowlist = (
+            offer_to_update_symlink_allowlist
+        )
+        if do_not_sync is not None:
+            ender_chest.do_not_sync = do_not_sync
+            chest_cfg_exclusion = "/".join(
+                (fs.ENDER_CHEST_FOLDER_NAME, fs.ENDER_CHEST_CONFIG_NAME)
+            )
+            if chest_cfg_exclusion not in do_not_sync:
+                GATHER_LOGGER.warning(
+                    "This EnderChest was not configured to exclude the EnderChest"
+                    " config file from sync operations."
+                    "\n That is being fixed now."
+                )
+                ender_chest.do_not_sync.insert(0, chest_cfg_exclusion)
+                ender_chest.write_to_cfg(config_file)
         return ender_chest
 
     def write_to_cfg(self, config_file: Path | None = None) -> str:
         """Write this EnderChest's configuration to INI
 
         Parameters
         ----------
@@ -294,79 +318,49 @@
         str
             An INI-syntax rendering of this EnderChest's config
 
         Notes
         -----
         The "root" attribute is ignored for this method
         """
-        config = ConfigParser(allow_no_value=True, interpolation=None)
-        config.optionxform = str  # type: ignore
-        config.add_section("properties")
-        config.set("properties", "name", self.name)
-        config.set("properties", "address", self._uri.netloc)
-        config.set("properties", "sync-protocol", self._uri.scheme)
-        config.set(
-            "properties",
-            "sync-confirmation-time",
-            str(self.sync_confirm_wait)
-            if self.sync_confirm_wait is not True
-            else "prompt",
-        )
-        config.set("properties", "last_modified", dt.datetime.now().isoformat(sep=" "))
-        config.set(
-            "properties", "generated_by_enderchest_version", get_versions()["version"]
-        )
+        properties: dict[str, Any] = {
+            "name": self.name,
+            "address": self._uri.netloc,
+            "sync-protocol": self._uri.scheme,
+        }
+        if self.sync_confirm_wait is True:
+            properties["sync-confirmation-time"] = "prompt"
+        else:
+            properties["sync-confirmation-time"] = self.sync_confirm_wait
+
+        properties[
+            "offer-to-update-symlink-allowlist"
+        ] = self.offer_to_update_symlink_allowlist
 
-        config.add_section("remotes")
-        for uri, name in self.remotes:
-            config.set("remotes", name, uri.geturl())
-        for instance in self.instances:
-            config.add_section(instance.name)
-            config.set(instance.name, "root", str(instance.root))
-            config.set(
-                instance.name,
-                "minecraft_version",
-                _list_to_ini(instance.minecraft_versions),
-            )
-            config.set(instance.name, "modloader", instance.modloader)
-            config.set(
-                instance.name,
-                "tags",
-                _list_to_ini(instance.tags),
-            )
+        properties["do-not-sync"] = self.do_not_sync
 
-        buffer = StringIO()
-        buffer.write(f"; {fs.ENDER_CHEST_CONFIG_NAME}\n")
-        config.write(buffer)
-        buffer.seek(0)  # rewind
-
-        if config_file:
-            config_file.write_text(buffer.read())
-            buffer.seek(0)
-        return buffer.read()
+        remotes: dict[str, str] = {name: uri.geturl() for uri, name in self.remotes}
 
+        instances: dict[str, dict[str, Any]] = {}
 
-def _list_to_ini(values: Sequence) -> str:
-    """Format a list of values into a string suitable for use in an INI entry
+        for instance in self.instances:
+            instances[instance.name] = {
+                "root": instance.root,
+                "minecraft-version": instance.minecraft_versions,
+                "modloader": instance.modloader,
+                "tags": instance.tags,
+            }
 
-    Parameters
-    ----------
-    values : list-like
-        the values in the list
+        config = cfg.dumps(
+            fs.ENDER_CHEST_CONFIG_NAME, properties, remotes=remotes, **instances
+        )
 
-    Returns
-    -------
-    str
-        The formatted INI value
-    """
-    if len(values) == 0:
-        return ""
-    if len(values) == 1:
-        return values[0]
-    return "\n" + "\n".join(values)
+        if config_file:
+            config_file.write_text(config)
+        return config
 
 
 def create_ender_chest(minecraft_root: Path, ender_chest: EnderChest) -> None:
     """Create an EnderChest based on the provided configuration
 
     Parameters
     ----------
```

### Comparing `enderchest-0.1.0rc6/enderchest/filesystem.py` & `enderchest-0.1.1rc1/enderchest/filesystem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functionality for managing the EnderChest and shulker box config files and folders"""
+import os
 from pathlib import Path
 from typing import Iterable
 
 from .loggers import GATHER_LOGGER
 
 ENDER_CHEST_FOLDER_NAME = "EnderChest"
 
@@ -20,15 +21,15 @@
     minecraft_root : Path
         The root directory that your minecraft stuff (or, at least, the one
         that's the parent of your EnderChest folder)
     check_exists : bool, optional
         By default, this method will raise an error if no EnderChest exists
         at that location (meaning no folder or no enderchest config file in
         that folder). To disable that check, call this method with
-        `check_exists=False`
+        `check_exists=False`.
 
     Returns
     -------
     Path
         The path to the EnderChest folder
 
     Raises
@@ -48,15 +49,15 @@
     ----------
     minecraft_root : Path
         The root directory that your minecraft stuff (or, at least, the one
         that's the parent of your EnderChest folder)
     check_exists : bool, optional
         By default, this method will raise an error if the enderchest config
         file does not already exist. To disable that check, call this method
-        with `check_exists=False`
+        with `check_exists=False`.
 
     Returns
     -------
     Path
         The path to the EnderChest config file
 
     Raises
@@ -160,7 +161,71 @@
 
     Notes
     -----
     This method does not check to make sure that those .minecraft folders
     contain valid minecraft instances, just that they exist
     """
     return search_path.rglob(".minecraft")
+
+
+def links_into_enderchest(
+    minecraft_root: Path, link: Path, check_exists: bool = True
+) -> bool:
+    """Determine whether a symlink's target is inside the EnderChest specified
+    by the Minecraft root.
+
+    Parameters
+    ----------
+    minecraft_root : Path
+        The root directory that your minecraft stuff (or, at least, the one
+        that's the parent of your EnderChest folder)
+    link : Path
+        The link to check
+    check_exists : bool, optional
+        By default, this method will raise an error if no EnderChest exists
+        at that location (meaning no folder or no enderchest config file in
+        that folder). To disable that check, call this method with
+        `check_exists=False`.
+
+    Returns
+    -------
+    bool
+        True if the path is inside of the EnderChest folder. False otherwise.
+
+    Notes
+    -----
+    This method only checks the *direct target* of the link as opposed to the
+    fully resolved path.
+
+    Raises
+    ------
+    FileNotFoundError
+        If no valid EnderChest installation exists within the given
+        minecraft root (and checking hasn't been disabled)
+    OSError
+        If the link provided isn't actually a symbolic link
+    """
+    chest_folder = os.path.normpath(
+        ender_chest_folder(minecraft_root, check_exists=check_exists)
+        .expanduser()
+        .absolute()
+    )
+
+    target = os.readlink(link)
+    if not os.path.isabs(target):
+        target = os.path.normpath(link.parent / target)
+
+    # Windows shenanigans: https://bugs.python.org/issue42957
+    if target.startswith(("\\\\?\\", "\\??\\")):  # pragma: no cover
+        try:
+            os.stat(target[4:])
+            target = target[4:]
+        except (OSError, FileNotFoundError):
+            # then maybe this is somehow legit
+            pass
+
+    # there's probably a better way to check if a file is inside a sub-path
+    try:
+        common_root = os.path.commonpath([target, chest_folder])
+    except ValueError:  # if they have no common root
+        common_root = ""
+    return common_root == chest_folder
```

### Comparing `enderchest-0.1.0rc6/enderchest/gather.py` & `enderchest-0.1.1rc1/enderchest/gather.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Functionality for finding, resolving and parsing local installations and instances"""
 import json
 import logging
+import os
+import re
 from configparser import ConfigParser, ParsingError
 from pathlib import Path
 from typing import Iterable, Sequence
 from urllib.parse import ParseResult
 
 from enderchest.sync import render_remote
 
 from . import filesystem as fs
 from .enderchest import EnderChest, create_ender_chest
-from .instance import InstanceSpec, _parse_version
+from .instance import InstanceSpec, normalize_modloader, parse_version
 from .loggers import GATHER_LOGGER
-from .shulker_box import ShulkerBox
+from .prompt import prompt
+from .shulker_box import ShulkerBox, _matches_version
 
 
 def load_ender_chest(minecraft_root: Path) -> EnderChest:
     """Load the configuration from the enderchest.cfg file in the EnderChest
     folder.
 
     Parameters
@@ -84,16 +87,16 @@
         GATHER_LOGGER.warning(
             f"There are no instances registered to the {minecraft_root} EnderChest",
         )
     else:
         GATHER_LOGGER.log(
             log_level,
             "These are the instances that are currently registered"
-            f" to the {minecraft_root} EnderChest:\n"
-            + "\n".join(
+            f" to the {minecraft_root} EnderChest:\n %s",
+            "\n".join(
                 [
                     f"  {i + 1}. {_render_instance(instance)}"
                     for i, instance in enumerate(instances)
                 ]
             ),
         )
     return instances
@@ -175,16 +178,16 @@
 def _report_shulker_boxes(
     shulker_boxes: Iterable[ShulkerBox], log_level: int, ender_chest_name: str
 ) -> None:
     """Log the list of shulker boxes in the order they'll be linked"""
     GATHER_LOGGER.log(
         log_level,
         f"These are the shulker boxes within {ender_chest_name}"
-        "\nlisted in the order in which they are linked:\n"
-        + "\n".join(
+        "\nlisted in the order in which they are linked:\n%s",
+        "\n".join(
             f"  {shulker_box.priority}. {_render_shulker_box(shulker_box)}"
             for shulker_box in shulker_boxes
         ),
     )
 
 
 def _load_shulker_box(config_file: Path) -> ShulkerBox:
@@ -278,24 +281,78 @@
         return []
 
     report = (
         "These are the remote EnderChest installations registered"
         f" to the one installed at {minecraft_root}"
     )
     remote_list: list[tuple[ParseResult, str]] = []
+    log_args: list[str] = []
     for remote, alias in remotes:
-        report += f"\n  - {render_remote(alias, remote)}"
+        report += "\n  - %s"
+        log_args.append(render_remote(alias, remote))
         remote_list.append((remote, alias))
-    GATHER_LOGGER.log(log_level, report)
+    GATHER_LOGGER.log(log_level, report, *log_args)
     return remote_list
 
 
-def load_shulker_box_matches(
+def get_shulker_boxes_matching_instance(
+    minecraft_root: Path, instance_name: str
+) -> list[ShulkerBox]:
+    """Get the list of shulker boxes that the specified instance links to
+
+    Parameters
+    ----------
+    minecraft_root : Path
+        The root directory that your minecraft stuff (or, at least, the one
+        that's the parent of your EnderChest folder)
+    instance_name : str
+        The name of the instance you're asking about
+
+    Returns
+    -------
+    list of ShulkerBox
+        The shulker boxes that are linked to by the specified instance
+    """
+    try:
+        chest = load_ender_chest(minecraft_root)
+    except (FileNotFoundError, ValueError) as bad_chest:
+        GATHER_LOGGER.error(
+            f"Could not load EnderChest from {minecraft_root}:\n  {bad_chest}"
+        )
+        return []
+    for mc in chest.instances:
+        if mc.name == instance_name:
+            break
+    else:
+        GATHER_LOGGER.error(
+            f"No instance named {instance_name} is registered to this EnderChest"
+        )
+        return []
+
+    matches = [
+        box
+        for box in load_shulker_boxes(minecraft_root, log_level=logging.DEBUG)
+        if box.matches(mc) and box.matches_host(chest.name)
+    ]
+
+    if len(matches) == 0:
+        report = "does not link to any shulker boxes in this chest"
+    else:
+        report = "links to the following shulker boxes:\n" + "\n".join(
+            f"  - {_render_shulker_box(box)}" for box in matches
+        )
+
+    GATHER_LOGGER.info(f"The instance {_render_instance(mc)} {report}")
+
+    return matches
+
+
+def get_instances_matching_shulker_box(
     minecraft_root: Path, shulker_box_name: str
-) -> Sequence[InstanceSpec]:
+) -> list[InstanceSpec]:
     """Get the list of registered instances that link to the specified shulker box
 
     Parameters
     ----------
     minecraft_root : Path
         The root directory that your minecraft stuff (or, at least, the one
         that's the parent of your EnderChest folder)
@@ -307,58 +364,56 @@
     list of InstanceSpec
         The instances that are / should be linked to the specified shulker box
     """
     try:
         config_file = fs.shulker_box_config(minecraft_root, shulker_box_name)
     except FileNotFoundError:
         GATHER_LOGGER.error(f"No EnderChest is installed in {minecraft_root}")
-        return ()
+        return []
     try:
         shulker_box = _load_shulker_box(config_file)
     except (FileNotFoundError, ValueError) as bad_box:
         GATHER_LOGGER.error(
             f"Could not load shulker box {shulker_box_name}\n  {bad_box}"
         )
-        return ()
+        return []
 
     chest = load_ender_chest(minecraft_root)
 
     if not shulker_box.matches_host(chest.name):
         GATHER_LOGGER.warning(
             "This shulker box will not link to any instances on this machine"
         )
-        return ()
+        return []
 
     if not chest.instances:
         GATHER_LOGGER.warning(
             "This EnderChest does not have any instances registered."
             " To register some, run the command:"
             "\nenderchest gather minecraft",
         )
-        return ()
+        return []
 
     GATHER_LOGGER.debug(
         "These are the instances that are currently registered"
-        f" to the {minecraft_root} EnderChest:\n"
-        + "\n".join(
+        f" to the {minecraft_root} EnderChest:\n%s",
+        "\n".join(
             [
                 f"  {i + 1}. {_render_instance(instance)}"
                 for i, instance in enumerate(chest.instances)
             ]
         ),
     )
 
-    if shulker_box is None:
-        return ()
     matches = [
         instance for instance in chest.instances if shulker_box.matches(instance)
     ]
 
     if len(matches) == 0:
-        report = "does not link to by any registered instances"
+        report = "is not link to by any registered instances"
     else:
         report = "is linked to by the following instances:\n" + "\n".join(
             f"  - {_render_instance(instance)}" for instance in matches
         )
 
     GATHER_LOGGER.info(f"The shulker box {_render_shulker_box(shulker_box)} {report}")
 
@@ -394,50 +449,57 @@
     -----
     - If a minecraft installation is found but cannot be parsed
       (or parsed as specified) this method will report that failure but then
       continue on.
     - As a corollary, if _no_ valid Minecraft installations can be found, this
       method will return an empty list.
     """
+    try:
+        ender_chest = load_ender_chest(minecraft_root)
+    except FileNotFoundError:
+        # because this method can be called during crafting
+        ender_chest = EnderChest(minecraft_root)
     GATHER_LOGGER.debug(f"Searching for Minecraft folders inside {search_path}")
     instances: list[InstanceSpec] = []
     for folder in fs.minecraft_folders(search_path):
         folder_path = folder.absolute()
         GATHER_LOGGER.debug(f"Found minecraft installation at {folder}")
         if official is not False:
             try:
                 instances.append(gather_metadata_for_official_instance(folder_path))
                 GATHER_LOGGER.info(
                     f"Gathered official Minecraft installation from {folder}"
                 )
+                _check_for_allowed_symlinks(ender_chest, instances[-1])
                 continue
             except ValueError as not_official:
                 GATHER_LOGGER.log(
                     logging.DEBUG if official is None else logging.WARNING,
                     (f"{folder} is not an official instance:" f"\n{not_official}",),
                 )
         if official is not True:
             try:
                 instances.append(gather_metadata_for_mmc_instance(folder_path))
                 GATHER_LOGGER.info(
                     f"Gathered MMC-like Minecraft installation from {folder}"
                 )
+                _check_for_allowed_symlinks(ender_chest, instances[-1])
                 continue
             except ValueError as not_mmc:
                 GATHER_LOGGER.log(
                     logging.DEBUG if official is None else logging.WARNING,
                     f"{folder} is not an MMC-like instance:\n{not_mmc}",
                 )
         GATHER_LOGGER.warning(
             f"{folder_path} does not appear to be a valid Minecraft instance"
         )
     for i, mc_instance in enumerate(instances):
         try:
             instances[i] = mc_instance._replace(
-                root=mc_instance.root.relative_to(minecraft_root)
+                root=mc_instance.root.relative_to(minecraft_root.resolve())
             )
         except ValueError:
             # TODO: if not Windows, try making relative to "~"
             pass  # instance isn't inside the minecraft root
     if not instances:
         GATHER_LOGGER.warning(
             f"Could not find any Minecraft instances inside {search_path}"
@@ -501,32 +563,32 @@
     except FileNotFoundError as no_json:
         raise ValueError(f"Could not find {version_manifest_file}") from no_json
     except json.JSONDecodeError as bad_json:
         raise ValueError(
             f"{version_manifest_file} is corrupt and could not be parsed"
         ) from bad_json
     except KeyError as weird_json:
-        GATHER_LOGGER.warn(
+        GATHER_LOGGER.warning(
             f"{version_manifest_file} has no latest-version lookup."
             "\nPlease check the parsed metadata to ensure that it's accurate.",
         )
         version_lookup = {}
 
     versions: list[str] = []
     tags: list[str] = ["vanilla"]
     for version in raw_versions:
         if version.startswith("latest-"):
             mapped_version = version_lookup.get(version[len("latest-") :])
             if mapped_version is not None:
-                versions.append(_parse_version(mapped_version))
+                versions.append(parse_version(mapped_version))
                 tags.append(version)
                 continue
-        versions.append(_parse_version(version))
+        versions.append(parse_version(version))
 
-    return InstanceSpec(name, minecraft_folder, tuple(versions), None, tuple(tags))
+    return InstanceSpec(name, minecraft_folder, tuple(versions), "", tuple(tags))
 
 
 def gather_metadata_for_mmc_instance(
     minecraft_folder: Path, instgroups_file: Path | None = None
 ) -> InstanceSpec:
     """Parse files to generate metadata for a MultiMC-like instance
 
@@ -560,25 +622,26 @@
 
         version: str | None = None
         modloader: str | None = None
 
         for component in components:
             match component.get("uid"), component.get("cachedName", ""):
                 case "net.minecraft", _:
-                    version = _parse_version(component["version"])
+                    version = parse_version(component["version"])
                 case "net.fabricmc.fabric-loader", _:
                     modloader = "Fabric Loader"
                 case "org.quiltmc.quilt-loader", _:
                     modloader = "Quilt Loader"
                 case ("net.minecraftforge", _) | (_, "Forge"):
                     modloader = "Forge"
                 case _, name if name.endswith("oader"):
                     modloader = name
                 case _:
                     continue
+            modloader = normalize_modloader(modloader)[0]
         if version is None:
             raise KeyError("Could not find a net.minecraft component")
     except FileNotFoundError as no_json:
         raise ValueError(f"Could not find {mmc_pack_file}") from no_json
     except json.JSONDecodeError as bad_json:
         raise ValueError(
             f"{mmc_pack_file} is corrupt and could not be parsed"
@@ -589,15 +652,15 @@
         ) from weird_json
 
     name = minecraft_folder.parent.name
 
     tags: list[str] = []
 
     if name == "":
-        GATHER_LOGGER.warn(
+        GATHER_LOGGER.warning(
             "Could not resolve the name of the parent folder"
             " and thus could not load tags."
         )
     else:
         instgroups_file = (
             instgroups_file or minecraft_folder.parent.parent / "instgroups.json"
         )
@@ -607,45 +670,51 @@
                 groups: dict[str, dict] = json.load(groups_json)["groups"]
             for tag, metadata in groups.items():
                 # interestingly this comes from the folder name, not the actual name
                 if name in metadata.get("instances", ()):
                     tags.append(tag)
 
         except FileNotFoundError as no_json:
-            GATHER_LOGGER.warn(
+            GATHER_LOGGER.warning(
                 f"Could not find {instgroups_file} and thus could not load tags"
             )
         except json.JSONDecodeError as bad_json:
-            GATHER_LOGGER.warn(
+            GATHER_LOGGER.warning(
                 f"{instgroups_file} is corrupt and could not be parsed for tags"
             )
         except KeyError as weird_json:
-            GATHER_LOGGER.warn(f"Could not parse tags from {instgroups_file}")
+            GATHER_LOGGER.warning(f"Could not parse tags from {instgroups_file}")
 
     instance_cfg = minecraft_folder.parent / "instance.cfg"
 
     try:
         parser = ConfigParser(allow_no_value=True, interpolation=None)
         parser.read_string("[instance]\n" + instance_cfg.read_text())
         name = parser["instance"]["name"]
     except FileNotFoundError as no_cfg:
-        GATHER_LOGGER.warn(
+        GATHER_LOGGER.warning(
             f"Could not find {instance_cfg} and thus could not load the instance name"
         )
     except ParsingError as no_cfg:
-        GATHER_LOGGER.warn(
+        GATHER_LOGGER.warning(
             f"{instance_cfg} is corrupt and could not be parsed the instance name"
         )
     except KeyError as weird_json:
-        GATHER_LOGGER.warn(f"Could not parse instance name from {instance_cfg}")
+        GATHER_LOGGER.warning(f"Could not parse instance name from {instance_cfg}")
 
     if name == "":
         raise ValueError("Could not determine the name of the instance.")
 
-    return InstanceSpec(name, minecraft_folder, (version,), modloader, tuple(tags))
+    return InstanceSpec(
+        name,
+        minecraft_folder,
+        (version,),
+        modloader or "",
+        tuple(tags),
+    )
 
 
 def update_ender_chest(
     minecraft_root: Path,
     search_paths: Iterable[str | Path] | None = None,
     official: bool | None = None,
     remotes: Iterable[str | ParseResult | tuple[str, str] | tuple[ParseResult, str]]
@@ -690,7 +759,106 @@
                 ender_chest.register_remote(remote)
             else:
                 ender_chest.register_remote(*remote)
         except ValueError as bad_remote:
             GATHER_LOGGER.warning(bad_remote)
 
     create_ender_chest(minecraft_root, ender_chest)
+
+
+def _check_for_allowed_symlinks(
+    ender_chest: EnderChest, instance: InstanceSpec
+) -> None:
+    """Check if the instance:
+        - is 1.20+
+        - has not already blanket-allowed symlinks into the EnderChest
+
+    and if it hasn't, offer to update the allow-list now *but only if* the user
+    hasn't already told EnderChest "shut up I know what I'm doing."
+
+    Parameters
+    ----------
+    ender_chest : EnderChest
+        This EnderChest
+    instance : InstanceSpec
+        The instance spec to check
+    """
+    if ender_chest.offer_to_update_symlink_allowlist is False:
+        return
+
+    if not any(
+        _needs_symlink_allowlist(version) for version in instance.minecraft_versions
+    ):
+        return
+    ender_chest_abspath = os.path.abspath(ender_chest.root)
+
+    symlink_allowlist = instance.root / "allowed_symlinks.txt"
+
+    try:
+        allowlist_contents = symlink_allowlist.read_text()
+        already_allowed = ender_chest_abspath in allowlist_contents.splitlines()
+        allowlist_needs_newline = not allowlist_contents.endswith("\n")
+    except FileNotFoundError:
+        already_allowed = False
+        allowlist_needs_newline = False
+
+    if already_allowed:
+        return
+
+    GATHER_LOGGER.warning(
+        """
+Starting with Minecraft 1.20, Mojang by default no longer allows worlds
+to load if they are or if they contain symbolic links.
+Read more: https://help.minecraft.net/hc/en-us/articles/16165590199181"""
+    )
+
+    response = prompt(
+        f"Would you like EnderChest to add {ender_chest_abspath} to {symlink_allowlist}?",
+        "Y/n",
+    )
+
+    if response.lower() not in ("y", "yes"):
+        return
+
+    with symlink_allowlist.open("a") as f:
+        if allowlist_needs_newline:
+            f.write("\n")
+        f.write(ender_chest_abspath + "\n")
+
+    GATHER_LOGGER.info(f"{symlink_allowlist} updated.")
+
+
+def _needs_symlink_allowlist(version: str) -> bool:
+    """Determine if a version needs `allowed_symlinks.txt` in order to link
+    to EnderChest. Note that this is going a little broader than is strictly
+    necessary.
+
+    Parameters
+    ----------
+    version: str
+        The version string to check against
+
+    Returns
+    -------
+    bool
+        Returns False if the Minecraft version predates the symlink ban. Returns
+        True if it doesn't (or is marginal).
+
+    Notes
+    -----
+    Have I mentioned that parsing Minecraft version strings is a pain in the
+    toucans?
+    """
+    # first see if it follows basic semver
+    if _matches_version(">1.19", parse_version(version.split("-")[0])):
+        return True
+    if _matches_version("1.20.0*", parse_version(version.split("-")[0])):
+        return True
+    # is it a snapshot?
+    if match := re.match("^([1-2][0-9])w([0-9]{1,2})", version.lower()):
+        year, week = match.groups()
+        if int(year) > 23:
+            return True
+        if int(year) == 23 and int(week) > 18:
+            return True
+
+    return False
```

### Comparing `enderchest-0.1.0rc6/enderchest/place.py` & `enderchest-0.1.1rc1/enderchest/place.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 """Symlinking functionality"""
+import fnmatch
 import itertools
 import logging
 import os
 from pathlib import Path
 from typing import Iterable
 
 from . import filesystem as fs
 from .gather import load_ender_chest, load_ender_chest_instances, load_shulker_boxes
-from .instance import InstanceSpec
 from .loggers import PLACE_LOGGER
 from .prompt import prompt
 from .shulker_box import ShulkerBox
 
 
 def place_ender_chest(
     minecraft_root: Path,
-    cleanup: bool = True,
+    keep_broken_links: bool = False,
+    keep_stale_links: bool = False,
     error_handling: str = "abort",
+    relative: bool = True,
     rollback=False,
 ) -> None:
     """Link all instance files and folders to all shulker boxes
 
     Parameters
     ----------
     minecraft_root : Path
         The root directory that your minecraft stuff (or, at least, the one
         that's the parent of your EnderChest folder)
-    cleanup : bool, optional
+    keep_broken_links : bool, optional
         By default, this method will remove any broken links in your instances
-        and servers folders. To disable this behavior, pass in `cleanup=False`
+        and servers folders. To disable this behavior, pass in
+        `keep_broken_links=True`.
+    keep_stale_links : bool, optional
+        By default, this method will remove any links into your EnderChest folder
+        that are no longer specified by any shulker box (such as because the
+        instance spec or shulker box configuration changed). To disable this
+        behavior, pass in `keep_stale_links=True`.
     error_handling : str, optional
         By default, if a linking failure occurs, this method will terminate
         immediately (`error_handling=abort`). Alternatively,
           - pass in `error_handling="ignore"` to continue as if the link failure
             hadn't occurred
           - pass in `error_handling="skip"` to abort linking the current instance
             to the current shulker box but otherwise continue on
           - pass in `error_handling="skip-instance"` to abort linking the current
             instance altogether but to otherwise continue on with other instances
           - pass in `error_handling="skip-shulker-box"` to abort linking to the current
             shulker box altogether but to otherwise continue on with other boxes
           - pass in `error_handling="prompt"` to ask what to do on each failure
+    relative : bool, optional
+        By default, links will use relative paths when possible. To use absolute
+        paths instead (see: https://bugs.mojang.com/projects/MC/issues/MC-263046),
+        pass in `relative=False`.
     rollback: bool, optional
         In the future in the event of linking errors passing in `rollback=True`
         can be used to roll back any changes that have already been applied
         based on the error-handling method specified.
     """
     if rollback is not False:
         raise NotImplementedError("Rollbacks are not currently supported")
@@ -63,34 +75,33 @@
 
     for shulker_box in load_shulker_boxes(minecraft_root, log_level=logging.DEBUG):
         if not shulker_box.matches_host(host):
             PLACE_LOGGER.debug(
                 f"{shulker_box.name} is not intended for linking to this host ({host})"
             )
             continue
-        else:
-            shulker_boxes.append(shulker_box)
+        shulker_boxes.append(shulker_box)
 
-    skip_instances: list[InstanceSpec] = []
+    skip_boxes: list[ShulkerBox] = []
 
-    def handle_error(instance: InstanceSpec) -> str:
+    def handle_error(shulker_box: ShulkerBox | None) -> str:
         """Centralized error-handling
 
         Parameters
         ----------
-        instance:
-            The current instance (in case it needs to be added to the skip list)
+        shulker_box:
+            The current shulker box (in case it needs to be added to the skip list)
 
         Returns
         -------
         str
             Instructions on what to do next. Options are:
               - return
               - break
-              - coninue
+              - continue
               - pass
         """
         if error_handling == "prompt":
             proceed_how = (
                 prompt(
                     "How would you like to proceed?"
                     "\n[Q]uit, [C]ontinue, abort linking the rest of this shulker/instance [M]atch?"
@@ -111,15 +122,15 @@
                     proceed_how = "ignore"
                 case "m" | "match" | "skip":
                     proceed_how = "skip"
                 case "s" | "shulker" | "shulkerbox" | "skipshulker":
                     proceed_how = "skip-shulker"
                 case _:
                     PLACE_LOGGER.error("Invalid selection.")
-                    return handle_error(instance)
+                    return handle_error(shulker_box)
         else:
             proceed_how = error_handling
 
         match proceed_how:
             case "abort" | "stop" | "quit" | "exit":
                 PLACE_LOGGER.error("Aborting")
                 return "return"
@@ -127,129 +138,163 @@
                 PLACE_LOGGER.debug("Ignoring")
                 return "pass"
             case "skip":
                 PLACE_LOGGER.warning("Skipping the rest of this match")
                 return "continue"
             case "skip-instance":
                 PLACE_LOGGER.warning("Skipping any more linking from this instance")
-                skip_instances.append(instance)
-                return "continue"
+
+                return "break"
             case "skip-shulker-box" | "skip-shulkerbox" | "skip-shulker":
                 PLACE_LOGGER.warning("Skipping any more linking into this shulker box")
-                return "break"
+                if shulker_box:
+                    skip_boxes.append(shulker_box)
+                return "continue"
             case _:
                 raise ValueError(
                     f"Unrecognized error-handling method: {error_handling}"
                 )
 
-    for shulker_box in shulker_boxes:
-        for instance in instances:
+    for instance in instances:
+        instance_root = (minecraft_root / instance.root.expanduser()).expanduser()
+        if not instance_root.exists():
+            PLACE_LOGGER.error(
+                "No minecraft instance exists at"
+                f" {instance_root.expanduser().absolute()}"
+            )
+            match handle_error(None):
+                case "return":
+                    return
+                case "break":
+                    break
+                case _:  # nothing to link, so might as well skip the rest
+                    continue
+
+        # start by removing all existing symlinks into the EnderChest
+        if not keep_stale_links:
+            for file in instance_root.rglob("*"):
+                if file.is_symlink():
+                    if fs.links_into_enderchest(minecraft_root, file):
+                        PLACE_LOGGER.debug(
+                            f"Removing old link: {file} -> {os.readlink(file)}"
+                        )
+                        file.unlink()
+
+        for shulker_box in shulker_boxes:
             if not shulker_box.matches(instance):
                 continue
-            if instance in skip_instances:
+            if shulker_box in skip_boxes:
                 continue
 
-            instance_root = (minecraft_root / instance.root.expanduser()).expanduser()
             box_root = shulker_box.root.expanduser().absolute()
 
-            if not instance_root.exists():
-                PLACE_LOGGER.error(
-                    f"No minecraft instance exists at {instance_root.expanduser().absolute()}"
-                )
-                match handle_error(instance):
-                    case "return":
-                        return
-                    case "break":
-                        break
-                    case _:  # nothing to link, so might as well skip the rest
-                        continue
-
             PLACE_LOGGER.info(f"Linking {instance.root} to {shulker_box.name}")
 
             resources = set(_rglob(box_root, shulker_box.max_link_depth))
-            resources.remove(fs.shulker_box_config(minecraft_root, shulker_box.name))
 
             match_exit = "pass"
             for link_folder in shulker_box.link_folders:
                 resources -= {box_root / link_folder}
                 resources -= set((box_root / link_folder).rglob("*"))
                 try:
-                    link_resource(link_folder, box_root, instance_root)
+                    link_resource(link_folder, box_root, instance_root, relative)
                 except (OSError, NotADirectoryError) as oh_no:
                     PLACE_LOGGER.error(
                         f"Error linking shulker box {shulker_box.name}"
                         f" to instance {instance.name}:"
                         f"\n  {(instance.root / link_folder)} is a"
                         " non-empty directory"
                     )
-                    match handle_error(instance):
+                    match handle_error(shulker_box):
                         case "return":
                             return
                         case "break":
                             match_exit = "break"
                             break
                         case "continue":
                             match_exit = "continue"
                             break
                         case "pass":
                             continue  # or pass--it's the end of the loop
 
             if match_exit not in ("break", "continue"):
                 for resource in resources:
                     resource_path = resource.relative_to(box_root)
-                    try:
-                        link_resource(
-                            resource_path,
-                            box_root,
-                            instance_root,
-                        )
-                    except (OSError, NotADirectoryError) as oh_no:
-                        PLACE_LOGGER.error(
-                            f"Error linking shulker box {shulker_box.name}"
-                            f" to instance {instance.name}:"
-                            f"\n  {(instance.root / resource_path)}"
-                            " already exists"
-                        )
-                        match handle_error(instance):
-                            case "return":
-                                return
-                            case "break":
-                                match_exit = "break"
-                                break
-                            case "continue":
-                                match_exit = "continue"  # technically does nothing
-                                break
-                            case "pass":
-                                continue  # or pass--it's the end of the loop
+                    for pattern in shulker_box.do_not_link:
+                        if fnmatch.fnmatchcase(
+                            str(resource_path), pattern
+                        ) or fnmatch.fnmatchcase(
+                            str(resource_path), os.path.join("*", pattern)
+                        ):
+                            PLACE_LOGGER.debug(
+                                "Skipping %s (matches pattern %s)",
+                                resource_path,
+                                pattern,
+                            )
+                            break
+                    else:
+                        try:
+                            link_resource(
+                                resource_path,
+                                box_root,
+                                instance_root,
+                                relative,
+                            )
+                        except (OSError, NotADirectoryError) as oh_no:
+                            PLACE_LOGGER.error(
+                                f"Error linking shulker box {shulker_box.name}"
+                                f" to instance {instance.name}:"
+                                f"\n  {(instance.root / resource_path)}"
+                                " already exists"
+                            )
+                            match handle_error(shulker_box):
+                                case "return":
+                                    return
+                                case "break":
+                                    match_exit = "break"
+                                    break
+                                case "continue":
+                                    match_exit = "continue"  # technically does nothing
+                                    break
+                                case "pass":
+                                    continue  # or pass--it's the end of the loop
 
-            if cleanup:  # consider this a "finally"
+            # consider this a "finally"
+            if not keep_broken_links:
                 # we clean up as we go, just in case of a failure
                 for file in instance_root.rglob("*"):
                     if not file.exists():
                         PLACE_LOGGER.debug(f"Removing broken link: {file}")
                         file.unlink()
 
             if match_exit == "break":
                 break
 
 
 def link_resource(
-    resource_path: str | Path, shulker_root: Path, instance_root: Path
+    resource_path: str | Path,
+    shulker_root: Path,
+    instance_root: Path,
+    relative: bool,
 ) -> None:
     """Create a symlink for the specified resource from an instance's space
     pointing to the tagged file / folder living inside a shulker box.
 
     Parameters
     ----------
     resource_path : str or Path
         Location of the resource relative to the instance's ".minecraft" folder
     shulker_root : Path
         The path to the shulker box
     instance_root : Path
         The path to the instance's ".minecraft" folder
+    relative : bool
+        If True, the link will be use a relative path if possible. Otherwise,
+        an absolute path will be used, regardless of whether a a relative or
+        absolute path was provided.
 
     Raises
     ------
     NotADirectoryError
         If a file already exists where you're attempting to place the symlink
     OSError
         If a non-empty directory already exists where you're attempting to
@@ -260,32 +305,32 @@
     - This method will create any folders that do not exist within an instance
     - This method will overwrite existing symlinks and empty folders
       but will not overwrite or delete any actual files.
     """
     instance_path = (instance_root / resource_path).expanduser().absolute()
     instance_path.parent.mkdir(parents=True, exist_ok=True)
 
-    relative_path = os.path.relpath(
-        (shulker_root / resource_path).expanduser().absolute(), instance_path.parent
-    )
+    target: str | Path = (shulker_root / resource_path).expanduser().absolute()
+    if relative:
+        target = os.path.relpath(target, instance_path.parent)
 
     if instance_path.is_symlink():
         # remove previous symlink in this spot
-        PLACE_LOGGER.debug(f"Removing old link at {instance_path}")
         instance_path.unlink()
+        PLACE_LOGGER.debug(f"Removed previous link at {instance_path}")
     else:
         try:
             os.rmdir(instance_path)
-            PLACE_LOGGER.debug(f"Removed empty diretory at {instance_path}")
+            PLACE_LOGGER.debug(f"Removed empty directory at {instance_path}")
         except FileNotFoundError:
             pass  # A-OK
 
-    PLACE_LOGGER.debug(f"Linking {instance_path} to {relative_path}")
+    PLACE_LOGGER.debug(f"Linking {instance_path} to {target}")
     os.symlink(
-        relative_path,
+        target,
         instance_path,
         target_is_directory=(shulker_root / resource_path).is_dir(),
     )
 
 
 def _rglob(root: Path, max_depth: int) -> Iterable[Path]:
     """Find all files (and directories* and symlinks) in the path up to the
```

### Comparing `enderchest-0.1.0rc6/enderchest/prompt.py` & `enderchest-0.1.1rc1/enderchest/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 
     Returns
     -------
     bool
         Whether the user has opted to continue
     """
 
-    confirm = prompt("Do you wish to continue?", "Y/n" if default else "y/N")
+    response = prompt("Do you wish to continue?", "Y/n" if default else "y/N")
 
-    if confirm == "":
+    if response == "":
         return default
 
-    if confirm in YES:
+    if response in YES:
         return True
 
     return False
```

### Comparing `enderchest-0.1.0rc6/enderchest/remote.py` & `enderchest-0.1.1rc1/enderchest/remote.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Higher-level functionality around synchronizing with different EnderCherts"""
 import logging
-import os
 from pathlib import Path
 from time import sleep
 from urllib.parse import ParseResult, urlparse
 
 from . import filesystem as fs
 from . import gather
 from .enderchest import EnderChest
-from .loggers import SYNC_LOGGER
+from .loggers import IMPORTANT, SYNC_LOGGER
 from .prompt import confirm
 from .sync import path_from_uri, pull, push, remote_file, render_remote
 
 
 def load_remote_ender_chest(uri: str | ParseResult) -> EnderChest:
     """Load an EnderChest configuration from another machine
 
@@ -75,16 +74,16 @@
     remote_chest = load_remote_ender_chest(uri)
     remotes: list[tuple[ParseResult, str]] = [
         (urlparse(uri) if isinstance(uri, str) else uri, remote_chest.name)
     ]
 
     remotes.extend(remote_chest.remotes)
     SYNC_LOGGER.info(
-        "Loaded the following remotes:\n"
-        + "\n".join(f"  - {render_remote(alias, uri)}" for uri, alias in remotes)
+        "Loaded the following remotes:\n %s",
+        "\n".join(f"  - {render_remote(alias, uri)}" for uri, alias in remotes),
     )
 
     if len(set(alias for _, alias in remotes)) != len(remotes):
         raise RuntimeError(
             f"There are duplicates aliases in the list of remotes pulled from {uri}"
         )
     return remotes
@@ -136,14 +135,17 @@
             'Invalid choice for sync operation. Choices are "pull" and "push"'
         )
     try:
         if sync_confirm_wait is None:
             sync_confirm_wait = gather.load_ender_chest(
                 minecraft_root
             ).sync_confirm_wait
+        this_chest = gather.load_ender_chest(minecraft_root)
+
+        # I know this is redundant, but we want those logs
         remotes = gather.load_ender_chest_remotes(
             minecraft_root, log_level=logging.DEBUG
         )
     except (FileNotFoundError, ValueError) as bad_chest:
         SYNC_LOGGER.error(
             f"Could not load EnderChest from {minecraft_root}:\n  {bad_chest}"
         )
@@ -157,19 +159,24 @@
         if dry_run:
             runs: tuple[bool, ...] = (True,)
         elif sync_confirm_wait is False or sync_confirm_wait <= 0:
             runs = (False,)
         else:
             runs = (True, False)
         for do_dry_run in runs:
+            if dry_run:
+                prefix = "Simulating an attempt"
+            else:
+                prefix = "Attempting"
             try:
                 if pull_or_push == "pull":
-                    SYNC_LOGGER.info(
-                        "Attempting to pull changes from"
-                        f" {render_remote(alias, remote_uri)}"
+                    SYNC_LOGGER.log(
+                        IMPORTANT,
+                        f"{prefix} to pull changes from %s",
+                        render_remote(alias, remote_uri),
                     )
                     remote_chest = remote_uri._replace(
                         path=urlparse(
                             (
                                 fs.ender_chest_folder(
                                     path_from_uri(remote_uri),
                                     check_exists=False,
@@ -177,46 +184,43 @@
                             ).as_uri()
                         ).path
                     )
                     pull(
                         remote_chest,
                         minecraft_root,
                         exclude=[
-                            os.path.join(
-                                fs.ENDER_CHEST_FOLDER_NAME, fs.ENDER_CHEST_CONFIG_NAME
-                            ),
-                            os.path.join(fs.ENDER_CHEST_FOLDER_NAME, ".*"),
+                            *this_chest.do_not_sync,
                             *(sync_kwargs.pop("exclude", None) or ()),
                         ],
                         dry_run=do_dry_run,
                         **sync_kwargs,
                     )
                 else:
-                    SYNC_LOGGER.info(
-                        f"Attempting to push changes to {render_remote(alias, remote_uri)}"
+                    SYNC_LOGGER.log(
+                        IMPORTANT,
+                        f"{prefix} to push changes"
+                        f" to {render_remote(alias, remote_uri)}",
                     )
                     local_chest = fs.ender_chest_folder(minecraft_root)
                     push(
                         local_chest,
                         remote_uri,
                         exclude=[
-                            os.path.join(
-                                fs.ENDER_CHEST_FOLDER_NAME, fs.ENDER_CHEST_CONFIG_NAME
-                            ),
-                            os.path.join(fs.ENDER_CHEST_FOLDER_NAME, ".*"),
+                            *this_chest.do_not_sync,
                             *(sync_kwargs.pop("exclude", None) or ()),
                         ],
                         dry_run=do_dry_run,
                         **sync_kwargs,
                     )
             except (
                 FileNotFoundError,
                 ValueError,
                 NotImplementedError,
                 TimeoutError,
+                RuntimeError,
             ) as sync_fail:
                 SYNC_LOGGER.warning(
                     f"Could not sync changes with {render_remote(alias, remote_uri)}:"
                     f"\n  {sync_fail}"
                 )
                 break
             if do_dry_run == runs[-1]:
```

### Comparing `enderchest-0.1.0rc6/enderchest/shulker_box.py` & `enderchest-0.1.1rc1/enderchest/shulker_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """Specification and configuration of a shulker box"""
-import datetime as dt
 import fnmatch
 import os
-from configparser import ConfigParser, ParsingError
-from io import StringIO
 from pathlib import Path
-from typing import NamedTuple
+from typing import Any, NamedTuple
 
 import semantic_version as semver
 
+from . import config as cfg
 from . import filesystem as fs
-from ._version import get_versions
-from .instance import InstanceSpec
+from .instance import InstanceSpec, normalize_modloader
 from .loggers import CRAFT_LOGGER
 
+_DEFAULT_PRIORITY = 0
+_DEFAULT_LINK_DEPTH = 2
+_DEFAULT_DO_NOT_LINK = ("shulkerbox.cfg", ".DS_Store")
+
 
 class ShulkerBox(NamedTuple):
-    """Specification of a ShulkerBox
+    """Specification of a shulker box
 
     Parameters
     ----------
     priority : int
         The priority for linking assets in the shulker box (higher priority
-        shulkers are linked last)
+        boxes are linked last)
     name : str
-        The name of the shulker box (which is incidetentally used to break
+        The name of the shulker box (which is incidentally used to break
         priority ties)
     root : Path
         The path to the root of the shulker box
     match_criteria : list-like of tuples
         The parameters for matching instances to this shulker box. Each element
         consists of:
 
@@ -42,28 +43,32 @@
     max_link_depth : int, optional
         By default, non-root-level folders (that is, folders inside of folders)
         will be treated as files for the purpose of linking. Put another way,
         only files with a depth of 2 or less from the shulker root will be
         linked. This behavior can be overridden by explicitly setting
         the `max_link_depth` value, but **this feature is highly experimental**,
         so use it at your own risk.
+    do_not_link : list-like of str, optional
+        Glob patterns of files that should not be linked. By default, this list
+        comprises `shulkerbox.cfg` and `.DS_Store` (for all you mac gamers).
 
     Notes
     -----
     A shulker box specification is immutable, so making changes (such as
-    updating the match critera) can only be done on copies created via the
+    updating the match criteria) can only be done on copies created via the
     `_replace` method, inherited from the NamedTuple parent class.
     """
 
     priority: int
     name: str
     root: Path
     match_criteria: tuple[tuple[str, tuple[str, ...]], ...]
     link_folders: tuple[str, ...]
-    max_link_depth: int = 2
+    max_link_depth: int = _DEFAULT_LINK_DEPTH
+    do_not_link: tuple[str, ...] = _DEFAULT_DO_NOT_LINK
 
     @classmethod
     def from_cfg(cls, config_file: Path) -> "ShulkerBox":
         """Parse a shulker box from its config file
 
         Parameters
         ----------
@@ -82,79 +87,81 @@
         FileNotFoundError
             If there is no config file at the specified location
         """
         priority = 0
         max_link_depth = 2
         root = config_file.parent
         name = root.name
-        parser = ConfigParser(
-            allow_no_value=True, inline_comment_prefixes=(";",), interpolation=None
-        )
-        parser.optionxform = str  # type: ignore
-        try:
-            assert parser.read(config_file)
-        except ParsingError as bad_cfg:
-            raise ValueError(f"Could not parse {config_file}") from bad_cfg
-        except AssertionError:
-            raise FileNotFoundError(f"Could not open {config_file}")
+        config = cfg.read_cfg(config_file)
 
         match_criteria: dict[str, tuple[str, ...]] = {}
 
-        for section in parser.sections():
+        for section in config.sections():
             normalized = (
                 section.lower().replace(" ", "").replace("-", "").replace("_", "")
             )
             if normalized.endswith("s"):
                 normalized = normalized[:-1]  # lazy de-pluralization
             if normalized in ("linkfolder", "folder"):
                 normalized = "link-folders"
+            if normalized in ("donotlink",):
+                normalized = "do-not-link"
             if normalized in ("minecraft", "version", "minecraftversion"):
                 normalized = "minecraft"
             if normalized in ("modloader", "loader"):
                 normalized = "modloader"
             if normalized in ("instance", "tag", "host"):
                 normalized += "s"  # lazy re-pluralization
 
             if normalized == "propertie":  # lulz
                 # TODO check to make sure properties hasn't been read before
                 # most of this section gets ignored
-                priority = parser[section].getint("priority", 0)
-                max_link_depth = parser[section].getint("max-link-depth", 2)
+                priority = config[section].getint("priority", _DEFAULT_PRIORITY)
+                max_link_depth = config[section].getint(
+                    "max-link-depth", _DEFAULT_LINK_DEPTH
+                )
                 # TODO: support specifying filters (and link-folders) in the properties section
                 continue
-            if normalized in match_criteria.keys():
+            if normalized in match_criteria:
                 raise ValueError(f"{config_file} specifies {normalized} more than once")
 
             if normalized == "minecraft":
                 minecraft_versions = []
-                for key, value in parser[section].items():
+                for key, value in config[section].items():
                     if value is None:
                         minecraft_versions.append(key)
                     elif key.lower().strip().startswith("version"):
                         minecraft_versions.append(value)
                     else:  # what happens if you specify ">=1.19" or "=1.12"
                         minecraft_versions.append("=".join((key, value)))
-                match_criteria["minecraft"] = tuple(minecraft_versions)
+                match_criteria[normalized] = tuple(minecraft_versions)
+            elif normalized == "modloader":
+                modloaders: set[str] = set()
+                for loader in config[section].keys():
+                    modloaders.update(normalize_modloader(loader))
+                match_criteria[normalized] = tuple(sorted(modloaders))
             else:
                 # really hoping delimiter shenanigans doesn't show up anywhere else
-                match_criteria[normalized] = tuple(parser[section].keys())
+                match_criteria[normalized] = tuple(config[section].keys())
 
         link_folders = match_criteria.pop("link-folders", ())
+        do_not_link = match_criteria.pop("do-not-link", _DEFAULT_DO_NOT_LINK)
 
         return cls(
             priority,
             name,
             root,
             tuple(match_criteria.items()),
             link_folders,
             max_link_depth=max_link_depth,
+            do_not_link=do_not_link,
         )
 
     def write_to_cfg(self, config_file: Path | None = None) -> str:
-        """Write this shulker's configuration to INI
+        """Write this box's configuration to INI
 
         Parameters
         ----------
         config_file : Path, optional
             The path to the config file, assuming you'd like to write the
             contents to file
 
@@ -163,43 +170,29 @@
         str
             An INI-syntax rendering of this shulker box's config
 
         Notes
         -----
         The "root" attribute is ignored for this method
         """
-        config = ConfigParser(allow_no_value=True, interpolation=None)
-        config.optionxform = str  # type: ignore
-        config.add_section("properties")
-        config.set("properties", "priority", str(self.priority))
-        if self.max_link_depth != 2:
-            config.set("properties", "max-link-depth", str(self.max_link_depth))
-        config.set("properties", "last_modified", dt.datetime.now().isoformat(sep=" "))
-        config.set(
-            "properties", "generated_by_enderchest_version", get_versions()["version"]
+        properties: dict[str, Any] = {"priority": self.priority}
+        if self.max_link_depth != _DEFAULT_LINK_DEPTH:
+            properties["max-link-depth"] = self.max_link_depth
+
+        config = cfg.dumps(
+            os.path.join(self.name, fs.SHULKER_BOX_CONFIG_NAME),
+            properties,
+            **dict(self.match_criteria),
+            link_folders=self.link_folders,
+            do_not_link=self.do_not_link,
         )
 
-        for condition, values in self.match_criteria:
-            config.add_section(condition)
-            for value in values:
-                config.set(condition, value)
-
-        config.add_section("link-folders")
-        for folder in self.link_folders:
-            config.set("link-folders", folder)
-
-        buffer = StringIO()
-        buffer.write(f"; {os.path.join(self.name, fs.SHULKER_BOX_CONFIG_NAME)}\n")
-        config.write(buffer)
-        buffer.seek(0)  # rewind
-
         if config_file:
-            config_file.write_text(buffer.read())
-            buffer.seek(0)
-        return buffer.read()
+            config_file.write_text(config)
+        return config
 
     def matches(self, instance: InstanceSpec) -> bool:
         """Determine whether the shulker box matches the given instance
 
         Parameters
         ----------
         instance : InstanceSpec
@@ -224,23 +217,17 @@
                         if fnmatch.filter(
                             [tag.lower() for tag in instance.tags], value.lower()
                         ):
                             break
                     else:
                         return False
                 case "modloader":
-                    normalized: list[str] = sum(
-                        [_normalize_modloader(value) for value in values], []
-                    )
-                    for value in normalized:
-                        if fnmatch.filter(
-                            [
-                                loader.lower()
-                                for loader in _normalize_modloader(instance.modloader)
-                            ],
+                    for value in values:
+                        if fnmatch.fnmatchcase(
+                            instance.modloader.lower(),
                             value.lower(),
                         ):
                             break
                     else:
                         return False
                 case "minecraft":
                     for value in values:
@@ -277,47 +264,14 @@
                     fnmatch.fnmatchcase(hostname.lower(), host_spec.lower())
                     for host_spec in values
                 ):
                     return False
         return True
 
 
-def _normalize_modloader(loader: str | None) -> list[str]:
-    """Implement common modloader aliases
-
-    Parameters
-    ----------
-    loader : str
-        User-provided modloader name
-
-    Returns
-    -------
-    list of str
-        The modloader values that should be checked against to match the user's
-        intent
-    """
-    if loader is None:  # this would be from the instance spec
-        return [""]
-    match loader.lower().replace(" ", "").replace("-", "").replace("_", "").replace(
-        "/", ""
-    ):
-        case "none" | "vanilla":
-            return [""]
-        case "fabric" | "fabricloader":
-            return ["Fabric Loader"]
-        case "quilt" | "quiltloader":
-            return ["Quilt Loader"]
-        case "fabricquilt" | "quiltfabric" | "fabriclike" | "fabriccompatible":
-            return ["Fabric Loader", "Quilt Loader"]
-        case "forge" | "forgeloader" | "minecraftforge":
-            return ["Forge"]
-        case _:
-            return [loader]
-
-
 def _matches_version(version_spec: str, version_string: str) -> bool:
     """Determine whether a version spec matches a version string, taking into
     account that neither users nor Mojang rigidly follow semver (or at least
     PEP440)
 
     Parameters
     ----------
```

### Comparing `enderchest-0.1.0rc6/enderchest/sync/file.py` & `enderchest-0.1.1rc1/enderchest/sync/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 
     ignore = ignore_patterns(*exclude)
     SYNC_LOGGER.debug(f"Ignoring patterns: {exclude}")
 
     destination_path = destination_folder / source_path.name
     if destination_path.exists():
         if destination_path.is_symlink():
-            SYNC_LOGGER.log(log_level, f"Removing symlink {destination_path}")
+            SYNC_LOGGER.log(log_level, "Removing symlink %s", destination_path)
             if not dry_run:
                 destination_path.unlink()
         elif destination_path.is_dir():
             clean(destination_path, ignore, dry_run)
         else:
-            SYNC_LOGGER.log(log_level, f"Deleting {destination_path}")
+            SYNC_LOGGER.log(log_level, "Deleting %s", destination_path)
             if not dry_run:
                 destination_path.unlink()
 
     if source_path.exists():
         SYNC_LOGGER.log(log_level, f"Copying {source_path} into {destination_folder}")
         if not dry_run:
             if source_path.is_dir():
@@ -197,16 +197,16 @@
     if not source_path.exists():
         SYNC_LOGGER.warning(
             f"{source_path} does not exist"
             " this will end up just deleting the local copy."
         )
     if unsupported_kwargs:
         SYNC_LOGGER.debug(
-            "The following command-line options are ignored for this protocol:\n"
-            + "\n".join("  {}: {}".format(*item) for item in unsupported_kwargs.items())
+            "The following command-line options are ignored for this protocol:\n%s",
+            "\n".join("  {}: {}".format(*item) for item in unsupported_kwargs.items()),
         )
 
     copy(source_path, destination_folder, exclude, dry_run)
 
 
 def push(
     local_path: Path,
@@ -256,12 +256,12 @@
     if not source_path.exists():
         SYNC_LOGGER.warning(
             f"{source_path} does not exist:"
             " this will end up just deleting the remote copy."
         )
     if unsupported_kwargs:
         SYNC_LOGGER.debug(
-            "The following command-line options are ignored for this protocol:\n"
-            + "\n".join("  {}: {}".format(*item) for item in unsupported_kwargs.items())
+            "The following command-line options are ignored for this protocol:\n%s",
+            "\n".join("  {}: {}".format(*item) for item in unsupported_kwargs.items()),
         )
 
     copy(source_path, destination_folder, exclude, dry_run)
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/conftest.py` & `enderchest-0.1.1rc1/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_cli.py` & `enderchest-0.1.1rc1/enderchest/test/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,21 +76,21 @@
             ["enderchest", *self.action.split(), *self.required_args, "--root", "/home"]
         )
         assert root == Path("/home")
 
     @pytest.mark.parametrize(
         "verbosity_flag, expected_verbosity",
         (
-            ("-v", logging.DEBUG),
-            ("-q", logging.WARNING),
-            ("--verbose", logging.DEBUG),
-            ("--quiet", logging.WARNING),
-            ("-vv", -1),
-            ("-qq", logging.ERROR),
-            ("-vvqvqqvqv", logging.DEBUG),
+            ("-v", logging.DEBUG - 9),
+            ("-q", logging.WARNING - 9),
+            ("--verbose", logging.DEBUG - 9),
+            ("--quiet", logging.WARNING - 9),
+            ("-vv", -9),
+            ("-qq", logging.ERROR - 9),
+            ("-vvqvqqvqv", logging.DEBUG - 9),
         ),
     )
     def test_altering_verbosity(self, verbosity_flag, expected_verbosity):
         _, _, log_level, _ = cli.parse_args(
             ["enderchest", *self.action.split(), verbosity_flag, *self.required_args]
         )
 
@@ -204,22 +204,40 @@
         def mock_place(path, **kwargs):
             place_log.append((path, kwargs))
 
         monkeypatch.setattr(place, "place_ender_chest", mock_place)
 
         yield place_log
 
-    def test_remove_broken_links_by_default(self):
-        *_, options = cli.parse_args(["enderchest", "place", "/home"])
-        assert options["cleanup"] is True
-
-    @pytest.mark.parametrize("flag", ("-k", "--keep-broken"))
-    def test_keep_broken_links(self, flag):
-        *_, options = cli.parse_args(["enderchest", "place", "/home", flag])
-        assert options["cleanup"] is False
+    @pytest.mark.parametrize("option", ("keep_broken_links", "keep_stale_links"))
+    def test_remove_broken_links_by_default(self, option, place_log):
+        action, minecraft_root, _, options = cli.parse_args(
+            ["enderchest", "place", "/home"]
+        )
+        action(minecraft_root, **options)
+        assert len(place_log) == 1
+        assert place_log[0][1][option] is False
+
+    @pytest.mark.parametrize("flag", ("-k", "--keep-stale-links"))
+    def test_keep_stale_links(self, flag, place_log):
+        action, minecraft_root, _, options = cli.parse_args(
+            ["enderchest", "place", "/home", flag]
+        )
+        action(minecraft_root, **options)
+        assert len(place_log) == 1
+        assert place_log[0][1]["keep_stale_links"] is True
+
+    @pytest.mark.parametrize("flag", ("-kk", "--keep-broken-links"))
+    def test_keep_broken_links(self, flag, place_log):
+        action, minecraft_root, _, options = cli.parse_args(
+            ["enderchest", "place", "/home", flag]
+        )
+        action(minecraft_root, **options)
+        assert len(place_log) == 1
+        assert place_log[0][1]["keep_broken_links"] is True
 
     def test_prompt_on_error_by_default(self):
         *_, options = cli.parse_args(["enderchest", "place"])
         assert (
             options["errors"],
             options["stop_at_first_failure"],
             options["ignore_errors"],
@@ -241,32 +259,51 @@
         ids=("--ignore-errors", "--errors=ignore"),
     )
     def test_ignore_errors(self, place_log, flags):
         action, *_, options = cli.parse_args(["enderchest", "place", *flags])
         action(Path(), **options)
         assert place_log[0][1]["error_handling"] == "ignore"
 
+    def test_absolute_path_links_is_the_default(self, place_log):
+        action, *_, options = cli.parse_args(["enderchest", "place"])
+        action(Path(), **options)
+        assert place_log[0][1]["relative"] is False
+
+    @pytest.mark.parametrize(
+        "flag, expected",
+        (("-a", False), ("--absolute", False), ("-r", True), ("--relative", True)),
+    )
+    def test_explicitly_specify_abs_or_rel(self, place_log, flag, expected):
+        action, *_, options = cli.parse_args(["enderchest", "place"])
+        action(Path(), **options)
+        assert place_log[0][1]["relative"] is False
+
 
 class TestGather(ActionTestSuite):
     action = "gather minecraft"
     required_args = ("~",)
 
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
-    def test_gather_requires_at_least_one_search_path(self, with_root):
+    def test_gather_requires_at_least_one_search_path(self, with_root, capsys):
         more_args = ("--root", "/minecraft") if with_root else ()
         with pytest.raises(SystemExit):
             cli.parse_args(["enderchest", *self.action.split(), *more_args])
 
+        _ = capsys.readouterr()  # suppress outputs
+
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
-    def test_single_arg_interpreted_as_search_path(self, with_root):
+    def test_single_arg_interpreted_as_search_path(self, with_root, capsys):
         more_args = ("--root", ".") if with_root else ()
 
         _, root, _, options = cli.parse_args(
             ["enderchest", *self.action.split(), *more_args, "~"]
         )
+
+        _ = capsys.readouterr()  # suppress outputs
+
         assert (root.resolve(), options["search_paths"]) == (
             Path(".").resolve(),
             [Path("~")],
         )
 
     def test_first_arg_interpreted_as_root(self):  # I actually really don't like this
         _, root, _, options = cli.parse_args(
@@ -287,19 +324,21 @@
 
 
 class TestGatherRemote(ActionTestSuite):
     action = "gather enderchests"
     required_args = ("sftp://openbagtwo@steamdeck/home/deck",)
 
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
-    def test_gather_requires_at_least_one_remote(self, with_root):
+    def test_gather_requires_at_least_one_remote(self, with_root, capsys):
         more_args = ("--root", "/minecraft") if with_root else ()
         with pytest.raises(SystemExit):
             cli.parse_args(["enderchest", *self.action.split(), *more_args])
 
+        _ = capsys.readouterr()  # suppress outputs
+
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
     def test_single_arg_interpreted_as_remote(self, with_root):
         more_args = ("--root", ".") if with_root else ()
 
         _, root, _, options = cli.parse_args(
             [
                 "enderchest",
@@ -330,14 +369,19 @@
                 "sftp://openbagtwo@steamdeck/home/deck",
                 "ipoac://birdhouse/your/soul",
                 "sneakernet://123.fake.street/mailbox",
             ],
         )
 
 
+class TestInstanceInventory(ActionTestSuite):
+    action = "inventory minecraft"
+    required_args = ("cherry grove",)
+
+
 class TestShulkerInventory(ActionTestSuite):
     action = "inventory shulker_box"
     required_args = ("nombre",)
 
 
 class TestOpen:
     action = "open"
@@ -353,14 +397,44 @@
 
         action, root, _, kwargs = cli.parse_args(["enderchest", *self.action.split()])
         action(root, **kwargs)
 
         assert len(sync_log) == 1
         assert sync_log[0][1] == self.op
 
+    @pytest.mark.parametrize(
+        "verbosity_flag, expected_verbosity",
+        (
+            ("-v", 1),
+            ("-q", -1),
+            ("--verbose", 1),
+            ("--quiet", -1),
+            ("-vv", 2),
+            ("-qq", -2),
+            ("-vvqvqqvqv", 1),
+        ),
+    )
+    def test_verbosity_modifier_is_passed_to_op(
+        self, monkeypatch, verbosity_flag, expected_verbosity
+    ):
+        sync_log: list[tuple[str, str, dict]] = []
+
+        def mock_sync(root, op, **kwargs):
+            sync_log.append((root, op, kwargs))
+
+        monkeypatch.setattr(remote, "sync_with_remotes", mock_sync)
+
+        action, root, _, kwargs = cli.parse_args(
+            ["enderchest", *self.action.split(), verbosity_flag]
+        )
+        action(root, **kwargs)
+
+        assert len(sync_log) == 1
+        assert sync_log[0][2]["verbosity"] == expected_verbosity
+
     def test_dry_run_is_false_by_default(self, monkeypatch):
         sync_log: list[tuple[str, str, dict]] = []
 
         def mock_sync(root, op, **kwargs):
             sync_log.append((root, op, kwargs))
 
         monkeypatch.setattr(remote, "sync_with_remotes", mock_sync)
@@ -399,13 +473,14 @@
 
         assert len(sync_log) == 1
         assert sync_log[0][2] == {
             "dry_run": True,
             "timeout": 15,
             "sync_confirm_wait": 0,
             "exclude": ["private", "*.secret"],
+            "verbosity": 0,
         }
 
 
 class TestClose(TestOpen):
     action = "close"
     op = "push"
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_craft.py` & `enderchest-0.1.1rc1/enderchest/test/test_craft.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,24 @@
-"""Tests for setting up folders and files"""
+"""Tests for setting up EnderChests and shulker boxes"""
 import logging
 import os
 from pathlib import Path
 from typing import Any
-from urllib.parse import urlparse
 
 import pytest
 
 from enderchest import EnderChest, ShulkerBox, craft
 from enderchest import filesystem as fs
 from enderchest.enderchest import create_ender_chest
-from enderchest.gather import load_ender_chest, load_shulker_boxes
-from enderchest.shulker_box import (
-    DEFAULT_SHULKER_FOLDERS,
-    STANDARD_LINK_FOLDERS,
-    create_shulker_box,
-)
+from enderchest.gather import load_ender_chest
+from enderchest.shulker_box import DEFAULT_SHULKER_FOLDERS, STANDARD_LINK_FOLDERS
 
 from . import utils
 
 
-class TestConfigWriting:
-    def test_shulker_box_config_roundtrip(self, minecraft_root):
-        original_shulker = ShulkerBox(
-            3,
-            "original",
-            minecraft_root / "EnderChest" / "original",
-            match_criteria=(
-                ("minecraft", (">=1.12,<2.0",)),
-                ("modloader", ("*",)),
-                ("tags", ("aether", "optifine")),
-                ("instances", ("aether legacy", "Paradise Lost")),
-            ),
-            link_folders=("screenshots", "logs"),
-        )
-
-        utils.pre_populate_enderchest(minecraft_root / "EnderChest")
-
-        create_shulker_box(minecraft_root, original_shulker)
-
-        parsed_shulkers = load_shulker_boxes(minecraft_root)
-
-        assert parsed_shulkers == [original_shulker]
-
-    def test_ender_chest_config_roundtrip(self, tmpdir):
-        (tmpdir / "EnderChest").mkdir()
-
-        original_ender_chest = EnderChest(
-            urlparse(Path(tmpdir).absolute().as_uri()),
-            name="tester",
-            remotes=[
-                "irc://you@irl/home/upstairs",
-                ("file:///lockbox", "undisclosed location"),
-            ],
-            instances=utils.TESTING_INSTANCES,
-        )
-
-        original_ender_chest.write_to_cfg(
-            Path(tmpdir) / "EnderChest" / "enderchest.cfg"
-        )
-
-        parsed_ender_chest = EnderChest.from_cfg(
-            Path(tmpdir) / "EnderChest" / "enderchest.cfg"
-        )
-
-        assert parsed_ender_chest == original_ender_chest
-
-
 class TestEnderChestCrafting:
     def test_ender_chest_aborts_right_away_if_minecraft_root_doesnt_exist(
         self, monkeypatch, minecraft_root
     ):
         def mock_prompt(root) -> Any:
             raise AssertionError("I was not to be called.")
 
@@ -187,48 +135,78 @@
         error_log = "\n".join(
             record.msg for record in caplog.records if record.levelname == "ERROR"
         )
         assert "There is already an EnderChest installed" in error_log
 
         assert fs.ender_chest_config(minecraft_root).read_text() == original_config
 
-    def test_craft_chest_from_config(self, minecraft_root, home, caplog):
+    @pytest.mark.parametrize("root_type", ("absolute", "relative"))
+    def test_craft_chest_from_config(
+        self,
+        minecraft_root,
+        home,
+        caplog,
+        monkeypatch,
+        capsys,
+        root_type,
+    ):
+        if root_type == "absolute":
+            root = minecraft_root
+        else:
+            root = Path(minecraft_root.name)
+            monkeypatch.chdir(minecraft_root.parent)
+
         # we'll be testing overwriting
         create_ender_chest(
-            minecraft_root,
+            root,
             EnderChest(
                 "sftp://openbagtwo@battlestation" + minecraft_root.absolute().as_posix()
             ),
         )
 
+        never = utils.scripted_prompt(["no"])
+        monkeypatch.setattr("builtins.input", never)
+
         craft.craft_ender_chest(
             minecraft_root,
             instance_search_paths=(minecraft_root / "instances", home),
             remotes=("rsync://deck@steamdeck/home/deck/minecraft",),
             overwrite=True,
         )
 
+        _ = capsys.readouterr()  # suppress outputs
+
         assert not [record for record in caplog.records if record.levelname == "ERROR"]
 
         chest = load_ender_chest(minecraft_root)
         assert len(chest.instances) == 4
         assert len(chest.remotes) == 1
 
+    @pytest.mark.parametrize("root_type", ("absolute", "relative"))
     def test_giving_default_responses_results_in_the_expected_chest(
         self,
         monkeypatch,
         minecraft_root,
         home,
         capsys,
         caplog,
+        root_type,
     ):
-        script_reader = utils.scripted_prompt([""] * 7)
+        if root_type == "absolute":
+            root = minecraft_root
+            n_responses = 8
+        else:
+            root = Path(minecraft_root.name)
+            monkeypatch.chdir(minecraft_root.parent)
+            n_responses = 9  # because now cwd != minecraft root
+
+        script_reader = utils.scripted_prompt([""] * n_responses)
         monkeypatch.setattr("builtins.input", script_reader)
 
-        chest = craft.specify_ender_chest_from_prompt(minecraft_root)
+        chest = craft.specify_ender_chest_from_prompt(root)
 
         _ = capsys.readouterr()  # suppress outputs
 
         assert not [record for record in caplog.records if record.levelname == "ERROR"]
 
         assert len(chest.instances) == 4
         assert len(chest.remotes) == 0
@@ -418,15 +396,15 @@
             ShulkerBox(0, "tester", Path("ignored"), (), ()), []
         )
 
         _ = capsys.readouterr()
 
         assert shulker_box.match_criteria == (
             ("minecraft", ("22w14infinite",)),
-            ("modloader", ("None",)),
+            ("modloader", ("",)),
             ("tags", ("*",)),
         )
 
         # make sure all responses were used
         with pytest.raises(StopIteration):
             script_reader()
 
@@ -481,20 +459,20 @@
             ShulkerBox(0, "tester", Path("ignored"), (), ()), utils.TESTING_INSTANCES
         )
 
         _ = capsys.readouterr()
 
         assert shulker_box.match_criteria == (
             ("minecraft", ("1.19",)),
-            ("modloader", ("None", "Fabric Loader", "Quilt Loader")),
+            ("modloader", ("", "Fabric Loader", "Quilt Loader")),
             ("tags", ("vanilla*",)),
         )
 
         # check that it was showing the right instances right up until the end
-        assert caplog.records[-1].msg == (
+        assert caplog.records[-1].msg % caplog.records[-1].args == (
             """Filters match the instances:
   - official
   - Chest Boat"""
         )
 
         # make sure all responses were used
         with pytest.raises(StopIteration):
@@ -517,15 +495,15 @@
 
         _ = capsys.readouterr()
 
         assert shulker_box.match_criteria == (
             ("instances", ("abra", "kadabra", "alakazam")),
         )
 
-        assert caplog.records[-1].msg == (
+        assert caplog.records[-1].msg % caplog.records[-1].args == (
             """You specified the following instances:
   - abra
   - kadabra
   - alakazam"""
         )
 
         # make sure all responses were used
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_instance.py` & `enderchest-0.1.1rc1/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_place.py` & `enderchest-0.1.1rc1/enderchest/test/test_place.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,14 +68,22 @@
 
         yield
 
         # check on teardown that all those "do_not_touch" files are untouched
         for path, contents in do_not_touch.items():
             assert path.read_text() == contents
 
+    @pytest.mark.parametrize("relative", (True, False), ids=("relative", "absolute"))
+    @utils.parametrize_over_instances("official", "axolotl")
+    def test_respects_the_relative_parameter(self, minecraft_root, instance, relative):
+        place.place_ender_chest(minecraft_root, relative=relative)
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+
+        assert (instance_folder / "logs").readlink().is_absolute() is (not relative)
+
     @utils.parametrize_over_instances("official", "axolotl")
     def test_place_replaces_empty_folders(self, minecraft_root, instance):
         place.place_ender_chest(minecraft_root)
         instance_folder = utils.resolve(instance.root, minecraft_root)
 
         assert (instance_folder / "logs").resolve() == (
             minecraft_root / "EnderChest" / "global" / "logs"
@@ -94,14 +102,29 @@
         assert not (instance_folder / "config").is_symlink()
 
         assert (instance_folder / "config" / "iris.properties").resolve() == (
             minecraft_root / "EnderChest" / "global" / "config" / "iris.properties"
         )
 
     @utils.parametrize_over_instances("official", "axolotl")
+    def test_place_doesnt_choke_on_relative_root(
+        self, minecraft_root, instance, monkeypatch
+    ):
+        monkeypatch.chdir(minecraft_root.parent)
+        place.place_ender_chest(Path(minecraft_root.name))
+
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+
+        assert not (instance_folder / "config").is_symlink()
+
+        assert (instance_folder / "config" / "iris.properties").resolve() == (
+            minecraft_root / "EnderChest" / "global" / "config" / "iris.properties"
+        )
+
+    @utils.parametrize_over_instances("official", "axolotl")
     def test_place_is_able_to_place_root_level_files(self, minecraft_root, instance):
         place.place_ender_chest(minecraft_root)
 
         instance_folder = utils.resolve(instance.root, minecraft_root)
 
         assert (
             instance_folder / "usercache.json"
@@ -115,14 +138,30 @@
     def test_does_not_place_shulker_config(self, minecraft_root, instance):
         place.place_ender_chest(minecraft_root)
 
         instance_folder = utils.resolve(instance.root, minecraft_root)
 
         assert not (instance_folder / fs.SHULKER_BOX_CONFIG_NAME).exists()
 
+    @utils.parametrize_over_instances("bee")
+    def test_shulker_configs_can_be_placed_if_you_really_want(
+        self, minecraft_root, instance
+    ):
+        # it's explicitly overridden in the forge config
+        utils.pre_populate_enderchest(
+            minecraft_root / "EnderChest", utils.OPTIFINE_SHULKER
+        )
+        place.place_ender_chest(minecraft_root)
+
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+
+        assert (
+            instance_folder / fs.SHULKER_BOX_CONFIG_NAME
+        ).resolve() == fs.shulker_box_config(minecraft_root, "optifine")
+
     @utils.parametrize_over_instances("official", "axolotl")
     def test_link_folder_can_be_a_symlink(self, minecraft_root, instance):
         place.place_ender_chest(minecraft_root)
 
         instance_folder = utils.resolve(instance.root, minecraft_root)
 
         # the counterpoint to the whole "one assertion per test" rule--this
@@ -178,18 +217,88 @@
         self, minecraft_root, instance
     ):
         instance_folder = utils.resolve(instance.root, minecraft_root)
         broken_link = instance_folder / "shaderpacks" / "Seuss CitH.zip.txt"
         broken_link.symlink_to(minecraft_root / "i-do-not-exist.txt")
         assert broken_link in broken_link.parent.iterdir()
 
-        place.place_ender_chest(minecraft_root, cleanup=False)
+        place.place_ender_chest(minecraft_root, keep_broken_links=True)
 
         assert broken_link in broken_link.parent.iterdir()
 
+    @pytest.mark.parametrize("link_type", ("absolute", "relative"))
+    @utils.parametrize_over_instances("official", "axolotl")
+    def test_place_cleans_up_stale_symlinks_by_default(
+        self, minecraft_root, instance, link_type
+    ):
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+        old_box = fs.shulker_box_root(minecraft_root, "Old Man Shulker")
+        old_box.mkdir()
+        old_file = old_box / "i-do-exist.txt"
+        old_file.write_text("Hello there\n")
+
+        stale_link = instance_folder / "old-file.txt"
+        if link_type == "absolute":
+            stale_link.symlink_to(old_file)
+        else:
+            stale_link.symlink_to(os.path.relpath(old_file, stale_link.parent))
+
+        place.place_ender_chest(minecraft_root)
+
+        assert stale_link not in stale_link.parent.iterdir()
+
+        # but make sure the original file is okay
+        assert old_file.read_text() == "Hello there\n"
+
+    @pytest.mark.parametrize("link_type", ("absolute", "relative"))
+    @utils.parametrize_over_instances("official", "axolotl")
+    def test_place_will_not_remove_links_pointing_outside_of_enderchest(
+        self,
+        minecraft_root,
+        instance,
+        link_type,
+    ):
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+        old_file = minecraft_root / "workspace" / "i-do-exist.txt"
+        old_file.write_text("Hello there\n")
+
+        stale_link = instance_folder / "old_file.txt"
+        if link_type == "absolute":
+            stale_link.symlink_to(old_file)
+        else:
+            stale_link.symlink_to(os.path.relpath(old_file, stale_link.parent))
+
+        place.place_ender_chest(minecraft_root)
+
+        assert stale_link in stale_link.parent.iterdir()
+
+    @pytest.mark.parametrize("link_type", ("absolute", "relative"))
+    @utils.parametrize_over_instances("official", "axolotl")
+    def test_place_can_be_told_to_leave_stale_links_alone(
+        self,
+        minecraft_root,
+        instance,
+        link_type,
+    ):
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+        old_box = fs.shulker_box_root(minecraft_root, "Old Man Shulker")
+        old_box.mkdir()
+        old_file = old_box / "i-do-exist.txt"
+        old_file.write_text("Hello there")
+
+        stale_link = instance_folder / "old-file.txt"
+        if link_type == "absolute":
+            stale_link.symlink_to(old_file)
+        else:
+            stale_link.symlink_to(os.path.relpath(old_file, stale_link.parent))
+
+        place.place_ender_chest(minecraft_root, keep_stale_links=True)
+
+        assert stale_link in stale_link.parent.iterdir()
+
     @utils.parametrize_over_instances("official", "axolotl")
     def test_place_will_not_overwrite_a_non_empty_folder(
         self, minecraft_root, instance, caplog
     ):
         instance_folder = utils.resolve(instance.root, minecraft_root)
         existing_file = instance_folder / "screenshots" / "thumbs.db"
         existing_file.write_text("opposable")
@@ -375,35 +484,74 @@
         assert self.matchall(tag_matching_shulker) == [
             "official",
             "axolotl",
             "Chest Boat",
         ]
 
     def test_loader_matching_is_case_insensitive(self):
+        # though in this case the values would have been normalized
         loader_matching_shulker = ShulkerBox(
             0,
             "forge instances",
             Path("ignoreme"),
             (("modloader", ("forge",)),),
             (),
         )
 
         assert self.matchall(loader_matching_shulker) == ["bee"]
 
-    @pytest.mark.parametrize("loader_spec", ("fabric", "quilt/fabric"))
-    def test_loader_matching_maps_common_aliases(self, loader_spec):
+    def test_loader_matching_treats_empty_string_as_vanilla(self):
+        loader_matching_shulker = ShulkerBox(
+            0,
+            "Vanilla Only",
+            Path("ignoreme"),
+            (("modloader", ("",)),),
+            (),
+        )
+
+        assert self.matchall(loader_matching_shulker) == ["official", "axolotl"]
+
+    def test_loader_matching_accepts_wildcards(self):
         loader_matching_shulker = ShulkerBox(
             0,
-            "fabric instances",
+            "Everybody",
             Path("ignoreme"),
-            (("modloader", (loader_spec,)),),
+            (("modloader", ("*",)),),
             (),
         )
 
-        assert self.matchall(loader_matching_shulker) == ["Chest Boat"]
+        assert self.matchall(loader_matching_shulker) == [
+            "official",
+            "axolotl",
+            "bee",
+            "Chest Boat",
+        ]
+
+    def test_loader_checks_multi_argument(self):
+        loader_matching_shulker = ShulkerBox(
+            0,
+            "Fabric Instances",
+            Path("ignoreme"),
+            (
+                (
+                    "modloader",
+                    (
+                        "",
+                        "*bric*",
+                    ),
+                ),
+            ),
+            (),
+        )
+
+        assert self.matchall(loader_matching_shulker) == [
+            "official",
+            "axolotl",
+            "Chest Boat",
+        ]
 
     def test_explicit_version_matching(self):
         minecraft_specific_shulker = ShulkerBox(
             0,
             "votey",
             Path("ignoreme"),
             (("minecraft", ("23w13a_or_b",)),),
@@ -435,15 +583,15 @@
 
     def test_instance_must_match_all_conditions(self):
         multi_condition_shulker = ShulkerBox(
             0,
             "finnicky",
             Path("ignoreme"),
             (
-                ("modloader", ("forge", "fabric")),
+                ("modloader", ("Forge", "Fabric Loader")),
                 ("tags", ("vanilla*",)),
                 ("instances", ("official", "axolotl", "bee", "Chest Boat")),
             ),
             (),
         )
         assert self.matchall(multi_condition_shulker) == ["Chest Boat"]
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_sync.py` & `enderchest-0.1.1rc1/enderchest/test/test_sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests around file transfer functionality."""
+import logging
 import os
 import shutil
 from pathlib import Path
 from urllib.parse import urlparse
 
 import pytest
 
@@ -85,14 +86,20 @@
             ignore("wind", ("leaf", "blows")),
         ) == ({"branch"}, {"leaf"})
 
 
 class TestFileSync:
     protocol = "file"
 
+    @pytest.fixture(autouse=True)
+    def check_output_suppression(self, capfd):
+        # teardown that helps me figure out where I need to add a -q flag
+        yield
+        assert capfd.readouterr().out == ""
+
     @pytest.fixture
     def remote(self, tmp_path, minecraft_root, home):
         utils.pre_populate_enderchest(
             minecraft_root / "EnderChest", *utils.TESTING_SHULKER_CONFIGS
         )
 
         local = gather.load_ender_chest(minecraft_root)
@@ -203,27 +210,46 @@
                 minecraft_root / "EnderChest" / "1.19" / "saves" / "olam",
                 minecraft_root / "worlds" / "olam",
             ),
         ):
             path.unlink(missing_ok=True)
             path.symlink_to(target, target_is_directory=target.is_dir())
 
-    def test_create_from_remote_chest(self, remote, minecraft_root):
-        craft.craft_ender_chest(
-            minecraft_root, copy_from=remote.geturl(), overwrite=True
-        )
+    @pytest.mark.parametrize("root_type", ("absolute", "relative"))
+    def test_create_from_remote_chest(
+        self, remote, minecraft_root, monkeypatch, root_type, capfd
+    ):
+        if root_type == "absolute":
+            root = minecraft_root
+        else:
+            root = Path(minecraft_root.name)
+            monkeypatch.chdir(minecraft_root.parent)
+
+        craft.craft_ender_chest(root, copy_from=remote.geturl(), overwrite=True)
 
         assert gather.load_ender_chest_remotes(minecraft_root) == [
             (remote, "closer than you think"),
             (urlparse("ipoac://yoursoul@birdhouse/minecraft"), "birdhouse"),
         ]
 
-    def test_open_grabs_files_from_upstream(self, minecraft_root, remote):
-        gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "pull")
+        # test that the enderchest spec-fetch is quiet by default
+        assert capfd.readouterr().out == ""
+
+    @pytest.mark.parametrize("root_type", ("absolute", "relative"))
+    def test_open_grabs_files_from_upstream(
+        self, minecraft_root, remote, monkeypatch, root_type
+    ):
+        if root_type == "absolute":
+            root = minecraft_root
+        else:
+            root = Path(minecraft_root.name)
+            monkeypatch.chdir(minecraft_root.parent)
+
+        gather.update_ender_chest(root, remotes=(remote,))
+        r.sync_with_remotes(root, "pull", verbosity=-1)
         assert (
             minecraft_root / "EnderChest" / "optifine" / "mods" / "optifine.jar"
         ).read_text() == "it's okay"
         assert not (
             minecraft_root / "EnderChest" / "optifine" / "mods" / "optifine.jar"
         ).is_symlink()
 
@@ -232,59 +258,72 @@
         r.sync_with_remotes(minecraft_root, "pull", dry_run=True)
         assert not (
             minecraft_root / "EnderChest" / "optifine" / "mods" / "optifine.jar"
         ).exists()
 
     def test_open_overwrites_local_files(self, minecraft_root, remote):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "pull")
+        r.sync_with_remotes(minecraft_root, "pull", verbosity=-1)
         assert (
             minecraft_root / "EnderChest" / "vanilla" / "conflict" / "diamond.png"
         ).read_text() == "lab-grown!"
         assert not (
             minecraft_root / "EnderChest" / "vanilla" / "conflict" / "diamond.png"
         ).is_symlink()
 
     def test_open_copies_over_symlinks(self, minecraft_root, remote):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "pull")
+        r.sync_with_remotes(minecraft_root, "pull", verbosity=-1)
         assert (
             minecraft_root / "EnderChest" / "1.19" / "saves" / "olam"
         ).resolve() != (minecraft_root / "worlds" / "olam")
 
     def test_open_processes_deletions_from_upstream(self, minecraft_root, remote):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "pull")
+        r.sync_with_remotes(minecraft_root, "pull", verbosity=-1)
         assert not (minecraft_root / "EnderChest" / "global").exists()
 
-    def test_open_does_not_overwrite_enderchest(self, minecraft_root, remote):
+    def test_open_does_not_overwrite_enderchest_by_default(
+        self, minecraft_root, remote
+    ):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
         original_config = fs.ender_chest_config(minecraft_root).read_text()
-        r.sync_with_remotes(minecraft_root, "pull")
+        r.sync_with_remotes(minecraft_root, "pull", verbosity=-1)
         assert original_config == fs.ender_chest_config(minecraft_root).read_text()
 
-    def test_open_not_touch_top_level_dot_folders(self, minecraft_root, remote):
+    def test_open_not_touch_top_level_dot_folders_by_default(
+        self, minecraft_root, remote
+    ):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "pull")
+        r.sync_with_remotes(minecraft_root, "pull", verbosity=-1)
         assert (
             minecraft_root / "EnderChest" / ".git" / "log"
         ).read_text() == "i committed some stuff\n"
 
     def test_open_will_sync_dot_folders_within_a_shulker_box(
         self, minecraft_root, remote
     ):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "pull")
+        r.sync_with_remotes(minecraft_root, "pull", verbosity=-1)
         assert (
             minecraft_root / "EnderChest" / "1.19" / ".bobby" / "chunk"
         ).read_text() == "chunky\n"
 
-    def test_close_overwrites_with_changes_from_local(self, minecraft_root, remote):
-        gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "push")
+    @pytest.mark.parametrize("root_type", ("absolute", "relative"))
+    def test_close_overwrites_with_changes_from_local(
+        self, minecraft_root, remote, monkeypatch, root_type
+    ):
+        if root_type == "absolute":
+            root = minecraft_root
+        else:
+            root = Path(minecraft_root.name)
+            monkeypatch.chdir(minecraft_root.parent)
+
+        gather.update_ender_chest(root, remotes=(remote,))
+        r.sync_with_remotes(root, "push", verbosity=-1)
         assert (
             path_from_uri(remote)
             / "EnderChest"
             / "vanilla"
             / "conflict"
             / "diamond.png"
         ).read_text() == "sparkle"
@@ -300,39 +339,200 @@
             / "diamond.png"
         ).read_text() == "lab-grown!"
 
     def test_close_deletes_remote_copies_when_locals_are_deleted(
         self, minecraft_root, remote
     ):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
-        r.sync_with_remotes(minecraft_root, "push")
+        r.sync_with_remotes(minecraft_root, "push", verbosity=-1)
         assert not (path_from_uri(remote) / "EnderChest" / "optifine").exists()
 
+    def test_close_not_touch_top_level_dot_folders_by_default(
+        self, minecraft_root, remote
+    ):
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, "push", verbosity=-1)
+        assert not (path_from_uri(remote) / "EnderChest" / ".git").exists()
+
+    def test_chest_obeys_its_own_ignore_list(self, minecraft_root, remote):
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+
+        chest = gather.load_ender_chest(minecraft_root)
+        chest.do_not_sync = ["EnderChest/enderchest.cfg"]
+        chest.write_to_cfg(fs.ender_chest_config(minecraft_root))
+
+        r.sync_with_remotes(minecraft_root, "push", verbosity=-1)
+        assert (
+            path_from_uri(remote) / "EnderChest" / ".git" / "log"
+        ).read_text() == "i committed some stuff\n"
+
     def test_open_stops_at_first_successful_sync(self, minecraft_root, remote, caplog):
         gather.update_ender_chest(
             minecraft_root, remotes=(remote, "prayer://unreachable")
         )
-        r.sync_with_remotes(minecraft_root, "pull")
+        r.sync_with_remotes(minecraft_root, "pull", verbosity=-1)
         warnings = [
             record.msg for record in caplog.records if record.levelname == "WARNING"
         ]
 
         assert len(warnings) == 0
 
     def test_close_will_attempt_to_push_to_all(self, minecraft_root, remote, caplog):
         gather.update_ender_chest(
             minecraft_root, remotes=(remote, "prayer://unreachable")
         )
-        r.sync_with_remotes(minecraft_root, "push")
+        r.sync_with_remotes(minecraft_root, "push", verbosity=-1)
         warnings = [
             record.msg for record in caplog.records if record.levelname == "WARNING"
         ]
 
         assert len(warnings) == 1
         assert "Could not sync changes with prayer://unreachable" in warnings[0]
 
 
 @pytest.mark.xfail(
     not shutil.which("rsync"), reason="rsync is not installed on this system"
 )
 class TestRsyncSync(TestFileSync):
     protocol = "rsync"
+
+    def test_rsync_summary_summarizes_at_the_shulker_box_level(
+        self, minecraft_root, remote, caplog
+    ):
+        caplog.set_level(logging.DEBUG)
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, "pull", dry_run=True)
+        info_log = ""
+        debug_log = ""
+        for record in caplog.records:
+            if record.levelname == "INFO":
+                info_log += record.msg % record.args + "\n"
+            elif record.levelname == "DEBUG":
+                debug_log += record.msg % record.args + "\n"
+
+        # meta-test--make sure that the creation is actually happening
+        assert (
+            "+++ " + os.path.sep.join(("EnderChest", "1.19", ".bobby", "chunk"))
+            in debug_log
+        )
+
+        # meta-test--make sure nothing in the report at the shulker+1 level
+        assert os.path.sep.join(("EnderChest", "1.19", ".bobby")) not in info_log
+
+        assert (
+            f"Within EnderChest{os.path.sep}1.19..."
+            "\n  - Creating 1 file"
+            "\n  - Updating 1 file"  # there's also the save symlink
+            "\n  - Deleting 0 files"
+        ) in info_log
+
+    def test_rsync_summary_doesnt_report_details_if_the_whole_shulker_is_being_created(
+        self, minecraft_root, remote, caplog
+    ):
+        caplog.set_level(logging.DEBUG)
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, "pull", dry_run=True)
+        info_log = ""
+        debug_log = ""
+        for record in caplog.records:
+            if record.levelname == "INFO":
+                info_log += record.msg + "\n"
+            elif record.levelname == "DEBUG":
+                debug_log += record.msg + "\n"
+
+        # meta-test--make sure that the creation is actually happening
+        assert (
+            "+++ "
+            + os.path.sep.join(("EnderChest", "optifine", "mods", "optifine.jar"))
+            in debug_log
+        )
+
+        # meta-test--make sure nothing in the report at the shulker+1 level
+        assert os.path.sep.join(("EnderChest", "optifine", "mods")) not in info_log
+
+        assert f"Creating EnderChest{os.path.sep}optifine" in info_log
+
+    @pytest.mark.parametrize("verbosity", ("v", "vv", "vvv"))
+    @pytest.mark.parametrize("op", ("pull", "push"))
+    def test_verbose_dry_run_doesnt_summarize(
+        self, monkeypatch, minecraft_root, remote, caplog, op, verbosity
+    ):
+        def mock_summarize(*args, **kwargs):
+            raise AssertionError("I was not to be called")
+
+        from enderchest.sync import rsync
+
+        monkeypatch.setattr(rsync, "summarize_rsync_report", mock_summarize)
+
+        caplog.set_level(logging.DEBUG)
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, op, dry_run=True, verbosity=len(verbosity))
+
+        debug_log = "\n".join(
+            record.msg for record in caplog.records if record.levelname == "DEBUG"
+        )
+
+        # this wouldn't be in the summary
+        assert f"EnderChest{os.sep}global{os.sep}config" in debug_log
+
+    @pytest.mark.parametrize("op", ("pull", "push"))
+    def test_quiet_dry_run_still_reports_stats(
+        self, minecraft_root, remote, caplog, op
+    ):
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, op, dry_run=True, verbosity=-1)
+
+        printed_log = "\n".join(
+            record.msg for record in caplog.records if record.levelno > logging.INFO
+        )
+
+        assert "Number of created files" in printed_log
+
+    @pytest.mark.parametrize("op", ("pull", "push"))
+    def test_super_quiet_dry_run_still_reports_stats(
+        self, minecraft_root, remote, caplog, op
+    ):
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, op, dry_run=True, verbosity=-1)
+
+        printed_log = "\n".join(
+            record.msg for record in caplog.records if record.levelno > logging.INFO
+        )
+
+        assert "Number of created files" in printed_log
+
+    @pytest.mark.parametrize("op", ("pull", "push"))
+    def test_regular_sync_only_reports_overall_progress(
+        self, minecraft_root, remote, capfd, op
+    ):
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, op)
+
+        printed_log = capfd.readouterr().out
+
+        assert f"EnderChest{os.sep}global" not in printed_log
+
+        # but, like, make sure that it prints *something*
+        assert "Number of created files" in printed_log
+
+    @pytest.mark.parametrize("verbosity", ("v", "vv", "vvv"))
+    @pytest.mark.parametrize("op", ("pull", "push"))
+    def test_verbose_sync_reports_file_level_progress(
+        self, minecraft_root, remote, capfd, op, verbosity
+    ):
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, op, verbosity=len(verbosity))
+
+        printed_log = capfd.readouterr().out
+
+        assert f"EnderChest{os.sep}global" in printed_log
+        assert "xfr#2, to-chk=" in printed_log
+
+    @pytest.mark.parametrize("quietude", ("q", "qq", "qqq"))
+    @pytest.mark.parametrize("op", ("pull", "push"))
+    def test_quiet_sync_is_silent(self, minecraft_root, remote, capfd, op, quietude):
+        gather.update_ender_chest(minecraft_root, remotes=(remote,))
+        r.sync_with_remotes(minecraft_root, op, verbosity=-len(quietude))
+
+        printed_log = capfd.readouterr().out
+
+        assert printed_log == ""
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.1rc1/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.1rc1/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/utils.py` & `enderchest-0.1.1rc1/enderchest/test/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import Callable, Iterable
 
 import pytest
 
 from enderchest import EnderChest, InstanceSpec, ShulkerBox
 from enderchest import filesystem as fs
-from enderchest.shulker_box import _normalize_modloader
+from enderchest.instance import normalize_modloader
 
 from . import testing_files
 
 # folders common to both official and MMC-derived .minecraft folders
 COMMON_FOLDERS: tuple[str, ...] = (
     "backups",
     "crash_reports",
@@ -242,16 +242,16 @@
     Returns
     -------
     list of ShulkerBox
         A list of parsed shulker boxes corresponding to the ones rendered
         on the system
     """
     enderchest_folder.mkdir(parents=True, exist_ok=True)
-    with as_file(testing_files.ENDERCHEST_CONFIG) as enderchest_cfg:
-        shutil.copy(enderchest_cfg, enderchest_folder)
+    with as_file(testing_files.ENDERCHEST_CONFIG) as config_file:
+        shutil.copy(config_file, enderchest_folder)
     shulker_boxes: list[ShulkerBox] = []
     for shulker_name, shulker_config in shulkers:
         (enderchest_folder / shulker_name).mkdir(parents=True, exist_ok=True)
         config_path = enderchest_folder / shulker_name / fs.SHULKER_BOX_CONFIG_NAME
         with config_path.open("w") as config_file:
             config_file.write(shulker_config)
         shulker_boxes.append(ShulkerBox.from_cfg(config_path))
@@ -316,14 +316,17 @@
 *
 
 [modloader]
 Forge
 
 [link-folders]
 shadercache  ; not that I think this is a thing
+
+[do-not-link]
+*.local
 """,
 )
 
 STEAMDECK_SHULKER = (
     "steamdeck",
     """; steamdeck/shulkerbox.cfg
 [properties]
@@ -356,17 +359,17 @@
     """Parse the above table of shulker-to-instance matches"""
     matches: list[tuple[str, str, bool]] = []
     rows = MATCH_CSV.splitlines()
     header = rows.pop(0)
     shulker_boxes = [cell.strip() for cell in header.split(",")[1:]]
     for row in rows:
         cells = [cell.strip() for cell in row.split(",")]
-        instance = cells.pop(0)
+        mc = cells.pop(0)
         for i, cell in enumerate(cells):
-            matches.append((shulker_boxes[i], instance, cell == "True"))
+            matches.append((shulker_boxes[i], mc, cell == "True"))
     return matches
 
 
 TESTING_SHULKER_INSTANCE_MATCHES = tuple(_parse_match_csv())
 
 
 def resolve(path: Path, minecraft_root: Path) -> Path:
@@ -402,15 +405,15 @@
         instances will be included
 
     Notes
     -----
       - The parametrized tests will be ordered as provided
       - The name of the parametrized argument provided to the test will be "instance"
     """
-    instance_lookup = {instance.name: instance for instance in TESTING_INSTANCES}
+    instance_lookup = {mc.name: mc for mc in TESTING_INSTANCES}
     if len(instance_names) == 0:
         instance_names = tuple(instance_lookup.keys())
 
     instances = [instance_lookup[name] for name in instance_names]
 
     return pytest.mark.parametrize("instance", instances, ids=instance_names)
 
@@ -444,22 +447,20 @@
     root: Path,
     minecraft_versions: Iterable[str] | None = None,
     modloader: str | None = None,
     tags: Iterable[str] | None = None,
 ) -> InstanceSpec:
     """Shortcut constructor"""
     return InstanceSpec(
-        name, root, tuple(minecraft_versions or ()), modloader, tuple(tags or ())
+        name, root, tuple(minecraft_versions or ()), modloader or "", tuple(tags or ())
     )
 
 
-def normalize_instance(instance: InstanceSpec) -> InstanceSpec:
+def normalize_instance(mc: InstanceSpec) -> InstanceSpec:
     """Normalize the values inside an instance tuple"""
-    return instance._replace(
+    return mc._replace(
         # this should be fully checked by instance.equals()
-        root=instance.root.expanduser().relative_to(
-            instance.root.expanduser().parent.parent
-        ),
-        modloader=_normalize_modloader(instance.modloader)[0],
-        minecraft_versions=tuple(sorted(instance.minecraft_versions)),
-        tags=tuple(sorted(tag.lower() for tag in instance.tags)),
+        root=mc.root.expanduser().relative_to(mc.root.expanduser().parent.parent),
+        modloader=normalize_modloader(mc.modloader)[0],
+        minecraft_versions=tuple(sorted(mc.minecraft_versions)),
+        tags=tuple(sorted(tag.lower() for tag in mc.tags)),
     )
```

### Comparing `enderchest-0.1.0rc6/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.1rc1/enderchest.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc6
+Version: 0.1.1rc1
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -15,37 +15,60 @@
 [![PyPI version](https://badge.fury.io/py/enderchest.svg)](https://badge.fury.io/py/enderchest)
 ![PyPI downloads](https://img.shields.io/pypi/dm/enderchest.svg)
 
 ![Linux](https://img.shields.io/badge/GNU/Linux-000000?style=flat-square&logo=linux&logoColor=white&color=eda445)
 ![SteamOS](https://img.shields.io/badge/SteamOS-3776AB.svg?style=flat-square&logo=steamdeck&logoColor=white&color=7055c3)
 ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)
 ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=flat-square&logo=apple&logoColor=white&color=434334)
+![RaspberryPi](https://img.shields.io/badge/Raspberry%20Pi-000000?style=flat-square&logo=raspberrypi&logoColor=white&color=c51a4a)
 
 [![python](https://img.shields.io/badge/Python-3.10,3.11-3776AB.svg?style=flat&logo=python&logoColor=white&color=ffdc53&labelColor=3d7aaa)](https://www.python.org)
-![coverage](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/coverage.svg)
-![lint](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/pylint.svg)
+[![coverage](https://openbagtwo.github.io/EnderChest/dev/img/coverage.svg)](https://openbagtwo.github.io/EnderChest/dev/coverage)
+[![lint](https://openbagtwo.github.io/EnderChest/dev/img/pylint.svg)](https://openbagtwo.github.io/EnderChest/dev/lint-report.txt)
 
 
 A system for managing your minecraft installations across instances and
 installations
 
 ## In a Nutshell
 
 EnderChest is a command-line utility for selectively sharing Minecraft assets
 (configurations, mods, worlds, etc.)...
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
+### A Note On Linking
+
+Starting with Minecraft 1.20, Mojang by default
+[no longer allows worlds to load if they are or if they contain symbolic links](https://help.minecraft.net/hc/en-us/articles/16165590199181).
+While it is true that an improper symlink could cause Minecraft to write data
+to a place it shouldn't, nothing in EnderChest will ever generate a symlink whose
+target is outside of your EnderChest folder _unless you place_ a symbolic link in
+your EnderChest pointing to somewhere else (which you may want to do so that your
+screenshots, for example, point to your "My Pictures" folder).
+
+If you still have concerns about symlinks or questions about how they work,
+read through
+[this guide](https://www.makeuseof.com/tag/what-is-a-symbolic-link-what-are-its-uses-makeuseof-explains/)
+or [watch this explainer](https://www.youtube.com/watch?v=mA08E59-zo8), and if
+you still have questions, feel free to
+[open an issue](https://github.com/OpenBagTwo/EnderChest/issues/new?assignees=OpenBagTwo&labels=question&title=symlink%20question).
+
 ## Installation
 
 EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
+Note that the recommended sync protocol is
+[`rsync`](https://www.digitalocean.com/community/tutorials/how-to-use-rsync-to-sync-local-and-remote-directories), and EnderChest requires
+[version 3.2 or newer](https://dev.to/al5ina5/updating-rsync-on-macos-so-you-re-not-stuck-with-14-year-old-software-1b5i).
+However, other protocols are available if a modern `rsync` is not an option for you.
+
 The latest release can be installed from PyPI via `pip`:
 
 ```bash
 $ python -m pip install --user enderchest
 ```
 
 Full installation instructions can be found on
```

### Comparing `enderchest-0.1.0rc6/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.1rc1/enderchest.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 versioneer.py
 enderchest/__init__.py
 enderchest/_version.py
 enderchest/cli.py
+enderchest/config.py
 enderchest/craft.py
 enderchest/enderchest.py
 enderchest/filesystem.py
 enderchest/gather.py
 enderchest/instance.py
 enderchest/loggers.py
 enderchest/place.py
@@ -21,17 +22,19 @@
 enderchest.egg-info/dependency_links.txt
 enderchest.egg-info/entry_points.txt
 enderchest.egg-info/requires.txt
 enderchest.egg-info/top_level.txt
 enderchest/sync/__init__.py
 enderchest/sync/file.py
 enderchest/sync/rsync.py
+enderchest/sync/utils.py
 enderchest/test/__init__.py
 enderchest/test/conftest.py
 enderchest/test/test_cli.py
+enderchest/test/test_config.py
 enderchest/test/test_craft.py
 enderchest/test/test_gather.py
 enderchest/test/test_instance.py
 enderchest/test/test_place.py
 enderchest/test/test_sync.py
 enderchest/test/utils.py
 enderchest/test/testing_files/__init__.py
```

### Comparing `enderchest-0.1.0rc6/setup.py` & `enderchest-0.1.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/versioneer.py` & `enderchest-0.1.1rc1/versioneer.py`

 * *Files identical despite different names*

