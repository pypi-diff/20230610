# Comparing `tmp/kr8s-0.4.1.tar.gz` & `tmp/kr8s-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.4.1.tar", max compression
+gzip compressed data, was "kr8s-0.5.0.tar", max compression
```

## Comparing `kr8s-0.4.1.tar` & `kr8s-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1549 2023-03-23 14:43:10.894081 kr8s-0.4.1/LICENSE
--rw-r--r--   0        0        0     2113 2023-04-24 13:00:16.267776 kr8s-0.4.1/README.md
--rw-r--r--   0        0        0      551 2023-05-24 13:50:46.605351 kr8s-0.4.1/kr8s/__init__.py
--rw-r--r--   0        0        0    10470 2023-05-24 13:50:04.093725 kr8s-0.4.1/kr8s/_api.py
--rw-r--r--   0        0        0     5250 2023-05-24 13:50:04.093725 kr8s-0.4.1/kr8s/_asyncio.py
--rw-r--r--   0        0        0     5854 2023-05-24 13:50:04.093725 kr8s-0.4.1/kr8s/_auth.py
--rw-r--r--   0        0        0      361 2023-04-04 19:30:47.872877 kr8s-0.4.1/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-04-27 12:49:41.923098 kr8s-0.4.1/kr8s/_exceptions.py
--rw-r--r--   0        0        0    24630 2023-05-24 13:50:04.097725 kr8s-0.4.1/kr8s/_objects.py
--rw-r--r--   0        0        0     7764 2023-05-24 13:50:04.097725 kr8s-0.4.1/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-05-24 13:50:04.097725 kr8s-0.4.1/kr8s/_testutils.py
--rw-r--r--   0        0        0       30 2023-05-10 09:14:38.833344 kr8s-0.4.1/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0      992 2023-05-24 13:50:04.097725 kr8s-0.4.1/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0      658 2023-05-05 12:16:31.343064 kr8s-0.4.1/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0       50 2023-04-30 18:57:48.474523 kr8s-0.4.1/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5575 2023-05-19 15:24:25.308428 kr8s-0.4.1/kr8s/conftest.py
--rw-r--r--   0        0        0     5739 2023-05-05 12:16:31.343064 kr8s-0.4.1/kr8s/objects.py
--rw-r--r--   0        0        0      157 2023-05-19 13:01:43.669318 kr8s-0.4.1/kr8s/portforward.py
--rw-r--r--   0        0        0       61 2023-03-31 20:28:17.436142 kr8s-0.4.1/kr8s/tests/resources/serviceaccount.yaml
--rwxr-xr-x   0        0        0      614 2023-04-03 16:55:51.155586 kr8s-0.4.1/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     4385 2023-05-24 13:50:04.097725 kr8s-0.4.1/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3144 2023-05-10 09:14:38.833344 kr8s-0.4.1/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      300 2023-04-04 19:30:47.872877 kr8s-0.4.1/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0    12439 2023-05-24 13:50:04.097725 kr8s-0.4.1/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-04-03 16:55:51.155586 kr8s-0.4.1/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2525 2023-05-24 13:50:46.605351 kr8s-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 kr8s-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-03-23 14:43:10.894081 kr8s-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2308 2023-06-10 19:46:29.901122 kr8s-0.5.0/README.md
+-rw-r--r--   0        0        0      551 2023-06-10 20:15:38.529821 kr8s-0.5.0/kr8s/__init__.py
+-rw-r--r--   0        0        0    10470 2023-06-10 19:46:29.905122 kr8s-0.5.0/kr8s/_api.py
+-rw-r--r--   0        0        0     5250 2023-06-10 19:46:29.905122 kr8s-0.5.0/kr8s/_asyncio.py
+-rw-r--r--   0        0        0     5854 2023-06-10 19:46:29.905122 kr8s-0.5.0/kr8s/_auth.py
+-rw-r--r--   0        0        0     1553 2023-06-10 19:46:29.909122 kr8s-0.5.0/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-04-27 12:49:41.923098 kr8s-0.5.0/kr8s/_exceptions.py
+-rw-r--r--   0        0        0    27605 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/_objects.py
+-rw-r--r--   0        0        0     7764 2023-06-10 19:46:29.909122 kr8s-0.5.0/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-06-10 19:46:29.913122 kr8s-0.5.0/kr8s/_testutils.py
+-rw-r--r--   0        0        0       30 2023-05-10 09:14:38.833344 kr8s-0.5.0/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-10 19:46:29.913122 kr8s-0.5.0/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0      685 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0       50 2023-04-30 18:57:48.474523 kr8s-0.5.0/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5575 2023-05-19 15:24:25.308428 kr8s-0.5.0/kr8s/conftest.py
+-rw-r--r--   0        0        0     5893 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/objects.py
+-rw-r--r--   0        0        0      157 2023-05-19 13:01:43.669318 kr8s-0.5.0/kr8s/portforward.py
+-rw-r--r--   0        0        0       61 2023-03-31 20:28:17.436142 kr8s-0.5.0/kr8s/tests/resources/serviceaccount.yaml
+-rwxr-xr-x   0        0        0      614 2023-04-03 16:55:51.155586 kr8s-0.5.0/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     4385 2023-06-10 19:46:29.913122 kr8s-0.5.0/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3144 2023-05-10 09:14:38.833344 kr8s-0.5.0/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      639 2023-06-10 19:46:29.917122 kr8s-0.5.0/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0    13951 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-04-03 16:55:51.155586 kr8s-0.5.0/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2577 2023-06-10 20:15:38.529821 kr8s-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 kr8s-0.5.0/PKG-INFO
```

### Comparing `kr8s-0.4.1/LICENSE` & `kr8s-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/README.md` & `kr8s-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 [![Test](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml/badge.svg)](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml)
 [![Codecov](https://img.shields.io/codecov/c/gh/kr8s-org/kr8s?logo=codecov&logoColor=ffffff)](https://app.codecov.io/gh/kr8s-org/kr8s)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kr8s-org/kr8s/main.svg)](https://results.pre-commit.ci/latest/github/kr8s-org/kr8s/main)
 [![Read the Docs](https://img.shields.io/readthedocs/kr8s?logo=readthedocs&logoColor=white)](https://kr8s.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kr8s)](https://pypi.org/project/kr8s/)
+[![Kubernetes Version Support](https://img.shields.io/badge/Kubernetes%20support-1.24%7C1.25%7C1.26%7C1.27-blue)](https://docs.kr8s.org/en/latest/installation.html#supported-kubernetes-versions)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - License](https://img.shields.io/pypi/l/kr8s)](https://pypi.org/project/kr8s/)
 
 > **Warning**
 > This is beta software and might not be ready for prime time.
 
 A Kubernetes API for Python
```

### Comparing `kr8s-0.4.1/kr8s/__init__.py` & `kr8s-0.5.0/kr8s/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ._api import ALL  # noqa
 from ._api import Api as _AsyncApi
 from ._asyncio import run_sync as _run_sync
 from ._asyncio import sync as _sync  # noqa
 from ._exceptions import NotFoundError  # noqa
 from .asyncio import api as _api  # noqa
 
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.4.1/kr8s/_api.py` & `kr8s-0.5.0/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/_asyncio.py` & `kr8s-0.5.0/kr8s/_asyncio.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/_auth.py` & `kr8s-0.5.0/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/_objects.py` & `kr8s-0.5.0/kr8s/_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 from __future__ import annotations
 
 import asyncio
 import json
+import re
 import time
-from typing import Any, Dict, List, Optional, Type
+from typing import Any, Dict, List, Optional, Type, Union
 
 import aiohttp
+import jsonpath
 from aiohttp import ClientResponse
+from async_timeout import timeout as async_timeout
 
 import kr8s
 import kr8s.asyncio
 from kr8s._api import Api
-from kr8s._data_utils import list_dict_unpack
+from kr8s._data_utils import dot_to_nested_dict, list_dict_unpack
 from kr8s._exceptions import NotFoundError
 from kr8s.asyncio.portforward import PortForward as AsyncPortForward
 from kr8s.portforward import PortForward as SyncPortForward
 
+JSONPATH_CONDITION_EXPRESSION = r"jsonpath='{(?P<expression>.*?)}'=(?P<condition>.*)"
+
 
 class APIObject:
     """Base class for Kubernetes objects."""
 
     namespaced = False
     scalable = False
     scalable_spec = "replicas"
@@ -105,15 +110,19 @@
         except KeyError:
             return {}
 
     @property
     def replicas(self) -> int:
         """Replicas of the Kubernetes resource."""
         if self.scalable:
-            return self.raw["spec"][self.scalable_spec]
+            keys = self.scalable_spec.split(".")
+            spec = self.raw["spec"]
+            for key in keys:
+                spec = spec[key]
+            return spec
         raise NotImplementedError(f"{self.kind} is not scalable")
 
     @classmethod
     async def get(
         cls,
         name: str,
         namespace: str = None,
@@ -227,16 +236,15 @@
             self.raw = await resp.json()
 
     async def scale(self, replicas: int = None) -> None:
         """Scale this object in Kubernetes."""
         if not self.scalable:
             raise NotImplementedError(f"{self.kind} is not scalable")
         await self._exists(ensure=True)
-        # TODO support dot notation in self.scalable_spec to support nested fields
-        await self._patch({"spec": {self.scalable_spec: replicas}})
+        await self._patch({"spec": dot_to_nested_dict(self.scalable_spec, replicas)})
         while self.replicas != replicas:
             await self._refresh()
             await asyncio.sleep(0.1)
 
     async def watch(self):
         """Watch this object in Kubernetes."""
         since = self.metadata.get("resourceVersion")
@@ -245,14 +253,58 @@
             namespace=self.namespace,
             field_selector=f"metadata.name={self.name}",
             since=since,
         ):
             self.raw = obj.raw
             yield event, self
 
+    async def _test_conditions(self, conditions: Union[List[str], str]) -> bool:
+        """Test if conditions are met."""
+        if isinstance(conditions, str):
+            conditions = [conditions]
+        for condition in conditions:
+            if condition.startswith("condition"):
+                condition = "=".join(condition.split("=")[1:])
+                if "=" in condition:
+                    field, value = condition.split("=")
+                    value = str(value)
+                else:
+                    field = condition
+                    value = str(True)
+                if value == "true" or value == "false":
+                    value = value.title()
+                status_conditions = list_dict_unpack(
+                    self.status.get("conditions", []), "type", "status"
+                )
+                if status_conditions.get(field, None) != value:
+                    return False
+            elif condition == "delete":
+                if await self._exists():
+                    return False
+            elif condition.startswith("jsonpath"):
+                matches = re.search(JSONPATH_CONDITION_EXPRESSION, condition)
+                expression = matches.group("expression")
+                condition = matches.group("condition")
+                [value] = jsonpath.findall(expression, self._raw)
+                if value != condition:
+                    return False
+            else:
+                raise ValueError(f"Unknown condition type {condition}")
+        return True
+
+    async def wait(self, conditions: list, timeout: int = None):
+        """Wait for conditions to be met."""
+        with async_timeout(timeout):
+            await self._refresh()
+            if await self._test_conditions(conditions):
+                return
+            async for _ in self.watch():
+                if await self._test_conditions(conditions):
+                    return
+
 
 ## v1 objects
 
 
 class Binding(APIObject):
     """A Kubernetes Binding."""
 
@@ -901,7 +953,34 @@
         A corresponding APIObject subclass instance.
 
     Raises:
         ValueError: If the resource kind or API version is not supported.
     """
     cls = get_class(spec["kind"], spec["apiVersion"])
     return cls(spec, api=api)
+
+
+async def object_from_name_type(
+    name: str, namespace: str = None, api: Api = None
+) -> APIObject:
+    """Create an APIObject from a Kubernetes resource name.
+
+    Args:
+        name: A Kubernetes resource name.
+
+    Returns:
+        A corresponding APIObject subclass instance.
+
+    Raises:
+        ValueError: If the resource kind or API version is not supported.
+    """
+    if "/" not in name:
+        raise ValueError(f"Invalid name: {name}. Expecting format of 'resource/name'.")
+    resource_type, name = name.split("/")
+    if "." in resource_type:
+        kind = resource_type.split(".")[0]
+        version = ".".join(resource_type.split(".")[1:])
+    else:
+        kind = resource_type
+        version = None
+    cls = get_class(kind, version)
+    return await cls.get(name, namespace=namespace, api=api)
```

### Comparing `kr8s-0.4.1/kr8s/_portforward.py` & `kr8s-0.5.0/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/_testutils.py` & `kr8s-0.5.0/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/asyncio/_api.py` & `kr8s-0.5.0/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/asyncio/objects.py` & `kr8s-0.5.0/kr8s/asyncio/objects.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,8 +31,9 @@
     Role,
     RoleBinding,
     Secret,
     Service,
     ServiceAccount,
     StatefulSet,
     Table,
+    object_from_name_type,
 )
```

### Comparing `kr8s-0.4.1/kr8s/conftest.py` & `kr8s-0.5.0/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/objects.py` & `kr8s-0.5.0/kr8s/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._asyncio import sync
+from ._asyncio import run_sync, sync
 from ._objects import (
     APIObject as _APIObject,
 )
 from ._objects import (
     Binding as _Binding,
 )
 from ._objects import (
@@ -103,17 +103,19 @@
 )
 from ._objects import (
     StatefulSet as _StatefulSet,
 )
 from ._objects import (
     Table as _Table,
 )
-from ._objects import (
-    object_from_spec,  # noqa
+from ._objects import (  # noqa
+    get_class,
+    object_from_spec,
 )
+from ._objects import object_from_name_type as _object_from_name_type
 
 
 @sync
 class APIObject(_APIObject):
     __doc__ = _APIObject.__doc__
     _asyncio = False
 
@@ -322,7 +324,10 @@
     _asyncio = False
 
 
 @sync
 class Table(_Table):
     __doc__ = _Table.__doc__
     _asyncio = False
+
+
+object_from_name_type = run_sync(_object_from_name_type)
```

### Comparing `kr8s-0.4.1/kr8s/tests/scripts/envexec.py` & `kr8s-0.5.0/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/tests/test_api.py` & `kr8s-0.5.0/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/tests/test_auth.py` & `kr8s-0.5.0/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/kr8s/tests/test_objects.py` & `kr8s-0.5.0/kr8s/tests/test_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import asyncio
 import time
 
 import aiohttp
 import pytest
 
 import kr8s
-from kr8s._objects import get_class, object_from_spec
 from kr8s.asyncio.objects import (
     APIObject,
     Deployment,
     PersistentVolume,
     Pod,
     Service,
+    object_from_name_type,
 )
 from kr8s.asyncio.portforward import PortForward
 from kr8s.objects import Pod as SyncPod
+from kr8s.objects import get_class, object_from_spec
 
 DEFAULT_TIMEOUT = aiohttp.ClientTimeout(30)
 
 
 @pytest.fixture
 async def nginx_pod(k8s_cluster, example_pod_spec):
     example_pod_spec["metadata"]["name"] = (
@@ -77,14 +78,43 @@
         await asyncio.sleep(0.1)
     await pod.delete()
     while await pod.exists():
         await asyncio.sleep(0.1)
     assert not await pod.exists()
 
 
+async def test_pod_object_from_name_type(example_pod_spec):
+    pod = await Pod(example_pod_spec)
+    await pod.create()
+    assert await pod.exists()
+    pod2 = await object_from_name_type(f"pod/{pod.name}", namespace=pod.namespace)
+    pod3 = await object_from_name_type(f"pod.v1/{pod.name}", namespace=pod.namespace)
+    assert pod2.name == pod.name
+    assert type(pod2) == type(pod)
+    assert pod3.name == pod.name
+    assert type(pod3) == type(pod)
+    await pod.delete()
+
+
+async def test_pod_wait_ready(example_pod_spec):
+    pod = await Pod(example_pod_spec)
+    await pod.create()
+    await pod.wait("condition=Ready")
+    with pytest.raises(asyncio.TimeoutError):
+        await pod.wait("jsonpath='{.status.phase}'=Foo", timeout=0.1)
+    await pod.wait("condition=Ready=true")
+    await pod.wait("condition=Ready=True")
+    await pod.wait("jsonpath='{.status.phase}'=Running")
+    with pytest.raises(ValueError):
+        await pod.wait("foo=NotARealCondition")
+    await pod.delete()
+    await pod.wait("condition=Ready=False")
+    await pod.wait("delete")
+
+
 def test_pod_create_and_delete_sync(example_pod_spec):
     pod = SyncPod(example_pod_spec)
     pod.create()
     with pytest.raises(NotImplementedError):
         pod.replicas
     assert pod.exists()
     while not pod.ready():
@@ -388,7 +418,22 @@
 
 async def test_unsupported_port_forward():
     pv = await PersistentVolume({})
     with pytest.raises(AttributeError):
         await pv.portforward(80)
     with pytest.raises(ValueError):
         await PortForward(pv, 80).start()
+
+
+async def test_scalable_dot_notation():
+    class Foo(APIObject):
+        version = "foo.kr8s.org/v1alpha1"
+        endpoint = "foos"
+        kind = "Foo"
+        plural = "foos"
+        singular = "foo"
+        namespaced = True
+        scalable = True
+        scalable_spec = "nested.replicas"
+
+    foo = await Foo({"metadata": {"name": "foo"}, "spec": {"nested": {"replicas": 1}}})
+    assert foo.replicas == 1
```

### Comparing `kr8s-0.4.1/kr8s/tests/test_testutils.py` & `kr8s-0.5.0/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.4.1/pyproject.toml` & `kr8s-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.4.1"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.5.0"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -34,14 +34,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.4"
 pyyaml = "^6.0"
 asyncio-atexit = "^1.0.1"
 aiofiles = "^23.1.0"
+python-jsonpath = "^0.7.1"
+async-timeout = "^4.0.2"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-kind = {git = "https://codeberg.org/hjacobs/pytest-kind.git"}
 pytest-timeout = "^2.1.0"
@@ -59,15 +61,15 @@
 sphinxcontrib-mermaid = "^0.8.1"
 sphinx-autoapi = "^2.1.0"
 
 [tool.pytest.ini_options]
 addopts = "-v --keep-cluster --durations=10 --cov=kr8s --cov-report term-missing --cov-report xml:coverage.xml"
 timeout = 300
 xfail_strict = true
-reruns = 5
+reruns = 1
 reruns_delay = 1
 asyncio_mode = "auto"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `kr8s-0.4.1/PKG-INFO` & `kr8s-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: async-timeout (>=4.0.2,<5.0.0)
 Requires-Dist: asyncio-atexit (>=1.0.1,<2.0.0)
+Requires-Dist: python-jsonpath (>=0.7.1,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 <div style="text-align: center; width: 100%;"><img src="branding/logo-wide.png" style="max-height: 200px;" /></div>
 
 [![Test](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml/badge.svg)](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml)
 [![Codecov](https://img.shields.io/codecov/c/gh/kr8s-org/kr8s?logo=codecov&logoColor=ffffff)](https://app.codecov.io/gh/kr8s-org/kr8s)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kr8s-org/kr8s/main.svg)](https://results.pre-commit.ci/latest/github/kr8s-org/kr8s/main)
 [![Read the Docs](https://img.shields.io/readthedocs/kr8s?logo=readthedocs&logoColor=white)](https://kr8s.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kr8s)](https://pypi.org/project/kr8s/)
+[![Kubernetes Version Support](https://img.shields.io/badge/Kubernetes%20support-1.24%7C1.25%7C1.26%7C1.27-blue)](https://docs.kr8s.org/en/latest/installation.html#supported-kubernetes-versions)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - License](https://img.shields.io/pypi/l/kr8s)](https://pypi.org/project/kr8s/)
 
 > **Warning**
 > This is beta software and might not be ready for prime time.
 
 A Kubernetes API for Python
```

