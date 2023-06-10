# Comparing `tmp/netbox-vlan-manager-0.0.3.tar.gz` & `tmp/netbox-vlan-manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-vlan-manager-0.0.3.tar", last modified: Tue Apr 25 15:13:14 2023, max compression
+gzip compressed data, was "netbox-vlan-manager-0.0.4.tar", last modified: Sat Jun 10 06:33:32 2023, max compression
```

## Comparing `netbox-vlan-manager-0.0.3.tar` & `netbox-vlan-manager-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/templatetags/view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/netbox_vlan_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/netbox_vlan_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/netbox_vlan_manager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/netbox_vlan_manager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/templatetags/view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-10 06:33:32.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-10 06:33:32.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 06:33:32.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 06:33:32.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 06:33:32.000000 netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 06:33:32.597244 netbox-vlan-manager-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-10 06:33:23.000000 netbox-vlan-manager-0.0.4/setup.py
```

### Comparing `netbox-vlan-manager-0.0.3/LICENSE` & `netbox-vlan-manager-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.3/PKG-INFO` & `netbox-vlan-manager-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NetBox VLAN Manager
 
@@ -27,14 +27,15 @@
 ## Compatibility
 
 Each Plugin Version listed below has been tested with its corresponding NetBox Version.
 
 | NetBox Version | Plugin Version |
 | :------------: | :------------: |
 |      3.4       |     0.0.1      |
+|      3.5       |     0.0.4      |
 
 ## Installation
 
 The plugin is available as a Python package in PyPI and can be installed with pip:
 
 ```bash
 pip install netbox-vlan-manager
```

### Comparing `netbox-vlan-manager-0.0.3/README.md` & `netbox-vlan-manager-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ## Compatibility
 
 Each Plugin Version listed below has been tested with its corresponding NetBox Version.
 
 | NetBox Version | Plugin Version |
 | :------------: | :------------: |
 |      3.4       |     0.0.1      |
+|      3.5       |     0.0.4      |
 
 ## Installation
 
 The plugin is available as a Python package in PyPI and can be installed with pip:
 
 ```bash
 pip install netbox-vlan-manager
```

### Comparing `netbox-vlan-manager-0.0.3/netbox_vlan_manager/forms.py` & `netbox-vlan-manager-0.0.4/netbox_vlan_manager/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/0001_initial.py` & `netbox-vlan-manager-0.0.4/netbox_vlan_manager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.3/netbox_vlan_manager/navigation.py` & `netbox-vlan-manager-0.0.4/netbox_vlan_manager/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.3/netbox_vlan_manager/tables.py` & `netbox-vlan-manager-0.0.4/netbox_vlan_manager/tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from netbox.models import NetBoxModel
 from django.urls import reverse
 import django_tables2 as tables
 from netbox.tables import NetBoxTable, BaseTable
 from .models import VLANGroupSet
 
 VLAN_STATUS = """
 {% if record.status == 'Available' %}
@@ -54,14 +55,15 @@
     vid = tables.Column(
         verbose_name='VID',
         linkify=lambda record: f'{reverse("ipam:vlan_list")}?vid={record["vid"]}'
     )
     status = tables.TemplateColumn(template_code=VLAN_STATUS)
 
     class Meta(BaseTable.Meta):
+        model = NetBoxModel
         template_name = 'netbox_vlan_manager/vlangroupset_vlans.html'
         empty_text = 'No VLANs found'
         fields = (
             'vid',
             'status',
         )
         row_attrs = {
```

### Comparing `netbox-vlan-manager-0.0.3/netbox_vlan_manager/urls.py` & `netbox-vlan-manager-0.0.4/netbox_vlan_manager/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/PKG-INFO` & `netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NetBox VLAN Manager
 
@@ -27,14 +27,15 @@
 ## Compatibility
 
 Each Plugin Version listed below has been tested with its corresponding NetBox Version.
 
 | NetBox Version | Plugin Version |
 | :------------: | :------------: |
 |      3.4       |     0.0.1      |
+|      3.5       |     0.0.4      |
 
 ## Installation
 
 The plugin is available as a Python package in PyPI and can be installed with pip:
 
 ```bash
 pip install netbox-vlan-manager
```

### Comparing `netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/SOURCES.txt` & `netbox-vlan-manager-0.0.4/netbox_vlan_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.3/setup.py` & `netbox-vlan-manager-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,12 +31,12 @@
     author='miyuk',
     author_email='miyuk@miyuk.net',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[],
     zip_safe=False,
     classifiers=[
-        'Development Status :: 1 - Planning',
+        'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Programming Language :: Python :: 3',
     ]
 )
```

