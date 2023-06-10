# Comparing `tmp/django-forbid-0.1.2.tar.gz` & `tmp/django-forbid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.1.2.tar", last modified: Mon May 29 17:50:08 2023, max compression
+gzip compressed data, was "django-forbid-0.1.4.tar", last modified: Sat Jun 10 14:11:24 2023, max compression
```

## Comparing `django-forbid-0.1.2.tar` & `django-forbid-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 17:49:55.000000 django-forbid-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 17:49:55.000000 django-forbid-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-29 17:50:08.087865 django-forbid-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-29 17:49:55.000000 django-forbid-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-29 17:49:55.000000 django-forbid-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-29 17:50:08.087865 django-forbid-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 17:49:55.000000 django-forbid-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.083865 django-forbid-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/forbid_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/forbid_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/forbid_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/templates/timezone.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-10 14:11:16.000000 django-forbid-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-10 14:11:16.000000 django-forbid-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-10 14:11:24.587829 django-forbid-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-10 14:11:16.000000 django-forbid-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 14:11:16.000000 django-forbid-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-10 14:11:24.587829 django-forbid-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-10 14:11:16.000000 django-forbid-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/forbid_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/forbid_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/forbid_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/templates/timezone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.1.2/LICENSE` & `django-forbid-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.2/PKG-INFO` & `django-forbid-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.2
+Version: 0.1.4
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
```

### Comparing `django-forbid-0.1.2/README.md` & `django-forbid-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.2/setup.cfg` & `django-forbid-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.2/src/django_forbid/skills/__init__.py` & `django-forbid-0.1.4/src/django_forbid/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.2/src/django_forbid/skills/forbid_device.py` & `django-forbid-0.1.4/src/django_forbid/skills/forbid_device.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.2/src/django_forbid/skills/forbid_location.py` & `django-forbid-0.1.4/src/django_forbid/skills/forbid_location.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
     def __call__(self, request):
         city = dict()
         geoip = GeoIP2()
         address = request.META.get("REMOTE_ADDR")
         address = request.META.get("HTTP_X_FORWARDED_FOR", address)
         client_ip = address.split(",")[0].strip()
+        verified_ip = request.session.get("VERIFIED_IP", "")
+
+        if verified_ip and verified_ip == client_ip:
+            return self.get_response(request)
 
         try:
             city = geoip.city(client_ip)
 
             countries = Settings.get("COUNTRIES", [])
             territories = Settings.get("TERRITORIES", [])
             granted = all([
@@ -43,14 +47,18 @@
             # comparing it with the timezone in the
             # POST request sent from user's browser
             # to detect if the user is using a VPN.
             timezone = city.get("time_zone", "N/A")
             request.session["GEOIP2_TZ"] = timezone
 
         if granted:
+            request.session["VERIFIED_IP"] = client_ip
             return self.get_response(request)
 
+        # Erases the timezone from the session.
+        request.session["VERIFIED_IP"] = ""
+
         # Redirects to the FORBIDDEN_LOC URL if set.
         if Settings.has("OPTIONS.URL.FORBIDDEN_LOC"):
             return redirect(Settings.get("OPTIONS.URL.FORBIDDEN_LOC"))
 
         return HttpResponseForbidden()
```

### Comparing `django-forbid-0.1.2/src/django_forbid/skills/forbid_network.py` & `django-forbid-0.1.4/src/django_forbid/skills/forbid_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import re
 
 from django.http import HttpResponse
 from django.http import HttpResponseForbidden
 from django.shortcuts import redirect
 from django.shortcuts import render
 
 from . import Settings
@@ -27,28 +26,19 @@
             if Settings.has("OPTIONS.URL.FORBIDDEN_NET"):
                 return redirect(Settings.get("OPTIONS.URL.FORBIDDEN_NET"))
             return HttpResponseForbidden()
 
         geoip2_tz = request.session.get("GEOIP2_TZ")
         verified_tz = request.session.get("VERIFIED_TZ", "")
 
-        if any([
-            verified_tz == geoip2_tz,
-            # Checks if VPN is False or not set.
-            not Settings.get("OPTIONS.VPN", False),
-            # Checks if the request is an AJAX request.
-            not re.search(
-                r"\w+\/(?:html|xhtml\+xml|xml)",
-                request.META.get("HTTP_ACCEPT"),
-            ),
-        ]):
+        # Checks if the user's timezone match with the last accessed one.
+        if verified_tz == geoip2_tz or not Settings.get("OPTIONS.VPN", False):
             return self.get_response(request)
-
         # Checks if GEOIP2_TZ and VERIFIED_TZ don't exist.
-        if all([verified_tz, geoip2_tz != "N/A"]):
+        elif verified_tz and geoip2_tz != "N/A":
             return forbidden_page()
 
         if all(map(request.session.has_key, ("GEOIP2_TZ", *response_attributes))):
             # Handles if the user's timezone differs from the
             # one determined by GeoIP API. If so, VPN is used.
             client_tz = request.POST.get("CLIENT_TZ", verified_tz)
```

### Comparing `django-forbid-0.1.2/src/django_forbid/templates/timezone.html` & `django-forbid-0.1.4/src/django_forbid/templates/timezone.html`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.2/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.1.4/src/django_forbid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.2
+Version: 0.1.4
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
```

### Comparing `django-forbid-0.1.2/src/django_forbid.egg-info/SOURCES.txt` & `django-forbid-0.1.4/src/django_forbid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

