# Comparing `tmp/django-dellavrite-0.1.tar.gz` & `tmp/django-dellavrite-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dellavrite-0.1.tar", last modified: Sat Jun 10 07:00:28 2023, max compression
+gzip compressed data, was "django-dellavrite-0.2.tar", last modified: Sat Jun 10 07:04:18 2023, max compression
```

## Comparing `django-dellavrite-0.1.tar` & `django-dellavrite-0.2.tar`

### file list

```diff
@@ -1,60 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.346256 django-dellavrite-0.1/
--rw-rw-rw-   0        0        0      120 2023-06-10 07:00:28.346256 django-dellavrite-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.301439 django-dellavrite-0.1/django-dellavrite/
--rw-rw-rw-   0        0        0        0 2023-06-10 06:44:03.000000 django-dellavrite-0.1/django-dellavrite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.302446 django-dellavrite-0.1/django-dellavrite/back/
--rw-rw-rw-   0        0        0        0 2023-06-10 06:46:57.000000 django-dellavrite-0.1/django-dellavrite/back/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.314183 django-dellavrite-0.1/django-dellavrite/back/app/
--rw-rw-rw-   0        0        0        0 2023-05-22 06:55:45.000000 django-dellavrite-0.1/django-dellavrite/back/app/__init__.py
--rw-rw-rw-   0        0        0       66 2023-05-22 06:55:45.000000 django-dellavrite-0.1/django-dellavrite/back/app/admin.py
--rw-rw-rw-   0        0        0      144 2023-05-22 06:55:45.000000 django-dellavrite-0.1/django-dellavrite/back/app/apps.py
--rw-rw-rw-   0        0        0      131 2023-05-11 08:39:36.000000 django-dellavrite-0.1/django-dellavrite/back/app/auth.py
--rw-rw-rw-   0        0        0     1400 2023-05-22 08:04:04.000000 django-dellavrite-0.1/django-dellavrite/back/app/exc.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.317365 django-dellavrite-0.1/django-dellavrite/back/app/migrations/
--rw-rw-rw-   0        0        0     4346 2023-05-22 07:38:47.000000 django-dellavrite-0.1/django-dellavrite/back/app/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-05-22 06:55:45.000000 django-dellavrite-0.1/django-dellavrite/back/app/migrations/__init__.py
--rw-rw-rw-   0        0        0      834 2023-05-11 09:28:43.000000 django-dellavrite-0.1/django-dellavrite/back/app/models.py
--rw-rw-rw-   0        0        0     1046 2023-05-22 07:46:57.000000 django-dellavrite-0.1/django-dellavrite/back/app/serializers.py
--rw-rw-rw-   0        0        0       63 2023-05-22 06:55:45.000000 django-dellavrite-0.1/django-dellavrite/back/app/tests.py
--rw-rw-rw-   0        0        0      513 2023-05-22 08:05:18.000000 django-dellavrite-0.1/django-dellavrite/back/app/urls.py
--rw-rw-rw-   0        0        0     6378 2023-05-22 08:04:04.000000 django-dellavrite-0.1/django-dellavrite/back/app/views.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.324340 django-dellavrite-0.1/django-dellavrite/back/laba228_back/
--rw-rw-rw-   0        0        0        0 2023-05-22 06:55:26.000000 django-dellavrite-0.1/django-dellavrite/back/laba228_back/__init__.py
--rw-rw-rw-   0        0        0      417 2023-05-22 06:55:26.000000 django-dellavrite-0.1/django-dellavrite/back/laba228_back/asgi.py
--rw-rw-rw-   0        0        0     3632 2023-05-22 07:38:37.000000 django-dellavrite-0.1/django-dellavrite/back/laba228_back/settings.py
--rw-rw-rw-   0        0        0      808 2023-05-22 07:22:36.000000 django-dellavrite-0.1/django-dellavrite/back/laba228_back/urls.py
--rw-rw-rw-   0        0        0      417 2023-05-22 06:55:26.000000 django-dellavrite-0.1/django-dellavrite/back/laba228_back/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.293769 django-dellavrite-0.1/django-dellavrite/front/
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.330199 django-dellavrite-0.1/django-dellavrite/front/assets/
--rw-rw-rw-   0        0        0     5272 2023-05-22 08:54:50.000000 django-dellavrite-0.1/django-dellavrite/front/assets/cart.html
--rw-rw-rw-   0        0        0     6389 2023-05-22 08:54:50.000000 django-dellavrite-0.1/django-dellavrite/front/assets/index.html
--rw-rw-rw-   0        0        0     2595 2023-05-22 08:54:50.000000 django-dellavrite-0.1/django-dellavrite/front/assets/login.html
--rw-rw-rw-   0        0        0     6463 2023-05-22 08:54:50.000000 django-dellavrite-0.1/django-dellavrite/front/assets/orders.html
--rw-rw-rw-   0        0        0     2999 2023-05-22 08:54:50.000000 django-dellavrite-0.1/django-dellavrite/front/assets/registration.html
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.337148 django-dellavrite-0.1/django-dellavrite/front/public/
--rw-rw-rw-   0        0        0     3870 2023-05-22 06:54:36.000000 django-dellavrite-0.1/django-dellavrite/front/public/favicon.ico
--rw-rw-rw-   0        0        0     1721 2023-05-22 06:54:36.000000 django-dellavrite-0.1/django-dellavrite/front/public/index.html
--rw-rw-rw-   0        0        0     5347 2023-05-22 06:54:42.000000 django-dellavrite-0.1/django-dellavrite/front/public/logo192.png
--rw-rw-rw-   0        0        0     9664 2023-05-22 06:54:42.000000 django-dellavrite-0.1/django-dellavrite/front/public/logo512.png
--rw-rw-rw-   0        0        0      492 2023-05-22 06:54:41.000000 django-dellavrite-0.1/django-dellavrite/front/public/manifest.json
--rw-rw-rw-   0        0        0       67 2023-05-22 06:54:43.000000 django-dellavrite-0.1/django-dellavrite/front/public/robots.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.297383 django-dellavrite-0.1/django-dellavrite/front/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.346256 django-dellavrite-0.1/django-dellavrite/front/src/components/
--rw-rw-rw-   0        0        0     3999 2023-05-22 09:45:03.000000 django-dellavrite-0.1/django-dellavrite/front/src/components/Cart.jsx
--rw-rw-rw-   0        0        0     2879 2023-05-22 09:33:19.000000 django-dellavrite-0.1/django-dellavrite/front/src/components/Login.jsx
--rw-rw-rw-   0        0        0     1881 2023-05-22 09:24:49.000000 django-dellavrite-0.1/django-dellavrite/front/src/components/Main.jsx
--rw-rw-rw-   0        0        0     2614 2023-05-22 09:44:37.000000 django-dellavrite-0.1/django-dellavrite/front/src/components/Orders.jsx
--rw-rw-rw-   0        0        0     3121 2023-05-22 09:36:15.000000 django-dellavrite-0.1/django-dellavrite/front/src/components/Register.jsx
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.346256 django-dellavrite-0.1/django-dellavrite/front/src/css/
--rw-rw-rw-   0        0        0   155845 2023-05-04 06:37:36.000000 django-dellavrite-0.1/django-dellavrite/front/src/css/bootstrap.min.css
--rw-rw-rw-   0        0        0      138 2023-05-11 07:08:30.000000 django-dellavrite-0.1/django-dellavrite/front/src/css/style.css
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.346256 django-dellavrite-0.1/django-dellavrite/front/src/http/
--rw-rw-rw-   0        0        0      357 2023-05-22 09:14:51.000000 django-dellavrite-0.1/django-dellavrite/front/src/http/Instance.jsx
-drwxrwxrwx   0        0        0        0 2023-06-10 07:00:28.346256 django-dellavrite-0.1/django_dellavrite.egg-info/
--rw-rw-rw-   0        0        0      120 2023-06-10 07:00:28.000000 django-dellavrite-0.1/django_dellavrite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1844 2023-06-10 07:00:28.000000 django-dellavrite-0.1/django_dellavrite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 07:00:28.000000 django-dellavrite-0.1/django_dellavrite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 07:00:28.000000 django-dellavrite-0.1/django_dellavrite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-06-10 07:00:28.000000 django-dellavrite-0.1/django_dellavrite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 07:00:28.362096 django-dellavrite-0.1/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-06-10 06:59:59.000000 django-dellavrite-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.634374 django-dellavrite-0.2/
+-rw-rw-rw-   0        0        0      120 2023-06-10 07:04:18.634374 django-dellavrite-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.547498 django-dellavrite-0.2/django-dellavrite/
+-rw-rw-rw-   0        0        0        0 2023-06-10 06:44:03.000000 django-dellavrite-0.2/django-dellavrite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.547498 django-dellavrite-0.2/django-dellavrite/back/
+-rw-rw-rw-   0        0        0        0 2023-06-10 06:46:57.000000 django-dellavrite-0.2/django-dellavrite/back/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.568170 django-dellavrite-0.2/django-dellavrite/back/app/
+-rw-rw-rw-   0        0        0        0 2023-05-22 06:55:45.000000 django-dellavrite-0.2/django-dellavrite/back/app/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-05-22 06:55:45.000000 django-dellavrite-0.2/django-dellavrite/back/app/admin.py
+-rw-rw-rw-   0        0        0      144 2023-05-22 06:55:45.000000 django-dellavrite-0.2/django-dellavrite/back/app/apps.py
+-rw-rw-rw-   0        0        0      131 2023-05-11 08:39:36.000000 django-dellavrite-0.2/django-dellavrite/back/app/auth.py
+-rw-rw-rw-   0        0        0     1400 2023-05-22 08:04:04.000000 django-dellavrite-0.2/django-dellavrite/back/app/exc.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.571623 django-dellavrite-0.2/django-dellavrite/back/app/migrations/
+-rw-rw-rw-   0        0        0     4346 2023-05-22 07:38:47.000000 django-dellavrite-0.2/django-dellavrite/back/app/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 06:55:45.000000 django-dellavrite-0.2/django-dellavrite/back/app/migrations/__init__.py
+-rw-rw-rw-   0        0        0      834 2023-05-11 09:28:43.000000 django-dellavrite-0.2/django-dellavrite/back/app/models.py
+-rw-rw-rw-   0        0        0     1046 2023-05-22 07:46:57.000000 django-dellavrite-0.2/django-dellavrite/back/app/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-05-22 06:55:45.000000 django-dellavrite-0.2/django-dellavrite/back/app/tests.py
+-rw-rw-rw-   0        0        0      513 2023-05-22 08:05:18.000000 django-dellavrite-0.2/django-dellavrite/back/app/urls.py
+-rw-rw-rw-   0        0        0     6378 2023-05-22 08:04:04.000000 django-dellavrite-0.2/django-dellavrite/back/app/views.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.579943 django-dellavrite-0.2/django-dellavrite/back/laba228_back/
+-rw-rw-rw-   0        0        0        0 2023-05-22 06:55:26.000000 django-dellavrite-0.2/django-dellavrite/back/laba228_back/__init__.py
+-rw-rw-rw-   0        0        0      417 2023-05-22 06:55:26.000000 django-dellavrite-0.2/django-dellavrite/back/laba228_back/asgi.py
+-rw-rw-rw-   0        0        0     3632 2023-05-22 07:38:37.000000 django-dellavrite-0.2/django-dellavrite/back/laba228_back/settings.py
+-rw-rw-rw-   0        0        0      808 2023-05-22 07:22:36.000000 django-dellavrite-0.2/django-dellavrite/back/laba228_back/urls.py
+-rw-rw-rw-   0        0        0      417 2023-05-22 06:55:26.000000 django-dellavrite-0.2/django-dellavrite/back/laba228_back/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.531476 django-dellavrite-0.2/django-dellavrite/front/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.585505 django-dellavrite-0.2/django-dellavrite/front/assets/
+-rw-rw-rw-   0        0        0     5272 2023-05-22 08:54:50.000000 django-dellavrite-0.2/django-dellavrite/front/assets/cart.html
+-rw-rw-rw-   0        0        0     6389 2023-05-22 08:54:50.000000 django-dellavrite-0.2/django-dellavrite/front/assets/index.html
+-rw-rw-rw-   0        0        0     2595 2023-05-22 08:54:50.000000 django-dellavrite-0.2/django-dellavrite/front/assets/login.html
+-rw-rw-rw-   0        0        0     6463 2023-05-22 08:54:50.000000 django-dellavrite-0.2/django-dellavrite/front/assets/orders.html
+-rw-rw-rw-   0        0        0     2999 2023-05-22 08:54:50.000000 django-dellavrite-0.2/django-dellavrite/front/assets/registration.html
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.596218 django-dellavrite-0.2/django-dellavrite/front/public/
+-rw-rw-rw-   0        0        0     3870 2023-05-22 06:54:36.000000 django-dellavrite-0.2/django-dellavrite/front/public/favicon.ico
+-rw-rw-rw-   0        0        0     1721 2023-05-22 06:54:36.000000 django-dellavrite-0.2/django-dellavrite/front/public/index.html
+-rw-rw-rw-   0        0        0     5347 2023-05-22 06:54:42.000000 django-dellavrite-0.2/django-dellavrite/front/public/logo192.png
+-rw-rw-rw-   0        0        0     9664 2023-05-22 06:54:42.000000 django-dellavrite-0.2/django-dellavrite/front/public/logo512.png
+-rw-rw-rw-   0        0        0      492 2023-05-22 06:54:41.000000 django-dellavrite-0.2/django-dellavrite/front/public/manifest.json
+-rw-rw-rw-   0        0        0       67 2023-05-22 06:54:43.000000 django-dellavrite-0.2/django-dellavrite/front/public/robots.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.601729 django-dellavrite-0.2/django-dellavrite/front/src/
+-rw-rw-rw-   0        0        0      564 2023-05-22 06:54:32.000000 django-dellavrite-0.2/django-dellavrite/front/src/App.css
+-rw-rw-rw-   0        0        0     3290 2023-06-10 06:48:42.000000 django-dellavrite-0.2/django-dellavrite/front/src/App.js
+-rw-rw-rw-   0        0        0      246 2023-05-22 06:54:38.000000 django-dellavrite-0.2/django-dellavrite/front/src/App.test.js
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.616777 django-dellavrite-0.2/django-dellavrite/front/src/components/
+-rw-rw-rw-   0        0        0     3999 2023-05-22 09:45:03.000000 django-dellavrite-0.2/django-dellavrite/front/src/components/Cart.jsx
+-rw-rw-rw-   0        0        0     2879 2023-05-22 09:33:19.000000 django-dellavrite-0.2/django-dellavrite/front/src/components/Login.jsx
+-rw-rw-rw-   0        0        0     1881 2023-05-22 09:24:49.000000 django-dellavrite-0.2/django-dellavrite/front/src/components/Main.jsx
+-rw-rw-rw-   0        0        0     2614 2023-05-22 09:44:37.000000 django-dellavrite-0.2/django-dellavrite/front/src/components/Orders.jsx
+-rw-rw-rw-   0        0        0     3121 2023-05-22 09:36:15.000000 django-dellavrite-0.2/django-dellavrite/front/src/components/Register.jsx
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.624099 django-dellavrite-0.2/django-dellavrite/front/src/css/
+-rw-rw-rw-   0        0        0   155845 2023-05-04 06:37:36.000000 django-dellavrite-0.2/django-dellavrite/front/src/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0      138 2023-05-11 07:08:30.000000 django-dellavrite-0.2/django-dellavrite/front/src/css/style.css
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.624099 django-dellavrite-0.2/django-dellavrite/front/src/http/
+-rw-rw-rw-   0        0        0      357 2023-05-22 09:14:51.000000 django-dellavrite-0.2/django-dellavrite/front/src/http/Instance.jsx
+-rw-rw-rw-   0        0        0      366 2023-05-22 06:54:34.000000 django-dellavrite-0.2/django-dellavrite/front/src/index.css
+-rw-rw-rw-   0        0        0      299 2023-05-22 09:15:16.000000 django-dellavrite-0.2/django-dellavrite/front/src/index.js
+-rw-rw-rw-   0        0        0     2632 2023-05-22 06:54:42.000000 django-dellavrite-0.2/django-dellavrite/front/src/logo.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 06:54:39.000000 django-dellavrite-0.2/django-dellavrite/front/src/reportWebVitals.js
+-rw-rw-rw-   0        0        0      241 2023-05-22 06:54:40.000000 django-dellavrite-0.2/django-dellavrite/front/src/setupTests.js
+drwxrwxrwx   0        0        0        0 2023-06-10 07:04:18.634374 django-dellavrite-0.2/django_dellavrite.egg-info/
+-rw-rw-rw-   0        0        0      120 2023-06-10 07:04:18.000000 django-dellavrite-0.2/django_dellavrite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-06-10 07:04:18.000000 django-dellavrite-0.2/django_dellavrite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 07:04:18.000000 django-dellavrite-0.2/django_dellavrite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-10 07:04:18.000000 django-dellavrite-0.2/django_dellavrite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-06-10 07:04:18.000000 django-dellavrite-0.2/django_dellavrite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 07:04:18.644329 django-dellavrite-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      653 2023-06-10 07:04:11.000000 django-dellavrite-0.2/setup.py
```

### Comparing `django-dellavrite-0.1/django-dellavrite/back/app/exc.py` & `django-dellavrite-0.2/django-dellavrite/back/app/exc.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/back/app/migrations/0001_initial.py` & `django-dellavrite-0.2/django-dellavrite/back/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/back/app/models.py` & `django-dellavrite-0.2/django-dellavrite/back/app/models.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/back/app/serializers.py` & `django-dellavrite-0.2/django-dellavrite/back/app/serializers.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/back/app/urls.py` & `django-dellavrite-0.2/django-dellavrite/back/app/urls.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/back/app/views.py` & `django-dellavrite-0.2/django-dellavrite/back/app/views.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/back/laba228_back/settings.py` & `django-dellavrite-0.2/django-dellavrite/back/laba228_back/settings.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/back/laba228_back/urls.py` & `django-dellavrite-0.2/django-dellavrite/back/laba228_back/urls.py`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/assets/cart.html` & `django-dellavrite-0.2/django-dellavrite/front/assets/cart.html`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/assets/index.html` & `django-dellavrite-0.2/django-dellavrite/front/assets/index.html`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/assets/login.html` & `django-dellavrite-0.2/django-dellavrite/front/assets/login.html`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/assets/orders.html` & `django-dellavrite-0.2/django-dellavrite/front/assets/orders.html`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/assets/registration.html` & `django-dellavrite-0.2/django-dellavrite/front/assets/registration.html`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/public/favicon.ico` & `django-dellavrite-0.2/django-dellavrite/front/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/public/index.html` & `django-dellavrite-0.2/django-dellavrite/front/public/index.html`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/public/logo192.png` & `django-dellavrite-0.2/django-dellavrite/front/public/logo192.png`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/public/logo512.png` & `django-dellavrite-0.2/django-dellavrite/front/public/logo512.png`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/src/components/Cart.jsx` & `django-dellavrite-0.2/django-dellavrite/front/src/components/Cart.jsx`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/src/components/Login.jsx` & `django-dellavrite-0.2/django-dellavrite/front/src/components/Login.jsx`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/src/components/Main.jsx` & `django-dellavrite-0.2/django-dellavrite/front/src/components/Main.jsx`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/src/components/Orders.jsx` & `django-dellavrite-0.2/django-dellavrite/front/src/components/Orders.jsx`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/src/components/Register.jsx` & `django-dellavrite-0.2/django-dellavrite/front/src/components/Register.jsx`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django-dellavrite/front/src/css/bootstrap.min.css` & `django-dellavrite-0.2/django-dellavrite/front/src/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-dellavrite-0.1/django_dellavrite.egg-info/SOURCES.txt` & `django-dellavrite-0.2/django_dellavrite.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,22 @@
 django-dellavrite/front/assets/registration.html
 django-dellavrite/front/public/favicon.ico
 django-dellavrite/front/public/index.html
 django-dellavrite/front/public/logo192.png
 django-dellavrite/front/public/logo512.png
 django-dellavrite/front/public/manifest.json
 django-dellavrite/front/public/robots.txt
+django-dellavrite/front/src/App.css
+django-dellavrite/front/src/App.js
+django-dellavrite/front/src/App.test.js
+django-dellavrite/front/src/index.css
+django-dellavrite/front/src/index.js
+django-dellavrite/front/src/logo.svg
+django-dellavrite/front/src/reportWebVitals.js
+django-dellavrite/front/src/setupTests.js
 django-dellavrite/front/src/components/Cart.jsx
 django-dellavrite/front/src/components/Login.jsx
 django-dellavrite/front/src/components/Main.jsx
 django-dellavrite/front/src/components/Orders.jsx
 django-dellavrite/front/src/components/Register.jsx
 django-dellavrite/front/src/css/bootstrap.min.css
 django-dellavrite/front/src/css/style.css
```

### Comparing `django-dellavrite-0.1/setup.py` & `django-dellavrite-0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-dellavrite',
-    version='0.1',
+    version='0.2',
     description='Cheat for ws',
     packages=find_packages(),
     package_data={
         'django-dellavrite': [
             'back/app/migrations/*.py',
             'back/app/migrations/__pycache__/*',
             'back/app/__pycache__/*',
             'back/laba228_back/__pycache__/*',
             'front/assets/*',
             'front/public/*',
             'front/src/components/*',
             'front/src/css/*',
             'front/src/http/*',
+            'front/src/*'
         ],
     },
     author_email='delavrite@gmail.com',
     zip_safe=False
 )
```

