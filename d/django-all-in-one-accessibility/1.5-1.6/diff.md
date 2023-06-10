# Comparing `tmp/django-all-in-one-accessibility-1.5.tar.gz` & `tmp/django-all-in-one-accessibility-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-all-in-one-accessibility-1.5.tar", last modified: Sat Jun 10 12:37:26 2023, max compression
+gzip compressed data, was "django-all-in-one-accessibility-1.6.tar", last modified: Sat Jun 10 12:39:18 2023, max compression
```

## Comparing `django-all-in-one-accessibility-1.5.tar` & `django-all-in-one-accessibility-1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:26.689315 django-all-in-one-accessibility-1.5/
--rw-rw-rw-   0        0        0     5615 2023-06-10 12:37:26.689315 django-all-in-one-accessibility-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4500 2023-06-10 12:36:56.000000 django-all-in-one-accessibility-1.5/Readme.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:26.649431 django-all-in-one-accessibility-1.5/accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.5/accessibility/__init__.py
--rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.5/accessibility/admin.py
--rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.5/accessibility/apps.py
--rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.5/accessibility/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:26.651425 django-all-in-one-accessibility-1.5/accessibility/migrations/
--rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.5/accessibility/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.5/accessibility/migrations/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.5/accessibility/models.py
--rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.5/accessibility/tests.py
--rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.5/accessibility/urls.py
--rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.5/accessibility/views.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:26.683328 django-all-in-one-accessibility-1.5/aioa_accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.5/aioa_accessibility/__init__.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.5/aioa_accessibility/asgi.py
--rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.5/aioa_accessibility/settings.py
--rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.5/aioa_accessibility/urls.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.5/aioa_accessibility/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:26.688319 django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/
--rw-rw-rw-   0        0        0     5615 2023-06-10 12:37:26.000000 django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-06-10 12:37:26.000000 django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:37:26.000000 django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-10 12:37:26.000000 django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-10 12:37:26.000000 django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-06-10 12:37:16.000000 django-all-in-one-accessibility-1.5/pyproject.toml
--rw-rw-rw-   0        0        0     1031 2023-06-10 12:37:26.690314 django-all-in-one-accessibility-1.5/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:39:18.889469 django-all-in-one-accessibility-1.6/
+-rw-rw-rw-   0        0        0     5604 2023-06-10 12:39:18.889469 django-all-in-one-accessibility-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4489 2023-06-10 12:39:10.000000 django-all-in-one-accessibility-1.6/Readme.md
+drwxrwxrwx   0        0        0        0 2023-06-10 12:39:18.860881 django-all-in-one-accessibility-1.6/accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.6/accessibility/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.6/accessibility/admin.py
+-rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.6/accessibility/apps.py
+-rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.6/accessibility/context_processors.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:39:18.861878 django-all-in-one-accessibility-1.6/accessibility/migrations/
+-rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.6/accessibility/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.6/accessibility/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.6/accessibility/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.6/accessibility/tests.py
+-rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.6/accessibility/urls.py
+-rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.6/accessibility/views.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:39:18.868873 django-all-in-one-accessibility-1.6/aioa_accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.6/aioa_accessibility/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.6/aioa_accessibility/asgi.py
+-rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.6/aioa_accessibility/settings.py
+-rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.6/aioa_accessibility/urls.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.6/aioa_accessibility/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:39:18.888470 django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/
+-rw-rw-rw-   0        0        0     5604 2023-06-10 12:39:18.000000 django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-10 12:39:18.000000 django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 12:39:18.000000 django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-10 12:39:18.000000 django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-06-10 12:39:18.000000 django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-06-10 12:38:53.000000 django-all-in-one-accessibility-1.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1031 2023-06-10 12:39:18.890464 django-all-in-one-accessibility-1.6/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.6/setup.py
```

### Comparing `django-all-in-one-accessibility-1.5/PKG-INFO` & `django-all-in-one-accessibility-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.5
+Version: 1.6
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -135,15 +135,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-There is some changes in base.html file for Oscar project <mark>when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer</mark>
+There is some changes in base.html file for Oscar project `when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer`
 ```python
 <footer>
 	<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
 </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.5
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.6
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -55,15 +55,15 @@
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
 Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
-There is some changes in base.html file for Oscar project when u are using
+There is some changes in base.html file for Oscar project `when u are using
 django oscar there is already base.html file exists so u need to go to oscar
 project directory which are locate in your site-packages(go to site-packages -
 > oscar -> templates ->oscar -> base.html) put this tag
- in oscar/templates/oscar/base.html footer ```python
+ in oscar/templates/oscar/base.html footer` ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.5/Readme.md` & `django-all-in-one-accessibility-1.6/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-There is some changes in base.html file for Oscar project <mark>when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer</mark>
+There is some changes in base.html file for Oscar project `when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer`
 ```python
 <footer>
 	<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
 </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -40,15 +40,15 @@
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
 Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
-There is some changes in base.html file for Oscar project when u are using
+There is some changes in base.html file for Oscar project `when u are using
 django oscar there is already base.html file exists so u need to go to oscar
 project directory which are locate in your site-packages(go to site-packages -
 > oscar -> templates ->oscar -> base.html) put this tag
- in oscar/templates/oscar/base.html footer ```python
+ in oscar/templates/oscar/base.html footer` ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.5/accessibility/admin.py` & `django-all-in-one-accessibility-1.6/accessibility/admin.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.5/accessibility/context_processors.py` & `django-all-in-one-accessibility-1.6/accessibility/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.5/accessibility/migrations/0001_initial.py` & `django-all-in-one-accessibility-1.6/accessibility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.5/accessibility/models.py` & `django-all-in-one-accessibility-1.6/accessibility/models.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.5/aioa_accessibility/settings.py` & `django-all-in-one-accessibility-1.6/aioa_accessibility/settings.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.5/aioa_accessibility/urls.py` & `django-all-in-one-accessibility-1.6/aioa_accessibility/urls.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/PKG-INFO` & `django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.5
+Version: 1.6
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -135,15 +135,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-There is some changes in base.html file for Oscar project <mark>when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer</mark>
+There is some changes in base.html file for Oscar project `when u are using django oscar there is already base.html file exists so u need to go to oscar project directory which are locate in your site-packages(go to site-packages -> oscar -> templates ->oscar -> base.html) put this tag <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script> in oscar/templates/oscar/base.html footer`
 ```python
 <footer>
 	<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
 </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.5
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.6
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -55,15 +55,15 @@
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
 Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
-There is some changes in base.html file for Oscar project when u are using
+There is some changes in base.html file for Oscar project `when u are using
 django oscar there is already base.html file exists so u need to go to oscar
 project directory which are locate in your site-packages(go to site-packages -
 > oscar -> templates ->oscar -> base.html) put this tag
- in oscar/templates/oscar/base.html footer ```python
+ in oscar/templates/oscar/base.html footer` ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.5/django_all_in_one_accessibility.egg-info/SOURCES.txt` & `django-all-in-one-accessibility-1.6/django_all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.5/pyproject.toml` & `django-all-in-one-accessibility-1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-all-in-one-accessibility"
-version = "1.5"
+version = "1.6"
 authors = [
   { name="Skynet Technologies USA LLC", email="developer3@skynettechnologies.com" },
 ]
 description = "All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button"
 readme = "Readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django-all-in-one-accessibility-1.5/setup.cfg` & `django-all-in-one-accessibility-1.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 616c 6c2d 696e   = django-all-in
 00000020: 2d6f 6e65 2d61 6363 6573 7369 6269 6c69  -one-accessibili
 00000030: 7479 0d0a 7665 7273 696f 6e20 3d20 312e  ty..version = 1.
-00000040: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
+00000040: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
 00000050: 2041 2044 6a61 6e67 6f20 4170 7020 6261   A Django App ba
 00000060: 7365 6420 6f6e 2061 7373 6973 7469 7665  sed on assistive
 00000070: 2074 6563 686e 6f6c 6f67 7920 7468 6174   technology that
 00000080: 2068 656c 7073 206f 7267 616e 697a 6174   helps organizat
 00000090: 696f 6e73 2065 6e68 616e 6365 2074 6865  ions enhance the
 000000a0: 2061 6363 6573 7369 6269 6c69 7479 2061   accessibility a
 000000b0: 6e64 2075 7361 6269 6c69 7479 206f 6620  nd usability of
```

