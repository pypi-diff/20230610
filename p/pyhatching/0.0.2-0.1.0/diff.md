# Comparing `tmp/pyhatching-0.0.2.tar.gz` & `tmp/pyhatching-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhatching-0.0.2.tar", last modified: Thu Jun  8 01:57:26 2023, max compression
+gzip compressed data, was "pyhatching-0.1.0.tar", last modified: Sat Jun 10 01:38:30 2023, max compression
```

## Comparing `pyhatching-0.0.2.tar` & `pyhatching-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.648196 pyhatching-0.0.2/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 03:15:48.000000 pyhatching-0.0.2/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-08 01:57:26.648060 pyhatching-0.0.2/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      248 2023-05-21 14:55:53.000000 pyhatching-0.0.2/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      576 2023-06-08 01:57:22.000000 pyhatching-0.0.2/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-08 01:57:26.648235 pyhatching-0.0.2/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.646129 pyhatching-0.0.2/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.647271 pyhatching-0.0.2/src/pyhatching/
--rw-r--r--   0 gormo      (501) staff       (20)      429 2023-06-08 01:57:22.000000 pyhatching-0.0.2/src/pyhatching/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)    10033 2023-06-05 03:35:35.000000 pyhatching-0.0.2/src/pyhatching/base.py
--rw-r--r--   0 gormo      (501) staff       (20)    16259 2023-06-08 01:55:08.000000 pyhatching-0.0.2/src/pyhatching/client.py
--rw-r--r--   0 gormo      (501) staff       (20)     6452 2023-05-21 19:16:04.000000 pyhatching-0.0.2/src/pyhatching/enums.py
--rw-r--r--   0 gormo      (501) staff       (20)      393 2023-06-08 01:29:54.000000 pyhatching-0.0.2/src/pyhatching/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)     1325 2023-05-21 19:44:15.000000 pyhatching-0.0.2/src/pyhatching/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.647877 pyhatching-0.0.2/src/pyhatching.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      369 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       32 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.321940 pyhatching-0.1.0/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 03:15:48.000000 pyhatching-0.1.0/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-10 01:38:30.321739 pyhatching-0.1.0/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      248 2023-05-21 14:55:53.000000 pyhatching-0.1.0/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      576 2023-06-10 01:38:25.000000 pyhatching-0.1.0/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-10 01:38:30.321989 pyhatching-0.1.0/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.305336 pyhatching-0.1.0/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.312252 pyhatching-0.1.0/src/pyhatching/
+-rw-r--r--   0 gormo      (501) staff       (20)    21819 2023-06-10 01:38:25.000000 pyhatching-0.1.0/src/pyhatching/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)      911 2023-06-10 01:37:05.000000 pyhatching-0.1.0/src/pyhatching/__main__.py
+-rw-r--r--   0 gormo      (501) staff       (20)     2936 2023-06-10 00:39:25.000000 pyhatching-0.1.0/src/pyhatching/_args.py
+-rw-r--r--   0 gormo      (501) staff       (20)     2656 2023-06-10 00:45:13.000000 pyhatching-0.1.0/src/pyhatching/_cmds.py
+-rw-r--r--   0 gormo      (501) staff       (20)    10093 2023-06-09 04:49:32.000000 pyhatching-0.1.0/src/pyhatching/base.py
+-rw-r--r--   0 gormo      (501) staff       (20)     6452 2023-05-21 19:16:04.000000 pyhatching-0.1.0/src/pyhatching/enums.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1046 2023-06-10 01:28:24.000000 pyhatching-0.1.0/src/pyhatching/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1325 2023-05-21 19:44:15.000000 pyhatching-0.1.0/src/pyhatching/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.320875 pyhatching-0.1.0/src/pyhatching.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       32 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/top_level.txt
```

### Comparing `pyhatching-0.0.2/LICENSE` & `pyhatching-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhatching-0.0.2/PKG-INFO` & `pyhatching-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhatching
-Version: 0.0.2
+Version: 0.1.0
 Summary: An async Python client for the Hatching Triage Sandbox.
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyhatching-0.0.2/pyproject.toml` & `pyhatching-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyhatching"
-version = "0.0.2"
+version = "0.1.0"
 description = "An async Python client for the Hatching Triage Sandbox."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "aiohttp==3.8.4",
     "pydantic==1.10.7",
 ]
```

### Comparing `pyhatching-0.0.2/src/pyhatching/base.py` & `pyhatching-0.1.0/src/pyhatching/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,29 @@
 class ErrorResponse(HatchingResponse):
     """An error from the Hatching Triage API."""
 
     error: enums.ErrorNames
     message: str
 
 
-class SamplesResponse(HatchingResponse):
-    """Response object for POST /samples."""
+class SampleInfo(HatchingResponse):
+    """Sample metadata."""
 
     id: str
     status: enums.SubmissionStatuses
     kind: enums.SampleKinds
     filename: Optional[str]
     url: Optional[str]
     private: bool
     submitted: datetime.datetime
+
+
+class SamplesResponse(SampleInfo):
+    """Response object for POST /samples."""
+
     completed: datetime.datetime
 
 
 class YaraRule(BaseModel):
     """A yara rule."""
 
     name: str
```

### Comparing `pyhatching-0.0.2/src/pyhatching/client.py` & `pyhatching-0.1.0/src/pyhatching/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,99 @@
-"""The pyhatching HTTP client implementation."""
+"""Async client to interact with the Hatching Triage Sandbox.
+
+Not a complete client - this library focuses on common use cases.
+
+All client calls return objects (see `pyhatching.base`) instead of dicts,
+unless bytes makes more sense for the endpoint (samples, pcaps).
+
+The following examples assume you have imported the following and that the
+example code is being executed with an async function::
+
+    import pprint
+    import pyhatching
+
+Examples:
+
+- Use a context manager to init the client::
+
+    async with pyhatching.PyHatchingClient(api_key=<token>) as client:
+        samples_details = await client.search("tag:beacon")
+        pprint.pp([s.dict() for s in samples_details], indent=2)
+
+- Using the new_client factory method - supports same args as PyHatchingClient::
+
+    client = async pyhatching.new_client(api_key=<token>)
+    # Catch all errors handled by Pyhatching
+    try:
+        sample = client.get_sample(<hash>)
+    except pyhatching.errors.PyHatchingError as err:
+        print(f"pyhatching didn't work: {err}")
+    
+    print(sample.dict())
+    client.close()  # Don't forget to close the client's session when you're done!
+
+- If you'd like to init the class itself, you'll need to call the ``start()``
+method before making any requests::
+
+    client = pyhatching.PyHatchingClient(api_key=<token>)
+    await client.start()
+    report = await client.overview(<hash>)
+    # If the sandbox API returns an error, the return type will reflect that.
+    if isinstance(report, pyhatching.base.ErrorResponse):
+        print(f"Error: {report}")
+    else:
+        pprint.pp(report.dict(), indent=2)
+    client.close()
+
+- If you don't like the above pattern of ``ErrorResponse`` return types, you
+can pass ``raise_on_api_err=True`` to ``PyHatchingClient``::
+
+    async with pyhatching.PyHatchingClient(
+        api_key=<token>, raise_on_api_err=True
+    ) as client:
+        try:
+            sandbox_profiles = await client.get_profiles()
+
+        # This is the error that get's raised when raise_on_api_err is True
+        except pyhatching.errors.PyHatchingApiError as err:
+            print(f"The Hatching Triage API returned an err: {err}")
+
+        # Catch the rest of our request errors. Alternatively, we could have
+        # caught PyHatchingConnError to replace both this except and the above.
+        except pyhatching.errors.PyHatchingRequestError as err:
+            print(f"Error connecting to Hatching Triage API: {err}")
+
+        # We'll let other things like validation errors raise for this example
+        else:
+            pprint.pp(sandbox_profiles)
+
+"""
+
 
-# import asyncio
 import functools
 from json import JSONDecodeError
 import pathlib
 
 import aiohttp
 from pydantic.error_wrappers import ValidationError  # pylint: disable=E0611
 
 from . import base
 from . import enums
 from . import errors
 from . import utils
-from . import BASE_URL, __version__
+
+
+__version__ = "0.1.0"
+"""The version of pyhatching."""
+
+BASE_URL = "https://tria.ge"
+"""The default URL for requests - the public/free version."""
+
+API_PATH = "/api/v0"
+"""The base path used by all API endpoints used for requests."""
 
 
 def convert_to_model(
     model: base.HatchingResponse,
     resp: aiohttp.ClientResponse,
     obj: dict,
     raise_on_api_err: bool = False,
@@ -39,18 +116,18 @@
     -------
     base.HatchingResponse | list[base.HatchingResponse]
         The API can return either a list or a single item depending on the endpoint
         so can this method. The objects returned are of the same type as ``model``.
 
     Raises
     ------
-    errors.PyHatchingParseError
+    errors.PyHatchingValidateError
         If ``obj`` could not be validated when passed to ``model``. Or when
         ``obj`` is not a dict.
-    errors.PyHatchingResponseError
+    errors.PyHatchingApiError
         If ``raise_on_api_err`` is ``True`` and ``obj`` represents an error
         returned by the Hatching Triage API and not a successful response.
     """
 
     ret = []
     url = resp.request_info.url
     try:
@@ -58,40 +135,60 @@
             for item in obj["data"]:
                 ret.append(model(resp_obj=obj, **item))
         elif "error" in obj:
             ret = base.ErrorResponse(resp_obj=resp, **obj)
         elif isinstance(obj, dict):
             ret = model(resp_obj=resp, **obj)
         else:
-            raise errors.PyHatchingParseError(
+            raise errors.PyHatchingValueError(
                 f"Unexpected response from the {url} endpoint: {obj}"
             )
     except ValidationError as err:
-        raise errors.PyHatchingParseError(
+        raise errors.PyHatchingValidateError(
             f"Unable to validate {url} response: {err}"
         ) from err
 
     if raise_on_api_err and isinstance(ret, base.ErrorResponse):
-        raise errors.PyHatchingResponseError(
+        raise errors.PyHatchingApiError(
             f"Hatching Triage API Error - {ret.error} - {ret.message}"
         )
 
     return ret
 
 
+async def new_client(
+    api_key: str,
+    url: str = BASE_URL,
+    timeout: int = 60,
+    raise_on_api_err: bool = False,
+    **kwargs,
+):
+    """Factory to create a new ``PyHatchingCLient`` instance."""
+
+    client = PyHatchingClient(
+        api_key,
+        url,
+        timeout,
+        raise_on_api_err,
+        **kwargs,
+    )
+    await client.start()
+    return client
+
+
 class PyHatchingClient:
     """An async HTTP client that interfaces with the Hatching Triage Sandbox.
 
     Any method that makes HTTP requests (calls ``_request``) may raise either
-    a ``PyHatchingRequestError`` or ``PyHatchingParseError``.
+    a ``PyHatchingRequestError`` or ``PyHatchingValidateError``.
 
     Additionally, any method that returns a Pydantic model (``base.HatchingResponse``)
-    may raise a ``PyHatchingParseError``. If ``raise_on_api_err`` is ``True``, these
-    methods may raise a ``PyHatchingResponseError`` as well.
-    
+    may raise a ``PyHatchingValidateError``. If ``raise_on_api_err`` is ``True``, these
+    methods may raise a ``PyHatchingApiError`` as well.
+
     If a specific method also explicitly raises exceptions, it will be documented.
 
     Catch all handled errors with ``PyHatchingError``.
 
     Parameters
     ----------
     api_key : str
@@ -125,28 +222,45 @@
     def __init__(
         self,
         api_key: str,
         url: str = BASE_URL,
         timeout: int = 60,
         raise_on_api_err: bool = False,
     ) -> None:
+        self.url = url
         self.api_key = api_key
         self.headers = {
             "Authorization": f"Bearer {self.api_key}",
             "User-Agent": f"{aiohttp.http.SERVER_SOFTWARE} pyhatching/{__version__}",
         }
+
         self.timeout = aiohttp.ClientTimeout(total=timeout)
-        self.session = aiohttp.ClientSession(
-            base_url=url, headers=self.headers, timeout=self.timeout
-        )
+        self.session = None
 
         self.convert_resp = functools.partial(
             convert_to_model, raise_on_api_err=raise_on_api_err
         )
 
+    async def __aenter__(self,):
+        await self.start()
+        return self
+
+    async def __aexit__(self, *args):
+        await self.close()
+
+    async def start(self):
+        """Start the client session."""
+        self.session = aiohttp.ClientSession(
+            base_url=self.url, headers=self.headers, timeout=self.timeout
+        )
+
+    async def close(self):
+        """Close the client session."""
+        await self.session.close()
+
     async def _request(
         self,
         method: str,
         uri: str,
         data: dict | None = None,
         json: dict | None = None,
         params: dict | None = None,
@@ -185,77 +299,118 @@
             The response JSON. An error is raised if this couldn't be deserialized.
 
         Raises
         ------
         PyHatchingRequestError
             If there was an error (not an HTTP response error code)
             in the process of making a request.
-        PyHatchingParseError
+        PyHatchingValidateError
             If the JSON response could not be parsed.
         """
 
         try:
             resp = await self.session.request(
-                method, uri, data=data, json=json, params=params
+                method, f"{API_PATH}{uri}", data=data, json=json, params=params
             )
 
             if raw:
                 return resp, {}
 
             resp_json = await resp.json()
 
         except aiohttp.ClientError as err:
             raise errors.PyHatchingRequestError(
                 f"Error making an HTTP request to Hatching Triage: {err}"
             ) from err
 
         except JSONDecodeError as err:
-            raise errors.PyHatchingParseError(
+            raise errors.PyHatchingJsonError(
                 f"Unable to parse the response json: {err}"
             ) from err
 
         return resp, resp_json
 
+    async def norm_sample(self, sample: str) -> str | None:
+        """Return a sample ID if sample is a hash, otherwise pass it back."""
+        if utils.is_hash(sample):
+            sample_id = await self.sample_id(sample)
+        else:
+            sample_id = sample
+        return sample_id
+
     async def download_sample(self, sample: str) -> bytes | None:
         """Download a sample's bytes by the given ID.
 
         Parameters
         ----------
         sample : str
             The sample to download, this can be any of the following
             as the value is passed to ``sample_id`` if needed to find the ID::
 
-                sample_id, md5, sha1, sha2, ssdeep
+                sample uuid, md5, sha1, sha2, ssdeep
+
+        Raises
+        ------
+        PyHatchingError
+            When a sample cannot be found.
 
         Returns
         -------
         bytes
             The downloaded bytes.
         None
-            If no bytes can be downloaded.
+            If no bytes can be downloaded or the sample is not found.
         """
 
-        if utils.is_hash(sample):
-            sample_id = await self.sample_id(sample)
-        else:
-            sample_id = sample
-
+        sample_id = await self.norm_sample(sample)
         if sample_id is None:
-            raise errors.PyHatchingParseError(
-                f"Unable to determine sample_id from: {sample}"
-            )
+            return None
 
         resp, _ = await self._request("get", f"/samples/{sample_id}/sample", raw=True)
 
         if resp.status == 200:
             sample_bytes = await resp.read()
             return sample_bytes
 
         return None
 
+    async def get_sample(self, sample: str) -> base.SampleInfo | base.ErrorResponse:
+        """Get metadata about a sample by hash or sample ID.
+
+        Parameters
+        ----------
+        sample : str
+            The sample to download, this can be any of the following
+            as the value is passed to ``sample_id`` if needed to find the ID::
+
+                sample uuid, md5, sha1, sha2, ssdeep
+
+        Raises
+        ------
+        PyHatchingError
+            When a sample cannot be found.
+
+        Returns
+        -------
+        base.SampleInfo
+            The sample's metadata
+        base.ErrorResponse
+            If the API returns an error.
+        None
+            If the sample is not found.
+        """
+
+        sample_id = await self.norm_sample(sample)
+        if sample_id is None:
+            return None
+
+        resp, resp_dict = await self._request("get", f"/samples/{sample}")
+
+        return self.convert_resp(base.SampleInfo, resp, resp_dict)
+
     async def get_profile(
         self, profile_id: str
     ) -> base.HatchingProfileResponse | base.ErrorResponse:
         """Get a sandbox analysis profile by either ID or name.
 
         Parameters
         ----------
@@ -283,54 +438,80 @@
         -------
         list[base.HatchingProfileResponse]
             If successful, the requested sandbox profiles.
         base.ErrorResponse
             If there was an error.
         """
 
+        resp, resp_dict = await self._request("get", "/profiles")
+
+        return self.convert_resp(base.HatchingProfileResponse, resp, resp_dict)
+
     async def get_rule(self, rule_name: str) -> base.YaraRule:
         """Get a single Yara rule by name.
 
         Parameters
         ----------
         rule_name : str
             The name of the rule.
 
         Returns
         -------
         base.YaraRule
             If successful, the returned Yara rule.
         """
 
+        resp, resp_dict = await self._request("get", f"/yara/{rule_name}")
+
+        return self.convert_resp(base.YaraRule, resp, resp_dict)
+
     async def get_rules(self) -> base.YaraRules:
         """Get all Yara rules tied to your account.
 
         Returns
         -------
         base.YaraRules
             If successful, the returned Yara rules.
         """
 
-    async def overview(self, sample: str) -> base.OverviewReport:
+        resp, resp_dict = await self._request("get", "/yara")
+
+        return self.convert_resp(base.YaraRules, resp, resp_dict)
+
+    async def overview(self, sample: str) -> base.OverviewReport | base.ErrorResponse:
         """Return a sample's Overview Report.
 
         Parameters
         ----------
         sample : str
             The sample to download, this can be any of the following
             as the value is passed to ``sample_id`` if needed to find the ID::
 
-                sample_id, md5, sha1, sha2, ssdeep
+                sample uuid, md5, sha1, sha2, ssdeep
 
         Returns
         -------
         base.OverviewReport
             If successful, the return Overview Report.
+        base.ErrorResponse
+            If there was an error.
+        None
+            If the sample is not found.
         """
 
+        sample_id = await self.norm_sample(sample)
+        if sample_id is None:
+            return None
+
+        resp, resp_dict = await self._request(
+            "get", f"/samples/{sample_id}/overview.json"
+        )
+
+        return self.convert_resp(base.OverviewReport, resp, resp_dict)
+
     async def sample_id(self, file_hash: str) -> str | None:
         """Find the ID of a sample by the given hash, uses ``search`` under the hood.
 
         Parameters
         ----------
         file_hash : str
             The hash (md5, sha1, sha2, ssdeep) of the file to get and ID for.
@@ -342,15 +523,15 @@
         None
             The sample ID could not be found.
         """
 
         hash_prefix = utils.hash_type(file_hash)
 
         if hash_prefix is None:
-            raise errors.PyHatchingParseError(
+            raise errors.PyHatchingValueError(
                 f"The input hash is not valid according to 'utils.hash_type': {file_hash}"
             )
 
         samples = await self.search(f"{hash_prefix}:{file_hash}")
 
         if isinstance(samples, base.ErrorResponse):
             return None
```

### Comparing `pyhatching-0.0.2/src/pyhatching/enums.py` & `pyhatching-0.1.0/src/pyhatching/enums.py`

 * *Files identical despite different names*

### Comparing `pyhatching-0.0.2/src/pyhatching/utils.py` & `pyhatching-0.1.0/src/pyhatching/utils.py`

 * *Files identical despite different names*

### Comparing `pyhatching-0.0.2/src/pyhatching.egg-info/PKG-INFO` & `pyhatching-0.1.0/src/pyhatching.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhatching
-Version: 0.0.2
+Version: 0.1.0
 Summary: An async Python client for the Hatching Triage Sandbox.
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

