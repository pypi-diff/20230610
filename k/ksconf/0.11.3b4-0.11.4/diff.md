# Comparing `tmp/ksconf-0.11.3b4.tar.gz` & `tmp/ksconf-0.11.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksconf-0.11.3b4.tar", last modified: Wed May 17 17:58:05 2023, max compression
+gzip compressed data, was "ksconf-0.11.4.tar", last modified: Sat Jun 10 00:05:57 2023, max compression
```

## Comparing `ksconf-0.11.3b4.tar` & `ksconf-0.11.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/commands/
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/promote.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/restexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/restpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/unarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/xmlformat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/setup_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/util/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/completers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/vc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/vc/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/xmlformat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:57:51.000000 ksconf-0.11.3b4/ksconf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.670607 ksconf-0.11.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-10 00:05:17.000000 ksconf-0.11.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-10 00:05:57.670607 ksconf-0.11.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-10 00:05:17.000000 ksconf-0.11.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.666607 ksconf-0.11.4/ksconf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-10 00:05:57.000000 ksconf-0.11.4/ksconf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.666607 ksconf-0.11.4/ksconf/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/app/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/app/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/app/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.666607 ksconf-0.11.4/ksconf/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/builder/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/builder/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/builder/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.670607 ksconf-0.11.4/ksconf/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/restexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/restpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/unarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/commands/xmlformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.670607 ksconf-0.11.4/ksconf/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/conf/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/conf/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/conf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/conf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.670607 ksconf-0.11.4/ksconf/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/setup_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.670607 ksconf-0.11.4/ksconf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/util/completers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/util/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/util/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/util/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.670607 ksconf-0.11.4/ksconf/vc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/vc/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-10 00:05:17.000000 ksconf-0.11.4/ksconf/xmlformat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:05:57.666607 ksconf-0.11.4/ksconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-10 00:05:57.000000 ksconf-0.11.4/ksconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-10 00:05:57.000000 ksconf-0.11.4/ksconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:05:57.000000 ksconf-0.11.4/ksconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-10 00:05:57.000000 ksconf-0.11.4/ksconf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-10 00:05:57.000000 ksconf-0.11.4/ksconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 00:05:57.000000 ksconf-0.11.4/ksconf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:05:38.000000 ksconf-0.11.4/ksconf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-10 00:05:57.670607 ksconf-0.11.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-10 00:05:17.000000 ksconf-0.11.4/setup.py
```

### Comparing `ksconf-0.11.3b4/LICENSE` & `ksconf-0.11.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/PKG-INFO` & `ksconf-0.11.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.3b4
+Version: 0.11.4
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: bash
+Provides-Extra: jinja
 Provides-Extra: thirdparty
 License-File: LICENSE
 
 # Ksconf Splunk CONFiguration tool
 
 This utility handles common Splunk app maintenance tasks in an installable python package.
 Specifically, this tool deals with many of the nuances of storing Splunk apps in a
```

### Comparing `ksconf-0.11.3b4/README.md` & `ksconf-0.11.4/README.md`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/__init__.py` & `ksconf-0.11.4/ksconf/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/__main__.py` & `ksconf-0.11.4/ksconf/__main__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/app/__init__.py` & `ksconf-0.11.4/ksconf/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/app/deploy.py` & `ksconf-0.11.4/ksconf/app/deploy.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/app/facts.py` & `ksconf-0.11.4/ksconf/app/facts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/app/manifest.py` & `ksconf-0.11.4/ksconf/app/manifest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/archive.py` & `ksconf-0.11.4/ksconf/archive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/builder/__init__.py` & `ksconf-0.11.4/ksconf/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/builder/cache.py` & `ksconf-0.11.4/ksconf/builder/cache.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/builder/core.py` & `ksconf-0.11.4/ksconf/builder/core.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/builder/steps.py` & `ksconf-0.11.4/ksconf/builder/steps.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/cli.py` & `ksconf-0.11.4/ksconf/cli.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/combine.py` & `ksconf-0.11.4/ksconf/combine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # -*- coding: utf-8 -*-
 """
-XXX: Move the overwrite-as-necessary logic into a subclass; for several use cases we just don't care because 'target' is a brand new directory
 """
 
 from __future__ import absolute_import, annotations, unicode_literals
 
 import os
 import re
 import sys
-from io import open
 from os import fspath
 from pathlib import Path
 from typing import Callable
 
 from ksconf.commands import ConfFileProxy
 from ksconf.compat import List, Tuple
 from ksconf.conf.delta import show_text_diff
 from ksconf.conf.merge import merge_conf_files
 from ksconf.conf.parser import PARSECONF_MID, PARSECONF_STRICT
 from ksconf.consts import SMART_CREATE, SMART_NOCHANGE, SMART_UPDATE
-from ksconf.layer import (DirectLayerRoot, DotDLayerRoot, LayerConfig,
+from ksconf.layer import (DirectLayerRoot, DotDLayerRoot, LayerContext,
                           LayerFile, LayerFilter, LayerRootBase)
 from ksconf.util.compare import file_compare
 from ksconf.util.file import _is_binary_file, smart_copy
 
 
 class LayerCombinerException(Exception):
     pass
@@ -64,55 +62,64 @@
 
     def __init__(self,
                  follow_symlink: bool = False,
                  banner: str = "",
                  dry_run: bool = False,
                  quiet: bool = False):
         self.layer_root: LayerRootBase = None
-        self.config = LayerConfig()
+        self.context = LayerContext()
         self.layer_filter = LayerFilter()
         self.banner = banner
         self.dry_run = dry_run
         self.quiet = quiet
 
-        self.config.follow_symlink = follow_symlink
+        self.context.follow_symlink = follow_symlink
 
         # Internal tracking variables
         self.layer_names_all = set()
         self.layer_names_used = set()
 
         # Not a great long-term design, but good enough for initial conversion from command-based design
         self.stdout = sys.stdout
         self.stderr = sys.stderr
 
     @classmethod
-    def register_regex(cls, regex_match):
-        """ Decorator that matches a filename regex and if it matches, it
-        executes the decorator handler.
+    def register_handler(cls, regex_match):
+        """ Decorator that registers a new file type handler.  The handler is
+        used if a file name matches a regex.  Regex 'search' mode is used.
         """
         cre = re.compile(regex_match)
 
         def match_f(file: Path):
             if cre.search(file.name):
                 return True
             return False
 
         def wrapper(handle_f):
             cls.filetype_handlers.append((match_f, handle_f))
             return handle_f
 
         return wrapper
 
+    def log(self, message):
+        # For historic reasons (idk) we send all messages to stderr, and diffs to stdout
+        if message:
+            self.stderr.write(f"{message}\n")
+
+    def debug(self, message):
+        if not self.quiet:
+            self.log(message)
+
     def set_source_dirs(self, sources: List[Path]):
-        self.layer_root = DirectLayerRoot(config=self.config)
+        self.layer_root = DirectLayerRoot(context=self.context)
         for src in sources:
             self.layer_root.add_layer(Path(src))
 
     def set_layer_root(self, root: LayerRootBase.Layer):
-        layer_root = DotDLayerRoot(config=self.config)
+        layer_root = DotDLayerRoot(context=self.context)
         layer_root.set_root(root)
         self.layer_root = layer_root
 
     def add_layer_filter(self, action, pattern):
         self.layer_filter.add_rule(action, pattern)
 
     def combine(self, target):
@@ -155,45 +162,43 @@
         del target
         return src_files
 
     def post_combine(self, target):
         """ Hook point for post-processing after all copy/merge operations have been completed. """
         del target
 
-    def combine_files(self, target, src_files):
+    def combine_files(self, target: Path, src_files: List[LayerFile]):
         layer_root = self.layer_root
         for src_file in sorted(src_files):
             do_copy = True
             sources = list(layer_root.get_file(src_file))
             try:
                 dest_fn = sources[0].logical_path
             except IndexError:
-                raise LayerCombinerException("File disappeared during execution?  {src_file}\n")
+                raise LayerCombinerException(f"File disappeared during execution?  {src_file}\n")
 
             dest_path: Path = target / dest_fn
 
             # Make missing destination folder, if missing
             dest_dir: Path = dest_path.parent
             if not dest_dir.is_dir() and not self.dry_run:
                 dest_dir.mkdir(parents=True)
 
             # Determine handling method based on source count and filename pattern
             if len(sources) > 1:
                 for matcher, handler in self.filetype_handlers:
                     if matcher(dest_fn):
-                        msg = handler(self, dest_path, sources, self.dry_run)
-                        if msg and not self.quiet:
-                            self.stderr.write(f"{msg}\n")
+                        handler(self, dest_path, sources, self.dry_run)
                         do_copy = False
 
             if do_copy:
-                # self.stderr.write(f"Considering {fspath(dest_fn):50}  NON-CONF Copy from source:  "
-                #                   f"{sources[-1].physical_path!r}\n")
+                # self.debug((f"Considering {fspath(dest_fn):50}  NON-CONF Copy from source:  "
+                #             f"{sources[-1].physical_path!r}")
                 # Always use the last file in the list (since last directory always wins)
-                src_file = sources[-1].physical_path
+                src_file = sources[-1].resource_path
                 if self.dry_run:
                     if dest_path.is_file():
                         if file_compare(src_file, dest_path):
                             smart_rc = SMART_NOCHANGE
                         else:
                             if (_is_binary_file(src_file) or _is_binary_file(dest_path)):
                                 # Binary files.  Can't compare...
@@ -202,55 +207,69 @@
                                 show_text_diff(self.stdout, dest_path, src_file)
                                 smart_rc = "DRY-RUN (DIFF)"
                     else:
                         smart_rc = "DRY-RUN (NEW)"
                 else:
                     smart_rc = smart_copy(src_file, dest_path)
                 if smart_rc != SMART_NOCHANGE:
-                    if not self.quiet:
-                        self.stderr.write(f"Copy <{smart_rc}>   {fspath(dest_path):50}  from {src_file}\n")
+                    self.debug(f"Copy <{smart_rc}>   {fspath(dest_path):50}  from {src_file}")
                 del src_file
 
 
-@LayerCombiner.register_regex(r"([a-z_-]+\.conf|(default|local)\.meta)$")
-def handle_merge_conf_files(context: LayerCombiner,
+# registration decorator
+register_handler = LayerCombiner.register_handler
+
+
+#
+# Combine handlers for specific file types
+#
+
+@register_handler(r"([a-z_-]+\.conf|(default|local)\.meta)$")
+def handle_merge_conf_files(combiner: LayerCombiner,
                             dest_path: Path,
                             sources: List[LayerFile],
                             dry_run):
+    """
+    Handle merging two or more ``.conf`` files.
+    """
     sources_physical = [fspath(p.physical_path) for p in sources]
-    message = None
     # Note that latest mtime logic is handled by merge_conf_files()
+    srcs = []
     try:
         # Handle merging conf files
         dest = ConfFileProxy(dest_path, "r+", parse_profile=PARSECONF_MID)
-        srcs = [ConfFileProxy(s, "r", parse_profile=PARSECONF_STRICT) for s in sources_physical]
-        # self.stderr.write(f"Considering {dest_fn:50}  CONF MERGE from source:  "
-        #                   f"{1!sources[0].physical_path}\n")
+        srcs = [ConfFileProxy(s.resource_path, "r", parse_profile=PARSECONF_STRICT) for s in sources]
+        # combiner.debug(f"Considering {dest_fn:50}  CONF MERGE from source:  "
+        #                f"{1!sources[0].physical_path}")
         smart_rc = merge_conf_files(dest, srcs, dry_run=dry_run,
-                                    banner_comment=context.banner)
+                                    banner_comment=combiner.banner)
         if smart_rc != SMART_NOCHANGE:
-            message = f"Merge <{smart_rc}>   {fspath(dest_path):50}  from {sources_physical!r}"
+            combiner.debug(f"Merge <{smart_rc}>   {fspath(dest_path):50}  from {sources_physical!r}")
+        return smart_rc
     finally:
         # Protect against any dangling open files:  (ResourceWarning: unclosed file)
         dest.close()
         for src in srcs:
             src.close()
-    return message
 
 
-@LayerCombiner.register_regex(r"\.conf\.spec$")
-def handle_spec_concatenate(context: LayerCombiner,
+@register_handler(r"\.conf\.spec$")
+def handle_spec_concatenate(combiner: LayerCombiner,
                             dest_path: Path,
                             sources: List[LayerFile],
                             dry_run):
-    sources_physical = [fspath(p.physical_path) for p in sources]
+    """
+    Concatenate multiple ``.spec`` files.  Likely a ``README.d`` situation.
+    """
+    sources_physical = []
     combined_content = ""
     last_mtime = max(src.mtime for src in sources)
     for src in sources:
-        content = src.physical_path.read_text()
+        sources_physical.append(src.physical_path)
+        content = src.resource_path.read_text()
         if not content.endswith("\n"):
             content += "\n"
         combined_content += content
     smart_rc = SMART_CREATE
     if dest_path.is_file():
         dest_content = dest_path.read_text()
         if dest_content == combined_content:
@@ -259,8 +278,9 @@
             smart_rc = SMART_UPDATE
 
     if not dry_run:
         dest_path.write_text(combined_content)
 
     os.utime(dest_path, (last_mtime, last_mtime))
     if smart_rc != SMART_NOCHANGE:
-        return f"Concatenate <{smart_rc}>   {fspath(dest_path):50}  from {sources_physical!r}"
+        combiner.debug(f"Concatenate <{smart_rc}>   {fspath(dest_path):50}  from {sources_physical!r}")
+    return smart_rc
```

### Comparing `ksconf-0.11.3b4/ksconf/commands/__init__.py` & `ksconf-0.11.4/ksconf/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 import logging
 import os
 import re
 import sys
 import textwrap
 from argparse import ArgumentParser, ArgumentTypeError
 from collections import namedtuple
-from io import open
+from io import StringIO, open
 from textwrap import dedent
 from warnings import warn
 
 from ksconf import KsconfPluginWarning
 from ksconf.compat import cache
 from ksconf.conf.parser import (ConfParserException, ParserConfig,
                                 detect_by_bom, parse_conf, smart_write_conf,
                                 write_conf)
-from ksconf.consts import EXIT_CODE_BAD_CONF_FILE, EXIT_CODE_NO_SUCH_FILE, SMART_CREATE, SmartEnum
+from ksconf.consts import (EXIT_CODE_BAD_ARGS, EXIT_CODE_BAD_CONF_FILE,
+                           EXIT_CODE_NO_SUCH_FILE, SMART_CREATE, SmartEnum)
 from ksconf.util import debug_traceback
 
 __all__ = [
     "KsconfCmd",
     "ConfDirProxy",
     "ConfFileProxy",
     "ConfFileType",
@@ -336,20 +337,20 @@
     def redirect_io(self, stdin=None, stdout=None, stderr=None):
         if stdin is not None:
             self.stdin = stdin
         if stdout is not None:
             self.stdout = stdout
         if stderr is not None:
             self.stderr = stderr
+    '''
 
     def exit(self, exit_code):
         """ Allow overriding for unittesting or other high-level functionality, like an
         interactive interface. """
         sys.exit(exit_code)
-    '''
 
     def add_parser(self, subparser):
         # Passing in the object return by 'ArgumentParser.add_subparsers()'
         kwargs = {
             "help": self.help,
             "description": self.description,
         }
@@ -438,14 +439,67 @@
             raise KsconfCmdReadConfException(EXIT_CODE_BAD_CONF_FILE)
         except TypeError as e:
             # debug_traceback()
             self.stderr.write(f"Parser config error '{path}': {e}\n")
             # I guess bad conf file.... can't remember what this one is for.
             raise KsconfCmdReadConfException(EXIT_CODE_BAD_CONF_FILE)
 
+    def parse_extra_vars(self, vars: str, arg_name="argument") -> dict:
+        """ Argument can be either a string, or a @file """
+        # XXX: Add more error checking and better user feedback!
+        if vars.startswith("@"):
+            filename = vars[1:]
+            payload = ""
+        else:
+            filename = ""
+            payload = vars
+
+        # I'm not sure this really makes sense, but why not?
+        if filename.endswith(".conf"):
+            return self.parse_conf(filename)
+
+        if not payload:
+            payload = open(filename).read()
+
+        try:
+            import json
+            data = json.loads(payload)
+            if not isinstance(data, dict):
+                self.stderr.write(f"Provided {arg_name} must contain a dict, not a {type(data)}\n")
+                return self.exit(EXIT_CODE_BAD_ARGS)
+        except ValueError:
+            # Couldn't parse as JSON; move on ...
+            pass
+
+        try:
+            import yaml
+            if filename:
+                with open(filename) as fp:
+                    data = yaml.safe_load(fp)
+            else:
+                data = yaml.safe_load(StringIO(payload))
+
+            if not isinstance(data, dict):
+                self.stderr.write(f"Provided {arg_name} must contain a dict, not a {type(data)}\n")
+                return self.exit(EXIT_CODE_BAD_ARGS)
+            return data
+        except ValueError:
+            # Not YAML?....
+            pass
+        except ImportError:
+            # PyYAML not installed
+            self.stderr.write("Unable to load from YAML as PyYAML not installed")
+            pass
+
+        if filename:
+            self.stderr.write(f"Unable to parse {arg_name} from file {filename}\n")
+        else:
+            self.stdout.write(f"Unable to parse {arg_name} from:\n{payload}\n\n")
+        self.exit(EXIT_CODE_BAD_ARGS)
+
 
 def add_splunkd_access_args(parser: ArgumentParser) -> ArgumentParser:
     parser.add_argument("--url", default="https://localhost:8089",
                         help="URL of Splunkd.  Default:  %(default)s")
     parser.add_argument("--user", default="admin",
                         help="Login username Splunkd.  Default:  %(default)s")
     parser.add_argument("--pass", dest="password", default="changeme",
@@ -465,14 +519,23 @@
                         help="Set the user who owns the content.  "
                              "The default of 'nobody' works well for app-level sharing.")
     parser.add_argument("--sharing", default="global", choices=["user", "app", "global"],
                         help="Set the sharing mode.")
     return parser
 
 
+def add_file_handler(parser: ArgumentParser) -> ArgumentParser:
+    from ksconf.layer import layer_file_factory
+    handlers = layer_file_factory.list_available_handlers()
+
+    parser.add_argument("--enable-handler", action="append", default=[], choices=handlers,
+                        help="Enable optional file handling support")
+    return parser
+
+
 def _get_entrypoints_lib(group, name=None):
     import entrypoints
 
     # Monkey patch some attributes for better API compatibility
     entrypoints.EntryPoint.dist = property(lambda self: self.distro)
 
     if name:
```

### Comparing `ksconf-0.11.3b4/ksconf/commands/check.py` & `ksconf-0.11.4/ksconf/commands/check.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/combine.py` & `ksconf-0.11.4/ksconf/commands/combine.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 
     cd MY_APP
     ksconf combine default.d/* --target=default
 
 """
 from __future__ import absolute_import, unicode_literals
 
-import os
-from io import open
 from pathlib import Path
 
 from ksconf.combine import LayerCombiner, LayerCombinerException
-from ksconf.commands import KsconfCmd, dedent
+from ksconf.commands import KsconfCmd, add_file_handler, dedent
 from ksconf.compat import List
 from ksconf.consts import (EXIT_CODE_BAD_ARGS, EXIT_CODE_COMBINE_MARKER_MISSING,
                            EXIT_CODE_MISSING_ARG, EXIT_CODE_NO_SUCH_FILE)
 from ksconf.filter import create_filtered_list
-from ksconf.layer import LayerFile
+from ksconf.layer import LayerFile, layer_file_factory
 from ksconf.util.completers import DirectoriesCompleter
 from ksconf.util.file import expand_glob_list, relwalk, splglob_simple
 
 CONTROLLED_DIR_MARKER = ".ksconf_controlled"
 
 
 class LayerCombinerExceptionCode(LayerCombinerException):
@@ -54,77 +52,77 @@
     def prepare_target_dir(self, target: Path):
         """
         Handle marker file and ensure that target directory gets created safely.
         """
         marker_file: Path = target / CONTROLLED_DIR_MARKER
         if target.is_dir():
             if not self.disable_marker and not marker_file.is_file():
-                self.stderr.write("Target directory already exists, but it appears to have been "
-                                  "created by some other means.  Marker file missing.\n")
+                self.log("Target directory already exists, but it appears to have been "
+                         "created by some other means.  Marker file missing.")
                 raise LayerCombinerExceptionCode("Target directory exists without marker file",
                                                  EXIT_CODE_COMBINE_MARKER_MISSING)
 
         elif self.dry_run:
-            self.stderr.write("Skipping creating destination directory {target} (dry-run)\n")
+            self.log(f"Skipping creating destination directory {target} (dry-run)")
         else:
             try:
                 target.mkdir()
             except OSError as e:
-                self.stderr.write(f"Unable to create destination directory {target}.  {e}\n")
+                self.log(f"Unable to create destination directory {target}.  {e}")
                 raise LayerCombinerExceptionCode(f"Unable to create destination directory {target}",
                                                  EXIT_CODE_NO_SUCH_FILE)
-            self.stderr.write(f"Created destination directory {target}\n")
+            self.log(f"Created destination directory {target}")
             if not self.disable_marker:
                 marker_file.write_text("This directory is managed by KSCONF.  Don't touch\n")
 
     def pre_combine_inventory(self, target: Path, src_files: List[LayerFile]) -> List[LayerFile]:
         """
         Find a set of files that exist in the target folder, but in NO source folder (for cleanup)
         """
-        config = self.config
+        context = self.context
 
-        self.stderr.write(f"Layers detected:  {self.layer_names_all}\n")
+        self.log(f"Layers detected:  {self.layer_names_all}")
         if self.layer_names_all != self.layer_names_used:
-            self.stderr.write(f"Layers after filter: {self.layer_names_used}\n")
+            self.log(f"Layers after filter: {self.layer_names_used}")
 
         # Convert src_files to a set to speed up
         src_files = set(src_files)
         self.target_extra_files = set()
-        for (root, _, files) in relwalk(target, followlinks=config.follow_symlink):
+        for (root, _, files) in relwalk(target, followlinks=context.follow_symlink):
             root = Path(root)
             for fn in files:
                 tgt_file = root / fn
                 if tgt_file not in src_files:
-                    if fn == CONTROLLED_DIR_MARKER or config.block_files.search(fn):
+                    if fn == CONTROLLED_DIR_MARKER or context.block_files.search(fn):
                         continue  # pragma: no cover (peephole optimization)
                     self.target_extra_files.add(tgt_file)
         return src_files
 
     def post_combine(self, target: Path):
         """
         Handle cleanup of extra files
         """
         target_extra_files = self.target_extra_files
         if target_extra_files:
             if self.disable_cleanup:
-                self.stderr.write("Cleanup operations disabled by user.\n")
+                self.log("Cleanup operations disabled by user.")
             else:
-                self.stderr.write("Found extra files not part of source tree(s):  "
-                                  f"{len(target_extra_files)} files.\n")
+                self.log("Found extra files not part of source tree(s):  "
+                         f"{len(target_extra_files)} files.")
 
             keep_existing = create_filtered_list("splunk", default=False)
             # splglob_simple:  Either full paths, or simple file-only match
             keep_existing.feedall(self.keep_existing, filter=splglob_simple)
             for dest_fn in target_extra_files:
                 if keep_existing.match_path(dest_fn):
-                    self.stderr.write(f"Keep existing file {dest_fn}\n")
+                    self.log(f"Keep existing file {dest_fn}")
                 elif self.disable_cleanup:
-                    self.stderr.write(f"Skip cleanup of unwanted file {dest_fn}\n")
+                    self.log(f"Skip cleanup of unwanted file {dest_fn}")
                 else:
-                    self.stderr.write(f"Remove unwanted file {dest_fn}\n")
+                    self.log(f"Remove unwanted file {dest_fn}")
                     f: Path = target / dest_fn
                     f.unlink()
 
 
 class CombineCmd(KsconfCmd):
     help = dedent("""\
     Combine configuration files across multiple source directories into a single
@@ -195,14 +193,20 @@
 
         parser.add_argument("-I", "--include", action="append", default=[], dest="layer_filter",
                             type=wb_type("include"), metavar="PATTERN",
                             help="Name or pattern of layers to include.")
         parser.add_argument("-E", "--exclude", action="append", default=[], dest="layer_filter",
                             type=wb_type("exclude"), metavar="PATTERN",
                             help="Name or pattern of layers to exclude from the target.")
+
+        add_file_handler(parser)
+        parser.add_argument("--template-vars",
+                            default=None, action="store",
+                            help="Set template variables as key=value or YAML/JSON, if filename prepend with @")
+
         parser.add_argument("--dry-run", "-D", default=False, action="store_true", help=dedent("""
             Enable dry-run mode.
             Instead of writing to TARGET, preview changes as a 'diff'.
             If TARGET doesn't exist, then show the merged file."""))
         parser.add_argument("--follow-symlink", "-l", action="store_true", default=False,
                             help="Follow symbolic links pointing to directories.  "
                                  "Symlinks to files are always followed.")
@@ -228,14 +232,20 @@
         combiner = RepeatableCombiner(follow_symlink=args.follow_symlink, banner=args.banner, dry_run=args.dry_run, quiet=args.quiet,
                                       keep_existing=args.keep_existing, disable_cleanup=args.disable_cleanup, disable_marker=args.disable_marker)
 
         # For now, just copy all settings from 'args' to class instance... needs work
         combiner.stdout = self.stdout
         combiner.stderr = self.stderr
 
+        for handler in args.enable_handler:
+            layer_file_factory.enable(handler)
+
+        if args.template_vars:
+            combiner.context.template_variables = self.parse_extra_vars(args.template_vars, "template-vars")
+
         for (action, pattern) in args.layer_filter:
             combiner.add_layer_filter(action, pattern)
 
         # Expand any globs in the CLI to individual directories
         args.source = list(expand_glob_list(args.source, do_sort=True))
 
         if args.layer_method == "auto":
```

### Comparing `ksconf-0.11.3b4/ksconf/commands/diff.py` & `ksconf-0.11.4/ksconf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/filter.py` & `ksconf-0.11.4/ksconf/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/merge.py` & `ksconf-0.11.4/ksconf/commands/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/minimize.py` & `ksconf-0.11.4/ksconf/commands/minimize.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/package.py` & `ksconf-0.11.4/ksconf/commands/package.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,41 @@
             --set-version={{git_tag}} \\
             --set-build=${TRAVIS_BUILD_NUMBER:-0}
 
 
 """
 
 import argparse
+import json
 import os
 
-from ksconf.commands import KsconfCmd, dedent
+from ksconf.commands import KsconfCmd, add_file_handler, dedent
 from ksconf.consts import EXIT_CODE_BAD_ARGS, EXIT_CODE_CLI_ARG_DEPRECATED, EXIT_CODE_SUCCESS
+from ksconf.layer import layer_file_factory
 from ksconf.package import AppPackager
 
 
 class PackageCmd(KsconfCmd):
     help = "Create a Splunk app .spl file from a source directory"
     description = dedent("""\
     Create a Splunk app or add on tarball (``.spl``) file from an app directory.
 
     ``ksconf package`` can do useful things like, exclude unwanted files, combine layers, set the
     application version and build number, drop or promote the ``local`` directory into ``default``.
 
     Note that some arguments, like the ``FILE`` support special values that can be automatically
     evaluated at runtime.  For example the placeholders ``{{version}}`` or ``{{git_tag}}`` can be
     expanded into the output tarball filename.
+
+    If both layering and templating are in use at the same time, be aware that templates are
+    rendered prior to layering operations.  This allows, for example, one layer to include a simple
+    ``indexes.conf`` file and another layer to include an ``indexes.conf.j2`` template.
     """)
     # format = "manual"
-    maturity = "alpha"
+    maturity = "beta"
 
     default_blocklist = [
         ".git*",
         "*.py[co]",
         "__pycache__",
         ".DS_Store"
     ]
@@ -95,14 +101,20 @@
         player.add_argument("-I", "--include", action="append", default=[], dest="layer_filter",
                             type=wb_type("include"), metavar="PATTERN",
                             help="Name or pattern of layers to include.")
         player.add_argument("-E", "--exclude", action="append", default=[], dest="layer_filter",
                             type=wb_type("exclude"), metavar="PATTERN",
                             help="Name or pattern of layers to exclude from the target.")
 
+        add_file_handler(parser)
+        parser.add_argument("--template-vars",
+                            default=None, action="store",
+                            help="Set template variables as key=value or YAML/JSON, "
+                            "if filename prepend with @")
+
         parser.add_argument("--follow-symlink", "-l", action="store_true", default=False,
                             help="Follow symbolic links pointing to directories.  "
                                  "Symlinks to files are always followed.")
 
         # Set app version or extra app version.
         parser.add_argument("--set-version", metavar="VERSION",
                             help="Set application version.  By default the application version "
@@ -181,27 +193,35 @@
                 app_name = os.path.basename(os.getcwd())
                 app_name_source = "extracted from working directory"
             else:
                 app_name = os.path.basename(args.source)
                 app_name_source = "extracted from source directory"
         '''
         self.stdout.write(f"Packaging {app_name}   (App name {app_name_source})\n")
-        packager = AppPackager(args.source, app_name, output=self.stderr)
+
+        for handler in args.enable_handler:
+            layer_file_factory.enable(handler)
+
+        template_vars = None
+        if args.template_vars:
+            template_vars = self.parse_extra_vars(args.template_vars, "template-vars")
+            self.stdout.write(f"Using variables: \n{json.dumps(template_vars, indent=2)}\n")
+
+        packager = AppPackager(args.source, app_name, output=self.stderr,
+                               template_variables=template_vars)
 
         if args.layer_method == "auto":
             # There'd no way to make this option legal but not shown in argparse.  :-(
             # Yeah, all this needs *LOTS* of work!
             self.stderr("The 'auto' option for layer_method is not longer supported.  "
                         "This will be an error in v0.11 and removed in v0.12\n")
             from ksconf import __version__
             if __version__.startswith("0.11."):
                 return EXIT_CODE_CLI_ARG_DEPRECATED
 
-        # XXX:  Make the combine step optional.  Either via detection (no .d folders/layers) OR manually opt-out
-        #       for faster packaging in simple scenarios (this may not matter once this is done in memory)
         with packager:
             packager.combine(args.source, args.layer_filter,
                              layer_method=args.layer_method,
                              allow_symlink=args.follow_symlink)
             # Handle local files
             if args.local == "merge":
                 packager.merge_local()
```

### Comparing `ksconf-0.11.3b4/ksconf/commands/promote.py` & `ksconf-0.11.4/ksconf/commands/promote.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/restexport.py` & `ksconf-0.11.4/ksconf/commands/restexport.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/restpublish.py` & `ksconf-0.11.4/ksconf/commands/restpublish.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/snapshot.py` & `ksconf-0.11.4/ksconf/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/sort.py` & `ksconf-0.11.4/ksconf/commands/sort.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/unarchive.py` & `ksconf-0.11.4/ksconf/commands/unarchive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/commands/xmlformat.py` & `ksconf-0.11.4/ksconf/commands/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/compat.py` & `ksconf-0.11.4/ksconf/compat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/conf/delta.py` & `ksconf-0.11.4/ksconf/conf/delta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/conf/merge.py` & `ksconf-0.11.4/ksconf/conf/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/conf/meta.py` & `ksconf-0.11.4/ksconf/conf/meta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/conf/parser.py` & `ksconf-0.11.4/ksconf/conf/parser.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/consts.py` & `ksconf-0.11.4/ksconf/consts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/filter.py` & `ksconf-0.11.4/ksconf/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/layer.py` & `ksconf-0.11.4/ksconf/layer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import re
 from collections import defaultdict
+from dataclasses import dataclass, field
 from fnmatch import fnmatch
 from os import PathLike, stat_result
 from pathlib import Path, PurePath
 from tempfile import NamedTemporaryFile
-from typing import Any, Callable, Iterator
+from typing import Callable, Iterator, Match
 
 from ksconf.compat import Dict, List, Set, Tuple
 from ksconf.util.file import relwalk
 
 """
 
 LayerRootBase has one or more 'Layer', each layer has one or more 'File's.
@@ -49,47 +50,113 @@
 def _path_join(*parts):
     """ A slightly smarter / more flexible path appender.
     Drop any None
     """
     return Path(*filter(None, parts))
 
 
-def path_in_layer(layer: Path, path: Path) -> Path:
-    """ Check to see if path exist within layer.
-    Returns either None, or the path without the shared prefix with layer.
-    """
-    # Using 'sep' over os.path.join / os.path.split should be okay here as we should only ever be
-    # given relative paths (no Windows UNC/drive letters)
-    if layer is None:
-        # Return as-is, since layer is root
-        return path
-    # layer_parts = layer.split(sep)
-    layer_parts = layer.parts
-    layer_count = len(layer_parts)
-    path_parts = path.parts
-    if len(path_parts) < layer_count:
-        return None
-    # Q: Are we recreating path.relative_to()?
-    path_suffix = path_parts[:layer_count]
-    if layer_parts != path_suffix:
-        return None
-    return Path(*path_parts[layer_count:])
-
-
 # Exceptions
 
 class LayerException(Exception):
     pass
 
 
 class LayerUsageException(LayerException):
     pass
 
 
+@dataclass
+class LayerContext:
+    follow_symlink: bool = False
+    block_files: Match = re.compile(r"\.(bak|swp)$")
+    block_dirs: set = field(default_factory=lambda: {".git"})
+    template_variables: dict = field(default_factory=dict)
+
+
+@dataclass
+class _FileFactoryHandler:
+    name: str
+    handler: LayerFile
+    priority: int = 0
+    enabled: bool = False
+
+
+class FileFactory:
+    _registered_handlers: Dict[str, _FileFactoryHandler] = {}
+    _enabled_handlers: List[Callable] = []
+
+    def __init__(self):
+        # Make this class a singleton?
+        self._context_state = None
+
+    def _recalculate(self):
+        self._enabled_handlers = [
+            h.handler for h in sorted(self._registered_handlers.values(),
+                                      key=lambda h: (-h.priority, h.name)) if h.enabled]
+
+    def enable(self, name, _enabled=True):
+        handler = self._registered_handlers[name]
+        handler.enabled = _enabled
+        self._recalculate()
+
+    def disable(self, name):
+        self.enable(name, False)
+
+    def list_available_handlers(self) -> List[str]:
+        return [h.name for h in self._registered_handlers.values() if not h.enabled]
+
+    def __call__(self, layer, path: PurePath, *args, **kwargs) -> LayerFile:
+        """
+        Factory thats finds the appropriate LayerFile class and returns a new instance.
+        """
+        for cls in self._enabled_handlers:
+            if cls.match(path):
+                return cls(layer, path, *args, **kwargs)
+
+    def register_handler(self, name: str, **kwargs):
+        def wrapper(handler_class: LayerFile):
+            handler = _FileFactoryHandler(name, handler_class, **kwargs)
+            self._registered_handlers[handler.name] = handler
+            self._recalculate()
+            return handler_class
+        return wrapper
+
+    def __enter__(self) -> FileFactory:
+        # The primary use case is for clean unit testing
+        assert not self._context_state, "Nested contexts are not supported"
+        from copy import deepcopy
+        self._context_state = (deepcopy(self._registered_handlers),
+                               deepcopy(self._enabled_handlers))
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._registered_handlers, self._enabled_handlers = self._context_state
+        self._context_state = None
+
+
+# Single shared instance
+layer_file_factory = FileFactory()
+register_file_handler = layer_file_factory.register_handler
+
+
+@register_file_handler("default", priority=-100, enabled=True)
 class LayerFile(PathLike):
+    '''
+    Abstraction of a file within a Layer
+
+    Paths:
+        * ``logical_path``:  Conceptual file path.  This is the final path after all layers are resolved.
+          Think of this as the 'destination' file.
+        * ``physical_path``:  Actual file path.  The location of the physical file found within a source layer.
+          Most of the time this is the 'source' file, however this doesn't take into considerations layer combining or
+          template expansion requirements.  (In the case of a template, this would be the template file)
+        * ``resource_path``:  Content location.  Often this the ``physical_path``, but in the case of abstracted layers
+          (like templates, or archived layers), this would be the location of a temporary resource that contains
+          the expanded/rendered content.
+    '''
     __slots__ = ["layer", "relative_path", "_stat"]
 
     def __init__(self,
                  layer: LayerRootBase.Layer,
                  relative_path: PurePath,
                  stat: stat_result = None):
         self.layer = layer
@@ -107,14 +174,15 @@
     def physical_path(self) -> Path:
         return _path_join(self.layer.root, self.layer.physical_path, self.relative_path)
 
     @property
     def logical_path(self) -> Path:
         return _path_join(self.layer.logical_path, self.relative_path)
 
+    # For "normal" files, the resource_path is the physical_path (not true for rendered files)
     resource_path = physical_path
 
     @property
     def stat(self) -> stat_result:
         if self._stat is None:
             self._stat = self.physical_path.stat()
         return self._stat
@@ -124,70 +192,89 @@
         return self.stat.st_size
 
     @property
     def mtime(self):
         return self.stat.st_mtime
 
 
-class TemplatedLayerFile(LayerFile):
-
-    __slots__ = ["_temp_resource"]
-    template_context: dict = {}
+class LayerRenderedFile(LayerFile):
+    """
+    Abstract LayerFile for rendered scenarios, such as template scenarios.
+    A subclass really only needs to implement ``match()`` ``render()``
+    """
+    __slots__ = ["_rendered_resource"]
 
     def __init__(self, *args, **kwargs):
-        super(TemplatedLayerFile, self).__init__(*args, **kwargs)
-        self._temp_resource = None
+        super(LayerRenderedFile, self).__init__(*args, **kwargs)
+        self._rendered_resource = None
 
     def __del__(self):
-        if getattr(self, "_temp_resource", None) and self._temp_resource.is_file():
-            self._temp_resource.unlink()
+        if getattr(self, "_rendered_resource", None) and self._rendered_resource.is_file():
+            self._rendered_resource.unlink()
 
-    @staticmethod
-    def match(path: PurePath):
-        return path.suffix == ".j2"
+    def render(self, template_path: Path) -> str:
+        raise NotImplementedError
 
     @staticmethod
     def transform_name(path: PurePath):
-        return path.with_name(path.name[:-3])
-
-    def render(self, template_path: Path) -> str:
-        from jinja2 import Environment, StrictUndefined
-        environment = Environment(undefined=StrictUndefined)
-        # TODO:  Use file system loader; allowing other file imports
-        template = environment.from_string(template_path.read_text())
-        return template.render(**self.template_context)
+        # Remove trailing suffix
+        return path.with_name(path.stem)
 
     @property
     def logical_path(self) -> Path:
         return _path_join(self.layer.logical_path,
                           self.transform_name(self.relative_path))
 
     @property
     def physical_path(self) -> Path:
         return _path_join(self.layer.root, self.layer.physical_path, self.relative_path)
 
     @property
     def resource_path(self) -> Path:
-        if not self._temp_resource:
-            # Temporary file will be removed in instance destructor
+        if not self._rendered_resource:
+            # Temporary file will be removed in instance destructor.  Multiple opens expected.
             tf = NamedTemporaryFile(delete=False)
-            self._temp_resource = Path(tf.name)
-            self._temp_resource.write_text(self.render(self.physical_path))
-        return self._temp_resource
+            self._rendered_resource = Path(tf.name)
+            content = self.render(self.physical_path)
+            self._rendered_resource.write_text(content)
+        return self._rendered_resource
 
 
-def layer_file_factory(layer, path: PurePath, *args, **kwargs) -> LayerFile:
-    # XXX: Add a dynamic registration process; decorators, subclass init hook?
-    classes = [
-        TemplatedLayerFile,
-        LayerFile,
-    ]
-    for cls in classes:
-        if cls.match(path):
-            return cls(layer, path, *args, **kwargs)
+@register_file_handler("jinja", priority=50, enabled=False)
+class LayerFile_Jinja2(LayerRenderedFile):
+    @staticmethod
+    def match(path: PurePath):
+        return path.suffix == ".j2"
+
+    @staticmethod
+    def transform_name(path: PurePath):
+        return path.with_name(path.name[:-3])
+
+    @property
+    def jinja2_env(self):
+        # Use context object to 'cache' the jinja2 environment
+        if not hasattr(self.layer.context, "jinja2_environment"):
+            self.layer.context.jinja2_environment = self._build_jinja2_env()
+        return self.layer.context.jinja2_environment
+
+    def _build_jinja2_env(self):
+        from jinja2 import Environment, FileSystemLoader, StrictUndefined
+        environment = Environment(
+            undefined=StrictUndefined,
+            loader=FileSystemLoader(self.layer.root),
+            auto_reload=False)
+        environment.globals.update(self.layer.context.template_variables)
+        return environment
+
+    def render(self, template_path: Path) -> str:
+        self.jinja2_env
+        rel_template_path = template_path.relative_to(self.layer.root)
+        template = self.jinja2_env.get_template("/".join(rel_template_path.parts))
+        value = template.render()
+        return value
 
 
 class LayerFilter:
     _valid_actions = ("include", "exclude")
 
     def __init__(self):
         self._rules = []
@@ -212,56 +299,47 @@
             if fnmatch(layer_name, rule_pattern):
                 response = rule_action == "include"
         return response
 
     __call__ = evaluate
 
 
-class LayerConfig:
-
-    def __init__(self):
-        # Set defaults
-        self.follow_symlink = False
-        self.block_files = re.compile(r"\.(bak|swp)$")
-        self.block_dirs = {".git"}
-
-
 R_walk = Iterator[Tuple[Path, List[str], List[str]]]
 
 
 class LayerRootBase:
     """ All 'path's here are relative to the ROOT. """
 
     class Layer:
         """ Basic layer Container:   Connects logical and physical paths. """
-        __slots__ = ["name", "root", "logical_path", "physical_path", "config",
+        __slots__ = ["name", "root", "logical_path", "physical_path", "context",
                      "_file_factory", "_cache_files"]
 
         def __init__(self, name: str,
                      root: Path,
                      physical: PurePath,
                      logical: PurePath,
-                     config: LayerConfig,
+                     context: LayerContext,
                      file_factory: Callable):
             self.name = name
             self.root = root
             self.physical_path = physical
             self.logical_path = logical
-            self.config = config
+            self.context = context
             self._file_factory = file_factory
             self._cache_files: List[LayerFile] = []
 
         def walk(self) -> R_walk:
             # In the simple case, this is good enough.   Some subclasses will need to override
             for (root, dirs, files) in relwalk(_path_join(self.root, self.physical_path),
-                                               followlinks=self.config.follow_symlink):
+                                               followlinks=self.context.follow_symlink):
                 root = Path(root)
-                files = [f for f in files if not self.config.block_files.search(f)]
+                files = [f for f in files if not self.context.block_files.search(f)]
                 for d in list(dirs):
-                    if d in self.config.block_dirs:
+                    if d in self.context.block_dirs:
                         dirs.remove(d)
                 yield (root, dirs, files)
 
         def iter_files(self) -> Iterator[LayerFile]:
             for (top, _, files) in self.walk():
                 for file in files:
                     yield self._file_factory(self, top / file)
@@ -269,36 +347,26 @@
         def list_files(self) -> List[LayerFile]:
             if not self._cache_files:
                 self._cache_files = list(self.iter_files())
             return self._cache_files
 
         def get_file(self, path: Path) -> LayerFile:
             """ Return file object (by logical path), if it exists in this layer. """
-            # TODO:  Optimize by making a dict with a logical_path as the key
+            # TODO:  Optimize by caching.  Use a dict with a logical_path as the key
             for file in self.list_files():
                 if file.logical_path == path:
                     if file.physical_path.is_file():
                         return file
                     else:
                         return None
 
-            '''
-            # XXX: There's probably ways to optimize this.  fine for now (correctness over speed)
-            rel_path = path_in_layer(self.logical_path, path)
-            if not rel_path:
-                return None
-            file_ = self._file_factory(self, rel_path)
-            if file_.physical_path.is_file():
-                return file_
-            '''
-
     # LayerRootBase
-    def __init__(self, config: LayerConfig = None):
+    def __init__(self, context: LayerContext = None):
         self._layers: List[LayerRootBase.Layer] = []
-        self.config = config or LayerConfig()
+        self.context = context or LayerContext()
 
     def apply_filter(self, layer_filter: LayerFilter) -> bool:
         """
         Apply a destructive filter to all layers.  layer_filter(layer) will be called one for each
         layer, if the filter returns True than the layer is kept.  Root layers are always kept.
 
         Returns True if layers were removed
@@ -366,15 +434,15 @@
     def add_layer(self, path: Path):
         Layer = self.Layer
         # Layer name should be considered arbitrary and unimportant here
         layer_name = path.name
         if not path.is_dir():
             raise LayerUsageException("Layers must be directories.  "
                                       f"Given path '{path}' is not a directory.")
-        layer = Layer(layer_name, path, None, None, config=self.config,
+        layer = Layer(layer_name, path, None, None, context=self.context,
                       file_factory=layer_file_factory)
         super(DirectLayerRoot, self).add_layer(layer)
 
     def order_layers(self):
         # No op.  Irrelevant as layers are given (CLI) in the order they should be applied.
         pass
 
@@ -426,18 +494,18 @@
     class Layer(LayerRootBase.Layer):
         __slots__ = ["prune_points"]
 
         def __init__(self, name: str,
                      root: Path,
                      physical: PurePath,
                      logical: PurePath,
-                     config: LayerConfig,
+                     context: LayerContext,
                      file_factory: Callable,
                      prune_points: Set[Path] = None):
-            super(DotDLayerRoot.Layer, self).__init__(name, root, physical, logical, config=config,
+            super(DotDLayerRoot.Layer, self).__init__(name, root, physical, logical, context=context,
                                                       file_factory=file_factory)
             self.prune_points: Set[Path] = set(prune_points) if prune_points else set()
 
         def walk(self) -> R_walk:
             for (root, dirs, files) in super(DotDLayerRoot.Layer, self).walk():
                 if root in self.prune_points:
                     # Cleanup files/dirs to keep walk() from descending deeper
@@ -458,16 +526,16 @@
         def __init__(self, path):
             super(DotDLayerRoot.MountDotD, self).__init__(path)
     '''
 
     mount_regex = re.compile(r"(?P<realname>[\w_.-]+)\.d$")
     layer_regex = re.compile(r"(?P<layer>\d\d-[\w_.-]+)")
 
-    def __init__(self, config=None):
-        super(DotDLayerRoot, self).__init__(config)
+    def __init__(self, context=None):
+        super(DotDLayerRoot, self).__init__(context)
         # self.root = None
         self._root_layer: LayerRootBase.Layer = None
         self._mount_points: Dict[Path, List[str]] = defaultdict(list)
 
     def apply_filter(self, layer_filter: LayerFilter):
         # Apply filter function, but also be sure to keep the root layer
         def fltr(l):
@@ -475,34 +543,35 @@
         return super(DotDLayerRoot, self).apply_filter(fltr)
 
     def set_root(self, root: Path, follow_symlinks=None):
         """ Set a root path, and auto discover all '.d' directories.
 
         Note:  We currently only support '.d/<layer>' directories, a file like
         `default.d/10-props.conf` won't be handled here.
+        A valid name would be ``default.d/10-name/props.conf``.
         """
         Layer = self.Layer
         root = Path(root)
         if follow_symlinks is None:
-            follow_symlinks = self.config.follow_symlink
+            follow_symlinks = self.context.follow_symlink
 
         for (top, dirs, files) in relwalk(root, topdown=False, followlinks=follow_symlinks):
             del files
             top = Path(top)
             mount_mo = self.mount_regex.match(top.name)
             if mount_mo:
                 for dir_ in dirs:
                     dir_mo = self.layer_regex.match(dir_)
                     if dir_mo:
                         # XXX: Nested layers breakage, must substitute multiple ".d" folders in `top`
                         layer = Layer(dir_mo.group("layer"),
                                       root,
                                       physical=top / dir_,
                                       logical=top.parent / mount_mo.group("realname"),
-                                      config=self.config,
+                                      context=self.context,
                                       file_factory=layer_file_factory)
                         self.add_layer(layer)
                         self._mount_points[top].append(dir_)
                     else:
                         # XXX: Give the user the option of logging the near-matches (could indicate a
                         # problem in the config, or could be some other legit directory structure)
                         '''
@@ -517,15 +586,15 @@
                 pass
 
         # XXX: Adding <root> should be skipped if (and only if) root itself if a '.d' folder
         # Very last operation, add the top directory as the final layer (lowest rank)
         prune_points = [mount / layer
                         for mount, layers in self._mount_points.items()
                         for layer in layers]
-        layer = Layer("<root>", root, None, None, config=self.config,
+        layer = Layer("<root>", root, None, None, context=self.context,
                       file_factory=layer_file_factory,
                       prune_points=prune_points)
         self.add_layer(layer, do_sort=False)
         self._root_layer = layer
 
     def list_layers(self) -> List[Layer]:
         # Return all but the root layer.
```

### Comparing `ksconf-0.11.3b4/ksconf/package.py` & `ksconf-0.11.4/ksconf/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import re
 import shutil
 import tarfile
 import tempfile
 from functools import wraps
 from os import fspath
-from typing import TextIO
+from typing import TextIO, Union
 
 from ksconf.app.manifest import AppManifest
 from ksconf.combine import LayerCombiner
 from ksconf.conf.merge import merge_app_local, merge_conf_dicts
 from ksconf.conf.parser import conf_attr_boolean, parse_conf, update_conf
 from ksconf.consts import KSCONF_DEBUG
 from ksconf.vc.git import git_cmd
@@ -52,21 +52,23 @@
 
 class PackagingException(Exception):
     pass
 
 
 class AppPackager:
 
-    def __init__(self, src_path, app_name: str, output: TextIO):
+    def __init__(self, src_path, app_name: str, output: TextIO,
+                 template_variables: dict = None):
         self.src_path = fspath(src_path)
         self.app_name = app_name
         self.build_dir = None
         self.app_dir = None
         self.output = output
         self._var_magic = None
+        self.template_variables = template_variables
 
     def require_active_context(funct):
         """ Decorator to mark member functions that cannot be used until the
         context manager has been activated.
         """
         @wraps(funct)
         def wrapper(self: AppPackager, *args, **kwargs):
@@ -76,36 +78,38 @@
 
     def cleanup(self):
         # Do we need  https://stackoverflow.com/a/21263493/315892  (Windows): -- See tests/cli_helper
         shutil.rmtree(self.build_dir)
         self.build_dir = None
         self.app_dir = None
 
-    def expand_var(self, value):
+    def expand_var(self, value: str) -> str:
         """ Expand a variable, if present
 
         :param str value:  String that main contain ``{{variable}}`` substitution.
         :return: Expanded value
         :rtype: str
         """
         return self._var_magic.expand(value)
 
-    def expand_new_only(self, value):
+    def expand_new_only(self, value: str) -> Union[str, None]:
         """ Expand a variable but return False if no substitution occurred
 
         :param str value:  String that may contain ``{{variable}}`` substitution.
         :return:  Expanded value if variables were expanded, else False
         :rtype: str
         """
         new_value = self._var_magic.expand(value)
         return new_value if new_value != value else False
 
     @require_active_context
     def combine(self, src, filters, layer_method="dir.d", allow_symlink=False):
         combiner = LayerCombiner(follow_symlink=allow_symlink, quiet=True)
+        if self.template_variables:
+            combiner.context.template_variables = self.template_variables
         if layer_method == "dir.d":
             combiner.set_layer_root(src)
         elif layer_method == "disable":
             combiner.set_source_dirs([src])
         else:
             raise NotImplementedError(f"layer_method of '{layer_method}' is not supported.  "
                                       "Please use 'dir.d' or 'disable'.")
@@ -257,29 +261,26 @@
         """
         app_name = self.expand_var(self.app_name)
         manifest = AppManifest.from_filesystem(self.app_dir, name=app_name,
                                                calculate_hash=calculate_hash)
         manifest.source = self.src_path
         return manifest
 
-    def __enter__(self):
+    def __enter__(self) -> AppPackager:
         self.build_dir = tempfile.mkdtemp("-ksconf-package-build")
         if self.app_name == "." or "{{" in self.app_name:
             # Use a placeholder app name, otherwise build_dir == app_dir
             self.app_dir = os.path.join(self.build_dir, "app")
         else:
             self.app_dir = os.path.join(self.build_dir, self.app_name)
         self._var_magic = AppVarMagic(self.src_path, self.app_dir)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        try:
-            self.cleanup()
-        finally:
-            self.app_dir = None
+        self.cleanup()
 
 
 class AppVarMagicException(KeyError):
     pass
 
 
 class AppVarMagic:
```

### Comparing `ksconf-0.11.3b4/ksconf/setup_entrypoints.py` & `ksconf-0.11.4/ksconf/setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/util/__init__.py` & `ksconf-0.11.4/ksconf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/util/compare.py` & `ksconf-0.11.4/ksconf/util/compare.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/util/completers.py` & `ksconf-0.11.4/ksconf/util/completers.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/util/file.py` & `ksconf-0.11.4/ksconf/util/file.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/util/rest.py` & `ksconf-0.11.4/ksconf/util/rest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/util/terminal.py` & `ksconf-0.11.4/ksconf/util/terminal.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/vc/git.py` & `ksconf-0.11.4/ksconf/vc/git.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf/xmlformat.py` & `ksconf-0.11.4/ksconf/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf.egg-info/PKG-INFO` & `ksconf-0.11.4/ksconf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.3b4
+Version: 0.11.4
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: bash
+Provides-Extra: jinja
 Provides-Extra: thirdparty
 License-File: LICENSE
 
 # Ksconf Splunk CONFiguration tool
 
 This utility handles common Splunk app maintenance tasks in an installable python package.
 Specifically, this tool deals with many of the nuances of storing Splunk apps in a
```

### Comparing `ksconf-0.11.3b4/ksconf.egg-info/SOURCES.txt` & `ksconf-0.11.4/ksconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/ksconf.egg-info/entry_points.txt` & `ksconf-0.11.4/ksconf.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b4/setup.py` & `ksconf-0.11.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,15 @@
           "lxml",         # Added as a hard requirement to allow pre-commit to work out of the box
       ],
       # Wacky reason for this explained in ksconf/setup_entrypoints.py
       entry_points=get_entrypoints_setup(),
       # Not required, but useful.
       extras_require={
           "bash": ["argcomplete"],
+          "jinja": ["jinja2"],
           "thirdparty": [
               "splunk-sdk>=1.7.0"
           ],
       },
       include_package_data=True,
       zip_safe=True
       )
```

