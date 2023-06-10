# Comparing `tmp/django_graphbox-1.2.4.tar.gz` & `tmp/django_graphbox-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_graphbox-1.2.4.tar", last modified: Mon May  8 00:49:29 2023, max compression
+gzip compressed data, was "django_graphbox-1.2.5.tar", last modified: Sat Jun 10 02:29:33 2023, max compression
```

## Comparing `django_graphbox-1.2.4.tar` & `django_graphbox-1.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:49:29.876333 django_graphbox-1.2.4/
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.4/LICENSE
--rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2022-07-20 15:01:25.000000 django_graphbox-1.2.4/MANIFEST.in
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18436 2023-05-08 00:49:29.876333 django_graphbox-1.2.4/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)    20300 2023-02-23 04:15:18.000000 django_graphbox-1.2.4/README.md
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:49:29.820340 django_graphbox-1.2.4/docs/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:49:29.868334 django_graphbox-1.2.4/docs/source/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    17893 2023-05-08 00:49:04.000000 django_graphbox-1.2.4/docs/source/quickstart.rst
--rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2022-07-20 15:01:25.000000 django_graphbox-1.2.4/pyproject.toml
--rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-05-08 00:49:29.880332 django_graphbox-1.2.4/setup.cfg
--rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2022-07-20 15:01:25.000000 django_graphbox-1.2.4/setup.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:49:29.824340 django_graphbox-1.2.4/src/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:49:29.872333 django_graphbox-1.2.4/src/django_graphbox/
--rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2022-07-20 02:16:01.000000 django_graphbox-1.2.4/src/django_graphbox/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    12707 2023-05-08 00:46:51.000000 django_graphbox-1.2.4/src/django_graphbox/builder.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1750 2023-04-28 18:44:37.000000 django_graphbox-1.2.4/src/django_graphbox/constants.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2022-07-30 04:00:13.000000 django_graphbox-1.2.4/src/django_graphbox/exceptions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2022-07-20 02:16:01.000000 django_graphbox-1.2.4/src/django_graphbox/hasher.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:49:29.876333 django_graphbox-1.2.4/src/django_graphbox/helpers/
--rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2022-07-20 02:16:01.000000 django_graphbox-1.2.4/src/django_graphbox/helpers/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    16165 2023-02-24 03:36:43.000000 django_graphbox-1.2.4/src/django_graphbox/helpers/mutations.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     6662 2023-05-07 23:58:24.000000 django_graphbox-1.2.4/src/django_graphbox/helpers/queries.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2022-07-30 04:08:45.000000 django_graphbox-1.2.4/src/django_graphbox/helpers/sessions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2022-07-20 02:16:01.000000 django_graphbox-1.2.4/src/django_graphbox/helpers/shared.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-02-23 21:40:53.000000 django_graphbox-1.2.4/src/django_graphbox/session.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:49:29.872333 django_graphbox-1.2.4/src/django_graphbox.egg-info/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18436 2023-05-08 00:49:29.000000 django_graphbox-1.2.4/src/django_graphbox.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-05-08 00:49:29.000000 django_graphbox-1.2.4/src/django_graphbox.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-05-08 00:49:29.000000 django_graphbox-1.2.4/src/django_graphbox.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-05-08 00:49:29.000000 django_graphbox-1.2.4/src/django_graphbox.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-05-08 00:49:29.000000 django_graphbox-1.2.4/src/django_graphbox.egg-info/top_level.txt
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.5/LICENSE
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2022-07-20 15:01:25.000000 django_graphbox-1.2.5/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18375 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    20300 2023-02-23 04:15:18.000000 django_graphbox-1.2.5/README.md
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.800131 django_graphbox-1.2.5/docs/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.804131 django_graphbox-1.2.5/docs/source/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    17832 2023-06-10 02:21:38.000000 django_graphbox-1.2.5/docs/source/quickstart.rst
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2022-07-20 15:01:25.000000 django_graphbox-1.2.5/pyproject.toml
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-06-10 02:29:33.812130 django_graphbox-1.2.5/setup.cfg
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2022-07-20 15:01:25.000000 django_graphbox-1.2.5/setup.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.800131 django_graphbox-1.2.5/src/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.804131 django_graphbox-1.2.5/src/django_graphbox/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    12736 2023-06-10 02:21:38.000000 django_graphbox-1.2.5/src/django_graphbox/builder.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1821 2023-06-10 02:26:09.000000 django_graphbox-1.2.5/src/django_graphbox/constants.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2022-07-30 04:00:13.000000 django_graphbox-1.2.5/src/django_graphbox/exceptions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/hasher.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/src/django_graphbox/helpers/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    16216 2023-06-10 02:27:05.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/mutations.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     6662 2023-05-07 23:58:24.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/queries.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2022-07-30 04:08:45.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/sessions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/shared.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-02-23 21:40:53.000000 django_graphbox-1.2.5/src/django_graphbox/session.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/src/django_graphbox.egg-info/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18375 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/top_level.txt
```

### Comparing `django_graphbox-1.2.4/LICENSE` & `django_graphbox-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/PKG-INFO` & `django_graphbox-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_graphbox
-Version: 1.2.4
+Version: 1.2.5
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -347,8 +347,7 @@
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
     * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
-    * Version 1.2.4 Fix custom attributes on the model Type.
```

### Comparing `django_graphbox-1.2.4/README.md` & `django_graphbox-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/docs/source/quickstart.rst` & `django_graphbox-1.2.5/docs/source/quickstart.rst`

 * *Files 0% similar despite different names*

```diff
@@ -330,9 +330,8 @@
             
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
-    * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
-    * Version 1.2.4 Fix custom attributes on the model Type.
+    * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
```

### Comparing `django_graphbox-1.2.4/setup.cfg` & `django_graphbox-1.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_graphbox
-version = 1.2.4
+version = 1.2.5
 description = Package for easy building GraphQL API with Django
 long_description = file:docs/source/quickstart.rst
 url = https://github.com/yefeza/django-graphbox
 author = Yeison Fernandez
 author_email = contacto@90horasporsemana.com
 license = MIT
 classifiers =
```

### Comparing `django_graphbox-1.2.4/src/django_graphbox/builder.py` & `django_graphbox-1.2.5/src/django_graphbox/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
             custom_attrs_for_type (list): List of custom attributes to add to the model type. [{'name': 'attr_name', 'value': 'attr_value'}, ...]
             ordering_field (str): Field to use for ordering the list_field operation.
         """
         #get the model name
         model_name = model.__name__
         #crreate the model type
         model_metaclass = type(f"Meta", (), {'model': model, 'exclude_fields': exclude_fields})
-        type_attrs={'Meta': model_metaclass}
+        model_type = type(f"{model_name}Type", (DjangoObjectType,), {'Meta': model_metaclass})
+        #add custom attributes to the model type
         for attr in custom_attrs_for_type:
-            type_attrs[attr['name']]=attr['value']
-        model_type = type(f"{model_name}Type", (DjangoObjectType,), type_attrs)
+            setattr(model_type, attr['name'], attr['value'])
         #create paginated type
         if pagination_length > 0 and pagination_style == 'paginated':
             paginated_type = type(f"{model_name}PageType", (graphene.ObjectType,), {'items': graphene.List(model_type), 'page': graphene.Int(), 'has_next_page': graphene.Boolean(), 'has_previous_page': graphene.Boolean(), 'total_pages': graphene.Int(), 'total_items': graphene.Int()})
         else:
             paginated_type = None
         #make a new model config
         config = {
```

### Comparing `django_graphbox-1.2.4/src/django_graphbox/constants.py` & `django_graphbox-1.2.5/src/django_graphbox/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     'PositiveSmallIntegerField': graphene.Int,
     'SlugField': graphene.String,
     'SmallIntegerField': graphene.Int,
     'TextField': graphene.String,
     'TimeField': graphene.Time,
     'URLField': graphene.String,
     'UUIDField': graphene.String,
-    'ForeignKey': graphene.ID
+    'ForeignKey': graphene.ID,
+    'JSONField': graphene.String,
+    'OneToOneField': graphene.ID,
 }
 
 NO_ERROR=0
 UNKNOWN_ERROR=1
 INVALID_CREDENTIALS=2
 INVALID_TOKEN=3
 EXPIRED_TOKEN=4
```

### Comparing `django_graphbox-1.2.4/src/django_graphbox/exceptions.py` & `django_graphbox-1.2.5/src/django_graphbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/src/django_graphbox/hasher.py` & `django_graphbox-1.2.5/src/django_graphbox/hasher.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/src/django_graphbox/helpers/mutations.py` & `django_graphbox-1.2.5/src/django_graphbox/helpers/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """
     class Arguments:
         pass
     exclude_fields = ['created_at', 'updated_at'] + fields_to_ignore
     for field in model._meta.fields:
         if field.name not in exclude_fields:
             field_type=field.get_internal_type()
-            if field_type!='ManyToManyField':
+            if field_type in MODEL_FIELD_TO_GRAPHENE_TYPE.keys():
                 argument_type=MODEL_FIELD_TO_GRAPHENE_TYPE[field_type]
                 required=True
                 if field.null or field_type in ['ImageField', 'FileField'] or field.name in fields_as_password:
                     required=False
                 setattr(Arguments, field.name.lower(), argument_type(required=required))
     return Arguments
 
@@ -113,15 +113,15 @@
                     fields_to_resolve=internal_field_resolvers.get('create_field')
                     kwargs.update(fields_to_resolve)
                 for key, value in kwargs.items():
                     field_type=instance._meta.get_field(key).__class__.__name__
                     if callable(value):
                         value=value(info, instance, **kwargs)
                     if value!=None:
-                        if field_type=='ForeignKey':
+                        if field_type=='ForeignKey' or field_type=='OneToOneField':
                             foreign_model=instance._meta.get_field(key).related_model
                             value=foreign_model.objects.get(id=value)
                             setattr(instance, key, value)
                         elif field_type=='FileField':
                             file=File(value)
                             extension=file.name.split('.')[-1]
                             sha1_file=HashManager.getSHA1file(file)
```

### Comparing `django_graphbox-1.2.4/src/django_graphbox/helpers/queries.py` & `django_graphbox-1.2.5/src/django_graphbox/helpers/queries.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/src/django_graphbox/helpers/sessions.py` & `django_graphbox-1.2.5/src/django_graphbox/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/src/django_graphbox/helpers/shared.py` & `django_graphbox-1.2.5/src/django_graphbox/helpers/shared.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/src/django_graphbox/session.py` & `django_graphbox-1.2.5/src/django_graphbox/session.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.4/src/django_graphbox.egg-info/PKG-INFO` & `django_graphbox-1.2.5/src/django_graphbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-graphbox
-Version: 1.2.4
+Version: 1.2.5
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -347,8 +347,7 @@
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
     * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
-    * Version 1.2.4 Fix custom attributes on the model Type.
```

### Comparing `django_graphbox-1.2.4/src/django_graphbox.egg-info/SOURCES.txt` & `django_graphbox-1.2.5/src/django_graphbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

