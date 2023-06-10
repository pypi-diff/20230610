# Comparing `tmp/netbox-ddns-1.2.7.tar.gz` & `tmp/netbox-ddns-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-ddns-1.2.7.tar", last modified: Sat May 20 13:55:55 2023, max compression
+gzip compressed data, was "netbox-ddns-1.2.8.tar", last modified: Sat Jun 10 12:44:57 2023, max compression
```

## Comparing `netbox-ddns-1.2.7.tar` & `netbox-ddns-1.2.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:55.640450 netbox-ddns-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-20 13:55:55.640450 netbox-ddns-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:55.636450 netbox-ddns-1.2.7/netbox_ddns/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/background_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:55.640450 netbox-ddns-1.2.7/netbox_ddns/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0002_add_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0003_dnsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0004_ensure_trailing_dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0005_extradnsname.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0006_extradns_cname.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0007_zone_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/0008_server_server_port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:55.636450 netbox-ddns-1.2.7/netbox_ddns/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:55.636450 netbox-ddns-1.2.7/netbox_ddns/templates/netbox_ddns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:55.640450 netbox-ddns-1.2.7/netbox_ddns/templates/netbox_ddns/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/templates/netbox_ddns/ipaddress/dns_extra.html
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/templates/netbox_ddns/ipaddress/dns_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/templates/netbox_ddns/ipaddress/dns_refresh_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/netbox_ddns/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:55:55.640450 netbox-ddns-1.2.7/netbox_ddns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-20 13:55:55.000000 netbox-ddns-1.2.7/netbox_ddns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-20 13:55:55.000000 netbox-ddns-1.2.7/netbox_ddns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:55:55.000000 netbox-ddns-1.2.7/netbox_ddns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:55:55.000000 netbox-ddns-1.2.7/netbox_ddns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 13:55:55.000000 netbox-ddns-1.2.7/netbox_ddns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 13:55:55.000000 netbox-ddns-1.2.7/netbox_ddns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-20 13:55:55.640450 netbox-ddns-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 13:55:45.000000 netbox-ddns-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:57.526764 netbox-ddns-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-10 12:44:57.526764 netbox-ddns-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:57.522764 netbox-ddns-1.2.8/netbox_ddns/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:57.526764 netbox-ddns-1.2.8/netbox_ddns/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0002_add_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0003_dnsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0004_ensure_trailing_dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0005_extradnsname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0006_extradns_cname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0007_zone_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/0008_server_server_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:57.522764 netbox-ddns-1.2.8/netbox_ddns/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:57.522764 netbox-ddns-1.2.8/netbox_ddns/templates/netbox_ddns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:57.526764 netbox-ddns-1.2.8/netbox_ddns/templates/netbox_ddns/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/templates/netbox_ddns/ipaddress/dns_extra.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/templates/netbox_ddns/ipaddress/dns_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/templates/netbox_ddns/ipaddress/dns_refresh_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/netbox_ddns/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:44:57.522764 netbox-ddns-1.2.8/netbox_ddns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-10 12:44:57.000000 netbox-ddns-1.2.8/netbox_ddns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-10 12:44:57.000000 netbox-ddns-1.2.8/netbox_ddns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:44:57.000000 netbox-ddns-1.2.8/netbox_ddns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:44:57.000000 netbox-ddns-1.2.8/netbox_ddns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-10 12:44:57.000000 netbox-ddns-1.2.8/netbox_ddns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 12:44:57.000000 netbox-ddns-1.2.8/netbox_ddns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-10 12:44:57.526764 netbox-ddns-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-10 12:44:48.000000 netbox-ddns-1.2.8/setup.py
```

### Comparing `netbox-ddns-1.2.7/LICENSE.txt` & `netbox-ddns-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/PKG-INFO` & `netbox-ddns-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-ddns
-Version: 1.2.7
+Version: 1.2.8
 Summary: Dynamic DNS Connector for NetBox
 Home-page: https://github.com/sjm-steffann/netbox-ddns
 Author: Sander Steffann
 Author-email: sander@steffann.nl
 License: Apache 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
```

### Comparing `netbox-ddns-1.2.7/README.md` & `netbox-ddns-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/__init__.py` & `netbox-ddns-1.2.8/netbox_ddns/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '1.2.7'
+VERSION = '1.2.8'
 
 try:
     from extras.plugins import PluginConfig
 except ImportError:
     # Dummy for when importing outside of netbox
     class PluginConfig:
         pass
```

### Comparing `netbox-ddns-1.2.7/netbox_ddns/admin.py` & `netbox-ddns-1.2.8/netbox_ddns/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/background_tasks.py` & `netbox-ddns-1.2.8/netbox_ddns/background_tasks.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/migrations/0001_initial.py` & `netbox-ddns-1.2.8/netbox_ddns/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/migrations/0002_add_ttl.py` & `netbox-ddns-1.2.8/netbox_ddns/migrations/0002_add_ttl.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/migrations/0003_dnsstatus.py` & `netbox-ddns-1.2.8/netbox_ddns/migrations/0003_dnsstatus.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/migrations/0004_ensure_trailing_dot.py` & `netbox-ddns-1.2.8/netbox_ddns/migrations/0004_ensure_trailing_dot.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/migrations/0005_extradnsname.py` & `netbox-ddns-1.2.8/netbox_ddns/migrations/0005_extradnsname.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/migrations/0008_server_server_port.py` & `netbox-ddns-1.2.8/netbox_ddns/migrations/0008_server_server_port.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/models.py` & `netbox-ddns-1.2.8/netbox_ddns/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         self.server = self.server.lower().rstrip('.')
 
         # Ensure trailing dots from domain-style fields
         self.tsig_key_name = normalize_fqdn(self.tsig_key_name.lower().rstrip('.'))
 
     @property
     def address(self) -> Optional[str]:
-        addrinfo = socket.getaddrinfo(self.server, 'domain', proto=socket.IPPROTO_UDP)
+        addrinfo = socket.getaddrinfo(self.server, self.server_port, proto=socket.IPPROTO_UDP)
         for family, _, _, _, sockaddr in addrinfo:
             if family in (socket.AF_INET, socket.AF_INET6) and sockaddr[0]:
                 return sockaddr[0]
 
     def create_update(self, zone: str) -> dns.update.Update:
         return dns.update.Update(
             zone=normalize_fqdn(zone),
```

### Comparing `netbox-ddns-1.2.7/netbox_ddns/signals.py` & `netbox-ddns-1.2.8/netbox_ddns/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/tables.py` & `netbox-ddns-1.2.8/netbox_ddns/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/template_content.py` & `netbox-ddns-1.2.8/netbox_ddns/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/templates/netbox_ddns/ipaddress/dns_extra.html` & `netbox-ddns-1.2.8/netbox_ddns/templates/netbox_ddns/ipaddress/dns_extra.html`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/templates/netbox_ddns/ipaddress/dns_info.html` & `netbox-ddns-1.2.8/netbox_ddns/templates/netbox_ddns/ipaddress/dns_info.html`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/urls.py` & `netbox-ddns-1.2.8/netbox_ddns/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/utils.py` & `netbox-ddns-1.2.8/netbox_ddns/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/validators.py` & `netbox-ddns-1.2.8/netbox_ddns/validators.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns/views.py` & `netbox-ddns-1.2.8/netbox_ddns/views.py`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/netbox_ddns.egg-info/PKG-INFO` & `netbox-ddns-1.2.8/netbox_ddns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-ddns
-Version: 1.2.7
+Version: 1.2.8
 Summary: Dynamic DNS Connector for NetBox
 Home-page: https://github.com/sjm-steffann/netbox-ddns
 Author: Sander Steffann
 Author-email: sander@steffann.nl
 License: Apache 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
```

### Comparing `netbox-ddns-1.2.7/netbox_ddns.egg-info/SOURCES.txt` & `netbox-ddns-1.2.8/netbox_ddns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-ddns-1.2.7/setup.cfg` & `netbox-ddns-1.2.8/setup.cfg`

 * *Files identical despite different names*

