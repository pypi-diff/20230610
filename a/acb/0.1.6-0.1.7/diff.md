# Comparing `tmp/acb-0.1.6.tar.gz` & `tmp/acb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.1.6.tar", last modified: Sat Jun 10 17:07:28 2023, max compression
+gzip compressed data, was "acb-0.1.7.tar", last modified: Sat Jun 10 17:25:32 2023, max compression
```

## Comparing `acb-0.1.6.tar` & `acb-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1001 2023-05-27 13:27:12.641564 acb-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-10 17:02:37.330792 acb-0.1.6/acb/__init__.py
--rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.6/acb/actions/__init__.py
--rw-r--r--   0        0        0     3302 2023-06-10 16:40:53.286529 acb-0.1.6/acb/actions/encode.py
--rw-r--r--   0        0        0      893 2023-05-28 11:01:16.821596 acb-0.1.6/acb/actions/hash.py
--rw-r--r--   0        0        0       86 2023-06-08 13:59:12.603285 acb-0.1.6/acb/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.6/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0     1566 2023-05-28 09:13:29.665468 acb-0.1.6/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.6/acb/adapters/database/__init__.py
--rw-r--r--   0        0        0       97 2023-05-27 21:16:18.244974 acb-0.1.6/acb/adapters/database/redis_om.py
--rw-r--r--   0        0        0    16633 2023-05-28 11:24:26.304819 acb-0.1.6/acb/adapters/database/sqlalchemy.py
--rw-r--r--   0        0        0     1848 2023-05-27 13:27:44.420088 acb-0.1.6/acb/adapters/database/sqlmodel.py
--rw-r--r--   0        0        0        0 2023-05-27 19:13:35.056779 acb-0.1.6/acb/adapters/debug/__init__.py
--rw-r--r--   0        0        0      471 2023-05-27 21:16:52.557919 acb-0.1.6/acb/adapters/debug/sentry.py
--rw-r--r--   0        0        0     4764 2023-05-28 09:40:25.073871 acb-0.1.6/acb/adapters/dns/cloud_dns.py
--rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.6/acb/adapters/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 20:21:31.954823 acb-0.1.6/acb/adapters/mail/gmail.py
--rw-r--r--   0        0        0     9916 2023-06-01 13:42:09.249464 acb-0.1.6/acb/adapters/mail/mailgun.py
--rw-r--r--   0        0        0        0 2023-05-27 13:39:02.267034 acb-0.1.6/acb/adapters/requests/__init__.py
--rw-r--r--   0        0        0      687 2023-05-27 21:16:18.575095 acb-0.1.6/acb/adapters/requests/httpx.py
--rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.6/acb/adapters/secrets/__init__.py
--rw-r--r--   0        0        0     7058 2023-06-08 14:00:12.903726 acb-0.1.6/acb/adapters/secrets/secret_manager.py
--rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.6/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     4938 2023-05-28 08:44:28.039395 acb-0.1.6/acb/adapters/storage/cloud_storage.py
--rw-r--r--   0        0        0     6374 2023-05-28 09:26:16.911587 acb-0.1.6/acb/adapters/storage/universal.py
--rw-r--r--   0        0        0     4807 2023-06-09 15:16:58.144879 acb-0.1.6/acb/config.py
--rw-r--r--   0        0        0     3439 2023-06-08 14:34:18.922003 acb-0.1.6/acb/logger.py
--rw-r--r--   0        0        0     1722 2023-06-10 17:07:28.954622 acb-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 acb-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1001 2023-05-27 13:27:12.641564 acb-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 17:02:37.330792 acb-0.1.7/acb/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.7/acb/actions/__init__.py
+-rw-r--r--   0        0        0     3302 2023-06-10 16:40:53.286529 acb-0.1.7/acb/actions/encode.py
+-rw-r--r--   0        0        0      893 2023-05-28 11:01:16.821596 acb-0.1.7/acb/actions/hash.py
+-rw-r--r--   0        0        0       86 2023-06-08 13:59:12.603285 acb-0.1.7/acb/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.7/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1566 2023-05-28 09:13:29.665468 acb-0.1.7/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.7/acb/adapters/database/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-27 21:16:18.244974 acb-0.1.7/acb/adapters/database/redis_om.py
+-rw-r--r--   0        0        0    16633 2023-05-28 11:24:26.304819 acb-0.1.7/acb/adapters/database/sqlalchemy.py
+-rw-r--r--   0        0        0     1848 2023-05-27 13:27:44.420088 acb-0.1.7/acb/adapters/database/sqlmodel.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:13:35.056779 acb-0.1.7/acb/adapters/debug/__init__.py
+-rw-r--r--   0        0        0      471 2023-05-27 21:16:52.557919 acb-0.1.7/acb/adapters/debug/sentry.py
+-rw-r--r--   0        0        0     4764 2023-05-28 09:40:25.073871 acb-0.1.7/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.7/acb/adapters/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:21:31.954823 acb-0.1.7/acb/adapters/mail/gmail.py
+-rw-r--r--   0        0        0     9916 2023-06-01 13:42:09.249464 acb-0.1.7/acb/adapters/mail/mailgun.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:39:02.267034 acb-0.1.7/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-27 21:16:18.575095 acb-0.1.7/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.7/acb/adapters/secrets/__init__.py
+-rw-r--r--   0        0        0     7058 2023-06-08 14:00:12.903726 acb-0.1.7/acb/adapters/secrets/secret_manager.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.7/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     4938 2023-05-28 08:44:28.039395 acb-0.1.7/acb/adapters/storage/cloud_storage.py
+-rw-r--r--   0        0        0     6374 2023-05-28 09:26:16.911587 acb-0.1.7/acb/adapters/storage/universal.py
+-rw-r--r--   0        0        0     4807 2023-06-09 15:16:58.144879 acb-0.1.7/acb/config.py
+-rw-r--r--   0        0        0     3439 2023-06-08 14:34:18.922003 acb-0.1.7/acb/logger.py
+-rw-r--r--   0        0        0     1722 2023-06-10 17:25:32.383123 acb-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 acb-0.1.7/PKG-INFO
```

### Comparing `acb-0.1.6/README.md` & `acb-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/actions/encode.py` & `acb-0.1.7/acb/actions/encode.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/actions/hash.py` & `acb-0.1.7/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/cache/redis.py` & `acb-0.1.7/acb/adapters/cache/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/database/sqlalchemy.py` & `acb-0.1.7/acb/adapters/database/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/database/sqlmodel.py` & `acb-0.1.7/acb/adapters/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/dns/cloud_dns.py` & `acb-0.1.7/acb/adapters/dns/cloud_dns.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/mail/mailgun.py` & `acb-0.1.7/acb/adapters/mail/mailgun.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/requests/httpx.py` & `acb-0.1.7/acb/adapters/requests/httpx.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/secrets/secret_manager.py` & `acb-0.1.7/acb/adapters/secrets/secret_manager.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/storage/cloud_storage.py` & `acb-0.1.7/acb/adapters/storage/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/adapters/storage/universal.py` & `acb-0.1.7/acb/adapters/storage/universal.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/config.py` & `acb-0.1.7/acb/config.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/acb/logger.py` & `acb-0.1.7/acb/logger.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.6/pyproject.toml` & `acb-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "acb"
-version = "0.1.6"
+version = "0.1.7"
 description = "Asynchronus Code Base"
 dependencies = [
     "itsdangerous>=2.1.2",
     "msgspec>=0.14.1",
     "aiopath>=0.6.11",
     "arrow>=1.2.3",
     "google-crc32c>=1.5.0",
```

### Comparing `acb-0.1.6/PKG-INFO` & `acb-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.1.6
+Version: 0.1.7
 Summary: Asynchronus Code Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/acb
 Project-URL: Documentation, https://github.com/lesleslie/acb
 Project-URL: Repository, https://github.com/lesleslie/acb
 Requires-Python: >=3.11
```

