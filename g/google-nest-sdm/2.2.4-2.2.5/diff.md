# Comparing `tmp/google_nest_sdm-2.2.4.tar.gz` & `tmp/google_nest_sdm-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_nest_sdm-2.2.4.tar", last modified: Wed Jan 25 06:25:53 2023, max compression
+gzip compressed data, was "google_nest_sdm-2.2.5.tar", last modified: Sat Jun 10 15:14:03 2023, max compression
```

## Comparing `google_nest_sdm-2.2.4.tar` & `google_nest_sdm-2.2.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 06:25:53.935038 google_nest_sdm-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-01-25 06:25:53.935038 google_nest_sdm-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 06:25:53.931038 google_nest_sdm-2.2.4/google_nest_sdm/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16859 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/device_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    36900 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/event_media.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/google_nest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/google_nest_sdm/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 06:25:53.935038 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-01-25 06:25:53.000000 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-25 06:25:53.000000 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 06:25:53.000000 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-25 06:25:53.000000 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 06:25:53.000000 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-25 06:25:53.000000 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-25 06:25:53.000000 google_nest_sdm-2.2.4/google_nest_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-25 06:25:53.935038 google_nest_sdm-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-25 06:25:45.000000 google_nest_sdm-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:03.781548 google_nest_sdm-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-10 15:14:03.777548 google_nest_sdm-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:03.777548 google_nest_sdm-2.2.5/google_nest_sdm/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32092 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/event_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/google_nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/google_nest_sdm/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:03.777548 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-10 15:14:03.000000 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-10 15:14:03.000000 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 15:14:03.000000 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-10 15:14:03.000000 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 15:14:03.000000 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 15:14:03.000000 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-10 15:14:03.000000 google_nest_sdm-2.2.5/google_nest_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 15:14:03.781548 google_nest_sdm-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-10 15:13:53.000000 google_nest_sdm-2.2.5/setup.py
```

### Comparing `google_nest_sdm-2.2.4/LICENSE` & `google_nest_sdm-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/PKG-INFO` & `google_nest_sdm-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 2.2.4
+Version: 2.2.5
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google-nest-sdm
 Author: Allen Porter
 Author-email: allen@thebends.org
 Keywords: google nest sdm camera therostat security doorbell
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `google_nest_sdm-2.2.4/README.md` & `google_nest_sdm-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/auth.py` & `google_nest_sdm-2.2.5/google_nest_sdm/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             raise ApiException(": ".join(detail)) from err
         except ClientError as err:
             raise ApiException(f"Error from API: {err}") from err
         return resp
 
     @staticmethod
     async def _error_detail(resp: aiohttp.ClientResponse) -> List[str]:
-        """Resturns an error message string from the APi response."""
+        """Returns an error message string from the APi response."""
         if resp.status < 400:
             return []
         try:
             result = await resp.json()
             error = result.get(ERROR, {})
         except ClientError:
             return []
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/camera_traits.py` & `google_nest_sdm-2.2.5/google_nest_sdm/camera_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import datetime
 import logging
 import urllib.parse as urlparse
 from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from enum import Enum
 from typing import Any, List, Mapping, Optional, cast
 
 from .event import (
     CameraClipPreviewEvent,
     CameraMotionEvent,
     CameraPersonEvent,
@@ -41,14 +42,15 @@
 EXPIRES_AT = "expiresAt"
 ANSWER_SDP = "answerSdp"
 MEDIA_SESSION_ID = "mediaSessionId"
 
 EVENT_IMAGE_CLIP_PREVIEW = "clip_preview"
 
 
+@dataclass
 class Resolution:
     """Maximum Resolution of an image or stream."""
 
     width: Optional[int] = None
     height: Optional[int] = None
 
 
@@ -160,15 +162,15 @@
     def __init__(self, data: Mapping[str, Any], cmd: Command):
         """Initialize RstpStream."""
         super().__init__(data)
         self._cmd = cmd
 
     @property
     def answer_sdp(self) -> str:
-        """An SDP answer to use with the local device dispalying the stream."""
+        """An SDP answer to use with the local device displaying the stream."""
         answer_sdp = self._data[ANSWER_SDP]
         assert isinstance(answer_sdp, str)
         return answer_sdp
 
     @property
     def media_session_id(self) -> str:
         """Media Session ID of the live stream."""
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/device.py` & `google_nest_sdm-2.2.5/google_nest_sdm/device.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/device_manager.py` & `google_nest_sdm-2.2.5/google_nest_sdm/device_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import Awaitable, Callable, Dict, Optional
 
 from .device import Device
 from .event import EventMessage, RelationUpdate
 from .event_media import CachePolicy
-from .structure import InfoTrait, RoomInfoTrait, Structure
+from .structure import Structure
 
 
 class DeviceManager:
     """DeviceManager holds current state of all devices."""
 
     def __init__(self, cache_policy: CachePolicy | None = None) -> None:
         """Initialize DeviceManager."""
@@ -70,17 +70,17 @@
             if device_id in self._devices:
                 device = self._devices[device_id]
                 await device.async_handle_event(event_message)
 
     def _structure_name(self, relation_subject: str) -> Optional[str]:
         if relation_subject in self._structures:
             structure = self._structures[relation_subject]
-            for trait_name in [InfoTrait.NAME, RoomInfoTrait.NAME]:
-                if trait_name in structure.traits:
-                    return structure.traits[trait_name].custom_name
+            for trait in [structure.info, structure.room_info]:
+                if trait and trait.custom_name:
+                    return trait.custom_name
         return "Unknown"
 
     def _handle_device_relation(self, relation: RelationUpdate) -> None:
         if relation.object not in self._devices:
             return
 
         device = self._devices[relation.object]
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/device_traits.py` & `google_nest_sdm-2.2.5/google_nest_sdm/device_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/diagnostics.py` & `google_nest_sdm-2.2.5/google_nest_sdm/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def __init__(self) -> None:
         """Initialize Diagnostics."""
         self._counter: Counter = Counter()
         self._subkeys: dict[str, Diagnostics] = {}
 
     def increment(self, key: str, count: int = 1) -> None:
-        """Increment a counter for the spcified key/event."""
+        """Increment a counter for the specified key/event."""
         self._counter.update(Counter({key: count}))
 
     def elapsed(self, key_prefix: str, elapsed_ms: int = 1) -> None:
         """Track a latency event for the specified key/event prefix."""
         self.increment(f"{key_prefix}_count", 1)
         self.increment(f"{key_prefix}_sum", elapsed_ms)
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/doorbell_traits.py` & `google_nest_sdm-2.2.5/google_nest_sdm/doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/event.py` & `google_nest_sdm-2.2.5/google_nest_sdm/event.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,35 +8,32 @@
 import hashlib
 import json
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Dict, Iterable, Mapping, Optional
 
+from pydantic import BaseModel, Field, root_validator, validate_arguments, validator
+
 from .auth import AbstractAuth
 from .diagnostics import EVENT_DIAGNOSTICS as DIAGNOSTICS
 from .exceptions import DecodeException
 from .registry import Registry
 from .traits import BuildTraits, Command
-from .typing import cast_assert, cast_optional
+from .typing import cast_assert
 
 EVENT_ID = "eventId"
 EVENT_SESSION_ID = "eventSessionId"
 TIMESTAMP = "timestamp"
 RESOURCE_UPDATE = "resourceUpdate"
 NAME = "name"
 TRAITS = "traits"
 EVENTS = "events"
-RELATION_UPDATE = "relationUpdate"
-TYPE = "type"
-SUBJECT = "subject"
-OBJECT = "object"
 PREVIEW_URL = "previewUrl"
 ZONES = "zones"
-EVENT_THREAD_STATE = "eventThreadState"
 EVENT_THREAD_STATE_ENDED = "ENDED"
 
 # Event images expire 30 seconds after the event is published
 EVENT_IMAGE_EXPIRE_SECS = 30
 
 # Camera clip previews don't list an expiration in the API. Lets say 15 minutes
 # as an arbitrary number for now.
@@ -47,32 +44,23 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 class EventProcessingError(Exception):
     """Raised when there was an error handling an event."""
 
 
+@dataclass
 class EventImageContentType:
     """Event image content type."""
 
-    def __init__(self, content_type: str) -> None:
-        """Initialize EventImageContentType."""
-        self._content_type = content_type
+    content_type: str
 
     def __str__(self) -> str:
         """Return a string representation of the event image type."""
-        return self._content_type
-
-    def __repr__(self) -> str:
-        return "<EventImageContentType %s>" % self._content_type
-
-    @property
-    def content_type(self) -> str:
-        """Return the content type of the image."""
-        return self._content_type
+        return self.content_type
 
 
 class EventImageType:
     IMAGE = EventImageContentType("image/jpeg")
     CLIP_PREVIEW = EventImageContentType("video/mp4")
     IMAGE_PREVIEW = EventImageContentType("image/gif")
 
@@ -89,16 +77,16 @@
             return EventImageContentType(content_type)
 
 
 @dataclass
 class EventToken:
     """Identifier for a unique event."""
 
-    event_session_id: str
-    event_id: str
+    event_session_id: str = Field(alias="eventSessionId")
+    event_id: str = Field(alias="eventId")
 
     def encode(self) -> str:
         """Encode the event token as a serialized string."""
         data = [self.event_session_id, self.event_id]
         b = json.dumps(data).encode("utf-8")
         return base64.b64encode(b).decode("utf-8")
 
@@ -159,15 +147,15 @@
     @property
     def event_session_id(self) -> str:
         """ID used to associate separate messages with a single event."""
         return cast_assert(str, self._data[EVENT_SESSION_ID])
 
     @property
     def timestamp(self) -> datetime.datetime:
-        """Timestap when the event occurred."""
+        """Timestamp when the event occurred."""
         return self._timestamp
 
     @property
     def expires_at(self) -> datetime.datetime:
         """Timestamp when the message expires."""
         return self._timestamp + datetime.timedelta(seconds=EVENT_IMAGE_EXPIRE_SECS)
 
@@ -306,48 +294,38 @@
         if not self._last_event:
             return None
         if self._last_event.is_expired:
             return None
         return self._last_event
 
     def handle_event(self, event: ImageEventBase) -> None:
-        """Recieve an event message."""
+        """Receive an event message."""
         self._last_event = event
 
 
-class RelationUpdate:
+class RelationUpdate(BaseModel):
     """Represents a relational update for a resource."""
 
-    def __init__(self, raw_data: Mapping[str, Any]):
-        """Initialize the RelationUpdate."""
-        self._raw_data = raw_data
+    type: str
+    """Type of relation event 'CREATED', 'UPDATED', 'DELETED'."""
 
-    @property
-    def type(self) -> str:
-        """Type of relation event 'CREATED', 'UPDATED', 'DELETED'."""
-        return cast_assert(str, self._raw_data[TYPE])
+    subject: str
+    """Resource that the object is now in relation with."""
 
-    @property
-    def subject(self) -> str:
-        """Resource that the object is now in relation with."""
-        return cast_assert(str, self._raw_data.get(SUBJECT))
-
-    @property
-    def object(self) -> str:
-        """Resource that triggered the event."""
-        return cast_assert(str, self._raw_data[OBJECT])
+    object: str
+    """Resource that triggered the event."""
 
 
 def _BuildEvents(
     events: Mapping[str, Any],
     timestamp: datetime.datetime,
 ) -> Dict[str, ImageEventBase]:
     """Build a trait map out of a response dict."""
     result = {}
-    for (event_type, event_data) in events.items():
+    for event_type, event_data in events.items():
         image_event = _BuildEvent(event_type, event_data, timestamp)
         if not image_event:
             continue
         result[event_type] = image_event
     return result
 
 
@@ -364,109 +342,111 @@
     """Determine the event type to use based on the events in the session."""
     for event in events:
         if event.event_image_type != EventImageType.IMAGE:
             return event.event_image_type
     return EventImageType.IMAGE
 
 
-class EventMessage:
+@validate_arguments
+def _validate_datetime(value: datetime.datetime) -> datetime.datetime:
+    return value
+
+
+class EventMessage(BaseModel):
     """Event for a change in trait value or device action."""
 
-    def __init__(self, raw_data: Mapping[str, Any], auth: AbstractAuth):
+    event_id: str = Field(alias="eventId")
+    timestamp: datetime.datetime
+    resource_update_name: Optional[str]
+    resource_update_events: Optional[dict[str, ImageEventBase]]
+    resource_update_traits: Optional[dict[str, Any]]
+    event_thread_state: Optional[str] = Field(alias="eventThreadState")
+    relation_update: Optional[RelationUpdate] = Field(alias="relationUpdate")
+
+    def __init__(self, raw_data: Mapping[str, Any], auth: AbstractAuth) -> None:
         """Initialize an EventMessage."""
         _LOGGER.debug("EventMessage raw_data=%s", raw_data)
-        self._raw_data = raw_data
+        super().__init__(**raw_data, auth=auth)
         self._auth = auth
 
-    @property
-    def event_id(self) -> Optional[str]:
-        """Event identifier."""
-        return self._raw_data.get(EVENT_ID)
-
-    @property
-    def timestamp(self) -> datetime.datetime:
-        """Time when the event was published."""
-        event_timestamp = self._raw_data[TIMESTAMP]
-        return datetime.datetime.fromisoformat(event_timestamp.replace("Z", "+00:00"))
-
-    @property
-    def resource_update_name(self) -> Optional[str]:
-        """Return the id of the device that was updated."""
-        if RESOURCE_UPDATE not in self._raw_data:
-            return None
-        return cast_optional(str, self._raw_data[RESOURCE_UPDATE].get(NAME))
-
-    @property
-    def resource_update_events(self) -> Optional[Dict[str, ImageEventBase]]:
-        """Return the set of events that happened."""
-        if RESOURCE_UPDATE not in self._raw_data:
-            return None
-        events = self._raw_data[RESOURCE_UPDATE].get(EVENTS, {})
-        assert isinstance(events, dict)
-        return _BuildEvents(events, self.timestamp)
+    @root_validator(pre=True)
+    def _parse_resource_update(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Parse resource updates."""
+        if update := values.get(RESOURCE_UPDATE):
+            if name := update.get(NAME):
+                values["resource_update_name"] = name
+            if events := update.get(EVENTS):
+                values["resource_update_events"] = events
+                values["resource_update_events"][TIMESTAMP] = values.get(TIMESTAMP)
+            if traits := update.get(TRAITS):
+                values["resource_update_traits"] = traits
+                values["resource_update_traits"][NAME] = update.get(NAME)
+                values["resource_update_traits"]["auth"] = values["auth"]
+        return values
+
+    @validator("resource_update_events", pre=True)
+    def _parse_resource_update_events(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Parse resource updates for events."""
+        return _BuildEvents(values, _validate_datetime(values[TIMESTAMP]))
+
+    @validator("resource_update_traits", pre=True)
+    def _parse_resource_update_traits(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Parse resource updates to traits."""
+        cmd = Command(values[NAME], values["auth"], DIAGNOSTICS)
+        return BuildTraits(values, cmd)
 
     @property
     def event_sessions(self) -> Optional[dict[str, dict[str, ImageEventBase]]]:
         events = self.resource_update_events
         if not events:
             return None
         event_sessions: dict[str, dict[str, ImageEventBase]] = {}
-        for (event_name, event) in events.items():
+        for event_name, event in events.items():
             d = event_sessions.get(event.event_session_id, {})
             d[event_name] = event
             event_sessions[event.event_session_id] = d
         # Build associations between all events
         for event_session_id, event_dict in event_sessions.items():
             event_image_type = session_event_image_type(events.values())
             for event_type, event in event_dict.items():
                 event.session_events = list(event_dict.values())
                 event.event_image_type = event_image_type
         return event_sessions
 
     @property
-    def resource_update_traits(self) -> Optional[dict]:
-        """Return the set of traits that were updated."""
-        if not self.resource_update_name:
-            return None
-        cmd = Command(self.resource_update_name, self._auth, DIAGNOSTICS)
-        events = self._raw_data[RESOURCE_UPDATE].get(TRAITS, {})
-        return BuildTraits(events, cmd)
-
-    @property
-    def relation_update(self) -> Optional[RelationUpdate]:
-        """Represent a relational update for a resource."""
-        if RELATION_UPDATE not in self._raw_data:
-            return None
-        return RelationUpdate(self._raw_data[RELATION_UPDATE])
-
-    @property
     def raw_data(self) -> Dict[str, Any]:
         """Return raw data for the event."""
-        return dict(self._raw_data)
+        return self.dict()
 
     def with_events(
         self,
         event_keys: Iterable[str],
         merge_data: dict[str, ImageEventBase] | None = None,
     ) -> EventMessage:
         """Create a new EventMessage minus some existing events by key."""
-        raw_data = dict(self._raw_data)
+        new_message = self.copy()
         if not merge_data:
             merge_data = {}
-        existing = self._raw_data[RESOURCE_UPDATE][EVENTS]
-        result = {}
+        new_events = {}
         for key in event_keys:
-            if key in existing:
-                result[key] = existing[key]
-            elif key in merge_data:
-                result[key] = merge_data[key].as_dict()["event_data"]
-        raw_data[RESOURCE_UPDATE][EVENTS] = result
-        return EventMessage(raw_data, self._auth)
+            if (
+                new_message.resource_update_events
+                and key in new_message.resource_update_events
+            ):
+                new_events[key] = new_message.resource_update_events[key]
+            elif merge_data and key in merge_data:
+                new_events[key] = merge_data[key]
+        new_message.resource_update_events = new_events
+        return new_message
 
     @property
     def is_thread_ended(self) -> bool:
         """Return true if the message indicates the thread is ended."""
-        return self._raw_data.get(EVENT_THREAD_STATE) == EVENT_THREAD_STATE_ENDED
+        return self.event_thread_state == EVENT_THREAD_STATE_ENDED
 
     def __repr__(self) -> str:
         """Debug information."""
         return f"EventMessage{self.raw_data}"
+
+    class Config:
+        arbitrary_types_allowed = True
+        extra = "allow"
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/exceptions.py` & `google_nest_sdm-2.2.5/google_nest_sdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/google_nest.py` & `google_nest_sdm-2.2.5/google_nest_sdm/google_nest.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/google_nest_api.py` & `google_nest_sdm-2.2.5/google_nest_sdm/google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/google_nest_subscriber.py` & `google_nest_sdm-2.2.5/google_nest_sdm/google_nest_subscriber.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import re
 import time
 from abc import ABC, abstractmethod
 from typing import Awaitable, Callable, Optional
 
 from aiohttp.client_exceptions import ClientError
 from google.api_core.exceptions import GoogleAPIError, NotFound, Unauthenticated
-from google.auth.exceptions import RefreshError
+from google.auth.exceptions import RefreshError, GoogleAuthError, TransportError
 from google.auth.transport.requests import Request
 from google.cloud import pubsub_v1
 from google.oauth2.credentials import Credentials
 from google.protobuf.duration_pb2 import Duration
 
 from .auth import AbstractAuth
 from .device_manager import DeviceManager
@@ -115,14 +115,34 @@
         raise ConfigurationException(
             "Subscription misconfigured. Expected topic name to "
             f"match '{EXPECTED_TOPIC_REGEXP.pattern}' but was "
             f"'{topic_name}'."
         )
 
 
+def refresh_creds(creds: Credentials) -> Credentials:
+    """Refresh credentials.
+
+    This is not part of the subscriber API, exposed only to facilitate testing.
+    """
+    try:
+        creds.refresh(Request())
+    except RefreshError as err:
+        raise AuthException(f"Authentication refresh failure: {err}") from err
+    except TransportError as err:
+        raise SubscriberException(
+            f"Connectivity error during authentication refresh: {err}"
+        ) from err
+    except GoogleAuthError as err:
+        raise SubscriberException(
+            f"Error during authentication refresh: {err}"
+        ) from err
+    return creds
+
+
 class AbstractSubscriberFactory(ABC):
     """Abstract class for creating a subscriber, to facilitate testing."""
 
     @abstractmethod
     async def async_create_subscription(
         self,
         creds: Credentials,
@@ -228,15 +248,15 @@
 
     def _delete_subscription(
         self,
         creds: Credentials,
         subscription_name: str,
     ) -> None:
         """Deletes a subscription."""
-        creds = self._refresh_creds(creds)
+        creds = refresh_creds(creds)
         subscriber = pubsub_v1.SubscriberClient(credentials=creds)
         _LOGGER.debug(f"Deleting subscription '{subscription_name}'")
         subscriber.delete_subscription(subscription=subscription_name)
 
     async def async_new_subscriber(
         self,
         creds: Credentials,
@@ -261,30 +281,22 @@
                 executor,
                 self._new_subscriber,
                 creds,
                 subscription_name,
                 callback_wrapper,
             )
 
-    def _refresh_creds(self, creds: Credentials) -> Credentials:
-        """Refresh credentials."""
-        try:
-            creds.refresh(Request())
-        except RefreshError as err:
-            raise AuthException(f"Access token failure: {err}") from err
-        return creds
-
     def _new_subscriber(
         self,
         creds: Credentials,
         subscription_name: str,
         callback_wrapper: Callable[[pubsub_v1.subscriber.message.Message], None],
     ) -> pubsub_v1.subscriber.futures.StreamingPullFuture:
         """Issue a command to verify subscriber creds are correct."""
-        creds = self._refresh_creds(creds)
+        creds = refresh_creds(creds)
         subscriber = pubsub_v1.SubscriberClient(credentials=creds)
         subscription = subscriber.get_subscription(subscription=subscription_name)
         if subscription.topic:
             _validate_topic_name(subscription.topic)
             _LOGGER.debug(
                 "Subscriber '%s' configured on topic '%s'",
                 subscription_name,
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/registry.py` & `google_nest_sdm-2.2.5/google_nest_sdm/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Decorator for creating a registry of objects."""
 
+from __future__ import annotations
+
 from typing import Callable, TypeVar
 
 CALLABLE_T = TypeVar("CALLABLE_T", bound=Callable)  # pylint: disable=invalid-name
 
 
 class Registry(dict):
     """Registry of items."""
 
-    def register(self) -> Callable[[CALLABLE_T], CALLABLE_T]:
+    def register(self, name: str | None = None) -> Callable[[CALLABLE_T], CALLABLE_T]:
         """Return decorator to register item with a specific name."""
 
         def decorator(func: CALLABLE_T) -> CALLABLE_T:
             """Register decorated function."""
-            self[func.NAME] = func  # type: ignore
+            nonlocal name
+            if name is None:
+                name = func.NAME  # type: ignore
+            self[name] = func
             return func
 
         return decorator
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/thermostat_traits.py` & `google_nest_sdm-2.2.5/google_nest_sdm/thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/traits.py` & `google_nest_sdm-2.2.5/google_nest_sdm/traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/transcoder.py` & `google_nest_sdm-2.2.5/google_nest_sdm/transcoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     async def transcode_clip(self, input_file: str, output_file: str) -> None:
         """Create a image preview for a thumbnail clip."""
         full_input_file = f"{self._path_prefix}/{input_file}"
         full_output_file = f"{self._path_prefix}/{output_file}"
         if not os.path.exists(full_input_file):
             raise TranscodeException(f"Input file does not exist: {full_input_file}")
         if os.path.exists(full_output_file):
-            raise TranscodeException(f"Ouput file already exists: {full_output_file}")
+            raise TranscodeException(f"Output file already exists: {full_output_file}")
         cmd = " ".join(
             [
                 self._ffmpeg_binary,
                 "-y",
                 "-i",
                 full_input_file,
                 "-vf setpts=2.0*PTS",
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm/typing.py` & `google_nest_sdm-2.2.5/google_nest_sdm/typing.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm.egg-info/PKG-INFO` & `google_nest_sdm-2.2.5/google_nest_sdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-nest-sdm
-Version: 2.2.4
+Version: 2.2.5
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google-nest-sdm
 Author: Allen Porter
 Author-email: allen@thebends.org
 Keywords: google nest sdm camera therostat security doorbell
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `google_nest_sdm-2.2.4/google_nest_sdm.egg-info/SOURCES.txt` & `google_nest_sdm-2.2.5/google_nest_sdm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
-setup.cfg
 setup.py
 google_nest_sdm/__init__.py
 google_nest_sdm/auth.py
 google_nest_sdm/camera_traits.py
 google_nest_sdm/device.py
 google_nest_sdm/device_manager.py
 google_nest_sdm/device_traits.py
@@ -14,14 +13,15 @@
 google_nest_sdm/doorbell_traits.py
 google_nest_sdm/event.py
 google_nest_sdm/event_media.py
 google_nest_sdm/exceptions.py
 google_nest_sdm/google_nest.py
 google_nest_sdm/google_nest_api.py
 google_nest_sdm/google_nest_subscriber.py
+google_nest_sdm/model.py
 google_nest_sdm/py.typed
 google_nest_sdm/registry.py
 google_nest_sdm/structure.py
 google_nest_sdm/thermostat_traits.py
 google_nest_sdm/traits.py
 google_nest_sdm/transcoder.py
 google_nest_sdm/typing.py
```

### Comparing `google_nest_sdm-2.2.4/setup.py` & `google_nest_sdm-2.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 
 from setuptools import setup
 
-VERSION = "2.2.4"
+VERSION = "2.2.5"
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="google_nest_sdm",
     version=VERSION,
@@ -23,14 +23,15 @@
     install_requires=[
         "aiohttp>=3.7.3",
         "google-auth>=1.22.0",
         "google-auth-oauthlib>=0.4.1",
         "google-cloud-pubsub>=2.1.0",
         "requests-oauthlib>=1.3.0",
         "PyYAML>=6.0",
+        "pydantic>=1.10.4",
     ],
     python_requires=">=3.9",
     entry_points={
         "console_scripts": [
             "google_nest=google_nest_sdm.google_nest:main",
         ],
     },
```

