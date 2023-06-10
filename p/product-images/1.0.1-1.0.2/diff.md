# Comparing `tmp/product-images-1.0.1.tar.gz` & `tmp/product-images-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product-images-1.0.1.tar", last modified: Sun Jan 15 17:10:45 2023, max compression
+gzip compressed data, was "product-images-1.0.2.tar", last modified: Sat Jun 10 13:48:50 2023, max compression
```

## Comparing `product-images-1.0.1.tar` & `product-images-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.394929 product-images-1.0.1/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 product-images-1.0.1/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 product-images-1.0.1/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-01-15 17:10:45.394929 product-images-1.0.1/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-14 15:22:21.000000 product-images-1.0.1/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      270 2022-09-07 19:14:03.000000 product-images-1.0.1/product_images/actions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      668 2022-09-07 19:14:03.000000 product-images-1.0.1/product_images/fields.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2081 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-07-21 04:00:27.000000 product-images-1.0.1/product_images/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     1803 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1319 2022-07-21 04:00:27.000000 product-images-1.0.1/product_images/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     2024 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/locale/uk/LC_MESSAGES/django.po
--rw-rw-r--   0 dev       (1000) dev       (1000)     2577 2022-09-07 19:14:03.000000 product-images-1.0.1/product_images/models.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/static/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images/static/dropzone/
--rw-rw-r--   0 dev       (1000) dev       (1000)     9717 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/static/dropzone/dropzone.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)    43003 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/static/dropzone/dropzone.min.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.394929 product-images-1.0.1/product_images/static/file-manager/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1090 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/static/file-manager/file-manager.css
--rw-rw-r--   0 dev       (1000) dev       (1000)     2953 2023-01-15 17:09:23.000000 product-images-1.0.1/product_images/static/file-manager/file-manager.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.394929 product-images-1.0.1/product_images/templates/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1034 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/templates/product-images-form.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      393 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      354 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/utils.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1585 2022-09-07 19:14:03.000000 product-images-1.0.1/product_images/views.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      402 2022-07-21 03:58:58.000000 product-images-1.0.1/product_images/widgets.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-01-15 17:10:45.390929 product-images-1.0.1/product_images.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-01-15 17:10:45.000000 product-images-1.0.1/product_images.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      914 2023-01-15 17:10:45.000000 product-images-1.0.1/product_images.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-01-15 17:10:45.000000 product-images-1.0.1/product_images.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       25 2023-01-15 17:10:45.000000 product-images-1.0.1/product_images.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       15 2023-01-15 17:10:45.000000 product-images-1.0.1/product_images.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       25 2023-01-15 17:10:32.000000 product-images-1.0.1/requirements.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-01-15 17:10:45.394929 product-images-1.0.1/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      537 2023-01-15 17:10:32.000000 product-images-1.0.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.100031 product-images-1.0.2/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 product-images-1.0.2/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 product-images-1.0.2/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-06-10 13:48:50.100031 product-images-1.0.2/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-14 15:22:21.000000 product-images-1.0.2/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      270 2022-09-07 19:14:03.000000 product-images-1.0.2/product_images/actions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      668 2022-09-07 19:14:03.000000 product-images-1.0.2/product_images/fields.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2081 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-07-21 04:00:27.000000 product-images-1.0.2/product_images/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1803 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1319 2022-07-21 04:00:27.000000 product-images-1.0.2/product_images/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2024 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1137 2023-06-10 13:48:13.000000 product-images-1.0.2/product_images/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:13.000000 product-images-1.0.2/product_images/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2577 2022-09-07 19:14:03.000000 product-images-1.0.2/product_images/models.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images/static/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.100031 product-images-1.0.2/product_images/static/dropzone/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     9717 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/static/dropzone/dropzone.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)    43003 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/static/dropzone/dropzone.min.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.100031 product-images-1.0.2/product_images/static/file-manager/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1090 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/static/file-manager/file-manager.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2953 2023-01-15 17:09:23.000000 product-images-1.0.2/product_images/static/file-manager/file-manager.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.100031 product-images-1.0.2/product_images/templates/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1034 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/templates/product-images-form.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      393 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      354 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/utils.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1585 2022-09-07 19:14:03.000000 product-images-1.0.2/product_images/views.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      402 2022-07-21 03:58:58.000000 product-images-1.0.2/product_images/widgets.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:50.096031 product-images-1.0.2/product_images.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-06-10 13:48:50.000000 product-images-1.0.2/product_images.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      994 2023-06-10 13:48:50.000000 product-images-1.0.2/product_images.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-06-10 13:48:50.000000 product-images-1.0.2/product_images.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       25 2023-06-10 13:48:50.000000 product-images-1.0.2/product_images.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       15 2023-06-10 13:48:50.000000 product-images-1.0.2/product_images.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       25 2023-01-15 17:10:32.000000 product-images-1.0.2/requirements.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-06-10 13:48:50.100031 product-images-1.0.2/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      537 2023-06-10 13:48:34.000000 product-images-1.0.2/setup.py
```

### Comparing `product-images-1.0.1/LICENSE` & `product-images-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/fields.py` & `product-images-1.0.2/product_images/fields.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/forms.py` & `product-images-1.0.2/product_images/forms.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/locale/ru/LC_MESSAGES/django.mo` & `product-images-1.0.2/product_images/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/locale/ru/LC_MESSAGES/django.po` & `product-images-1.0.2/product_images/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/locale/uk/LC_MESSAGES/django.mo` & `product-images-1.0.2/product_images/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/locale/uk/LC_MESSAGES/django.po` & `product-images-1.0.2/product_images/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/models.py` & `product-images-1.0.2/product_images/models.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/static/dropzone/dropzone.min.css` & `product-images-1.0.2/product_images/static/dropzone/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/static/dropzone/dropzone.min.js` & `product-images-1.0.2/product_images/static/dropzone/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/static/file-manager/file-manager.css` & `product-images-1.0.2/product_images/static/file-manager/file-manager.css`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/static/file-manager/file-manager.js` & `product-images-1.0.2/product_images/static/file-manager/file-manager.js`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/templates/product-images-form.html` & `product-images-1.0.2/product_images/templates/product-images-form.html`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images/views.py` & `product-images-1.0.2/product_images/views.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.1/product_images.egg-info/SOURCES.txt` & `product-images-1.0.2/product_images.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -18,12 +18,14 @@
 product_images.egg-info/dependency_links.txt
 product_images.egg-info/requires.txt
 product_images.egg-info/top_level.txt
 product_images/locale/ru/LC_MESSAGES/django.mo
 product_images/locale/ru/LC_MESSAGES/django.po
 product_images/locale/uk/LC_MESSAGES/django.mo
 product_images/locale/uk/LC_MESSAGES/django.po
+product_images/migrations/0001_initial.py
+product_images/migrations/__init__.py
 product_images/static/dropzone/dropzone.min.css
 product_images/static/dropzone/dropzone.min.js
 product_images/static/file-manager/file-manager.css
 product_images/static/file-manager/file-manager.js
 product_images/templates/product-images-form.html
```

### Comparing `product-images-1.0.1/setup.py` & `product-images-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 
-version = '1.0.1'
+version = '1.0.2'
 url = 'https://github.com/pmaigutyak/product-images'
 
 
 setup(
     name='product-images',
     version=version,
     description='Django run app',
```

