# Comparing `tmp/Flask-BigApp-2023.1.9.2.tar.gz` & `tmp/Flask-BigApp-2023.1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-BigApp-2023.1.9.2.tar", last modified: Thu May 18 11:18:49 2023, max compression
+gzip compressed data, was "Flask-BigApp-2023.1.9.3.tar", last modified: Sat Jun 10 15:06:04 2023, max compression
```

## Comparing `Flask-BigApp-2023.1.9.2.tar` & `Flask-BigApp-2023.1.9.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/
--rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.9.2/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.9.2/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      699 2023-05-04 14:17:25.000000 Flask-BigApp-2023.1.9.2/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      271 2023-04-10 18:03:50.000000 Flask-BigApp-2023.1.9.2/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      174 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-05-18 11:18:34.000000 Flask-BigApp-2023.1.9.2/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.276734 Flask-BigApp-2023.1.9.2/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-05-18 11:18:49.000000 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-05-18 11:18:49.000000 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-18 11:18:49.000000 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-05-18 11:18:49.000000 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)      101 2023-05-18 11:18:49.000000 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-05-18 11:18:49.000000 Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp/
--rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    10308 2023-04-05 11:13:29.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    11183 2023-05-18 11:18:16.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/bigapp.py
--rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-05-18 10:09:34.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/blueprint.py
--rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-04-01 16:09:06.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-05-03 21:04:51.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/orm.py
--rw-rw-r--   0 david     (1000) david     (1000)      788 2023-05-18 10:27:54.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/registeries.py
--rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/resources.py
--rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-04-09 22:17:36.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/security.py
--rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-03-31 22:23:19.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp/utilities.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.276734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.276734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
--rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
--rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
--rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.276734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.276734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
--rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
--rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
--rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
--rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
--rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
--rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
--rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/resources.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 11:18:49.280734 Flask-BigApp-2023.1.9.2/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     2462 2023-05-18 10:22:21.000000 Flask-BigApp-2023.1.9.2/tests/test_group.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/
+-rw-rw-r--   0 david     (1000) david     (1000)    25342 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      699 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      271 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      174 2023-06-10 15:06:04.925279 Flask-BigApp-2023.1.9.3/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-06-10 14:58:31.000000 Flask-BigApp-2023.1.9.3/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-10 14:53:19.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)      101 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp/
+-rw-rw-r--   0 david     (1000) david     (1000)      305 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10522 2023-06-10 14:56:44.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/auth.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11183 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/bigapp.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/blueprint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/orm.py
+-rw-rw-r--   0 david     (1000) david     (1000)      788 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/registeries.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/resources.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/security.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/utilities.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
+-rw-rw-r--   0 david     (1000) david     (1000)       45 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
+-rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
+-rw-rw-r--   0 david     (1000) david     (1000)      268 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
+-rw-rw-r--   0 david     (1000) david     (1000)      315 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
+-rw-rw-r--   0 david     (1000) david     (1000)      302 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
+-rw-rw-r--   0 david     (1000) david     (1000)      766 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
+-rw-rw-r--   0 david     (1000) david     (1000)       13 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
+-rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)      992 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/resources.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2537 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/tests/test_group.py
```

### Comparing `Flask-BigApp-2023.1.9.2/LICENSE` & `Flask-BigApp-2023.1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/PKG-INFO` & `Flask-BigApp-2023.1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.2
+Version: 2023.1.9.3
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.2/README.md` & `Flask-BigApp-2023.1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/setup.py` & `Flask-BigApp-2023.1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path(pathlib.Path.cwd() / "README.md").read_text()
 
 setup(
     name='Flask-BigApp',
-    version=f'2023.1.9.2',
+    version=f'2023.1.9.3',
     url='https://github.com/Flask-Planet/Flask-BigApp',
     license='GNU Lesser General Public License v2.1',
     author='David Carmichael',
     author_email='carmichaelits@gmail.com',
     description='A Flask auto importer that allows your Flask apps to grow big.',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
```

### Comparing `Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/PKG-INFO` & `Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.2
+Version: 2023.1.9.3
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.2/src/Flask_BigApp.egg-info/SOURCES.txt` & `Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/auth.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,28 +104,33 @@
         this is used to pepper the password
         :param password:
         :return str:
         """
         return "".join(choice(ascii_letters) for _ in range(1)) + password
 
     @classmethod
-    def sha_password(cls, password: str, salt: str, encrypt: int = 512) -> str:
+    def hash_password(cls, password: str, salt: str, encrypt: int = 512) -> str:
         """
         Takes user's password, peppers in, salts it, then converts it to sha
         Can set encryption to 256/512 - 256 is system
         :param password:
         :param salt:
         :param encrypt:
         :return str: hash:
         """
         sha = sha512() if encrypt == 512 else sha256()
         sha.update((cls.generate_pepper(password) + salt).encode("utf-8"))
         return sha.hexdigest()
 
     @classmethod
+    def sha_password(cls, password: str, salt: str, encrypt: int = 512) -> str:
+        """ Legacy method, use hash_password instead """
+        return cls.hash_password(password, salt, encrypt)
+
+    @classmethod
     def auth_password(cls, input_password: str, database_password: str, database_salt: str,
                       encrypt: int = 512) -> bool:
         """
         Takes user's password (input_password), loops over all possible ascii_letters joining
         to the password as a pepper, then salts using salt value in the database, then converts it
         to sha, then compares that loop result to the database password to find a match
         Can set encryption to 256/512 - 256 is system
```

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/bigapp.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/bigapp.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/blueprint.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/blueprint.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/helpers.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/orm.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/orm.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/registeries.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/registeries.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/resources.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/security.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/security.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp/utilities.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp/utilities.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/cli.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/src/flask_bigapp_cli/resources.py` & `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.2/tests/test_group.py` & `Flask-BigApp-2023.1.9.3/tests/test_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+
+
 def test_general_setup(client):
     """
     If this test is successful, the app is set up and running correctly.
     """
     response = client.get('/tests/')
     assert response.status_code == 200
 
@@ -70,14 +73,16 @@
     assert b"Database created." in response.data
 
 
 def test_mixin_create(client):
     """
     If this test is successful, the mixin is working correctly.
     """
+    if os.environ.get("DOCKER_TESTING", False):
+        return
     response = client.get('/tests/mixin-add')
     assert b"MixinTest" in response.data
 
 
 def test_database_population(client):
     """
     If this test is successful, the database has been populated correctly.
```

