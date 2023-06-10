# Comparing `tmp/flask-useful-0.2.4.tar.gz` & `tmp/flask-useful-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-useful-0.2.4.tar", last modified: Mon Jun  5 19:07:46 2023, max compression
+gzip compressed data, was "flask-useful-0.2.5.tar", last modified: Sat Jun 10 18:25:19 2023, max compression
```

## Comparing `flask-useful-0.2.4.tar` & `flask-useful-0.2.5.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.405021 flask-useful-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-05 19:07:30.000000 flask-useful-0.2.4/.github/workflows/publish-stable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-05 19:07:30.000000 flask-useful-0.2.4/.github/workflows/publish-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 19:07:30.000000 flask-useful-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 19:07:30.000000 flask-useful-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-05 19:07:46.413021 flask-useful-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 19:07:30.000000 flask-useful-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/api/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v1/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v2/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-05 19:07:30.000000 flask-useful-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 19:07:46.413021 flask-useful-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.405021 flask-useful-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/src/flask_useful/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/flask_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/src/flask_useful/sqla/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/src/flask_useful/wtforms/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/src/flask_useful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.679531 flask-useful-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.671531 flask-useful-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-10 18:25:09.000000 flask-useful-0.2.5/.github/workflows/publish-stable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-10 18:25:09.000000 flask-useful-0.2.5/.github/workflows/publish-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 18:25:09.000000 flask-useful-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-10 18:25:09.000000 flask-useful-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-10 18:25:19.679531 flask-useful-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-10 18:25:09.000000 flask-useful-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/examples/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/examples/blueprints/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/examples/blueprints/routes/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/routes/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/examples/blueprints/routes/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/routes/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/routes/api/v1/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/examples/blueprints/routes/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/routes/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/routes/api/v2/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-10 18:25:09.000000 flask-useful-0.2.5/examples/blueprints/routes/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-10 18:25:09.000000 flask-useful-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 18:25:19.679531 flask-useful-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.675531 flask-useful-0.2.5/src/flask_useful/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/confirmation_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/flask_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.679531 flask-useful-0.2.5/src/flask_useful/sqla/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/sqla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/sqla/confirmation_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/sqla/ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/sqla/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/sqla/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.679531 flask-useful-0.2.5/src/flask_useful/wtforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/wtforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/wtforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/wtforms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/wtforms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-10 18:25:09.000000 flask-useful-0.2.5/src/flask_useful/wtforms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:25:19.679531 flask-useful-0.2.5/src/flask_useful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-10 18:25:19.000000 flask-useful-0.2.5/src/flask_useful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-10 18:25:19.000000 flask-useful-0.2.5/src/flask_useful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:25:19.000000 flask-useful-0.2.5/src/flask_useful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-10 18:25:19.000000 flask-useful-0.2.5/src/flask_useful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 18:25:19.000000 flask-useful-0.2.5/src/flask_useful.egg-info/top_level.txt
```

### Comparing `flask-useful-0.2.4/.github/workflows/publish-stable.yml` & `flask-useful-0.2.5/.github/workflows/publish-stable.yml`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/.github/workflows/publish-test.yml` & `flask-useful-0.2.5/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/LICENSE` & `flask-useful-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/PKG-INFO` & `flask-useful-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-useful
-Version: 0.2.4
+Version: 0.2.5
 Summary: A set of useful tools for the Flask microframework.
 Author-email: Kirill Vercetti <office@kyzima-spb.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kyzima-spb/flask-useful
 Project-URL: Repository, https://github.com/kyzima-spb/flask-useful.git
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -48,11 +48,11 @@
    :target: https://github.com/kyzima-spb/flask-useful/stargazers
    :alt: GitHub stars
 
 .. |DOWNLOADS| image:: https://pepy.tech/badge/flask-useful
    :target: https://pepy.tech/project/flask-useful
 
 .. |DOWNLOADS_M| image:: https://pepy.tech/badge/flask-useful/month
-   :target: https://pepy.tech/project/flask-useful)
+   :target: https://pepy.tech/project/flask-useful
 
 .. |DOWNLOADS_W| image:: https://pepy.tech/badge/flask-useful/week
-   :target: https://pepy.tech/project/flask-useful)
+   :target: https://pepy.tech/project/flask-useful
```

### Comparing `flask-useful-0.2.4/README.rst` & `flask-useful-0.2.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,11 +27,11 @@
    :target: https://github.com/kyzima-spb/flask-useful/stargazers
    :alt: GitHub stars
 
 .. |DOWNLOADS| image:: https://pepy.tech/badge/flask-useful
    :target: https://pepy.tech/project/flask-useful
 
 .. |DOWNLOADS_M| image:: https://pepy.tech/badge/flask-useful/month
-   :target: https://pepy.tech/project/flask-useful)
+   :target: https://pepy.tech/project/flask-useful
 
 .. |DOWNLOADS_W| image:: https://pepy.tech/badge/flask-useful/week
-   :target: https://pepy.tech/project/flask-useful)
+   :target: https://pepy.tech/project/flask-useful
```

### Comparing `flask-useful-0.2.4/pyproject.toml` & `flask-useful-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/app.py` & `flask-useful-0.2.5/src/flask_useful/app.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/blueprints.py` & `flask-useful-0.2.5/src/flask_useful/blueprints.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/decorators.py` & `flask-useful-0.2.5/src/flask_useful/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/flask_access.py` & `flask-useful-0.2.5/src/flask_useful/flask_access.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/mail.py` & `flask-useful-0.2.5/src/flask_useful/mail.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/sqla/ma.py` & `flask-useful-0.2.5/src/flask_useful/sqla/ma.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 import typing as t
 
-from marshmallow.validate import (
-    Validator,
-    ValidationError,
-)
+from marshmallow.exceptions import ValidationError
+from marshmallow.validate import Validator
 from sqlalchemy import inspect, select
 
 from .session import sqla_session
 from .utils import get_primary_columns
 
 
 __all__ = (
```

### Comparing `flask-useful-0.2.4/src/flask_useful/sqla/session.py` & `flask-useful-0.2.5/src/flask_useful/sqla/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
-from types import TracebackType
+from contextlib import contextmanager
 import typing as t
 
 from flask import current_app
 from sqlalchemy.orm import Session
 from werkzeug.local import LocalProxy
 
 
 __all__ = (
     'get_sqla_session',
     'sqla_session',
-    'SessionMixin',
 )
 
 
-sqla_session = t.cast(
-    Session,
-    LocalProxy(lambda: get_sqla_session()),
-)
+class SupportsAutocommit(t.Protocol):
+    @property
+    @contextmanager
+    def autocommit(self) -> t.Iterator[Session]: ...
+
+
+class SessionProxyType(Session, SupportsAutocommit):
+    ...
 
 
 def get_sqla_session() -> Session:
     """Returns the current session instance from application context."""
     ext = current_app.extensions.get('sqlalchemy')
 
     if ext is None:
@@ -29,29 +32,28 @@
             'An extension named sqlalchemy was not found '
             'in the list of registered extensions for the current application.'
         )
 
     return t.cast(Session, ext.db.session)
 
 
-class SessionMixin:
-    """
-    The mixin adds a property with the current session
-    and an auto-commit context manager.
-    """
-
-    def __enter__(self) -> Session:
-        return self.session
-
-    def __exit__(
-        self,
-        err_type: t.Optional[t.Type[BaseException]],
-        err: t.Optional[BaseException],
-        traceback: t.Optional[TracebackType]
-    ) -> t.Optional[bool]:
-        if err is None:
-            self.session.commit()
-        return None
+class SessionProxy(LocalProxy[Session]):
+    def __init__(self) -> None:
+        super().__init__(lambda: get_sqla_session())
 
     @property
-    def session(self) -> Session:
-        return sqla_session
+    @contextmanager
+    def autocommit(self) -> t.Iterator[Session]:
+        """
+        Returns the current session as the value of the context manager.
+
+        If successful, commits the changes.
+        """
+        try:
+            yield self._get_current_object()
+        except Exception:
+            raise
+        else:
+            self._get_current_object().commit()
+
+
+sqla_session = t.cast(SessionProxyType, SessionProxy())
```

### Comparing `flask-useful-0.2.4/src/flask_useful/sqla/utils.py` & `flask-useful-0.2.5/src/flask_useful/sqla/utils.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/utils.py` & `flask-useful-0.2.5/src/flask_useful/utils.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/views.py` & `flask-useful-0.2.5/src/flask_useful/views.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/wtforms/fields.py` & `flask-useful-0.2.5/src/flask_useful/wtforms/fields.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/wtforms/filters.py` & `flask-useful-0.2.5/src/flask_useful/wtforms/filters.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/wtforms/validators.py` & `flask-useful-0.2.5/src/flask_useful/wtforms/validators.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful/wtforms/widgets.py` & `flask-useful-0.2.5/src/flask_useful/wtforms/widgets.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.4/src/flask_useful.egg-info/PKG-INFO` & `flask-useful-0.2.5/src/flask_useful.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-useful
-Version: 0.2.4
+Version: 0.2.5
 Summary: A set of useful tools for the Flask microframework.
 Author-email: Kirill Vercetti <office@kyzima-spb.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kyzima-spb/flask-useful
 Project-URL: Repository, https://github.com/kyzima-spb/flask-useful.git
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -48,11 +48,11 @@
    :target: https://github.com/kyzima-spb/flask-useful/stargazers
    :alt: GitHub stars
 
 .. |DOWNLOADS| image:: https://pepy.tech/badge/flask-useful
    :target: https://pepy.tech/project/flask-useful
 
 .. |DOWNLOADS_M| image:: https://pepy.tech/badge/flask-useful/month
-   :target: https://pepy.tech/project/flask-useful)
+   :target: https://pepy.tech/project/flask-useful
 
 .. |DOWNLOADS_W| image:: https://pepy.tech/badge/flask-useful/week
-   :target: https://pepy.tech/project/flask-useful)
+   :target: https://pepy.tech/project/flask-useful
```

### Comparing `flask-useful-0.2.4/src/flask_useful.egg-info/SOURCES.txt` & `flask-useful-0.2.5/src/flask_useful.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 examples/blueprints/routes/api/v1/__init__.py
 examples/blueprints/routes/api/v1/users.py
 examples/blueprints/routes/api/v2/__init__.py
 examples/blueprints/routes/api/v2/users.py
 src/flask_useful/__init__.py
 src/flask_useful/app.py
 src/flask_useful/blueprints.py
+src/flask_useful/confirmation_token.py
 src/flask_useful/decorators.py
 src/flask_useful/flask_access.py
 src/flask_useful/mail.py
 src/flask_useful/py.typed
 src/flask_useful/utils.py
 src/flask_useful/views.py
 src/flask_useful.egg-info/PKG-INFO
 src/flask_useful.egg-info/SOURCES.txt
 src/flask_useful.egg-info/dependency_links.txt
 src/flask_useful.egg-info/requires.txt
 src/flask_useful.egg-info/top_level.txt
 src/flask_useful/sqla/__init__.py
+src/flask_useful/sqla/confirmation_token.py
 src/flask_useful/sqla/ma.py
 src/flask_useful/sqla/session.py
 src/flask_useful/sqla/utils.py
 src/flask_useful/wtforms/__init__.py
 src/flask_useful/wtforms/fields.py
 src/flask_useful/wtforms/filters.py
 src/flask_useful/wtforms/validators.py
```

