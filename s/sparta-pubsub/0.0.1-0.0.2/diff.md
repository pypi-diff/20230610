# Comparing `tmp/sparta-pubsub-0.0.1.tar.gz` & `tmp/sparta-pubsub-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparta-pubsub-0.0.1.tar", last modified: Thu Oct 20 11:07:22 2022, max compression
+gzip compressed data, was "sparta-pubsub-0.0.2.tar", last modified: Sat Jun 10 11:53:00 2023, max compression
```

## Comparing `sparta-pubsub-0.0.1.tar` & `sparta-pubsub-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:07:22.939715 sparta-pubsub-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1073 2022-10-20 11:05:42.000000 sparta-pubsub-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      668 2022-10-20 11:07:22.939715 sparta-pubsub-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2022-10-20 11:05:42.000000 sparta-pubsub-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-20 11:07:22.939715 sparta-pubsub-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1486 2022-10-20 11:05:42.000000 sparta-pubsub-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:07:22.935715 sparta-pubsub-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:07:22.935715 sparta-pubsub-0.0.1/src/sparta/
--rw-r--r--   0 root         (0) root         (0)       56 2022-10-20 11:05:42.000000 sparta-pubsub-0.0.1/src/sparta/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:07:22.935715 sparta-pubsub-0.0.1/src/sparta/pubsub/
--rw-r--r--   0 root         (0) root         (0)       76 2022-10-20 11:05:42.000000 sparta-pubsub-0.0.1/src/sparta/pubsub/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2692 2022-10-20 11:05:42.000000 sparta-pubsub-0.0.1/src/sparta/pubsub/consumer.py
--rw-r--r--   0 root         (0) root         (0)     1049 2022-10-20 11:05:42.000000 sparta-pubsub-0.0.1/src/sparta/pubsub/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:07:22.935715 sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      668 2022-10-20 11:07:22.000000 sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2022-10-20 11:07:22.000000 sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-20 11:07:22.000000 sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-20 11:07:22.000000 sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       64 2022-10-20 11:07:22.000000 sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-20 11:07:22.000000 sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:53:00.953648 sparta-pubsub-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-10 11:52:35.000000 sparta-pubsub-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-10 11:53:00.953648 sparta-pubsub-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-10 11:52:35.000000 sparta-pubsub-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 11:53:00.953648 sparta-pubsub-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-06-10 11:52:35.000000 sparta-pubsub-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:53:00.949648 sparta-pubsub-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:53:00.949648 sparta-pubsub-0.0.2/src/sparta/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-10 11:52:35.000000 sparta-pubsub-0.0.2/src/sparta/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:53:00.953648 sparta-pubsub-0.0.2/src/sparta/pubsub/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-10 11:52:35.000000 sparta-pubsub-0.0.2/src/sparta/pubsub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-06-10 11:52:35.000000 sparta-pubsub-0.0.2/src/sparta/pubsub/consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-06-10 11:52:35.000000 sparta-pubsub-0.0.2/src/sparta/pubsub/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:53:00.953648 sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-10 11:53:00.000000 sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2023-06-10 11:53:00.000000 sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 11:53:00.000000 sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 11:53:00.000000 sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-10 11:53:00.000000 sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 11:53:00.000000 sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/top_level.txt
```

### Comparing `sparta-pubsub-0.0.1/LICENSE` & `sparta-pubsub-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparta-pubsub-0.0.1/PKG-INFO` & `sparta-pubsub-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-pubsub
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sparta pubsub library
 Home-page: https://github.com/Spartan-Approach/sparta-pubsub
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparta-pubsub-0.0.1/README.md` & `sparta-pubsub-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sparta-pubsub-0.0.1/setup.py` & `sparta-pubsub-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sparta-pubsub-0.0.1/src/sparta/pubsub/consumer.py` & `sparta-pubsub-0.0.2/src/sparta/pubsub/consumer.py`

 * *Files identical despite different names*

### Comparing `sparta-pubsub-0.0.1/src/sparta/pubsub/publisher.py` & `sparta-pubsub-0.0.2/src/sparta/pubsub/publisher.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,28 @@
         publisher_options = pubsub_v1.types.PublisherOptions(
             enable_message_ordering=enable_message_ordering
         )
         self.publisher = pubsub_v1.PublisherClient(publisher_options=publisher_options)
         self.topic_path = self.publisher.topic_path(project_id, topic_id)
         self._logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
 
+    def publish_and_wait_for_message_id(self, data: bytes, ordering_key=None, **attrs):
+        future = self._publish(data, ordering_key, **attrs)
+        message_id = future.result()
+        self._logger.debug(f"Published data={data} > message_id={message_id} ")
+        return message_id
+
     def publish(self, data: bytes, ordering_key=None, **attrs):
+        future = self._publish(data, ordering_key, **attrs)
+        self._logger.debug(f"Published data={data}")
+        return future
+
+    def _publish(self, data: bytes, ordering_key=None, **attrs):
         _attrs = {
             k: v for k, v in attrs.items() if v is not None and isinstance(v, str)
         }
-        future = self.publisher.publish(
+        return self.publisher.publish(
             topic=self.topic_path,
             data=data,
             ordering_key=ordering_key if ordering_key else "",
             **_attrs,
         )
-        message_id = future.result()
-        self._logger.debug(f"Published message_id={message_id} data={data}")
-        return message_id
```

### Comparing `sparta-pubsub-0.0.1/src/sparta_pubsub.egg-info/PKG-INFO` & `sparta-pubsub-0.0.2/src/sparta_pubsub.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-pubsub
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sparta pubsub library
 Home-page: https://github.com/Spartan-Approach/sparta-pubsub
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

