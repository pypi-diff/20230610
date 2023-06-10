# Comparing `tmp/django-all-in-one-accessibility-1.3.tar.gz` & `tmp/django-all-in-one-accessibility-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-all-in-one-accessibility-1.3.tar", last modified: Fri Jun  9 09:51:01 2023, max compression
+gzip compressed data, was "django-all-in-one-accessibility-1.4.tar", last modified: Sat Jun 10 12:35:12 2023, max compression
```

## Comparing `django-all-in-one-accessibility-1.3.tar` & `django-all-in-one-accessibility-1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.167836 django-all-in-one-accessibility-1.3/
--rw-rw-rw-   0        0        0     3956 2023-06-09 09:51:01.168829 django-all-in-one-accessibility-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2841 2023-06-09 09:50:31.000000 django-all-in-one-accessibility-1.3/Readme.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.135712 django-all-in-one-accessibility-1.3/accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/__init__.py
--rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.3/accessibility/admin.py
--rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/apps.py
--rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.3/accessibility/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.138670 django-all-in-one-accessibility-1.3/accessibility/migrations/
--rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.3/accessibility/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/migrations/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.3/accessibility/models.py
--rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/tests.py
--rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.3/accessibility/urls.py
--rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.3/accessibility/views.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.155859 django-all-in-one-accessibility-1.3/aioa_accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/__init__.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/asgi.py
--rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/settings.py
--rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/urls.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.165873 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/
--rw-rw-rw-   0        0        0     3956 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-06-09 09:49:49.000000 django-all-in-one-accessibility-1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1032 2023-06-09 09:51:01.170851 django-all-in-one-accessibility-1.3/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:35:12.247040 django-all-in-one-accessibility-1.4/
+-rw-rw-rw-   0        0        0     5637 2023-06-10 12:35:12.247040 django-all-in-one-accessibility-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4522 2023-06-10 12:34:21.000000 django-all-in-one-accessibility-1.4/Readme.md
+drwxrwxrwx   0        0        0        0 2023-06-10 12:35:12.222094 django-all-in-one-accessibility-1.4/accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.4/accessibility/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.4/accessibility/admin.py
+-rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.4/accessibility/apps.py
+-rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.4/accessibility/context_processors.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:35:12.224088 django-all-in-one-accessibility-1.4/accessibility/migrations/
+-rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.4/accessibility/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.4/accessibility/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.4/accessibility/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.4/accessibility/tests.py
+-rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.4/accessibility/urls.py
+-rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.4/accessibility/views.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:35:12.242053 django-all-in-one-accessibility-1.4/aioa_accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.4/aioa_accessibility/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.4/aioa_accessibility/asgi.py
+-rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.4/aioa_accessibility/settings.py
+-rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.4/aioa_accessibility/urls.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.4/aioa_accessibility/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:35:12.246042 django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/
+-rw-rw-rw-   0        0        0     5637 2023-06-10 12:35:12.000000 django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-10 12:35:12.000000 django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 12:35:12.000000 django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-10 12:35:12.000000 django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-06-10 12:35:12.000000 django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-06-10 12:30:45.000000 django-all-in-one-accessibility-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1031 2023-06-10 12:35:12.248037 django-all-in-one-accessibility-1.4/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.4/setup.py
```

### Comparing `django-all-in-one-accessibility-1.3/PKG-INFO` & `django-all-in-one-accessibility-1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.3
+Version: 1.4
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,29 +28,33 @@
 - Screen Reader, dynamic widget color and position, supports multiple languages (40 languages)
 - Reduces the risk of time-consuming accessibility lawsuits.
 - Use apps to connect to external services and manage data flows
 
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
-
+#### You can use this package in Django/Django-CMS/Django-Oscar
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.3`
+-   Run `pip install django-all-in-one-accessibility`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
 
 ## Usage
 
+
+<mark>Steps for Django and Django CMS.</mark>
+---
+
 ### Settings.INSTALLED_APPS
 Just add `accessibility` in to your setting.INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
@@ -95,9 +99,63 @@
 ```
 
 ### Restart 
 Restart your app server with this command and check the admin panel the model is ready to use
 ```python
 python manage.py runserver
 ```
+---
+<mark>Steps for Django Oscar.</mark>
+---
+### Settings.INSTALLED_APPS
+Just add `accessibility` in to your setting.INSTALLED_APPS:
 
+```python
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'accessibility',
+]
+```
+
+### Settings.TEMPLATES
+Just add `accessibility.context_processors.admin_AIOA` in your setting.TEMPLATES:
+```python
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': [],
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                'accessibility.context_processors.admin_AIOA',
+            ],
+        },
+    },
+]
+```
+
+### Base.html
+There is some changes in base.html file for Oscar project <mark>when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer</mark>
+```python
+<footer>
+	<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
+</footer>
+```
+
+### Migrate
+Migrate your app
+```python
+python manage.py migrate
+
+```
+
+### Restart 
+Restart your app server with this command and check the admin panel the model is ready to use
+```python
+python manage.py runserver
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.3
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.4
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -22,30 +22,48 @@
 connect to external services and manage data flows It uses the accessibility
 interface which handles UI and design related adjustments. All in One
 Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
-watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.3` - Add
-`accessibility` in `settings.INSTALLED_APPS` - Add
-`accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
-context_processors` - Add `
+watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . ####
+You can use this package in Django/Django-CMS/Django-Oscar --- ## Installation
+- Run `pip install django-all-in-one-accessibility` - Add `accessibility` in
+`settings.INSTALLED_APPS` - Add `accessibility.context_processors.admin_AIOA`
+in `settings.TEMPLATES context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
-### Settings.INSTALLED_APPS Just add `accessibility` in to your
-setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
-'django.contrib.auth', 'django.contrib.contenttypes',
+Steps for Django and Django CMS. --- ### Settings.INSTALLED_APPS Just add
+`accessibility` in to your setting.INSTALLED_APPS: ```python INSTALLED_APPS =
+[ 'django.contrib.admin', 'django.contrib.auth', 'django.contrib.contenttypes',
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
 Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
 website) `
 `: ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
+model is ready to use ```python python manage.py runserver ``` --- Steps for
+Django Oscar. --- ### Settings.INSTALLED_APPS Just add `accessibility` in to
+your setting.INSTALLED_APPS: ```python INSTALLED_APPS =
+[ 'django.contrib.admin', 'django.contrib.auth', 'django.contrib.contenttypes',
+'django.contrib.sessions', 'django.contrib.messages',
+'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
+Just add `accessibility.context_processors.admin_AIOA` in your
+setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
+'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
+True, 'OPTIONS': { 'context_processors':
+[ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
+There is some changes in base.html file for Oscar project when u are using
+django oscar there is already base.html file exists so u need to go to oscar
+project directory which are locate in your site-packages(go to site-packages -
+> oscar -> templates ->oscar -> base.html) put this tag
+ in oscar/templates/oscar/base.html footer ```python
+  ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
+Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.3/Readme.md` & `django-all-in-one-accessibility-1.4/Readme.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 - Screen Reader, dynamic widget color and position, supports multiple languages (40 languages)
 - Reduces the risk of time-consuming accessibility lawsuits.
 - Use apps to connect to external services and manage data flows
 
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
-
+#### You can use this package in Django/Django-CMS/Django-Oscar
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.3`
+-   Run `pip install django-all-in-one-accessibility`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
 
 ## Usage
 
+
+<mark>Steps for Django and Django CMS.</mark>
+---
+
 ### Settings.INSTALLED_APPS
 Just add `accessibility` in to your setting.INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
@@ -71,9 +75,63 @@
 ```
 
 ### Restart 
 Restart your app server with this command and check the admin panel the model is ready to use
 ```python
 python manage.py runserver
 ```
+---
+<mark>Steps for Django Oscar.</mark>
+---
+### Settings.INSTALLED_APPS
+Just add `accessibility` in to your setting.INSTALLED_APPS:
 
+```python
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'accessibility',
+]
+```
+
+### Settings.TEMPLATES
+Just add `accessibility.context_processors.admin_AIOA` in your setting.TEMPLATES:
+```python
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': [],
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                'accessibility.context_processors.admin_AIOA',
+            ],
+        },
+    },
+]
+```
+
+### Base.html
+There is some changes in base.html file for Oscar project <mark>when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer</mark>
+```python
+<footer>
+	<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
+</footer>
+```
+
+### Migrate
+Migrate your app
+```python
+python manage.py migrate
+
+```
+
+### Restart 
+Restart your app server with this command and check the admin panel the model is ready to use
+```python
+python manage.py runserver
+```
```

#### html2text {}

```diff
@@ -7,30 +7,48 @@
 Use apps to connect to external services and manage data flows It uses the
 accessibility interface which handles UI and design related adjustments. All in
 One Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
-watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.3` - Add
-`accessibility` in `settings.INSTALLED_APPS` - Add
-`accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
-context_processors` - Add `
+watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . ####
+You can use this package in Django/Django-CMS/Django-Oscar --- ## Installation
+- Run `pip install django-all-in-one-accessibility` - Add `accessibility` in
+`settings.INSTALLED_APPS` - Add `accessibility.context_processors.admin_AIOA`
+in `settings.TEMPLATES context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
-### Settings.INSTALLED_APPS Just add `accessibility` in to your
-setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
-'django.contrib.auth', 'django.contrib.contenttypes',
+Steps for Django and Django CMS. --- ### Settings.INSTALLED_APPS Just add
+`accessibility` in to your setting.INSTALLED_APPS: ```python INSTALLED_APPS =
+[ 'django.contrib.admin', 'django.contrib.auth', 'django.contrib.contenttypes',
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
 Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
 website) `
 `: ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
+model is ready to use ```python python manage.py runserver ``` --- Steps for
+Django Oscar. --- ### Settings.INSTALLED_APPS Just add `accessibility` in to
+your setting.INSTALLED_APPS: ```python INSTALLED_APPS =
+[ 'django.contrib.admin', 'django.contrib.auth', 'django.contrib.contenttypes',
+'django.contrib.sessions', 'django.contrib.messages',
+'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
+Just add `accessibility.context_processors.admin_AIOA` in your
+setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
+'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
+True, 'OPTIONS': { 'context_processors':
+[ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
+There is some changes in base.html file for Oscar project when u are using
+django oscar there is already base.html file exists so u need to go to oscar
+project directory which are locate in your site-packages(go to site-packages -
+> oscar -> templates ->oscar -> base.html) put this tag
+ in oscar/templates/oscar/base.html footer ```python
+  ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
+Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.3/accessibility/admin.py` & `django-all-in-one-accessibility-1.4/accessibility/admin.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.3/accessibility/context_processors.py` & `django-all-in-one-accessibility-1.4/accessibility/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.3/accessibility/migrations/0001_initial.py` & `django-all-in-one-accessibility-1.4/accessibility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.3/accessibility/models.py` & `django-all-in-one-accessibility-1.4/accessibility/models.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.3/aioa_accessibility/settings.py` & `django-all-in-one-accessibility-1.4/aioa_accessibility/settings.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.3/aioa_accessibility/urls.py` & `django-all-in-one-accessibility-1.4/aioa_accessibility/urls.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/PKG-INFO` & `django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.3
+Version: 1.4
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,29 +28,33 @@
 - Screen Reader, dynamic widget color and position, supports multiple languages (40 languages)
 - Reduces the risk of time-consuming accessibility lawsuits.
 - Use apps to connect to external services and manage data flows
 
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
-
+#### You can use this package in Django/Django-CMS/Django-Oscar
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.3`
+-   Run `pip install django-all-in-one-accessibility`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
 
 ## Usage
 
+
+<mark>Steps for Django and Django CMS.</mark>
+---
+
 ### Settings.INSTALLED_APPS
 Just add `accessibility` in to your setting.INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
@@ -95,9 +99,63 @@
 ```
 
 ### Restart 
 Restart your app server with this command and check the admin panel the model is ready to use
 ```python
 python manage.py runserver
 ```
+---
+<mark>Steps for Django Oscar.</mark>
+---
+### Settings.INSTALLED_APPS
+Just add `accessibility` in to your setting.INSTALLED_APPS:
 
+```python
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'accessibility',
+]
+```
+
+### Settings.TEMPLATES
+Just add `accessibility.context_processors.admin_AIOA` in your setting.TEMPLATES:
+```python
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': [],
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                'accessibility.context_processors.admin_AIOA',
+            ],
+        },
+    },
+]
+```
+
+### Base.html
+There is some changes in base.html file for Oscar project <mark>when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer</mark>
+```python
+<footer>
+	<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
+</footer>
+```
+
+### Migrate
+Migrate your app
+```python
+python manage.py migrate
+
+```
+
+### Restart 
+Restart your app server with this command and check the admin panel the model is ready to use
+```python
+python manage.py runserver
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.3
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.4
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -22,30 +22,48 @@
 connect to external services and manage data flows It uses the accessibility
 interface which handles UI and design related adjustments. All in One
 Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
-watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.3` - Add
-`accessibility` in `settings.INSTALLED_APPS` - Add
-`accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
-context_processors` - Add `
+watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . ####
+You can use this package in Django/Django-CMS/Django-Oscar --- ## Installation
+- Run `pip install django-all-in-one-accessibility` - Add `accessibility` in
+`settings.INSTALLED_APPS` - Add `accessibility.context_processors.admin_AIOA`
+in `settings.TEMPLATES context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
-### Settings.INSTALLED_APPS Just add `accessibility` in to your
-setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
-'django.contrib.auth', 'django.contrib.contenttypes',
+Steps for Django and Django CMS. --- ### Settings.INSTALLED_APPS Just add
+`accessibility` in to your setting.INSTALLED_APPS: ```python INSTALLED_APPS =
+[ 'django.contrib.admin', 'django.contrib.auth', 'django.contrib.contenttypes',
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
 Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
 website) `
 `: ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
+model is ready to use ```python python manage.py runserver ``` --- Steps for
+Django Oscar. --- ### Settings.INSTALLED_APPS Just add `accessibility` in to
+your setting.INSTALLED_APPS: ```python INSTALLED_APPS =
+[ 'django.contrib.admin', 'django.contrib.auth', 'django.contrib.contenttypes',
+'django.contrib.sessions', 'django.contrib.messages',
+'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
+Just add `accessibility.context_processors.admin_AIOA` in your
+setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
+'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
+True, 'OPTIONS': { 'context_processors':
+[ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
+There is some changes in base.html file for Oscar project when u are using
+django oscar there is already base.html file exists so u need to go to oscar
+project directory which are locate in your site-packages(go to site-packages -
+> oscar -> templates ->oscar -> base.html) put this tag
+ in oscar/templates/oscar/base.html footer ```python
+  ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
+Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/SOURCES.txt` & `django-all-in-one-accessibility-1.4/django_all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.3/pyproject.toml` & `django-all-in-one-accessibility-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-all-in-one-accessibility"
-version = "1.3"
+version = "1.4"
 authors = [
   { name="Skynet Technologies USA LLC", email="developer3@skynettechnologies.com" },
 ]
 description = "All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button"
 readme = "Readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django-all-in-one-accessibility-1.3/setup.cfg` & `django-all-in-one-accessibility-1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 616c 6c2d 696e   = django-all-in
 00000020: 2d6f 6e65 2d61 6363 6573 7369 6269 6c69  -one-accessibili
 00000030: 7479 0d0a 7665 7273 696f 6e20 3d20 312e  ty..version = 1.
-00000040: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
+00000040: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
 00000050: 2041 2044 6a61 6e67 6f20 4170 7020 6261   A Django App ba
 00000060: 7365 6420 6f6e 2061 7373 6973 7469 7665  sed on assistive
 00000070: 2074 6563 686e 6f6c 6f67 7920 7468 6174   technology that
 00000080: 2068 656c 7073 206f 7267 616e 697a 6174   helps organizat
 00000090: 696f 6e73 2065 6e68 616e 6365 2074 6865  ions enhance the
 000000a0: 2061 6363 6573 7369 6269 6c69 7479 2061   accessibility a
 000000b0: 6e64 2075 7361 6269 6c69 7479 206f 6620  nd usability of 
 000000c0: 7468 6569 7220 7765 6273 6974 650d 0a6c  their website..l
 000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000e0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e72  = file: README.r
-000000f0: 7374 0d0a 7572 6c20 3d20 6874 7470 733a  st..url = https:
-00000100: 2f2f 7777 772e 736b 796e 6574 7465 6368  //www.skynettech
-00000110: 6e6f 6c6f 6769 6573 2e63 6f6d 0d0a 6175  nologies.com..au
-00000120: 7468 6f72 203d 2053 6b79 6e65 7420 5465  thor = Skynet Te
-00000130: 6368 6e6f 6c6f 6769 6573 2055 5341 204c  chnologies USA L
-00000140: 4c43 0d0a 6175 7468 6f72 5f65 6d61 696c  LC..author_email
-00000150: 203d 2064 6576 656c 6f70 6572 3340 736b   = developer3@sk
-00000160: 796e 6574 7465 6368 6e6f 6c6f 6769 6573  ynettechnologies
-00000170: 2e63 6f6d 0d0a 636c 6173 7369 6669 6572  .com..classifier
-00000180: 7320 3d20 0d0a 0945 6e76 6972 6f6e 6d65  s = ...Environme
-00000190: 6e74 203a 3a20 5765 6220 456e 7669 726f  nt :: Web Enviro
-000001a0: 6e6d 656e 740d 0a09 4672 616d 6577 6f72  nment...Framewor
-000001b0: 6b20 3a3a 2044 6a61 6e67 6f0d 0a09 4672  k :: Django...Fr
-000001c0: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
-000001d0: 6f20 3a3a 2033 2e32 0d0a 0949 6e74 656e  o :: 3.2...Inten
-000001e0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000001f0: 4465 7665 6c6f 7065 7273 0d0a 094c 6963  Developers...Lic
-00000200: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000210: 6f76 6564 203a 3a20 4253 4420 4c69 6365  oved :: BSD Lice
-00000220: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-00000230: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000240: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
-00000250: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000260: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
-00000270: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000280: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002b0: 203a 3a20 3320 3a3a 204f 6e6c 790d 0a09   :: 3 :: Only...
-000002c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002e0: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
-000002f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000300: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-00000310: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
-00000320: 7420 3a3a 2057 5757 2f48 5454 500d 0a09  t :: WWW/HTTP...
-00000330: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
-00000340: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
-00000350: 2044 796e 616d 6963 2043 6f6e 7465 6e74   Dynamic Content
-00000360: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
-00000370: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000380: 6174 6120 3d20 7472 7565 0d0a 7061 636b  ata = true..pack
-00000390: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-000003a0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000003b0: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
-000003c0: 6571 7569 7265 7320 3d20 0d0a 0944 6a61  equires = ...Dja
-000003d0: 6e67 6f20 3e3d 2033 2e32 0d0a 0d0a 5b65  ngo >= 3.2....[e
-000003e0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000003f0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000400: 203d 2030 0d0a 0d0a                       = 0....
+000000e0: 3d20 6669 6c65 3a20 5265 6164 6d65 2e6d  = file: Readme.m
+000000f0: 640d 0a75 726c 203d 2068 7474 7073 3a2f  d..url = https:/
+00000100: 2f77 7777 2e73 6b79 6e65 7474 6563 686e  /www.skynettechn
+00000110: 6f6c 6f67 6965 732e 636f 6d0d 0a61 7574  ologies.com..aut
+00000120: 686f 7220 3d20 536b 796e 6574 2054 6563  hor = Skynet Tec
+00000130: 686e 6f6c 6f67 6965 7320 5553 4120 4c4c  hnologies USA LL
+00000140: 430d 0a61 7574 686f 725f 656d 6169 6c20  C..author_email 
+00000150: 3d20 6465 7665 6c6f 7065 7233 4073 6b79  = developer3@sky
+00000160: 6e65 7474 6563 686e 6f6c 6f67 6965 732e  nettechnologies.
+00000170: 636f 6d0d 0a63 6c61 7373 6966 6965 7273  com..classifiers
+00000180: 203d 200d 0a09 456e 7669 726f 6e6d 656e   = ...Environmen
+00000190: 7420 3a3a 2057 6562 2045 6e76 6972 6f6e  t :: Web Environ
+000001a0: 6d65 6e74 0d0a 0946 7261 6d65 776f 726b  ment...Framework
+000001b0: 203a 3a20 446a 616e 676f 0d0a 0946 7261   :: Django...Fra
+000001c0: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
+000001d0: 203a 3a20 332e 320d 0a09 496e 7465 6e64   :: 3.2...Intend
+000001e0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+000001f0: 6576 656c 6f70 6572 730d 0a09 4c69 6365  evelopers...Lice
+00000200: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000210: 7665 6420 3a3a 2042 5344 204c 6963 656e  ved :: BSD Licen
+00000220: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+00000230: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000240: 7065 6e64 656e 740d 0a09 5072 6f67 7261  pendent...Progra
+00000250: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000260: 3a20 5079 7468 6f6e 0d0a 0950 726f 6772  : Python...Progr
+00000270: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000280: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002b0: 3a3a 2033 203a 3a20 4f6e 6c79 0d0a 0950  :: 3 :: Only...P
+000002c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002e0: 2033 2e38 0d0a 0950 726f 6772 616d 6d69   3.8...Programmi
+000002f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000300: 7974 686f 6e20 3a3a 2033 2e39 0d0a 0954  ython :: 3.9...T
+00000310: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00000320: 203a 3a20 5757 572f 4854 5450 0d0a 0954   :: WWW/HTTP...T
+00000330: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00000340: 203a 3a20 5757 572f 4854 5450 203a 3a20   :: WWW/HTTP :: 
+00000350: 4479 6e61 6d69 6320 436f 6e74 656e 740d  Dynamic Content.
+00000360: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 696e  ...[options]..in
+00000370: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000380: 7461 203d 2074 7275 650d 0a70 6163 6b61  ta = true..packa
+00000390: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+000003a0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000003b0: 3d33 2e38 0d0a 696e 7374 616c 6c5f 7265  =3.8..install_re
+000003c0: 7175 6972 6573 203d 200d 0a09 446a 616e  quires = ...Djan
+000003d0: 676f 203e 3d20 332e 320d 0a0d 0a5b 6567  go >= 3.2....[eg
+000003e0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000003f0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000400: 3d20 300d 0a0d 0a                        = 0....
```

