# Comparing `tmp/urllib3_ext_hface-0.3.0.tar.gz` & `tmp/urllib3_ext_hface-0.3.1.tar.gz`

## Comparing `urllib3_ext_hface-0.3.0.tar` & `urllib3_ext_hface-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,31 @@
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/dev-requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/changelog.rst
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/cli.rst
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/common.rst
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/conf.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/connections.rst
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/facade.rst
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/index.rst
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/install.rst
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/intro.rst
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/license.rst
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/protocols.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/_static/custom.css
--rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/_static/hface.png
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/_aioquic.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/helpers.py
--rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/test_http1.py
--rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/test_http2.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/NOTICE
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/dev-requirements.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/_aioquic.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/helpers.py
+-rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/test_http1.py
+-rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/test_http2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/NOTICE
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.3.0/CHANGELOG.rst` & `urllib3_ext_hface-0.3.1/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v0.3.1 (2023-06-10)
+-------------------
+
+* Allow passing extra config parameter for HTTP2Protocol through the factory.
+* Remove server-side code in the primary (h11) HTTP1Protocol.
+
 v0.3.0 (2023-06-03)
 -------------------
 
 * Breaking: Conception simplification. Remove HTTPFactories in favor of a single unified HTTPFactory.
 * Lazy import HTTPProtocol implementation.
 
 v0.2.12 (2023-05-25)
```

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,41 +37,49 @@
 class HTTPProtocolFactory(metaclass=ABCMeta):
     @staticmethod
     def new(
         type_protocol: type[HTTPProtocol],
         implementation: str | None = None,
         **kwargs: Any,
     ) -> HTTPOverQUICProtocol | HTTPOverTCPProtocol:
-        assert type_protocol != HTTPProtocol
+        """Create a new state-machine that target given protocol type."""
+        assert (
+            type_protocol != HTTPProtocol
+        ), "HTTPProtocol is ambiguous and cannot be requested in the factory."
 
         version_target: str = "".join(
             c
             for c in str(type_protocol).replace("urllib3_ext_hface", "")
             if c.isdigit()
         )
         module_expr: str = f".protocols.http{version_target}"
 
         if implementation:
             module_expr += f"._{implementation.lower()}"
 
-        http_module = importlib.import_module(
-            f".protocols.http{version_target}", "urllib3_ext_hface"
-        )
+        try:
+            http_module = importlib.import_module(module_expr, "urllib3_ext_hface")
+        except ImportError as e:
+            raise NotImplementedError(
+                f"{type_protocol} cannot be loaded. Tried to import '{module_expr}'."
+            ) from e
 
         implementations: list[
             tuple[str, type[HTTPOverQUICProtocol | HTTPOverTCPProtocol]]
         ] = inspect.getmembers(
             http_module,
             lambda e: isinstance(e, type)
             and issubclass(e, (HTTPOverQUICProtocol, HTTPOverTCPProtocol)),
         )
 
         if not implementations:
-            raise ImportError(
-                "Unable to instantiate a HTTPProtocol for given type target and implementation."
+            raise NotImplementedError(
+                f"{type_protocol} cannot be loaded. "
+                "No compatible implementation available. "
+                "Make sure your implementation inherit either from HTTPOverQUICProtocol or HTTPOverTCPProtocol."
             )
 
         implementation_target: type[
             HTTPOverQUICProtocol | HTTPOverTCPProtocol
         ] = implementations.pop()[1]
 
         return implementation_target(**kwargs)
```

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,27 @@
     @abstractmethod
     def bytes_to_send(self) -> bytes:
         """
         Returns data for sending out of the internal data buffer.
         """
         raise NotImplementedError
 
-
-class OverTCPProtocol(BaseProtocol):
-    """
-    Interface for sans-IO protocols on top TCP.
-    """
-
-    # Receiving direction
-
     @abstractmethod
     def connection_lost(self) -> None:
         """
         Called when the connection is lost or closed.
         """
         raise NotImplementedError
 
+
+class OverTCPProtocol(BaseProtocol):
+    """
+    Interface for sans-IO protocols on top TCP.
+    """
+
     @abstractmethod
     def eof_received(self) -> None:
         """
         Called when the other end signals it won’t send any more data.
         """
         raise NotImplementedError
 
@@ -91,23 +89,14 @@
         If the protocol implementation needs to handle any timeouts,
         it should return the closes timeout from this method.
 
         :return: time in seconds or None if no timer is necessary
         """
         raise NotImplementedError
 
-    # Receiving direction
-
-    @abstractmethod
-    def connection_lost(self) -> None:
-        """
-        Called when the connection is lost or closed.
-        """
-        raise NotImplementedError
-
 
 class OverQUICProtocol(OverUDPProtocol):
     @property
     @abstractmethod
     def connection_ids(self) -> Sequence[bytes]:
         """
         QUIC connection IDs
```

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_h11.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_h11.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,21 +159,16 @@
     pseudo_headers = [(b":status", str(response.status_code).encode())]
     return pseudo_headers + regular_headers
 
 
 class HTTP1ProtocolHyperImpl(HTTP1Protocol):
     implementation: str = "h11"
 
-    def __init__(
-        self,
-        *,
-        scheme: str = "http",
-    ) -> None:
+    def __init__(self) -> None:
         self._connection: h11.Connection = h11.Connection(h11.CLIENT)
-        self._scheme: bytes = scheme.encode()
         self._data_buffer: list[bytes] = []
         self._event_buffer: deque[Event] = deque()
         self._terminated: bool = False
         self._switched: bool = False
 
         self._current_stream_id: int = 1
 
@@ -306,16 +301,14 @@
                 a(self._connection_terminated(e.error_status_hint, str(e)))
                 break
             if h11_event is h11.NEED_DATA or h11_event is h11.PAUSED:
                 if h11.MUST_CLOSE == self._connection.their_state:
                     a(self._connection_terminated())
                 else:
                     break
-            elif isinstance(h11_event, h11.Request):
-                a(self._headers_from_h11_request(h11_event))
             elif isinstance(h11_event, (h11.Response, h11.InformationalResponse)):
                 a(self._headers_from_h11_response(h11_event))
             elif isinstance(h11_event, h11.Data):
                 a(self._data_from_h11(h11_event))
             elif isinstance(h11_event, h11.EndOfMessage):
                 # HTTP/2 and HTTP/3 send END_STREAM flag with HEADERS and DATA frames.
                 # We emulate similar behavior for HTTP/1.
@@ -328,18 +321,14 @@
                     a(last_event)
                 if self._connection.their_state != h11.MIGHT_SWITCH_PROTOCOL:  # type: ignore[attr-defined]
                     last_event.end_stream = True
                 self._maybe_start_next_cycle()
             elif isinstance(h11_event, h11.ConnectionClosed):
                 a(self._connection_terminated())
 
-    def _headers_from_h11_request(self, h11_event: h11.Request) -> Event:
-        headers = headers_from_request(h11_event, scheme=self._scheme)
-        return HeadersReceived(self._current_stream_id, headers)
-
     def _headers_from_h11_response(
         self, h11_event: h11.Response | h11.InformationalResponse
     ) -> Event:
         headers = headers_from_response(h11_event)
         return HeadersReceived(self._current_stream_id, headers)
 
     def _data_from_h11(self, h11_event: h11.Data) -> Event:
```

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/_h2.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/_h2.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,20 +34,29 @@
 )
 from .._protocols import HTTP2Protocol
 
 
 class HTTP2ProtocolHyperImpl(HTTP2Protocol):
     implementation: str = "h2"
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        *,
+        validate_outbound_headers: bool = False,
+        validate_inbound_headers: bool = False,
+        normalize_outbound_headers: bool = True,
+        normalize_inbound_headers: bool = True,
+    ) -> None:
         self._connection: h2.connection.H2Connection = h2.connection.H2Connection(
             h2.config.H2Configuration(
                 client_side=True,
-                validate_outbound_headers=False,
-                validate_inbound_headers=False,
+                validate_outbound_headers=validate_outbound_headers,
+                normalize_outbound_headers=normalize_outbound_headers,
+                validate_inbound_headers=validate_inbound_headers,
+                normalize_inbound_headers=normalize_inbound_headers,
             )
         )
         self._connection.initiate_connection()
         self._events: deque[Event] = deque()
         self._terminated: bool = False
 
     @staticmethod
```

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/_aioquic.py` & `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/_aioquic.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/tests/helpers.py` & `urllib3_ext_hface-0.3.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/tests/test_http1.py` & `urllib3_ext_hface-0.3.1/tests/test_http1.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/tests/test_http2.py` & `urllib3_ext_hface-0.3.1/tests/test_http2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/tests/test_integration.py` & `urllib3_ext_hface-0.3.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/LICENSE` & `urllib3_ext_hface-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/NOTICE` & `urllib3_ext_hface-0.3.1/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.0/pyproject.toml` & `urllib3_ext_hface-0.3.1/pyproject.toml`

 * *Files identical despite different names*

