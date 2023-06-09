# Comparing `tmp/dbt-redshift-1.6.0b2.tar.gz` & `tmp/dbt-redshift-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.6.0b2.tar", last modified: Thu May 25 17:40:34 2023, max compression
+gzip compressed data, was "dbt-redshift-1.6.0b3.tar", last modified: Fri Jun  9 17:22:04 2023, max compression
```

## Comparing `dbt-redshift-1.6.0b2.tar` & `dbt-redshift-1.6.0b3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.871782 dbt-redshift-1.6.0b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.871782 dbt-redshift-1.6.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.811966 dbt-redshift-1.6.0b3/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.807966 dbt-redshift-1.6.0b3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.815966 dbt-redshift-1.6.0b3/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.807966 dbt-redshift-1.6.0b3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.823966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/setup.py
```

### Comparing `dbt-redshift-1.6.0b2/LICENSE.md` & `dbt-redshift-1.6.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/PKG-INFO` & `dbt-redshift-1.6.0b3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b2 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b3 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.6.0b2/README.md` & `dbt-redshift-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.6.0b3/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.6.0b3/dbt/adapters/redshift/connections.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,20 +9,33 @@
 import redshift_connector
 import urllib.request
 import json
 from redshift_connector.utils.oids import get_datatype_name
 
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse, Connection, Credentials
+from dbt.contracts.util import Replaceable
+from dbt.dataclass_schema import FieldEncoder, dbtClassMixin, StrEnum, ValidationError
 from dbt.events import AdapterLogger
-import dbt.exceptions
+from dbt.exceptions import DbtRuntimeError, CompilationError
 import dbt.flags
-from dbt.dataclass_schema import FieldEncoder, dbtClassMixin, StrEnum
 from dbt.helper_types import Port
 
+
+class SSLConfigError(CompilationError):
+    def __init__(self, exc: ValidationError):
+        self.exc = exc
+        super().__init__(msg=self.get_message())
+
+    def get_message(self) -> str:
+        validator_msg = self.validator_error_message(self.exc)
+        msg = f"Could not parse SSL config: {validator_msg}"
+        return msg
+
+
 logger = AdapterLogger("Redshift")
 
 drop_lock: Lock = dbt.flags.MP_CONTEXT.Lock()  # type: ignore
 
 IAMDuration = NewType("IAMDuration", int)
 
 
@@ -53,14 +66,74 @@
 
 
 class RedshiftConnectionMethod(StrEnum):
     DATABASE = "database"
     IAM = "iam"
 
 
+class UserSSLMode(StrEnum):
+    disable = "disable"
+    allow = "allow"
+    prefer = "prefer"
+    require = "require"
+    verify_ca = "verify-ca"
+    verify_full = "verify-full"
+
+    @classmethod
+    def default(cls) -> "UserSSLMode":
+        # default for `psycopg2`, which aligns with dbt-redshift 1.4 and provides backwards compatibility
+        return cls.prefer
+
+
+class RedshiftSSLMode(StrEnum):
+    verify_ca = "verify-ca"
+    verify_full = "verify-full"
+
+
+SSL_MODE_TRANSLATION = {
+    UserSSLMode.disable: None,
+    UserSSLMode.allow: RedshiftSSLMode.verify_ca,
+    UserSSLMode.prefer: RedshiftSSLMode.verify_ca,
+    UserSSLMode.require: RedshiftSSLMode.verify_ca,
+    UserSSLMode.verify_ca: RedshiftSSLMode.verify_ca,
+    UserSSLMode.verify_full: RedshiftSSLMode.verify_full,
+}
+
+
+@dataclass
+class RedshiftSSLConfig(dbtClassMixin, Replaceable):  # type: ignore
+    ssl: bool = True
+    sslmode: Optional[RedshiftSSLMode] = SSL_MODE_TRANSLATION[UserSSLMode.default()]
+
+    @classmethod
+    def parse(cls, user_sslmode: UserSSLMode) -> "RedshiftSSLConfig":
+        try:
+            raw_redshift_ssl = {
+                "ssl": user_sslmode != UserSSLMode.disable,
+                "sslmode": SSL_MODE_TRANSLATION[user_sslmode],
+            }
+            cls.validate(raw_redshift_ssl)
+        except ValidationError as exc:
+            raise SSLConfigError(exc)
+
+        redshift_ssl = cls.from_dict(raw_redshift_ssl)
+
+        if redshift_ssl.ssl:
+            message = (
+                f"Establishing connection using ssl with `sslmode` set to '{user_sslmode}'."
+                f"To connect without ssl, set `sslmode` to 'disable'."
+            )
+        else:
+            message = "Establishing connection without ssl."
+
+        logger.debug(message)
+
+        return redshift_ssl
+
+
 @dataclass
 class RedshiftCredentials(Credentials):
     host: str
     user: str
     port: Port
     method: str = RedshiftConnectionMethod.DATABASE  # type: ignore
     password: Optional[str] = None  # type: ignore
@@ -70,37 +143,48 @@
     )
     iam_profile: Optional[str] = None
     autocreate: bool = False
     db_groups: List[str] = field(default_factory=list)
     ra3_node: Optional[bool] = False
     connect_timeout: Optional[int] = None
     role: Optional[str] = None
-    sslmode: Optional[str] = None
+    sslmode: Optional[UserSSLMode] = field(default_factory=UserSSLMode.default)
     retries: int = 1
     region: Optional[str] = None  # if not provided, will be determined from host
-    autocommit: Optional[bool] = False
+    # opt-in by default per team deliberation on https://peps.python.org/pep-0249/#autocommit
+    autocommit: Optional[bool] = True
 
     _ALIASES = {"dbname": "database", "pass": "password"}
 
     @property
     def type(self):
         return "redshift"
 
     def _connection_keys(self):
         return (
             "host",
-            "port",
             "user",
+            "port",
             "database",
-            "schema",
             "method",
             "cluster_id",
             "iam_profile",
+            "schema",
             "sslmode",
             "region",
+            "sslmode",
+            "region",
+            "iam_profile",
+            "autocreate",
+            "db_groups",
+            "ra3_node",
+            "connect_timeout",
+            "role",
+            "retries",
+            "autocommit",
         )
 
     @property
     def unique_field(self) -> str:
         return self.host
 
 
@@ -142,16 +226,16 @@
 
         # Validate the set region
         if not _is_valid_region(kwargs["region"]):
             raise dbt.exceptions.FailedToConnectError(
                 "Invalid region provided: {}".format(kwargs["region"])
             )
 
-        if self.credentials.sslmode:
-            kwargs["sslmode"] = self.credentials.sslmode
+        redshift_ssl_config = RedshiftSSLConfig.parse(self.credentials.sslmode)
+        kwargs.update(redshift_ssl_config.to_dict())
 
         # Support missing 'method' for backwards compatibility
         if method == RedshiftConnectionMethod.DATABASE or method is None:
             # this requirement is really annoying to encode into json schema,
             # so validate it here
             if self.credentials.password is None:
                 raise dbt.exceptions.FailedToConnectError(
@@ -338,15 +422,15 @@
             connection, cursor = super().add_query(
                 query, auto_begin, bindings=bindings, abridge_sql_log=abridge_sql_log
             )
 
         if cursor is None:
             conn = self.get_thread_connection()
             conn_name = conn.name if conn and conn.name else "<None>"
-            raise dbt.exceptions.DbtRuntimeError(f"Tried to run invalid SQL: {sql} on {conn_name}")
+            raise DbtRuntimeError(f"Tried to run invalid SQL: {sql} on {conn_name}")
 
         return connection, cursor
 
     @classmethod
     def get_credentials(cls, credentials):
         return credentials
```

### Comparing `dbt-redshift-1.6.0b2/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.6.0b3/dbt/adapters/redshift/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,7 +159,11 @@
 
     @property
     def default_python_submission_method(self) -> str:
         return super().default_python_submission_method
 
     def generate_python_submission_response(self, submission_result: Any) -> AdapterResponse:
         return super().generate_python_submission_response(submission_result)
+
+    def debug_query(self):
+        """Override for DebugTask method"""
+        self.execute("select 1 as id")
```

### Comparing `dbt-redshift-1.6.0b2/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.6.0b3/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters.sql`

 * *Files 10% similar despite different names*

```diff
@@ -221,15 +221,32 @@
   {% endcall %}
   {% set table = load_result('get_columns_in_relation').table %}
   {{ return(sql_convert_columns_in_relation(table)) }}
 {% endmacro %}
 
 
 {% macro redshift__list_relations_without_caching(schema_relation) %}
-  {{ return(postgres__list_relations_without_caching(schema_relation)) }}
+  {% call statement('list_relations_without_caching', fetch_result=True) -%}
+    select
+      '{{ schema_relation.database }}' as database,
+      tablename as name,
+      schemaname as schema,
+      'table' as type
+    from pg_tables
+    where schemaname ilike '{{ schema_relation.schema }}'
+    union all
+    select
+      '{{ schema_relation.database }}' as database,
+      viewname as name,
+      schemaname as schema,
+      'view' as type
+    from pg_views
+    where schemaname ilike '{{ schema_relation.schema }}'
+  {% endcall %}
+  {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 
 {% macro redshift__information_schema_name(database) -%}
   {{ return(postgres__information_schema_name(database)) }}
 {%- endmacro %}
```

### Comparing `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.6.0b3/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.6.0b3/dbt_redshift.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b2 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b3 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.6.0b2/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.6.0b3/dbt_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b2/setup.py` & `dbt-redshift-1.6.0b3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import sys
 
-if sys.version_info < (3, 7):
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 try:
     from setuptools import find_namespace_packages
 except ImportError:
     print("Error: dbt requires setuptools v40.1.0 or higher.")
@@ -90,15 +90,14 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

