# Comparing `tmp/ckanext-toolbelt-0.3.9.tar.gz` & `tmp/ckanext-toolbelt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-toolbelt-0.3.9.tar", last modified: Thu Apr 13 18:04:17 2023, max compression
+gzip compressed data, was "ckanext-toolbelt-0.4.0.tar", last modified: Sat Jun 10 18:43:55 2023, max compression
```

## Comparing `ckanext-toolbelt-0.3.9.tar` & `ckanext-toolbelt-0.4.0.tar`

### file list

```diff
@@ -1,94 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/search_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_gh_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_gulp-sass.js
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_black.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_commitizen.toml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_isort.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_pyright.toml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_pytest.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/magic/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/magic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/cascade_organization_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/safe_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/types/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.944797 ckanext-toolbelt-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-06-10 18:43:55.944797 ckanext-toolbelt-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-10 18:43:55.944797 ckanext-toolbelt-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.932797 ckanext-toolbelt-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.936797 ckanext-toolbelt-0.4.0/src/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.936797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.936797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.936797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/ckan/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/ckan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/ckan/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/ckan/search_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_gh_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.936797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/action_release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/action_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/config_gulp-sass.js
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/config_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/template_black.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/template_commitizen.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/template_isort.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/template_pyright.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/template_pytest.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/template_ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.936797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/magic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/cascade_organization_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_scroll/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_scroll/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/group_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/group_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/safe_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.932797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.932797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/group/
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.932797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/plugins/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/plugins/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/utils/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/utils/test_hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.940797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.944797 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/scheming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-10 18:43:46.000000 ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:43:55.944797 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-06-10 18:43:55.000000 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-10 18:43:55.000000 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:43:55.000000 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 18:43:55.000000 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 18:43:55.000000 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-10 18:43:55.000000 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 18:43:55.000000 ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/top_level.txt
```

### Comparing `ckanext-toolbelt-0.3.9/LICENSE` & `ckanext-toolbelt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/PKG-INFO` & `ckanext-toolbelt-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: ckanext-toolbelt
-Version: 0.3.9
-Home-page: https://github.com/DataShades/ckanext-toolbelt
-Author: Sergey Motornyuk
-Author-email: sergey.motornyuk@linkdigital.com.au
-License: AGPL
-Keywords: CKAN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ckanext-toolbelt
 
 Collection of different tools for daily use.
 
 
 ## Requirements
 
@@ -33,21 +15,22 @@
 ## Content
 
 * [Decorators](#decorators)
   * [Collector](#collector)
   * [Cache](#cache)
 * [Plugins](#plugins)
 * [CLI](#cli)
+* [Misc](#misc)
 
 
 ## Decorators (`ckanext.toolbelt.decorators`)
 
 ### `Collector`
 
-Creates a decorator that can collect functions and return them in a
+Creates a decorator that collects functions and returns them in a
 dictionary. Originally designed for actions, auth functions, validators and
 helpers.
 
 :information_source: CKAN v2.10 has `tk.blanket` module. It does the same
 things in a bit different manner.
 
 Can be used as decorator. Call `Collector.get_collection` when you need
@@ -163,24 +146,30 @@
 
 ## Plugins
 
 ### `toolbelt_fdt_sqlalchemy`
 
 Adapter for
 [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/). Enables
-SQLAlchemy panel on FlaskDebugToolbar. You have to install appropriate version
-of `flask-sqlalchemy` to use this plugin:
+SQLAlchemy panel on FlaskDebugToolbar. You have to install `flask-sqlalchemy`
+extra to use this plugin:
+
+```sh
+pip install 'ckanext-toolbelt[flask-sqlalchemy]'
+```
+
+### `toolbelt_cascade_organization_updates`
+
+Reindex all organization's datasets when organization updated. Requires
+background worker.
+
+### `toolbelt_composite_groups` / `toolbelt_composite_organizations`
 
-| Environment                     | Version | Command                             |
-|---------------------------------|---------|-------------------------------------|
-| Flask 2.0(CKAN <= 2.10)         | 2.5     | `pip install flask-sqlalchemy~=2.5` |
-| Flask 2.2(CKAN >= 2.11, master) | 3.0     | `pip install flask-sqlalchemy~=3.0` |
+Enable repeating subfields(ckanext-scheming) for organization and group schemas
 
-Note: `flask-sqlalchemy~=2.5` works with the latest CKAN version, so you can
-always use the first line from the table above.
 
 [Back to content](#content)
 ---
 
 ## CLI
 
 As soon as you've installed ckanext-toolbelt, it will register `ckan toolbelt`
@@ -200,14 +189,15 @@
 Global commands, available via `ctb` and `ckan toolbelt` routes:
 
 ```sh
 # create a generic configuration. Supported types:
 # * deps-makefile  CKAN dependency manager
 # * pre-commit     Pre-commit
 # * pyproject      pyproject.toml
+# * gulp-sass      gulpfile.js with SASS configuration
 make config <type>
 
 # create a configuration for GitHub Action. Supported types:
 # * pypi-publish    Publish package to PyPI when vX.Y.Z tag added.
 # * release-please  Create a PR that compiles changelog and publishes GitHub release.
 # * test            Test workflow.
 make gh-action <type>
@@ -229,7 +219,67 @@
 search-index clear-missing
 
 # Clean the DB, optionally keeping data in the given tables.
 db clean --yes [-k user] [-k group] [-k ...]
 ```
 
 [Back to content](#content)
+
+---
+
+## Misc
+
+### `ckanext.toolbelt.utils.cache`
+#### `DontCache`
+#### `Cache`
+
+### `ckanext.toolbelt.utils.fs`
+#### StaticPath
+
+No-op wrapper around filepath that can be used as a context manager:
+```python
+with StaticPath("/tmp/x.txt") as path:
+    with open(path) as src:
+        ...
+# nothing is changed
+```
+
+#### RemovablePath
+
+Context manager that removes file on exit:
+```python
+with RemovablePath("/tmp/x.txt") as path:
+    with open(path) as src:
+        ...
+# /tmp/x.txt is removed
+```
+
+#### `path_to_resource(res_dict, max_size=0)`
+
+Returns a filepath for a resource.
+
+If resource is stored locally, return StaticPath. If resource stored remotely,
+download it to /tmp and return RemovablePath. Remote resources with size
+exceeding `max_size` are not downloaded and empty StaticPath returned.
+
+Example:
+```python
+with path_to_resource(resource) as path:
+    with open(path) as src:
+        print(src.read())
+```
+
+
+### `ckanext.toolbelt.utils.scheming`
+#### `get_validation_schema`
+
+### `ckanext.toolbelt.utils.structures`
+#### `Node`
+
+### `ckanext.toolbelt.utils.hierarchy`
+#### `Node`
+#### `Strategy`
+#### `ParentReference`
+#### `package_hierarchy`
+
+
+[Back to content](#content)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/_shared.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/_shared.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 from string import Template
-from typing import Any, Optional
+from typing import Any
 
 import click
 
 option_plugin = click.option(
     "-p",
     "--plugin",
     default="",
@@ -28,32 +28,35 @@
     if not plugin:
         plugin = os.path.basename(os.getcwd())
         if plugin.startswith("ckanext-"):
             plugin = plugin[8:]
     return plugin
 
 
-def render(tpl: str, data: Optional[dict[str, Any]] = None) -> str:
+def render(tpl: str, data: dict[str, Any] | None = None) -> str:
     source = os.path.join(os.path.dirname(__file__), "templates", tpl)
-    return Template(open(source).read()).safe_substitute(**data or {})
+    with open(source) as stream:
+        return Template(stream.read()).safe_substitute(**data or {})
 
 
 def template_source(name: str) -> str:
     return f"template_{name}.toml"
 
 
 def ensure_root():
     ext = os.path.basename(os.getcwd())
     if not ext.startswith("ckanext-"):
         click.secho(
-            "Can be executed only from the root directory of the extension", fg="red"
+            "Can be executed only from the root directory of the extension",
+            fg="red",
         )
-        raise click.Abort()
+        raise click.Abort
 
 
 def produce(src: str, dest: str, data: dict[str, Any], write: bool):
-    file = None
-    if write:
-        file = open(dest, "w")
-
     content = render(src, data).strip()
-    click.echo(content, file)
+
+    if write:
+        with open(dest, "w") as file:
+            click.echo(content, file)
+    else:
+        click.echo(content)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/db.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/ckan/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import click
 
-import ckan.model as model
 import ckan.plugins.toolkit as tk
+from ckan import model
 
 
 @click.group(short_help="Extra tools for managing DB")
 def db():
     pass
 
 
@@ -15,15 +15,15 @@
 @click.option("-y", "--yes", is_flag=True, help="Confirm your intention.")
 @click.option("-k", "--keep", multiple=True, help="Tables that should not be cleaned")
 def clean(yes: bool, keep: tuple[str]):
     if not yes:
         tk.error_shout("This command will erase data from your portal's DB.")
         tk.error_shout("All the datasets, organizations and users will be removed")
         tk.error_shout("Run it with `--yes` flag if you know what you are doing.")
-        raise click.Abort()
+        raise click.Abort
 
     model.repo.session.remove()
     ## use raw connection for performance
     connection = model.repo.session.connection()
     tables = reversed(model.repo.metadata.sorted_tables)
 
     for table in tables:
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/search_index.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/ckan/search_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 
-import ckan.model as model
 import ckan.plugins.toolkit as tk
+from ckan import model
 from ckan.lib.search import clear, query_for
 
 
 @click.group(short_help="Extra tools for managing search-index")
 def search_index():
     pass
 
@@ -34,15 +34,15 @@
 
     click.echo("Following packages are missing from the database:")
     for id in ids:
         click.echo("\t" + id)
 
     if not no_confirm:
         abort = not click.confirm(
-            "Do you want to remove these packages from the search index?"
+            "Do you want to remove these packages from the search index?",
         )
         if abort:
-            raise click.Abort()
+            raise click.Abort
 
     with click.progressbar(ids) as bar:
         for id_ in bar:
             clear(id_)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/dev.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/dev.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,35 +6,39 @@
 from aiosmtpd.handlers import Debugging
 
 
 class DecodingDebugging(Debugging):
     def _print_message_content(self, peer, data: bytes):
         msg = email.message_from_bytes(data)
         print("# Headers:", file=self.stream)
-        for (header, value) in msg.items():
+        for header, value in msg.items():
             print(header, ": ", value, file=self.stream)
         print("# Message:", file=self.stream)
         for part in msg.walk():
             print("---------- a part: ----------", file=self.stream)
             maybe_decoded_payload = part.get_payload(decode=True)
             if maybe_decoded_payload is not None:
+                try:
+                    decoded = bytes.decode(maybe_decoded_payload, encoding="utf-8")
+                except UnicodeError as e:
+                    decoded = f"<{e}>"
+
                 print(
-                    bytes.decode(maybe_decoded_payload, encoding="utf-8"),
+                    decoded,
                     file=self.stream,
                 )
 
 
 @click.group()
 def dev():
     """Tools for debugging and development."""
-    pass
 
 
 @dev.command()
 @click.option("-p", "--port", default=8025, type=int)
 @click.option("-h", "--host", default="localhost")
-def mail_server(port, host):
+def mail_server(port: int, host: str):
     """Start mail server that will catch outcomming mails."""
     loop = asyncio.get_event_loop()
-    ctrl = Controller(DecodingDebugging())
+    ctrl = Controller(DecodingDebugging(), host, port)
     ctrl.start()
     loop.run_forever()
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_config.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 @_shared.option_write
 def pyproject(plugin: str, write: bool):
     """pyproject.toml"""
     _shared.ensure_root()
     plugin = _shared.safe_plugin_name(plugin)
     data = {
         f"{part.upper()}_CONFIG": _shared.render(
-            _shared.template_source(part), {"PLUGIN": plugin}
+            _shared.template_source(part),
+            {"PLUGIN": plugin},
         )
         for part in ["black", "ruff", "isort", "pytest", "pyright", "commitizen"]
     }
     data["PLUGIN"] = plugin
 
     _shared.produce(*_config_files("pyproject"), data, write)
 
@@ -77,8 +78,8 @@
     if name == "deps-makefile":
         return f"config_{name}.sh", "Makefile"
 
     if name == "gulp-sass":
         return f"config_{name}.js", "gulpfile.js"
 
     click.secho(f"Unsupported config: {name}", fg="red")
-    raise click.Abort()
+    raise click.Abort
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_gh_action.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_gh_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from . import _shared
 
 
 @click.group()
 def gh_action():
     """Make GitHub actions."""
-    pass
 
 
 @gh_action.command()
 @_shared.option_plugin
 @_shared.option_write
 def test(plugin: str, write: bool):
     """Test workflow."""
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_readme.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """Print declared config options for the given plugins."""
 
     from ckan.config.declaration import Declaration
     from ckan.config.declaration.serialize import handler
 
     if not plugins:
         click.secho("At leas one plugin must be specified", fg="red")
-        raise click.Abort()
+        raise click.Abort
     handler.register("ckanext-readme")(_ckanext_readme)
 
     decl = Declaration()
     for name in plugins:
         decl.load_plugin(name)
 
     if decl:
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_template.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/make_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-from typing import Optional
-
 import click
 
 from . import _shared
 
 option_file = click.option(
     "-f",
     "--file",
@@ -20,85 +18,85 @@
 def template():
     """Print fragments that are used by other make commands."""
 
 
 @template.command()
 @_shared.option_plugin
 @option_file
-def black(plugin: str, file: Optional[str]):
+def black(plugin: str, file: str | None):
     """Black configuration"""
     _shared.ensure_root()
     _shared.produce(
         _shared.template_source("black"),
         file or "",
         {"PLUGIN": _shared.safe_plugin_name(plugin)},
         bool(file),
     )
 
 
 @template.command()
 @_shared.option_plugin
 @option_file
-def isort(plugin: str, file: Optional[str]):
+def isort(plugin: str, file: str | None):
     """Isort configuration"""
     _shared.ensure_root()
     _shared.produce(
         _shared.template_source("isort"),
         file or "",
         {"PLUGIN": _shared.safe_plugin_name(plugin)},
         bool(file),
     )
 
 
 @template.command()
 @_shared.option_plugin
 @option_file
-def ruff(plugin: str, file: Optional[str]):
+def ruff(plugin: str, file: str | None):
     """Ruff configuration"""
     _shared.ensure_root()
     _shared.produce(
         _shared.template_source("ruff"),
         file or "",
         {"PLUGIN": _shared.safe_plugin_name(plugin)},
         bool(file),
     )
 
 
 @template.command()
 @_shared.option_plugin
 @option_file
-def pyright(plugin: str, file: Optional[str]):
+def pyright(plugin: str, file: str | None):
     """Pyrigh configuration"""
     _shared.ensure_root()
     _shared.produce(
         _shared.template_source("pyright"),
         file or "",
         {"PLUGIN": _shared.safe_plugin_name(plugin)},
         bool(file),
     )
 
 
 @template.command()
 @_shared.option_plugin
 @option_file
-def pytest(plugin: str, file: Optional[str]):
+def pytest(plugin: str, file: str | None):
     """Pytest configuration"""
     _shared.ensure_root()
     _shared.produce(
         _shared.template_source("pytest"),
         file or "",
         {"PLUGIN": _shared.safe_plugin_name(plugin)},
         bool(file),
     )
 
 
 @template.command()
 @_shared.option_plugin
 @option_file
-def commitizen(plugin: str, file: Optional[str]):
+def commitizen(plugin: str, file: str | None):
     """Commitizen configuration"""
     _shared.ensure_root()
     _shared.produce(
         _shared.template_source("commitizen"),
         file or "",
         {"PLUGIN": _shared.safe_plugin_name(plugin)},
         bool(file),
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_test.yaml` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/action_test.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_gulp-sass.js` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/config_gulp-sass.js`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_pyright.toml` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/cli/templates/template_pyright.toml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/magic/__init__.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/magic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 log = logging.getLogger(__name__)
 
 
 def conjure_fast_group_activities():
     log.info("ieiunium sicut ventus")
 
     def ___group_activity_perfomance_patch(group_id, include_hidden_activity=False):
-        import ckan.model as model
+        from ckan import model
 
         group = model.Group.get(group_id)
         if not group:
             # Return a query with no results.
             return model.Session.query(model.Activity).filter(text("0=1"))  # noqa
 
         q = model.Session.query(model.Activity)
@@ -38,15 +38,15 @@
         packages_sq = (
             model.Session.query(model.Package.id)
             .filter_by(owner_org=group_id, private=False)
             .subquery()
         )
 
         member_activity = model.Session.query(model.Activity).filter(
-            model.Activity.object_id.in_(packages_sq)
+            model.Activity.object_id.in_(packages_sq),
         )
 
         if not include_hidden_activity:
             group_activity = _filter_activitites_from_users(group_activity)  # noqa
             member_activity = _filter_activitites_from_users(member_activity)  # noqa
         return _activities_union_all(group_activity, member_activity)  # noqa
 
@@ -62,15 +62,15 @@
     """Proces a file before uploading it to datastore.
 
     Accepts callable, that receives path to original file and resource
     ID. Callable can override file in order to provide a valid CSV that can be
     ingested into datastore.
 
     """
-    import ckanext.xloader.loader as loader
+    from ckanext.xloader import loader
 
     log.info("quae non sunt ut simplex")
 
     _o = loader.load_csv
 
     def _wrapper(csv_filepath, resource_id, mimetype="text/csv", logger=None):
         new_path = func(csv_filepath, resource_id)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from __future__ import annotations
 
 import logging
+from typing import TYPE_CHECKING
 
 from werkzeug.utils import import_string
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
 from ckan import model
 
+if TYPE_CHECKING:
+    from ckan.common import CKANConfig
+    from ckan.config.middleware.flask_app import CKANFlask
+
+
 SQLAlchemy = import_string("flask_sqlalchemy:SQLAlchemy", True)
 
 _EngineDebuggingSignalEvents = import_string(
     "flask_sqlalchemy:_EngineDebuggingSignalEvents",
     True,
 )
 record_queries = import_string("flask_sqlalchemy.record_queries", True)
@@ -20,15 +26,15 @@
 log = logging.getLogger(__name__)
 
 
 class FdtSqlalchemyPlugin(p.SingletonPlugin):
     p.implements(p.IConfigurable)
     p.implements(p.IMiddleware, inherit=True)
 
-    def make_middleware(self, app, config):
+    def make_middleware(self, app: CKANFlask, config: CKANConfig):
         if not SQLAlchemy:
             version = "3.0" if tk.check_ckan_version("2.11.0") else "2.5"
             log.error(
                 "Flask-SQLAlchemy is not installed. "
                 "Run `pip install flask-sqlalchemy~=%s` and restart the application",
                 version,
             )
@@ -36,13 +42,15 @@
 
         app.config.setdefault("SQLALCHEMY_TRACK_MODIFICATIONS", False)
         app.config["SQLALCHEMY_DATABASE_URI"] = config["sqlalchemy.url"]
         SQLAlchemy().init_app(app)
 
         return app
 
-    def configure(self, _config):
+    def configure(self, _config: CKANConfig):
+        # v2.5
         if _EngineDebuggingSignalEvents:
             _EngineDebuggingSignalEvents(model.meta.engine, "ckan").register()
 
+        # v3.0 / select and explain are not compatible with flask-debugtoolbar
         if record_queries:
             record_queries._listen(model.meta.engine)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_changes.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/group_changes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import logging
 from datetime import datetime
 from typing import Any
 
 from flask import Blueprint
 
-import ckan.model as model
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
+from ckan import model
 from ckan.views.group import _replace_group_org, set_org
 
 log = logging.getLogger(__name__)
 
 toolbelt = Blueprint("toolbelt_group_changes", __name__)
 
 CONFIG_WATCH_FIELDS = "ckanext.toolbelt.group_changes.watch_fields"
@@ -78,34 +78,34 @@
             {
                 "type": field,
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "new_value": new.get(field),
                 "old_value": old.get(field),
                 "method": "change",
-            }
+            },
         )
     elif not new.get(field):
         change_list.append(
             {
                 "type": field,
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "method": "remove",
-            }
+            },
         )
     else:
         change_list.append(
             {
                 "type": field,
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "new_value": new.get(field),
                 "method": "add",
-            }
+            },
         )
 
 
 def _description_change(change_list, old, new):
     """
     Appends a summary of a change to a organization's description between two
     versions (old and new) to change_list.
@@ -117,34 +117,34 @@
             {
                 "type": "description",
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "new_description": new.get("description"),
                 "old_description": old.get("description"),
                 "method": "change",
-            }
+            },
         )
     elif not new.get("description"):
         change_list.append(
             {
                 "type": "description",
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "method": "remove",
-            }
+            },
         )
     else:
         change_list.append(
             {
                 "type": "description",
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "new_description": new.get("description"),
                 "method": "add",
-            }
+            },
         )
 
 
 def _image_url_change(change_list, old, new):
     """
     Appends a summary of a change to a organization's image URL between two
     versions (old and new) to change_list.
@@ -155,37 +155,37 @@
             {
                 "type": "image_url",
                 "method": "change",
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "new_image_url": new.get("image_url"),
                 "old_image_url": old.get("image_url"),
-            }
+            },
         )
     # if the user removed the image URL
     elif not new.get("image_url"):
         change_list.append(
             {
                 "type": "image_url",
                 "method": "remove",
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "old_image_url": old.get("image_url"),
-            }
+            },
         )
     # if there wasn't one there before
     else:
         change_list.append(
             {
                 "type": "image_url",
                 "method": "add",
                 "pkg_id": new.get("id"),
                 "title": new.get("title"),
                 "new_image_url": new.get("image_url"),
-            }
+            },
         )
 
 
 def compare_group_dicts(old: dict[str, Any], new: dict[str, Any], old_activity_id: str):
     """
     Takes two package dictionaries that represent consecutive versions of
     the same organization and returns a list of detailed & formatted summaries
@@ -234,26 +234,27 @@
             {
                 "id": activity_id,
                 "object_type": "group",
                 "diff_type": "html",
             },
         )
     except tk.ObjectNotFound as e:
-        log.info("Activity not found: {} - {}".format(str(e), activity_id))
+        log.info("Activity not found: %s - %s", e, activity_id)
         return tk.abort(404, tk._("Activity not found"))
     except tk.NotAuthorized:
         return tk.abort(403, tk._("Unauthorized to view activity data"))
 
     # 'group_dict' needs to go to the templates for page title & breadcrumbs.
     # Use the current version of the package, in case the name/title have
     # changed, and we need a link to it which works
     group_id = activity_diff["activities"][1]["data"]["group"]["id"]
     current_group_dict = tk.get_action(group_type + "_show")(context, {"id": group_id})
     group_activity_list = tk.get_action(group_type + "_activity_list")(
-        context, {"id": group_id, "limit": 100}
+        context,
+        {"id": group_id, "limit": 100},
     )
 
     extra_vars: dict[str, Any] = {
         "activity_diffs": [activity_diff],
         "group_dict": current_group_dict,
         "group_activity_list": group_activity_list,
         "group_type": current_group_dict["type"],
@@ -282,18 +283,20 @@
         "user": tk.g.user,
         "auth_user_obj": tk.g.userobj,
     }
 
     # check to ensure that the old activity is actually older than
     # the new activity
     old_activity = tk.get_action("activity_show")(
-        context, {"id": old_id, "include_data": False}
+        context,
+        {"id": old_id, "include_data": False},
     )
     new_activity = tk.get_action("activity_show")(
-        context, {"id": new_id, "include_data": False}
+        context,
+        {"id": new_id, "include_data": False},
     )
 
     old_timestamp = old_activity["timestamp"]
     new_timestamp = new_activity["timestamp"]
 
     t1 = datetime.strptime(old_timestamp, "%Y-%m-%dT%H:%M:%S.%f")
     t2 = datetime.strptime(new_timestamp, "%Y-%m-%dT%H:%M:%S.%f")
@@ -318,30 +321,31 @@
                 {
                     "id": current_id,
                     "object_type": "group",
                     "diff_type": "html",
                 },
             )
         except tk.ObjectNotFound as e:
-            log.info("Activity not found: {} - {}".format(str(e), current_id))
+            log.info("Activity not found: %s - %s", e, current_id)
             return tk.abort(404, tk._("Activity not found"))
         except tk.NotAuthorized:
             return tk.abort(403, tk._("Unauthorized to view activity data"))
 
         diff_list.append(activity_diff)
 
         if activity_diff["activities"][0]["id"] == old_id:
             done = True
         else:
             current_id = activity_diff["activities"][0]["id"]
 
     group_id: str = diff_list[0]["activities"][1]["data"]["group"]["id"]
     current_group_dict = tk.get_action(group_type + "_show")(context, {"id": group_id})
     group_activity_list = tk.get_action(group_type + "_activity_list")(
-        context, {"id": group_id, "limit": 100}
+        context,
+        {"id": group_id, "limit": 100},
     )
 
     extra_vars: dict[str, Any] = {
         "activity_diffs": diff_list,
         "group_dict": current_group_dict,
         "group_activity_list": group_activity_list,
         "group_type": current_group_dict["type"],
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_composite.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/group_composite.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         Validate and convert for package_create, package_update and
         package_show actions.
         """
         thing, action_type = action.split("_")
         t = data_dict.get("type")
         if not t or t not in self._schemas:
             return data_dict, {
-                "type": "Unsupported {thing} type: {t}".format(thing=thing, t=t)
+                "type": f"Unsupported {thing} type: {t}",
             }
 
         scheming_schema = self._expanded_schemas[t]
 
         before = scheming_schema.get("before_validators")
         after = scheming_schema.get("after_validators")
         if action_type == "show":
@@ -37,39 +37,46 @@
         elif action_type == "create":
             get_validators = _field_create_validators
         else:
             get_validators = _field_validators
 
         if before:
             schema["__before"] = validation.validators_from_string(
-                before, None, scheming_schema
+                before,
+                None,
+                scheming_schema,
             )
         if after:
             schema["__after"] = validation.validators_from_string(
-                after, None, scheming_schema
+                after,
+                None,
+                scheming_schema,
             )
         fg = ((scheming_schema["fields"], schema, True),)
 
         composite_convert_fields = []
         for field_list, destination, convert_extras in fg:
             for f in field_list:
                 convert_this = convert_extras and f["field_name"] not in schema
                 destination[f["field_name"]] = get_validators(
-                    f, scheming_schema, convert_this
+                    f,
+                    scheming_schema,
+                    convert_this,
                 )
                 if convert_this and "repeating_subfields" in f:
                     composite_convert_fields.append(f["field_name"])
 
         def composite_convert_to(key, data, errors, context):
             unflat = unflatten(data)
             for f in composite_convert_fields:
                 if f not in unflat:
                     continue
                 data[(f,)] = json.dumps(
-                    unflat[f], default=lambda x: None if x == tk.missing else x
+                    unflat[f],
+                    default=lambda x: None if x == tk.missing else x,
                 )
                 convert_to_extras((f,), data, errors, context)
                 del data[(f,)]
 
         if action_type == "show":
             if composite_convert_fields:
                 for ex in data_dict["extras"]:
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/safe_upload.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/safe_upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import os
 import uuid
-from typing import Optional
 
 import magic
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
 from ckan.lib import uploader
 
@@ -17,22 +16,23 @@
     # IUploader
 
     def get_resource_uploader(self, data_dict):
         for plugin in p.PluginImplementations(p.IUploader):
             if isinstance(plugin, type(self)):
                 continue
             return plugin.get_resource_uploader(data_dict)
+        return None
 
     def get_uploader(self, upload_to, old_filename=None):
         return SafeUpload(upload_to, old_filename)
 
 
 class SafeUpload(uploader.Upload):
     storage_path: str
-    filename: Optional[str]
+    filename: str | None
 
     def update_data_dict(self, data_dict, url_field, file_field, clear_field):
         super().update_data_dict(data_dict, url_field, file_field, clear_field)
         if self.filename:
             self.verify_type()
 
             self.filename = str(uuid.uuid3(uuid.NAMESPACE_DNS, self.filename))
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/cache.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,82 @@
 import json
 import logging
 import pickle  # nosec: B403
-from functools import wraps
-from typing import Any, Callable, Generic, Optional, TypeVar, Union, cast
+from functools import update_wrapper
+from typing import Any, Callable, Generic, Optional, Protocol, TypeVar, Union, cast
+
+from typing_extensions import ParamSpec
 
 from ckan.lib import redis
 
 from . import constantly
 
 log = logging.getLogger(__name__)
 T = TypeVar("T")
+TC = TypeVar("TC", covariant=True)
+P = ParamSpec("P")
 
 
 class DontCache(Generic[T]):
     __slots__ = ("value",)
     value: T
 
     def __init__(self, value: T):
         self.value = value
 
     def unwrap(self) -> T:
         return self.value
 
 
 MaybeNotCached = Union[T, DontCache[T]]
-CacheAwareCallable = Callable[..., MaybeNotCached[T]]
-NaiveCallable = Callable[..., T]
+CacheAwareCallable = Callable[P, MaybeNotCached[T]]
+
+
+class NaiveCallable(Generic[P, TC], Protocol):
+    def reset(self, *args: P.args, **kwargs: P.kwargs) -> int:
+        ...
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> TC:
+        ...
 
-CacheDecorator = Callable[[CacheAwareCallable[T]], NaiveCallable[T]]
+
+CacheDecorator = Callable[[CacheAwareCallable[P, T]], NaiveCallable[P, T]]
 
 Duration = Optional[int]
 DurationStrategy = Callable[..., Duration]
 
 KeyStr = Union[str, bytes]
 KeyStrategy = Callable[..., KeyStr]
 
 Dumper = Callable[[T], KeyStr]
 Loader = Callable[[KeyStr], T]
 
 
-def default_key_strategy(func, *args, **kwargs) -> bytes:
+def default_key_strategy(func: Callable[..., Any], *args: Any, **kwargs: Any) -> bytes:
     return bytes(f"{func.__module__}:{func.__name__}", "utf8") + pickle.dumps(
         (args, kwargs),
     )
 
 
 def decorate_key_strategy(prefix: bytes, after: bool = False) -> KeyStrategy:
-    def strategy(*args, **kwargs):
+    def strategy(*args: Any, **kwargs: Any):
         left = prefix
         right = default_key_strategy(*args, **kwargs)
         if after:
             left, right = right, left
 
         return left + right
 
     return strategy
 
 
 class Cache(Generic[T]):
     duration: DurationStrategy
     key: KeyStrategy
-    conn: redis.Redis
+    conn: "redis.Redis[bytes]"
     dumper: Dumper[T]
     loader: Loader[T]
 
     def __init__(
         self,
         duration: Union[DurationStrategy, Duration] = None,
         key: Union[KeyStrategy, KeyStr] = default_key_strategy,
@@ -83,32 +95,36 @@
 
         self.conn = redis.connect_to_redis()
 
     @staticmethod
     def dont_cache(value: T):
         return DontCache(value)
 
-    def __call__(self, func: CacheAwareCallable[T]) -> NaiveCallable[T]:
-        @wraps(func)
-        def wrapper(*args: Any, **kwargs: Any) -> T:
-            key = self.key(func, *args, **kwargs)
-            old_value = self.conn.get(key)
-
-            if old_value:
-                log.debug("Hit cache for key %s", key)
-                return self.loader(old_value)
-
-            value = func(*args, **kwargs)
-            if isinstance(value, DontCache):
-                return cast(T, value.unwrap())
-
-            duration = self.duration(func, *args, **kwargs)
-            self.conn.set(key, self.dumper(value), ex=duration or None)
-            return value
-
-        def reset(*args: Any, **kwargs: Any) -> int:
-            key = self.key(func, *args, **kwargs)
-            return self.conn.delete(key)
-
-        wrapper.reset = reset
-
-        return wrapper
+    def __call__(self, func: CacheAwareCallable[P, T]) -> NaiveCallable[P, T]:
+        caller = Caller(func, self)
+        return cast(Caller[P, T], update_wrapper(caller, func))
+
+
+class Caller(NaiveCallable[P, T]):
+    def __init__(self, func: CacheAwareCallable[P, T], cache: Cache[T]):
+        self.func = func
+        self.cache = cache
+
+    def reset(self, *args: P.args, **kwargs: P.kwargs) -> int:
+        key = self.cache.key(self.func, *args, **kwargs)
+        return self.cache.conn.delete(key)
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
+        key = self.cache.key(self.func, *args, **kwargs)
+        old_value = self.cache.conn.get(key)
+
+        if old_value:
+            log.debug("Hit cache for key %s", key)
+            return self.cache.loader(old_value)
+
+        value = self.func(*args, **kwargs)
+        if isinstance(value, DontCache):
+            return cast(T, value.unwrap())
+
+        duration = self.cache.duration(self.func, *args, **kwargs)
+        self.cache.conn.set(key, self.cache.dumper(value), ex=duration or None)
+        return value
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/collector.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/collector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import copy
-from typing import Any, Callable, Generic, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar
 
-from typing_extensions import Self
+if TYPE_CHECKING:
+    from typing_extensions import Self
 
 TFunc = TypeVar("TFunc", bound=Callable[..., Any])
 
 
 class Collector(Generic[TFunc]):
     collection: dict[str, TFunc]
 
@@ -19,23 +20,23 @@
 
         else:
             self.prefix = ""
 
     def split(self) -> tuple[Self, Callable[[], dict[str, TFunc]]]:
         return self, self.get_collection
 
-    def __call__(self, func_or_name: Union[str, TFunc]):
+    def __call__(self, func_or_name: str | TFunc):
         name: str
 
         def adder(func: TFunc):
             self.collection[name] = func
             return func
 
         if isinstance(func_or_name, str):
             name = func_or_name
             return adder
 
-        name = self.prefix + getattr(func_or_name, "__name__")
+        name = self.prefix + func_or_name.__name__
         return adder(func_or_name)
 
     def get_collection(self) -> dict[str, TFunc]:
         return copy.copy(self.collection)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/fs.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/fs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import logging
 import os
 import tempfile
-from typing import Optional
 
 import requests
 
 import ckan.plugins as p
 from ckan.lib.uploader import get_resource_uploader
 
 log = logging.getLogger(__name__)
 
 DEFAULT_DOWNLOAD_TIMEOUT = 2
 
 
 class StaticPath:
-    def __init__(self, path: Optional[str]):
+    def __init__(self, path: str | None):
         self.path = path
 
     def __bool__(self):
         return bool(self.path)
 
     def __enter__(self):
         return self.path
@@ -32,15 +31,26 @@
 class RemovablePath(StaticPath):
     def __exit__(self, type_, value, traceback):
         if self.path:
             os.remove(self.path)
 
 
 def path_to_resource(res, max_size: int = 0) -> StaticPath:
-    """Returns a filepath for a resource that will be indexed"""
+    """Returns a filepath for a resource.
+
+    If resource is stored locally, return StaticPath. If resource stored
+    remotely, download it to /tmp and return RemovablePath.
+
+    Example:
+
+      with path_to_resource(resource) as path:
+          with open(path) as src:
+              print(src.read())
+
+    """
     res_id = res["id"]
     res_url = res["url"]
 
     if res["url_type"] == "upload":
         uploader = get_resource_uploader(res)
 
         # TODO temporary workaround for ckanext-cloudstorage support
@@ -59,63 +69,63 @@
     if max_size > 0:
         filepath = _download_remote_file(res_id, res_url, max_size)
         return RemovablePath(filepath)
 
     return StaticPath(None)
 
 
-def _download_remote_file(res_id: str, url: str, max_size: int) -> Optional[str]:
+def _download_remote_file(res_id: str, url: str, max_size: int) -> str | None:
     """
     Downloads remote resource and save it as temporary file
     Returns path to this file
     """
 
     try:
         resp = requests.get(
             url,
             timeout=DEFAULT_DOWNLOAD_TIMEOUT,
             stream=True,
             headers={"user-agent": "python/toolbelt"},
         )
-    except Exception as e:
+    except requests.RequestException as e:
         log.warning(
             "Unable to make GET request for resource %s with url <%s>: %s",
             res_id,
             url,
             e,
         )
-        return
+        return None
 
     if not resp.ok:
         log.warning(
             "Unsuccessful GET request for resource %s with url <%s>. \
             Status code: %s",
             res_id,
             url,
             resp.status_code,
         )
-        return
+        return None
 
     try:
         size = int(resp.headers.get("content-length", 0))
     except ValueError:
         log.warning("Incorrect Content-length header from url <%s>", url)
-        return
+        return None
 
     if not size:
         log.debug("Cannot determine size")
-        return
+        return None
 
     if size > max_size:
         log.debug("File exceeds allowed size(%d): %d", max_size, size)
-        return
+        return None
 
     dest = tempfile.NamedTemporaryFile(delete=False)
     try:
         with dest:
             for chunk in resp.iter_content(1024 * 64):
                 dest.write(chunk)
-    except requests.exceptions.RequestException as e:
-        log.error("Cannot index remote resource %s with url <%s>: %s", res_id, url, e)
+    except requests.RequestException:
+        log.exception("Cannot index remote resource %s with url <%s>", res_id, url)
         os.remove(dest.name)
-        return
+        return None
     return dest.name
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/hierarchy.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/hierarchy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import abc
 import logging
-from typing import Any, Iterable, Optional, Type
-
-from typing_extensions import TypeAlias
+from typing import TYPE_CHECKING, Any, Iterable
 
 import ckan.plugins.toolkit as tk
 from ckan.lib.search.query import solr_literal
 
 from ckanext.toolbelt.utils.structures import Node
 
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
 log = logging.getLogger(__name__)
 
 PackageDict: TypeAlias = "dict[str, Any]"
 
 CONFIG_PARENT_FIELD = "ckanext.toolbelt.package_hierarchy.parent_field"
 DEFAULT_PARENT_FIELD = "parent_id"
 
@@ -57,35 +58,35 @@
 
         parent_distance = config_parent_distance()
         child_distance = config_child_distance()
         sibling_limit = config_sibling_limit()
 
         if tk.request:
             parent_distance = tk.asint(
-                tk.request.args.get("__relationship_parent_distance", parent_distance)
+                tk.request.args.get("__relationship_parent_distance", parent_distance),
             )
             child_distance = tk.asint(
-                tk.request.args.get("__relationship_child_distance", child_distance)
+                tk.request.args.get("__relationship_child_distance", child_distance),
             )
 
             sibling_limit = tk.asint(
-                tk.request.args.get("__relationship_sibling_limit", sibling_limit)
+                tk.request.args.get("__relationship_sibling_limit", sibling_limit),
             )
 
         self.parent_distance = parent_distance
         self.child_distance = child_distance
         self.sibling_limit = sibling_limit
 
     @abc.abstractmethod
     def root(self, pkg: PackageDict) -> tuple[PackageDict, int]:
-        raise NotImplementedError()
+        raise NotImplementedError
 
     @abc.abstractmethod
     def children(self, pkg: PackageDict) -> Iterable[PackageDict]:
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
 class ParentReference(Strategy):
     def __init__(self, context: dict[str, Any]):
         super().__init__(context)
         self.parent_field = config_parent_field()
         self.reference_field = config_reference_field()
@@ -128,44 +129,42 @@
                 "rows": self.sibling_limit,
             },
         )["results"]
 
 
 def package_hierarchy(
     id_: str,
-    context: Optional[dict[str, Any]] = None,
-    strategy_factory: Type[Strategy] = ParentReference,
+    context: dict[str, Any] | None = None,
+    strategy_factory: type[Strategy] = ParentReference,
 ) -> Node[PackageDict]:
     """Return a Node starting from the **reacheable** root of the package's
     hierarchy.
     """
     ctx = context or {}
     root: PackageDict = tk.get_action("package_show")(dict(ctx), {"id": id_})
 
     strategy = strategy_factory(ctx)
     root, distance = strategy.root(root)
 
-    hierarchy = _package_as_node(root, distance, strategy)
-    return hierarchy
+    return _package_as_node(root, distance, strategy)
 
 
 def _package_as_node(
-    pkg: PackageDict, buffer: int, strategy: Strategy
+    pkg: PackageDict,
+    buffer: int,
+    strategy: Strategy,
 ) -> Node[PackageDict]:
     """Recursive function that wraps package into Node and attach children to
     it as leaves.
 
     """
     children: Iterable[PackageDict]
 
     depth_capacity = buffer + strategy.child_distance
-    if depth_capacity:
-        children = strategy.children(pkg)
-    else:
-        children = []
+    children = strategy.children(pkg) if depth_capacity else []
 
     node = Node(
         pkg,
         [_package_as_node(child, buffer - 1, strategy) for child in children],
     )
 
     for child in node.leaves:
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/structures.py` & `ckanext-toolbelt-0.4.0/src/ckanext/toolbelt/utils/structures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import dataclasses
-from collections.abc import Collection
-from typing import Any, Generic, Optional, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
+
+if TYPE_CHECKING:
+    from collections.abc import Collection
+
 
 T = TypeVar("T")
 
 
 @dataclasses.dataclass
 class Node(Generic[T]):
     value: T
     leaves: Collection[Node[T]] = ()
-    parent: Optional[Node] = None
+    parent: Node[T] | None = None
     data: dict[str, Any] = dataclasses.field(default_factory=dict)
 
     def __iter__(self):
         return iter(self.leaves)
 
     def __len__(self):
         return len(self.leaves)
 
-    def __eq__(self, other: Any):
+    def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Node):
             return False
 
-        return self.value == other.value and self.leaves == other.leaves
+        return bool(self.value == other.value and self.leaves == other.leaves)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/PKG-INFO` & `ckanext-toolbelt-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.3.9
+Version: 0.4.0
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: flask-sqlalchemy
 License-File: LICENSE
 
 # ckanext-toolbelt
 
 Collection of different tools for daily use.
 
 
@@ -33,21 +34,22 @@
 ## Content
 
 * [Decorators](#decorators)
   * [Collector](#collector)
   * [Cache](#cache)
 * [Plugins](#plugins)
 * [CLI](#cli)
+* [Misc](#misc)
 
 
 ## Decorators (`ckanext.toolbelt.decorators`)
 
 ### `Collector`
 
-Creates a decorator that can collect functions and return them in a
+Creates a decorator that collects functions and returns them in a
 dictionary. Originally designed for actions, auth functions, validators and
 helpers.
 
 :information_source: CKAN v2.10 has `tk.blanket` module. It does the same
 things in a bit different manner.
 
 Can be used as decorator. Call `Collector.get_collection` when you need
@@ -163,24 +165,30 @@
 
 ## Plugins
 
 ### `toolbelt_fdt_sqlalchemy`
 
 Adapter for
 [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/). Enables
-SQLAlchemy panel on FlaskDebugToolbar. You have to install appropriate version
-of `flask-sqlalchemy` to use this plugin:
+SQLAlchemy panel on FlaskDebugToolbar. You have to install `flask-sqlalchemy`
+extra to use this plugin:
 
-| Environment                     | Version | Command                             |
-|---------------------------------|---------|-------------------------------------|
-| Flask 2.0(CKAN <= 2.10)         | 2.5     | `pip install flask-sqlalchemy~=2.5` |
-| Flask 2.2(CKAN >= 2.11, master) | 3.0     | `pip install flask-sqlalchemy~=3.0` |
+```sh
+pip install 'ckanext-toolbelt[flask-sqlalchemy]'
+```
+
+### `toolbelt_cascade_organization_updates`
+
+Reindex all organization's datasets when organization updated. Requires
+background worker.
+
+### `toolbelt_composite_groups` / `toolbelt_composite_organizations`
+
+Enable repeating subfields(ckanext-scheming) for organization and group schemas
 
-Note: `flask-sqlalchemy~=2.5` works with the latest CKAN version, so you can
-always use the first line from the table above.
 
 [Back to content](#content)
 ---
 
 ## CLI
 
 As soon as you've installed ckanext-toolbelt, it will register `ckan toolbelt`
@@ -200,14 +208,15 @@
 Global commands, available via `ctb` and `ckan toolbelt` routes:
 
 ```sh
 # create a generic configuration. Supported types:
 # * deps-makefile  CKAN dependency manager
 # * pre-commit     Pre-commit
 # * pyproject      pyproject.toml
+# * gulp-sass      gulpfile.js with SASS configuration
 make config <type>
 
 # create a configuration for GitHub Action. Supported types:
 # * pypi-publish    Publish package to PyPI when vX.Y.Z tag added.
 # * release-please  Create a PR that compiles changelog and publishes GitHub release.
 # * test            Test workflow.
 make gh-action <type>
@@ -229,7 +238,67 @@
 search-index clear-missing
 
 # Clean the DB, optionally keeping data in the given tables.
 db clean --yes [-k user] [-k group] [-k ...]
 ```
 
 [Back to content](#content)
+
+---
+
+## Misc
+
+### `ckanext.toolbelt.utils.cache`
+#### `DontCache`
+#### `Cache`
+
+### `ckanext.toolbelt.utils.fs`
+#### StaticPath
+
+No-op wrapper around filepath that can be used as a context manager:
+```python
+with StaticPath("/tmp/x.txt") as path:
+    with open(path) as src:
+        ...
+# nothing is changed
+```
+
+#### RemovablePath
+
+Context manager that removes file on exit:
+```python
+with RemovablePath("/tmp/x.txt") as path:
+    with open(path) as src:
+        ...
+# /tmp/x.txt is removed
+```
+
+#### `path_to_resource(res_dict, max_size=0)`
+
+Returns a filepath for a resource.
+
+If resource is stored locally, return StaticPath. If resource stored remotely,
+download it to /tmp and return RemovablePath. Remote resources with size
+exceeding `max_size` are not downloaded and empty StaticPath returned.
+
+Example:
+```python
+with path_to_resource(resource) as path:
+    with open(path) as src:
+        print(src.read())
+```
+
+
+### `ckanext.toolbelt.utils.scheming`
+#### `get_validation_schema`
+
+### `ckanext.toolbelt.utils.structures`
+#### `Node`
+
+### `ckanext.toolbelt.utils.hierarchy`
+#### `Node`
+#### `Strategy`
+#### `ParentReference`
+#### `package_hierarchy`
+
+
+[Back to content](#content)
```

### Comparing `ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/entry_points.txt` & `ckanext-toolbelt-0.4.0/src/ckanext_toolbelt.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,7 +14,10 @@
 toolbelt_safe_upload = ckanext.toolbelt.plugins.safe_upload:SafeUploadPlugin
 
 [ckan.system_plugins]
 toolbelt_fdt_scroll = ckanext.toolbelt.plugins.fdt_scroll.plugin:FdtScrollPlugin
 
 [console_scripts]
 ctb = ckanext.toolbelt.cli:toolbelt
+
+[pytest11]
+toolbelt = pytest_toolbelt.plugin
```

### Comparing `ckanext-toolbelt-0.3.9/setup.cfg` & `ckanext-toolbelt-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-toolbelt
-version = 0.3.9
+version = 0.4.0
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-toolbelt
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
@@ -20,19 +20,20 @@
 
 [options]
 python_requires = >= 3.7
 install_requires = 
 	click
 	aiosmtpd
 	typing_extensions
-packages = find:
 namespace_packages = ckanext
 include_package_data = True
 
 [options.extras_require]
+flask-sqlalchemy = 
+	flask-sqlalchemy~=2.5
 
 [options.entry_points]
 ckan.plugins = 
 	toolbelt = ckanext.toolbelt.plugins:ToolbeltPlugin
 	
 	toolbelt_safe_upload = ckanext.toolbelt.plugins.safe_upload:SafeUploadPlugin
 	
@@ -44,14 +45,16 @@
 	toolbelt_cascade_organization_updates = ckanext.toolbelt.plugins.cascade_organization_updates:CascadeOrganizationUpdatesPlugin
 	
 	toolbelt_fdt_sqlalchemy = ckanext.toolbelt.plugins.fdt_sqlalchemy:FdtSqlalchemyPlugin
 ckan.system_plugins = 
 	toolbelt_fdt_scroll = ckanext.toolbelt.plugins.fdt_scroll.plugin:FdtScrollPlugin
 ckan.click_command = 
 	toolbelt = ckanext.toolbelt.cli.ckan:toolbelt
+pytest11 = 
+	toolbelt = pytest_toolbelt.plugin
 console_scripts = 
 	ctb = ckanext.toolbelt.cli:toolbelt
 babel.extractors = 
 	ckan = ckan.lib.extract:extract_ckan
 
 [extract_messages]
 keywords = translate isPlural
```

