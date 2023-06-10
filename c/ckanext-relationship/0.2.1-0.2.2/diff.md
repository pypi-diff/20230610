# Comparing `tmp/ckanext-relationship-0.2.1.tar.gz` & `tmp/ckanext-relationship-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-relationship-0.2.1.tar", last modified: Sat Mar 11 15:43:37 2023, max compression
+gzip compressed data, was "ckanext-relationship-0.2.2.tar", last modified: Sat Jun 10 18:46:39 2023, max compression
```

## Comparing `ckanext-relationship-0.2.1.tar` & `ckanext-relationship-0.2.2.tar`

### file list

```diff
@@ -1,52 +1,60 @@
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)    34500 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/LICENSE
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      216 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/MANIFEST.in
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/PKG-INFO
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4414 2023-03-11 15:42:59.000000 ckanext-relationship-0.2.1/README.md
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.622561 ckanext-relationship-0.2.1/ckanext/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      221 2023-03-08 22:38:22.000000 ckanext-relationship-0.2.1/ckanext/__init__.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/__init__.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/assets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      335 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/assets/webassets.yml
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2140 2023-03-11 11:44:20.000000 ckanext-relationship-0.2.1/ckanext/relationship/helpers.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/logic/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/logic/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     5522 2023-03-11 06:53:47.000000 ckanext-relationship-0.2.1/ckanext/relationship/logic/action.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      598 2023-03-08 22:38:22.000000 ckanext-relationship-0.2.1/ckanext/relationship/logic/auth.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1885 2023-03-08 22:38:22.000000 ckanext-relationship-0.2.1/ckanext/relationship/logic/schema.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2330 2023-03-11 15:06:22.000000 ckanext-relationship-0.2.1/ckanext/relationship/logic/validators.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.622561 ckanext-relationship-0.2.1/ckanext/relationship/migration/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1820 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/alembic.ini
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2228 2023-03-08 22:38:44.000000 ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/env.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      494 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/script.py.mako
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/versions/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      660 2023-03-08 22:38:22.000000 ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/model/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/model/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       83 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/model/base.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     3064 2023-03-11 06:47:49.000000 ckanext-relationship-0.2.1/ckanext/relationship/model/relationship.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4930 2023-03-11 06:47:49.000000 ckanext-relationship-0.2.1/ckanext/relationship/plugin.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      323 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/presets.yaml
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.622561 ckanext-relationship-0.2.1/ckanext/relationship/templates/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.622561 ckanext-relationship-0.2.1/ckanext/relationship/templates/scheming/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/templates/scheming/display_snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      658 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/templates/scheming/display_snippets/related_entity.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/templates/scheming/form_snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2029 2023-03-11 15:08:00.000000 ckanext-relationship-0.2.1/ckanext/relationship/templates/scheming/form_snippets/related_entity.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext/relationship/tests/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/ckanext/relationship/tests/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1218 2023-03-11 06:49:18.000000 ckanext-relationship-0.2.1/ckanext/relationship/tests/test_plugin.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2213 2023-03-11 06:54:59.000000 ckanext-relationship-0.2.1/ckanext/relationship/utils.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-03-11 15:43:37.626561 ckanext-relationship-0.2.1/ckanext_relationship.egg-info/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-03-11 15:43:37.000000 ckanext-relationship-0.2.1/ckanext_relationship.egg-info/PKG-INFO
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1377 2023-03-11 15:43:37.000000 ckanext-relationship-0.2.1/ckanext_relationship.egg-info/SOURCES.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        1 2023-03-11 15:43:37.000000 ckanext-relationship-0.2.1/ckanext_relationship.egg-info/dependency_links.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      134 2023-03-11 15:43:37.000000 ckanext-relationship-0.2.1/ckanext_relationship.egg-info/entry_points.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-03-11 15:43:37.000000 ckanext-relationship-0.2.1/ckanext_relationship.egg-info/namespace_packages.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-03-11 15:43:37.000000 ckanext-relationship-0.2.1/ckanext_relationship.egg-info/top_level.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2979 2023-03-11 06:50:51.000000 ckanext-relationship-0.2.1/pyproject.toml
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       23 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.1/requirements.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      613 2023-03-11 15:43:37.630560 ckanext-relationship-0.2.1/setup.cfg
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     3727 2023-03-11 15:06:13.000000 ckanext-relationship-0.2.1/setup.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)    34500 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/LICENSE
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      216 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/MANIFEST.in
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/PKG-INFO
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4414 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/README.md
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      221 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/__init__.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/__init__.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/assets/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/assets/js/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)    10889 2023-06-10 18:34:43.000000 ckanext-relationship-0.2.2/ckanext/relationship/assets/js/relationship-autocomplete.js
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      340 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.2/ckanext/relationship/assets/webassets.yml
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2535 2023-06-10 09:11:53.000000 ckanext-relationship-0.2.2/ckanext/relationship/helpers.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/logic/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     5522 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/action.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      598 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/auth.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1885 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/schema.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2702 2023-06-10 18:38:05.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/validators.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/migration/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1820 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/alembic.ini
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2228 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/env.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      494 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/script.py.mako
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/versions/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      660 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/model/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/model/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       83 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/model/base.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3064 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/model/relationship.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4769 2023-06-10 09:11:35.000000 ckanext-relationship-0.2.2/ckanext/relationship/plugin.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      323 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/presets.yaml
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/templates/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      126 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/page.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/templates/relationship/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/templates/relationship/snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       43 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/relationship/snippets/asset.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/display_snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      658 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/display_snippets/related_entity.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2036 2023-06-10 11:22:47.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/related_entity.html
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1150 2023-06-10 09:49:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/tests/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/tests/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1218 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/tests/test_plugin.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2213 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/utils.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1316 2023-06-10 18:38:05.000000 ckanext-relationship-0.2.2/ckanext/relationship/views.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/PKG-INFO
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1664 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        1 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      134 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/entry_points.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/namespace_packages.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/top_level.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2979 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/pyproject.toml
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       23 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/requirements.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      613 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/setup.cfg
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3727 2023-06-10 18:38:51.000000 ckanext-relationship-0.2.2/setup.py
```

### Comparing `ckanext-relationship-0.2.1/LICENSE` & `ckanext-relationship-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/PKG-INFO` & `ckanext-relationship-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-relationship
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/DataShades/ckanext-relationship
 Author: Oleksandr Ivaniuk
 Author-email: aleks.ivaniuk@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-relationship-0.2.1/README.md` & `ckanext-relationship-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/logic/action.py` & `ckanext-relationship-0.2.2/ckanext/relationship/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/logic/auth.py` & `ckanext-relationship-0.2.2/ckanext/relationship/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/logic/schema.py` & `ckanext-relationship-0.2.2/ckanext/relationship/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/logic/validators.py` & `ckanext-relationship-0.2.2/ckanext/relationship/logic/validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 
 from ckantoolkit import missing
+from six import string_types
 
 import ckan.plugins.toolkit as tk
 
 from ckanext.scheming.validation import (
     scheming_multiple_choice_output,
     scheming_validator,
 )
@@ -20,18 +21,19 @@
 
     def validator(key, data, errors, context):
         if field.get("required") and data[key] is missing:
             errors[key].append(tk._("Select at least one"))
 
         entity_id = data.get(("id",))
 
-        current_relations = _get_current_relations(
+        current_relations = get_current_relations(
             entity_id, related_entity, related_entity_type, relation_type
         )
-        selected_relations = _get_selected_relations(data[key])
+
+        selected_relations = get_selected_relations(data[key])
 
         data[key] = json.dumps([value for value in selected_relations])
 
         add_relations = selected_relations - current_relations
         del_relations = current_relations - selected_relations
 
         data[("add_relations",)] = data.get(("add_relations",), [])
@@ -39,15 +41,15 @@
 
         data[("add_relations",)].extend([(rel, relation_type) for rel in add_relations])
         data[("del_relations",)].extend([(rel, relation_type) for rel in del_relations])
 
     return validator
 
 
-def _get_current_relations(
+def get_current_relations(
     entity_id, related_entity, related_entity_type, relation_type
 ):
     if entity_id:
         current_relations = tk.get_action("relationship_relations_list")(
             {},
             {
                 "subject_id": entity_id,
@@ -58,15 +60,24 @@
         )
         current_relations = [rel["object_id"] for rel in current_relations]
     else:
         current_relations = []
     return set(current_relations)
 
 
-def _get_selected_relations(selected):
-    selected_relations = selected
+def get_selected_relations(selected_relations):
+    if isinstance(selected_relations, string_types) and "," in selected_relations:
+        selected_relations = selected_relations.split(",")
+
+    if (
+        len(selected_relations) == 1
+        and isinstance(selected_relations[0], string_types)
+        and "," in selected_relations[0]
+    ):
+        selected_relations = selected_relations[0].split(",")
+
     if selected_relations is not missing:
-        selected_relations = scheming_multiple_choice_output(selected)
+        selected_relations = scheming_multiple_choice_output(selected_relations)
         selected_relations = [] if selected_relations == [""] else selected_relations
     else:
         selected_relations = []
     return set(selected_relations)
```

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/alembic.ini` & `ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/env.py` & `ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py` & `ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/model/relationship.py` & `ckanext-relationship-0.2.2/ckanext/relationship/model/relationship.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/plugin.py` & `ckanext-relationship-0.2.2/ckanext/relationship/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 import ckanext.relationship.utils as utils
 
 
 @tk.blanket.actions
 @tk.blanket.auth_functions
 @tk.blanket.validators
 @tk.blanket.helpers
+@tk.blanket.blueprints
 class RelationshipPlugin(plugins.SingletonPlugin):
     plugins.implements(plugins.IConfigurer)
-    plugins.implements(plugins.IActions)
-    plugins.implements(plugins.IAuthFunctions)
-    plugins.implements(plugins.IValidators)
-    plugins.implements(plugins.ITemplateHelpers)
     plugins.implements(plugins.IPackageController, inherit=True)
 
     # IConfigurer
     def update_config(self, config_):
         tk.add_template_directory(config_, "templates")
         tk.add_public_directory(config_, "public")
-        tk.add_resource("fanstatic", "relationship")
+        tk.add_resource("assets", "relationship")
 
     # IPackageController
     def after_dataset_create(self, context, pkg_dict):
         context = context.copy()
         context.pop("__auth_audit", None)
         return _update_relations(context, pkg_dict)
```

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/templates/scheming/display_snippets/related_entity.html` & `ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/display_snippets/related_entity.html`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/templates/scheming/form_snippets/related_entity.html` & `ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/related_entity.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ) %}
 
   {% set current_entity_id = data.get('id', None) %}
   {% set entities = h.relationship_get_entity_list(field.related_entity, field.related_entity_type) %}
   {% set choices = [] %}
 
   {% for entity in entities if entity.id != current_entity_id %}
-    {% if 'updatable_only' not in (field) or
+    {% if not field.get('updatable_only', false) or
           h.check_access(field.related_entity ~ '_update', {'id': entity.id }) %}
       {% do choices.append((entity.id, entity.get('title') or entity.get('name'))) %}
     {% endif %}
   {% endfor %}
 
   {% set choices = choices|sort(case_sensitive=false, attribute=1) %}
```

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/tests/test_plugin.py` & `ckanext-relationship-0.2.2/ckanext/relationship/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext/relationship/utils.py` & `ckanext-relationship-0.2.2/ckanext/relationship/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/ckanext_relationship.egg-info/PKG-INFO` & `ckanext-relationship-0.2.2/ckanext_relationship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-relationship
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/DataShades/ckanext-relationship
 Author: Oleksandr Ivaniuk
 Author-email: aleks.ivaniuk@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-relationship-0.2.1/ckanext_relationship.egg-info/SOURCES.txt` & `ckanext-relationship-0.2.2/ckanext_relationship.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,34 @@
 setup.py
 ckanext/__init__.py
 ckanext/relationship/__init__.py
 ckanext/relationship/helpers.py
 ckanext/relationship/plugin.py
 ckanext/relationship/presets.yaml
 ckanext/relationship/utils.py
+ckanext/relationship/views.py
 ckanext/relationship/assets/webassets.yml
+ckanext/relationship/assets/js/relationship-autocomplete.js
 ckanext/relationship/logic/__init__.py
 ckanext/relationship/logic/action.py
 ckanext/relationship/logic/auth.py
 ckanext/relationship/logic/schema.py
 ckanext/relationship/logic/validators.py
 ckanext/relationship/migration/relationship/alembic.ini
 ckanext/relationship/migration/relationship/env.py
 ckanext/relationship/migration/relationship/script.py.mako
 ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py
 ckanext/relationship/model/__init__.py
 ckanext/relationship/model/base.py
 ckanext/relationship/model/relationship.py
+ckanext/relationship/templates/page.html
+ckanext/relationship/templates/relationship/snippets/asset.html
 ckanext/relationship/templates/scheming/display_snippets/related_entity.html
 ckanext/relationship/templates/scheming/form_snippets/related_entity.html
+ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html
 ckanext/relationship/tests/__init__.py
 ckanext/relationship/tests/test_plugin.py
 ckanext_relationship.egg-info/PKG-INFO
 ckanext_relationship.egg-info/SOURCES.txt
 ckanext_relationship.egg-info/dependency_links.txt
 ckanext_relationship.egg-info/entry_points.txt
 ckanext_relationship.egg-info/namespace_packages.txt
```

### Comparing `ckanext-relationship-0.2.1/pyproject.toml` & `ckanext-relationship-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/setup.cfg` & `ckanext-relationship-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.1/setup.py` & `ckanext-relationship-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description = f.read()
 
 setup(
     name="""ckanext-relationship""",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version="0.2.1",
+    version="0.2.2",
     description="""""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/DataShades/ckanext-relationship",
     # Author details
     author="""Oleksandr Ivaniuk""",
```

