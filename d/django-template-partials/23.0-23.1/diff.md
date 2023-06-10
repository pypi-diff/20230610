# Comparing `tmp/django-template-partials-23.0.tar.gz` & `tmp/django-template-partials-23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-template-partials-23.0.tar", last modified: Wed May 17 18:17:15 2023, max compression
+gzip compressed data, was "django-template-partials-23.1.tar", last modified: Sat Jun 10 08:11:07 2023, max compression
```

## Comparing `django-template-partials-23.0.tar` & `django-template-partials-23.1.tar`

### file list

```diff
@@ -1,4 +1,16 @@
--rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-23.0/LICENSE
--rw-r--r--   0        0        0      449 2023-05-17 18:16:52.540400 django-template-partials-23.0/pyproject.toml
--rw-r--r--   0        0        0      142 2023-05-17 18:16:14.327124 django-template-partials-23.0/src/template_partials/__init__.py
--rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 django-template-partials-23.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-06-10 08:10:09.840430 django-template-partials-23.1/.gitignore
+-rw-r--r--   0        0        0      133 2023-06-10 07:15:27.155706 django-template-partials-23.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-23.1/LICENSE
+-rw-r--r--   0        0        0     2391 2023-06-10 08:06:13.659056 django-template-partials-23.1/README.md
+-rw-r--r--   0        0        0      213 2023-06-10 08:07:19.133058 django-template-partials-23.1/justfile
+-rw-r--r--   0        0        0      706 2023-06-10 08:09:04.575213 django-template-partials-23.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-06-10 08:06:27.533153 django-template-partials-23.1/src/template_partials/__init__.py
+-rw-r--r--   0        0        0     2013 2023-06-10 07:52:39.943743 django-template-partials-23.1/src/template_partials/loader.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:14:20.655108 django-template-partials-23.1/src/template_partials/templatetags/__init__.py
+-rw-r--r--   0        0        0     3120 2023-06-10 07:34:55.088077 django-template-partials-23.1/src/template_partials/templatetags/partials.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:31:47.903235 django-template-partials-23.1/tests/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-10 07:48:57.417739 django-template-partials-23.1/tests/settings.py
+-rw-r--r--   0        0        0       37 2023-06-10 07:39:17.702320 django-template-partials-23.1/tests/templates/base.html
+-rw-r--r--   0        0        0      205 2023-06-10 07:40:08.278885 django-template-partials-23.1/tests/templates/example.html
+-rw-r--r--   0        0        0     1131 2023-06-10 07:50:15.127276 django-template-partials-23.1/tests/tests.py
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 django-template-partials-23.1/PKG-INFO
```

### Comparing `django-template-partials-23.0/LICENSE` & `django-template-partials-23.1/LICENSE`

 * *Files identical despite different names*

