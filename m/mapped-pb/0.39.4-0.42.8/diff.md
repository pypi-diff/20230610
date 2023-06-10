# Comparing `tmp/mapped_pb-0.39.4.tar.gz` & `tmp/mapped_pb-0.42.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapped_pb-0.39.4.tar", max compression
+gzip compressed data, was "mapped_pb-0.42.8.tar", max compression
```

## Comparing `mapped_pb-0.39.4.tar` & `mapped_pb-0.42.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       41 2023-05-15 18:12:26.686784 mapped_pb-0.39.4/README.md
--rw-r--r--   0        0        0        0 2023-05-15 18:12:39.423076 mapped_pb-0.39.4/mapped_pb/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 18:12:39.423076 mapped_pb-0.39.4/mapped_pb/cloud/__init__.py
--rw-r--r--   0        0        0    21055 2023-05-15 18:12:39.423076 mapped_pb-0.39.4/mapped_pb/cloud/types/__init__.py
--rw-r--r--   0        0        0     1540 2023-05-15 18:12:39.423076 mapped_pb-0.39.4/mapped_pb/cloud/types/calendar_period_pb2.py
--rw-r--r--   0        0        0     1377 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/date_pb2.py
--rw-r--r--   0        0        0     1554 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/dayofweek_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/geojson_pb2.py
--rw-r--r--   0        0        0     1546 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/interval_pb2.py
--rw-r--r--   0        0        0     2209 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/metadata_pb2.py
--rw-r--r--   0        0        0     1382 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/money_pb2.py
--rw-r--r--   0        0        0     1629 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/month_pb2.py
--rw-r--r--   0        0        0     1719 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/phone_number_pb2.py
--rw-r--r--   0        0        0     1909 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/postal_address_pb2.py
--rw-r--r--   0        0        0     1484 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/timeofday_pb2.py
--rw-r--r--   0        0        0     7205 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/cloud/types/typed_value_pb2.py
--rw-r--r--   0        0        0     5913 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/gateway/__init__.py
--rw-r--r--   0        0        0     3579 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/gateway/edgecontrol_pb2.py
--rw-r--r--   0        0        0     1856 2023-05-15 18:12:39.427076 mapped_pb-0.39.4/mapped_pb/gateway/redispoint_pb2.py
--rw-r--r--   0        0        0      616 2023-05-15 18:12:49.291305 mapped_pb-0.39.4/pyproject.toml
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 mapped_pb-0.39.4/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-06-10 05:47:28.673032 mapped_pb-0.42.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/__init__.py
+-rw-r--r--   0        0        0    21055 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/__init__.py
+-rw-r--r--   0        0        0     1540 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/calendar_period_pb2.py
+-rw-r--r--   0        0        0     1377 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/date_pb2.py
+-rw-r--r--   0        0        0     1554 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/dayofweek_pb2.py
+-rw-r--r--   0        0        0     1347 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/geojson_pb2.py
+-rw-r--r--   0        0        0     1546 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/interval_pb2.py
+-rw-r--r--   0        0        0     2209 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/metadata_pb2.py
+-rw-r--r--   0        0        0     1382 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/money_pb2.py
+-rw-r--r--   0        0        0     1629 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/month_pb2.py
+-rw-r--r--   0        0        0     1719 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/phone_number_pb2.py
+-rw-r--r--   0        0        0     1909 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/postal_address_pb2.py
+-rw-r--r--   0        0        0     1484 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/timeofday_pb2.py
+-rw-r--r--   0        0        0     7205 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/typed_value_pb2.py
+-rw-r--r--   0        0        0     6175 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/gateway/__init__.py
+-rw-r--r--   0        0        0     3579 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/gateway/edgecontrol_pb2.py
+-rw-r--r--   0        0        0     1914 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/gateway/redispoint_pb2.py
+-rw-r--r--   0        0        0      616 2023-06-10 05:47:51.729015 mapped_pb-0.42.8/pyproject.toml
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 mapped_pb-0.42.8/PKG-INFO
```

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/__init__.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/calendar_period_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/calendar_period_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/date_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/date_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/dayofweek_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/dayofweek_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/geojson_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/geojson_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/interval_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/interval_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/metadata_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/money_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/money_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/month_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/month_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/phone_number_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/phone_number_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/postal_address_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/postal_address_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/timeofday_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/timeofday_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/cloud/types/typed_value_pb2.py` & `mapped_pb-0.42.8/mapped_pb/cloud/types/typed_value_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/gateway/__init__.py` & `mapped_pb-0.42.8/mapped_pb/gateway/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,21 @@
     consecutive_network_error_count: int = betterproto.uint32_field(4)
     """
     A count of how many consecutive network errors have been observed since
     `network_error_start` A zero value (==0) here means there are there were no
     network errors in the last update to this point
     """
 
+    new_mapping_key: str = betterproto.string_field(5)
+    """
+    If this point has changed mappingKeys, likely because of an IP change, this
+    will contain the new mappingKey and last_update will be the timestamp of
+    when the mappingKey changed.
+    """
+
 
 class EdgeControlServiceStub(betterproto.ServiceStub):
     async def write_props(
         self,
         write_props_request: "WritePropsRequest",
         *,
         timeout: Optional[float] = None,
```

### Comparing `mapped_pb-0.39.4/mapped_pb/gateway/edgecontrol_pb2.py` & `mapped_pb-0.42.8/mapped_pb/gateway/edgecontrol_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.39.4/mapped_pb/gateway/redispoint_pb2.py` & `mapped_pb-0.42.8/mapped_pb/gateway/redispoint_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from mapped.cloud.types import typed_value_pb2 as mapped_dot_cloud_dot_types_dot_typed__value__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fmapped/gateway/redispoint.proto\x12\x0emapped.gateway\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$mapped/cloud/types/typed_value.proto\"\xa1\x02\n\nRedisPoint\x12\x43\n\rpresent_value\x18\x01 \x01(\x0b\x32\x1e.mapped.cloud.types.TypedValueR\x0cpresentValue\x12;\n\x0blast_update\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\nlastUpdate\x12J\n\x13network_error_start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11networkErrorStart\x12\x45\n\x1f\x63onsecutive_network_error_count\x18\x04 \x01(\rR\x1c\x63onsecutiveNetworkErrorCountBI\n\x12\x63om.mapped.gatewayP\x01Z go.mapped.dev/pb/gateway;gateway\xaa\x02\x0eMapped.Gatewayb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fmapped/gateway/redispoint.proto\x12\x0emapped.gateway\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$mapped/cloud/types/typed_value.proto\"\xc9\x02\n\nRedisPoint\x12\x43\n\rpresent_value\x18\x01 \x01(\x0b\x32\x1e.mapped.cloud.types.TypedValueR\x0cpresentValue\x12;\n\x0blast_update\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\nlastUpdate\x12J\n\x13network_error_start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11networkErrorStart\x12\x45\n\x1f\x63onsecutive_network_error_count\x18\x04 \x01(\rR\x1c\x63onsecutiveNetworkErrorCount\x12&\n\x0fnew_mapping_key\x18\x05 \x01(\tR\rnewMappingKeyBI\n\x12\x63om.mapped.gatewayP\x01Z go.mapped.dev/pb/gateway;gateway\xaa\x02\x0eMapped.Gatewayb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mapped.gateway.redispoint_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.mapped.gatewayP\001Z go.mapped.dev/pb/gateway;gateway\252\002\016Mapped.Gateway'
   _REDISPOINT._serialized_start=123
-  _REDISPOINT._serialized_end=412
+  _REDISPOINT._serialized_end=452
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mapped_pb-0.39.4/pyproject.toml` & `mapped_pb-0.42.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mapped.pb"
-version = "0.39.4"
+version = "0.42.8"
 description = "public Mapped Platform Service Definitions using protobuf"
 authors = ["Mapped <support@mapped.com>"]
 license = "Apache-2.0"
 homepage = "https://www.mapped.com"
 repository = "https://github.com/mapped/pb"
 keywords = ["mapped", "protobuf"]
 readme = "README.md"
```

### Comparing `mapped_pb-0.39.4/PKG-INFO` & `mapped_pb-0.42.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapped-pb
-Version: 0.39.4
+Version: 0.42.8
 Summary: public Mapped Platform Service Definitions using protobuf
 Home-page: https://www.mapped.com
 License: Apache-2.0
 Keywords: mapped,protobuf
 Author: Mapped
 Author-email: support@mapped.com
 Requires-Python: >=3.8,<4.0
```

