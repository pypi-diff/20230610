# Comparing `tmp/django-torque-0.5.0a1.tar.gz` & `tmp/django-torque-0.5.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-torque-0.5.0a1.tar", last modified: Mon Apr 17 15:31:00 2023, max compression
+gzip compressed data, was "django-torque-0.5.0a2.tar", last modified: Sat Jun 10 11:47:21 2023, max compression
```

## Comparing `django-torque-0.5.0a1.tar` & `django-torque-0.5.0a2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1624 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/README.md
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/django_torque.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3016 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       68 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/top_level.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1186 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.072728 django-torque-0.5.0a1/torque/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/apps.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.076728 django-torque-0.5.0a1/torque/cache_rebuilder/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/cache_rebuilder/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      475 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/cache_rebuilder/apps.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6295 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/cache_rebuilder/background.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.072728 django-torque-0.5.0a1/torque/management/
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.076728 django-torque-0.5.0a1/torque/management/commands/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/management/commands/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/management/commands/remove_unattached.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/torque/migrations/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12576 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0001_initial.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      437 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0002_auto_20210321_1604.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      451 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0003_auto_20210321_1725.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      729 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0005_auto_20210323_1303.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      573 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0006_auto_20210323_1623.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      839 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0007_auto_20210406_1738.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      373 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0008_auto_20210406_1909.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0009_sheetconfig_search_cache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1360 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0010_tableofcontentscache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0011_auto_20210416_1739.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0012_searchcacherow_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0013_spreadsheet_last_updated.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      404 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0014_tableofcontentscache_rendered_html.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      364 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2472 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0016_auto_20210721_1444.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      661 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0017_auto_20210721_1621.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      303 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0018_delete_permissiongroup.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      825 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0019_auto_20210721_1720.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0020_tableofcontents_raw.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      326 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0021_remove_column_type.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      636 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0022_auto_20210905_1430.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      837 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0023_auto_20210905_1454.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      767 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0024_auto_20210905_1535.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      791 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0025_auto_20210905_1624.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      893 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0026_auto_20210905_1638.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1333 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0027_auto_20210905_1642.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1328 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0028_auto_20210905_1659.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2538 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0029_auto_20210905_1716.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      580 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0030_auto_20210927_1304.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      707 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0031_auto_20210930_1328.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      399 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0032_searchcachedocument_filtered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      877 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0033_csvspecification.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1643 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0034_auto_20220209_1209.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0035_template_in_config.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      803 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      472 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0037_template_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      521 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0038_wiki_linked_wiki_keys.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0039_document_attached.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      456 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0040_value_unique_value_for_field_document.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      417 2023-03-28 11:03:24.000000 django-torque-0.5.0a1/torque/migrations/0041_searchcachedocument_explore_rank.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1245 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/torque/migrations/0042_documentdictcache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/torque/migrations/0043_documentdictcache_unique_document_dict.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      414 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/torque/migrations/0044_documentdictcache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      669 2023-04-10 15:44:16.000000 django-torque-0.5.0a1/torque/migrations/0045_templatecachedocument_dirty_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      325 2023-04-10 15:44:16.000000 django-torque-0.5.0a1/torque/migrations/0046_delete_templatecachedocument.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1585 2023-04-10 15:44:16.000000 django-torque-0.5.0a1/torque/migrations/0047_templatecachedocument_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-04-12 11:15:37.000000 django-torque-0.5.0a1/torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    25665 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/models.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     4809 2023-03-28 11:03:24.000000 django-torque-0.5.0a1/torque/urls.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3489 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/utils.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       30 2023-04-17 15:28:54.000000 django-torque-0.5.0a1/torque/version.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    36134 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/views.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.454963 django-torque-0.5.0a2/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-06-10 11:47:21.450963 django-torque-0.5.0a2/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1624 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/README.md
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.450963 django-torque-0.5.0a2/django_torque.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3016 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       68 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/top_level.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-06-10 11:47:21.454963 django-torque-0.5.0a2/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1186 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.438964 django-torque-0.5.0a2/torque/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/apps.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.438964 django-torque-0.5.0a2/torque/cache_rebuilder/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/cache_rebuilder/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      475 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/cache_rebuilder/apps.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6295 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/cache_rebuilder/background.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.434963 django-torque-0.5.0a2/torque/management/
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.438964 django-torque-0.5.0a2/torque/management/commands/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/management/commands/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/management/commands/remove_unattached.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.450963 django-torque-0.5.0a2/torque/migrations/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12576 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0001_initial.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      437 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0002_auto_20210321_1604.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      451 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0003_auto_20210321_1725.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      729 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0005_auto_20210323_1303.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      573 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0006_auto_20210323_1623.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      839 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0007_auto_20210406_1738.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      373 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0008_auto_20210406_1909.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0009_sheetconfig_search_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1360 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0010_tableofcontentscache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0011_auto_20210416_1739.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0012_searchcacherow_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0013_spreadsheet_last_updated.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      404 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0014_tableofcontentscache_rendered_html.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      364 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2472 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0016_auto_20210721_1444.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      661 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0017_auto_20210721_1621.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      303 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0018_delete_permissiongroup.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      825 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0019_auto_20210721_1720.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0020_tableofcontents_raw.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      326 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0021_remove_column_type.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      636 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0022_auto_20210905_1430.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      837 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0023_auto_20210905_1454.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      767 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0024_auto_20210905_1535.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      791 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0025_auto_20210905_1624.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      893 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0026_auto_20210905_1638.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1333 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0027_auto_20210905_1642.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1328 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0028_auto_20210905_1659.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2538 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0029_auto_20210905_1716.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      580 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0030_auto_20210927_1304.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      707 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0031_auto_20210930_1328.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      399 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0032_searchcachedocument_filtered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      877 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0033_csvspecification.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1643 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0034_auto_20220209_1209.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0035_template_in_config.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      803 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      472 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0037_template_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      521 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0038_wiki_linked_wiki_keys.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0039_document_attached.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      456 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0040_value_unique_value_for_field_document.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      417 2023-03-28 11:03:24.000000 django-torque-0.5.0a2/torque/migrations/0041_searchcachedocument_explore_rank.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1245 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0042_documentdictcache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0043_documentdictcache_unique_document_dict.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      414 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0044_documentdictcache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      669 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0045_templatecachedocument_dirty_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      325 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0046_delete_templatecachedocument.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1585 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0047_templatecachedocument_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    25665 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/models.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     4809 2023-03-28 11:03:24.000000 django-torque-0.5.0a2/torque/urls.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3489 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/utils.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       30 2023-06-10 11:44:02.000000 django-torque-0.5.0a2/torque/version.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    36146 2023-06-10 11:38:15.000000 django-torque-0.5.0a2/torque/views.py
```

### Comparing `django-torque-0.5.0a1/PKG-INFO` & `django-torque-0.5.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.5.0a1
+Version: 0.5.0a2
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `django-torque-0.5.0a1/README.md` & `django-torque-0.5.0a2/README.md`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/django_torque.egg-info/PKG-INFO` & `django-torque-0.5.0a2/django_torque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.5.0a1
+Version: 0.5.0a2
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `django-torque-0.5.0a1/django_torque.egg-info/SOURCES.txt` & `django-torque-0.5.0a2/django_torque.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/setup.py` & `django-torque-0.5.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/cache_rebuilder/background.py` & `django-torque-0.5.0a2/torque/cache_rebuilder/background.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/management/commands/remove_unattached.py` & `django-torque-0.5.0a2/torque/management/commands/remove_unattached.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0001_initial.py` & `django-torque-0.5.0a2/torque/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0005_auto_20210323_1303.py` & `django-torque-0.5.0a2/torque/migrations/0005_auto_20210323_1303.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0006_auto_20210323_1623.py` & `django-torque-0.5.0a2/torque/migrations/0006_auto_20210323_1623.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0007_auto_20210406_1738.py` & `django-torque-0.5.0a2/torque/migrations/0007_auto_20210406_1738.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0010_tableofcontentscache.py` & `django-torque-0.5.0a2/torque/migrations/0010_tableofcontentscache.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0016_auto_20210721_1444.py` & `django-torque-0.5.0a2/torque/migrations/0016_auto_20210721_1444.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0017_auto_20210721_1621.py` & `django-torque-0.5.0a2/torque/migrations/0017_auto_20210721_1621.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0019_auto_20210721_1720.py` & `django-torque-0.5.0a2/torque/migrations/0019_auto_20210721_1720.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0022_auto_20210905_1430.py` & `django-torque-0.5.0a2/torque/migrations/0022_auto_20210905_1430.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0023_auto_20210905_1454.py` & `django-torque-0.5.0a2/torque/migrations/0023_auto_20210905_1454.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0024_auto_20210905_1535.py` & `django-torque-0.5.0a2/torque/migrations/0024_auto_20210905_1535.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0025_auto_20210905_1624.py` & `django-torque-0.5.0a2/torque/migrations/0025_auto_20210905_1624.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0026_auto_20210905_1638.py` & `django-torque-0.5.0a2/torque/migrations/0026_auto_20210905_1638.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0027_auto_20210905_1642.py` & `django-torque-0.5.0a2/torque/migrations/0027_auto_20210905_1642.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0028_auto_20210905_1659.py` & `django-torque-0.5.0a2/torque/migrations/0028_auto_20210905_1659.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0029_auto_20210905_1716.py` & `django-torque-0.5.0a2/torque/migrations/0029_auto_20210905_1716.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0030_auto_20210927_1304.py` & `django-torque-0.5.0a2/torque/migrations/0030_auto_20210927_1304.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0031_auto_20210930_1328.py` & `django-torque-0.5.0a2/torque/migrations/0031_auto_20210930_1328.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0033_csvspecification.py` & `django-torque-0.5.0a2/torque/migrations/0033_csvspecification.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0034_auto_20220209_1209.py` & `django-torque-0.5.0a2/torque/migrations/0034_auto_20220209_1209.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py` & `django-torque-0.5.0a2/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0038_wiki_linked_wiki_keys.py` & `django-torque-0.5.0a2/torque/migrations/0038_wiki_linked_wiki_keys.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0042_documentdictcache.py` & `django-torque-0.5.0a2/torque/migrations/0042_documentdictcache.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0045_templatecachedocument_dirty_and_more.py` & `django-torque-0.5.0a2/torque/migrations/0045_templatecachedocument_dirty_and_more.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/migrations/0047_templatecachedocument_and_more.py` & `django-torque-0.5.0a2/torque/migrations/0047_templatecachedocument_and_more.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/models.py` & `django-torque-0.5.0a2/torque/models.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/urls.py` & `django-torque-0.5.0a2/torque/urls.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/utils.py` & `django-torque-0.5.0a2/torque/utils.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a1/torque/views.py` & `django-torque-0.5.0a2/torque/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1025,15 +1025,15 @@
                 ):
                     row.extend(
                         settings.TORQUE_CSV_PROCESSORS[field_name].process_value(
                             python_value
                         )
                     )
                 elif field_name in getattr(settings, "TORQUE_CSV_PROCESSORS", {}):
-                    settings.TORQUE_CSV_PROCESSORS[field_name].default_value(field_name)
+                    row.extend(settings.TORQUE_CSV_PROCESSORS[field_name].default_value(field_name))
                 elif python_value:
                     row.append(python_value)
                 else:
                     row.append("")
             writer.writerow(row)
 
         return response
```

