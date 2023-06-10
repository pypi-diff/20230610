# Comparing `tmp/pyobihai-1.4.1.tar.gz` & `tmp/pyobihai-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobihai-1.4.1.tar", last modified: Wed Mar 15 18:35:14 2023, max compression
+gzip compressed data, was "pyobihai-1.4.2.tar", last modified: Sat Jun 10 17:53:54 2023, max compression
```

## Comparing `pyobihai-1.4.1.tar` & `pyobihai-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:35:14.546576 pyobihai-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-15 18:35:05.000000 pyobihai-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-15 18:35:14.546576 pyobihai-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-15 18:35:05.000000 pyobihai-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:35:14.546576 pyobihai-1.4.1/pyobihai/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-03-15 18:35:05.000000 pyobihai-1.4.1/pyobihai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-15 18:35:05.000000 pyobihai-1.4.1/pyobihai/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-15 18:35:05.000000 pyobihai-1.4.1/pyobihai/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:35:14.546576 pyobihai-1.4.1/pyobihai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-15 18:35:14.000000 pyobihai-1.4.1/pyobihai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-15 18:35:14.000000 pyobihai-1.4.1/pyobihai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 18:35:14.000000 pyobihai-1.4.1/pyobihai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-15 18:35:14.000000 pyobihai-1.4.1/pyobihai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-15 18:35:14.000000 pyobihai-1.4.1/pyobihai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-15 18:35:05.000000 pyobihai-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 18:35:14.546576 pyobihai-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-15 18:35:05.000000 pyobihai-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:35:14.546576 pyobihai-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-15 18:35:05.000000 pyobihai-1.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-15 18:35:05.000000 pyobihai-1.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-15 18:35:05.000000 pyobihai-1.4.1/tests/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-03-15 18:35:05.000000 pyobihai-1.4.1/tests/test_pyobihai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:53:54.085068 pyobihai-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 17:53:44.000000 pyobihai-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-10 17:53:54.085068 pyobihai-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-10 17:53:44.000000 pyobihai-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:53:54.085068 pyobihai-1.4.2/pyobihai/
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-10 17:53:44.000000 pyobihai-1.4.2/pyobihai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-10 17:53:44.000000 pyobihai-1.4.2/pyobihai/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-10 17:53:44.000000 pyobihai-1.4.2/pyobihai/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:53:54.085068 pyobihai-1.4.2/pyobihai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-10 17:53:54.000000 pyobihai-1.4.2/pyobihai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-10 17:53:54.000000 pyobihai-1.4.2/pyobihai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:53:54.000000 pyobihai-1.4.2/pyobihai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 17:53:54.000000 pyobihai-1.4.2/pyobihai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-10 17:53:54.000000 pyobihai-1.4.2/pyobihai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-10 17:53:44.000000 pyobihai-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:53:54.085068 pyobihai-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-10 17:53:44.000000 pyobihai-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:53:54.085068 pyobihai-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-10 17:53:44.000000 pyobihai-1.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-10 17:53:44.000000 pyobihai-1.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-10 17:53:44.000000 pyobihai-1.4.2/tests/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-06-10 17:53:44.000000 pyobihai-1.4.2/tests/test_pyobihai.py
```

### Comparing `pyobihai-1.4.1/LICENSE` & `pyobihai-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobihai-1.4.1/PKG-INFO` & `pyobihai-1.4.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobihai
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python wrapper for Obihai
 Home-page: https://github.com/ejpenney/pyobihai
 Author: Emory Penney
 Author-email: treadstoneit@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyobihai-1.4.1/pyobihai/parsing.py` & `pyobihai-1.4.2/pyobihai/parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Obihai Result Parsers."""
 
 from datetime import datetime, timedelta, timezone
-from xml.etree.ElementTree import Element
+from xml.etree.ElementTree import Element  # nosec
 
 
 def parse_last_reboot(obj: Element) -> datetime:
     """Get Last Reboot."""
 
     for exc in obj.findall("./parameter[@name='UpTime']/value"):
         days = exc.attrib.get("current", "").split()[0]
         tstamp = datetime.strptime(exc.attrib.get("current", "").split()[2], "%H:%M:%S")
-        now = datetime.now(timezone.utc)
+        now = datetime.now(tz=timezone.utc)
         state = now - timedelta(
             days=float(days),
             hours=tstamp.hour,
             minutes=tstamp.minute,
             seconds=tstamp.second,
             microseconds=now.microsecond,
         )
```

### Comparing `pyobihai-1.4.1/pyobihai.egg-info/PKG-INFO` & `pyobihai-1.4.2/pyobihai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobihai
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python wrapper for Obihai
 Home-page: https://github.com/ejpenney/pyobihai
 Author: Emory Penney
 Author-email: treadstoneit@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyobihai-1.4.1/setup.py` & `pyobihai-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyobihai",
-    version="1.4.1",
+    version="1.4.2",
     author="Emory Penney",
     author_email="treadstoneit@gmail.com",
     description="A Python wrapper for Obihai",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ejpenney/pyobihai",
```

### Comparing `pyobihai-1.4.1/tests/const.py` & `pyobihai-1.4.2/tests/const.py`

 * *Files identical despite different names*

### Comparing `pyobihai-1.4.1/tests/test_pyobihai.py` & `pyobihai-1.4.2/tests/test_pyobihai.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Test pyobihai."""
 
 import datetime
 from typing import Callable
 from unittest.mock import MagicMock, patch
 
 import pytest
-from requests import RequestException
+from requests.exceptions import RequestException
 
 from pyobihai import PyObihai
 
 from . import MockResponse
 from .const import (
     FAILED_REQUEST,
     INBOUND_CALL_HTML,
@@ -25,21 +25,21 @@
 
 pytestmark = pytest.mark.usefixtures("mock_response")
 
 
 def test_get_line_state() -> None:
     """Test PyObihai.get_line_state"""
 
+    my_obi = PyObihai(*MOCK_LOGIN)
     with patch(_GET_REQUEST_PATCH, MagicMock(return_value=LINE_STATE_XML)):
-        my_obi = PyObihai(*MOCK_LOGIN)
         line_state = my_obi.get_line_state()
 
     assert line_state == {
-        "PHONE1 port": "On Hook",
-        "PHONE1 port last caller info": "15552345678",
+        "PHONE1 Port": "On Hook",
+        "PHONE1 Port last caller info": "15552345678",
     }
 
 
 @pytest.mark.parametrize(
     "to_call,expected_result",
     [
         pytest.param(PyObihai.get_device_mac, "9CADEF000000", id="get_device_mac"),
@@ -54,45 +54,83 @@
             id="get_software_version",
         ),
     ],
 )
 def test_get_status(to_call: Callable, expected_result: str) -> None:
     """Test PyObihai device info functions."""
 
-    with patch(_GET_REQUEST_PATCH, MagicMock(return_value=STATUS_XML)):
-        my_obi = PyObihai(*MOCK_LOGIN)
+    my_obi = PyObihai(*MOCK_LOGIN)
+    with patch(_GET_REQUEST_PATCH, MagicMock(return_value=STATUS_XML)) as mock_request:
         result = to_call(my_obi)
 
+    mock_request.assert_called_once()
     assert result == expected_result
 
+    # Verify we use the cache after querying.
+    mock_request.reset_mock()
+    cached_result = to_call(my_obi)
+    assert cached_result == expected_result
+    mock_request.assert_not_called()
+
+
+def test_get_status_from_cache() -> None:
+    """
+    Test PyObihai device info functions don't query the device if we have
+    (reasonably) up-to-date data.
+    """
+
+    my_obi = PyObihai(*MOCK_LOGIN)
+    my_obi._cached_status = STATUS_XML
+
+    with patch(_GET_REQUEST_PATCH, MagicMock()) as mock_request:
+        my_obi._get_device_info("Product Information", "HardwareVersion")
+
+    mock_request.assert_not_called()
+
+
+def test_get_status_cache_update() -> None:
+    """Test PyObihai device info functions update the cache after Obihai reboots."""
+
+    my_obi = PyObihai(*MOCK_LOGIN)
+    my_obi._cached_status = MockResponse("GARBAGE_DATA", 200)
+    my_obi._last_status_check = datetime.datetime.now(
+        tz=datetime.timezone.utc
+    ) - datetime.timedelta(hours=1)
+
+    with patch(_GET_REQUEST_PATCH, MagicMock(return_value=STATUS_XML)) as mock_request:
+        result = my_obi._get_device_info("Product Information", "HardwareVersion")
+
+    assert result == "1.4"
+    mock_request.assert_called()
+
 
 def test_get_state() -> None:
     """Test PyObihai.get_line_state"""
 
+    my_obi = PyObihai(*MOCK_LOGIN)
     with patch(_GET_REQUEST_PATCH, MagicMock(return_value=STATUS_XML)):
-        my_obi = PyObihai(*MOCK_LOGIN)
         status = my_obi.get_state()
 
     # I'm worried these could potentially not match up
-    now = datetime.datetime.now(datetime.timezone.utc)
+    now = datetime.datetime.now(tz=datetime.timezone.utc)
     last_reboot = now - datetime.timedelta(
         days=7,
         hours=0,
         minutes=28,
         seconds=58,
         microseconds=now.microsecond,
     )
 
     assert status == {
-        "Reboot required": "false",
-        "Last reboot": last_reboot,
-        "SP1 service status": "0",
-        "SP2 service status": "0",
-        "SP4 service status": "0",
-        "OBiTALK service status": "Normal",
+        "Reboot Required": "false",
+        "Last Reboot": last_reboot,
+        "SP1 Service Status": "0",
+        "SP2 Service Status": "0",
+        "SP4 Service Status": "0",
+        "OBiTALK Service Status": "Normal",
     }
 
 
 @pytest.mark.parametrize(
     "to_call,response,expected_result",
     [
         pytest.param(
@@ -106,32 +144,32 @@
 def test_services(
     to_call: Callable,
     response: MockResponse,
     expected_result: bool,
 ) -> None:
     """Test PyObihai services functions."""
 
+    my_obi = PyObihai(*MOCK_LOGIN)
     with patch("pyobihai.requests.get", MagicMock(return_value=response)):
-        my_obi = PyObihai(*MOCK_LOGIN)
         result = to_call(my_obi)
 
     assert result == expected_result
 
 
 def test_failed_get_request() -> None:
     """Test PyObihai._get_request() logs an error."""
 
     side_effect = RequestException("Failure")
-    with patch("pyobihai.requests.get", side_effect=side_effect):
-        with patch("pyobihai.LOGGER.error") as logger:
-            my_obi = PyObihai(*MOCK_LOGIN)
-            result = my_obi._get_request("testing")
+    with pytest.raises(RequestException):
+        with patch("pyobihai.requests.get", side_effect=side_effect):
+            with patch("pyobihai.LOGGER.debug") as logger:
+                my_obi = PyObihai(*MOCK_LOGIN)
+                my_obi._get_request("testing")
 
-    logger.assert_called_once_with(side_effect)
-    assert result is False
+    logger.assert_called_with(side_effect)
 
 
 def test_non_admin_user() -> None:
     """Test PyObihai generates a user URL."""
 
     my_obi = PyObihai("192.168.1.100", "user", "password")
     assert my_obi._server.endswith("/user/")
@@ -144,12 +182,12 @@
         pytest.param(INBOUND_CALL_HTML, "Inbound Call", id="inbound_call"),
         pytest.param(OUTBOUND_CALL_HTML, "Outbound Call", id="outbound_call"),
     ],
 )
 def test_get_call_direction(response: MockResponse, expected_result: str) -> None:
     """Test PyObihai call direction lookup."""
 
+    my_obi = PyObihai(*MOCK_LOGIN)
     with patch(_GET_REQUEST_PATCH, MagicMock(return_value=response)):
-        my_obi = PyObihai(*MOCK_LOGIN)
         result = my_obi.get_call_direction()
 
-    assert result == {"Call direction": expected_result}
+    assert result == {"Call Direction": expected_result}
```

