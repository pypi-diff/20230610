# Comparing `tmp/pyhatching-0.1.0.tar.gz` & `tmp/pyhatching-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhatching-0.1.0.tar", last modified: Sat Jun 10 01:38:30 2023, max compression
+gzip compressed data, was "pyhatching-0.2.0.tar", last modified: Sat Jun 10 17:19:14 2023, max compression
```

## Comparing `pyhatching-0.1.0.tar` & `pyhatching-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.321940 pyhatching-0.1.0/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 03:15:48.000000 pyhatching-0.1.0/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-10 01:38:30.321739 pyhatching-0.1.0/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      248 2023-05-21 14:55:53.000000 pyhatching-0.1.0/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      576 2023-06-10 01:38:25.000000 pyhatching-0.1.0/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-10 01:38:30.321989 pyhatching-0.1.0/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.305336 pyhatching-0.1.0/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.312252 pyhatching-0.1.0/src/pyhatching/
--rw-r--r--   0 gormo      (501) staff       (20)    21819 2023-06-10 01:38:25.000000 pyhatching-0.1.0/src/pyhatching/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)      911 2023-06-10 01:37:05.000000 pyhatching-0.1.0/src/pyhatching/__main__.py
--rw-r--r--   0 gormo      (501) staff       (20)     2936 2023-06-10 00:39:25.000000 pyhatching-0.1.0/src/pyhatching/_args.py
--rw-r--r--   0 gormo      (501) staff       (20)     2656 2023-06-10 00:45:13.000000 pyhatching-0.1.0/src/pyhatching/_cmds.py
--rw-r--r--   0 gormo      (501) staff       (20)    10093 2023-06-09 04:49:32.000000 pyhatching-0.1.0/src/pyhatching/base.py
--rw-r--r--   0 gormo      (501) staff       (20)     6452 2023-05-21 19:16:04.000000 pyhatching-0.1.0/src/pyhatching/enums.py
--rw-r--r--   0 gormo      (501) staff       (20)     1046 2023-06-10 01:28:24.000000 pyhatching-0.1.0/src/pyhatching/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)     1325 2023-05-21 19:44:15.000000 pyhatching-0.1.0/src/pyhatching/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 01:38:30.320875 pyhatching-0.1.0/src/pyhatching.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       32 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-10 01:38:30.000000 pyhatching-0.1.0/src/pyhatching.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 17:19:14.656784 pyhatching-0.2.0/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 03:15:48.000000 pyhatching-0.2.0/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-10 17:19:14.656635 pyhatching-0.2.0/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      248 2023-05-21 14:55:53.000000 pyhatching-0.2.0/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      576 2023-06-10 17:19:10.000000 pyhatching-0.2.0/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-10 17:19:14.656828 pyhatching-0.2.0/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 17:19:14.654133 pyhatching-0.2.0/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 17:19:14.655500 pyhatching-0.2.0/src/pyhatching/
+-rw-r--r--   0 gormo      (501) staff       (20)    26071 2023-06-10 17:19:10.000000 pyhatching-0.2.0/src/pyhatching/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1000 2023-06-10 16:48:59.000000 pyhatching-0.2.0/src/pyhatching/__main__.py
+-rw-r--r--   0 gormo      (501) staff       (20)     5405 2023-06-10 16:42:58.000000 pyhatching-0.2.0/src/pyhatching/_args.py
+-rw-r--r--   0 gormo      (501) staff       (20)     4521 2023-06-10 17:15:01.000000 pyhatching-0.2.0/src/pyhatching/_cmds.py
+-rw-r--r--   0 gormo      (501) staff       (20)    10941 2023-06-10 16:35:23.000000 pyhatching-0.2.0/src/pyhatching/base.py
+-rw-r--r--   0 gormo      (501) staff       (20)     6452 2023-05-21 19:16:04.000000 pyhatching-0.2.0/src/pyhatching/enums.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1184 2023-06-10 04:46:43.000000 pyhatching-0.2.0/src/pyhatching/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1349 2023-06-10 03:04:34.000000 pyhatching-0.2.0/src/pyhatching/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-10 17:19:14.656369 pyhatching-0.2.0/src/pyhatching.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-10 17:19:14.000000 pyhatching-0.2.0/src/pyhatching.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-10 17:19:14.000000 pyhatching-0.2.0/src/pyhatching.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-10 17:19:14.000000 pyhatching-0.2.0/src/pyhatching.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       32 2023-06-10 17:19:14.000000 pyhatching-0.2.0/src/pyhatching.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-10 17:19:14.000000 pyhatching-0.2.0/src/pyhatching.egg-info/top_level.txt
```

### Comparing `pyhatching-0.1.0/LICENSE` & `pyhatching-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhatching-0.1.0/PKG-INFO` & `pyhatching-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhatching
-Version: 0.1.0
+Version: 0.2.0
 Summary: An async Python client for the Hatching Triage Sandbox.
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyhatching-0.1.0/pyproject.toml` & `pyhatching-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyhatching"
-version = "0.1.0"
+version = "0.2.0"
 description = "An async Python client for the Hatching Triage Sandbox."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "aiohttp==3.8.4",
     "pydantic==1.10.7",
 ]
```

### Comparing `pyhatching-0.1.0/src/pyhatching/__init__.py` & `pyhatching-0.2.0/src/pyhatching/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,41 +15,39 @@
 
 - Use a context manager to init the client::
 
     async with pyhatching.PyHatchingClient(api_key=<token>) as client:
         samples_details = await client.search("tag:beacon")
         pprint.pp([s.dict() for s in samples_details], indent=2)
 
-- Using the new_client factory method - supports same args as PyHatchingClient::
+- Using the ``new_client`` factory method - supports same args as ``PyHatchingClient``::
 
     client = async pyhatching.new_client(api_key=<token>)
     # Catch all errors handled by Pyhatching
     try:
         sample = client.get_sample(<hash>)
     except pyhatching.errors.PyHatchingError as err:
         print(f"pyhatching didn't work: {err}")
     
     print(sample.dict())
     client.close()  # Don't forget to close the client's session when you're done!
 
-- If you'd like to init the class itself, you'll need to call the ``start()``
-method before making any requests::
+- If you'd like to init the class itself, you'll need to call the ``start()`` method before making any requests::
 
     client = pyhatching.PyHatchingClient(api_key=<token>)
     await client.start()
     report = await client.overview(<hash>)
     # If the sandbox API returns an error, the return type will reflect that.
     if isinstance(report, pyhatching.base.ErrorResponse):
         print(f"Error: {report}")
     else:
         pprint.pp(report.dict(), indent=2)
     client.close()
 
-- If you don't like the above pattern of ``ErrorResponse`` return types, you
-can pass ``raise_on_api_err=True`` to ``PyHatchingClient``::
+- If you don't like the above pattern of ``ErrorResponse`` return types, you can pass ``raise_on_api_err=True`` to ``PyHatchingClient``::
 
     async with pyhatching.PyHatchingClient(
         api_key=<token>, raise_on_api_err=True
     ) as client:
         try:
             sandbox_profiles = await client.get_profiles()
 
@@ -66,27 +64,29 @@
         else:
             pprint.pp(sandbox_profiles)
 
 """
 
 
 import functools
+import hashlib
 from json import JSONDecodeError
+import os
 import pathlib
 
 import aiohttp
 from pydantic.error_wrappers import ValidationError  # pylint: disable=E0611
 
 from . import base
 from . import enums
 from . import errors
 from . import utils
 
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 """The version of pyhatching."""
 
 BASE_URL = "https://tria.ge"
 """The default URL for requests - the public/free version."""
 
 API_PATH = "/api/v0"
 """The base path used by all API endpoints used for requests."""
@@ -196,15 +196,15 @@
     url : str, optional
         The URL to use as a base in all requests, by default BASE_URL.
     timeout : int, optional
         The total timeout for all requests, by default 60.
     raise_on_api_err : bool, optional
         Whether to raise when the Hatching Triage API returns an API error response
         (an HTTP 200 response that describes a handled error with the request).
-        See the `docs`_ for further information.
+        See the `API docs`_ for further information.
 
     Attributes
     ----------
     api_key : str
         The Hatching Triage Sandbox API key to use for requests.
     headers : dict
         The headers used with every request, has API key and custom User Agent.
@@ -212,15 +212,15 @@
         The underlying ClientSession used to make requests.
     timeout : aiohttp.ClientTimeout
         The timeout object used by ``session``.
     convert_resp : typing.Callable
         A ``functools.partial`` for ``convert_to_model`` with ```raise_on_api_err``
         saved so that it doesn't have to be passed to each method call.
 
-    .. _docs: https://tria.ge/docs/cloud-api/conventions/
+    .. _API docs: https://tria.ge/docs/cloud-api/conventions/
     """
 
     def __init__(
         self,
         api_key: str,
         url: str = BASE_URL,
         timeout: int = 60,
@@ -236,15 +236,17 @@
         self.timeout = aiohttp.ClientTimeout(total=timeout)
         self.session = None
 
         self.convert_resp = functools.partial(
             convert_to_model, raise_on_api_err=raise_on_api_err
         )
 
-    async def __aenter__(self,):
+    async def __aenter__(
+        self,
+    ):
         await self.start()
         return self
 
     async def __aexit__(self, *args):
         await self.close()
 
     async def start(self):
@@ -257,15 +259,15 @@
         """Close the client session."""
         await self.session.close()
 
     async def _request(
         self,
         method: str,
         uri: str,
-        data: dict | None = None,
+        data: aiohttp.MultipartWriter | None = None,
         json: dict | None = None,
         params: dict | None = None,
         raw: bool = False,
     ) -> tuple[aiohttp.ClientResponse, dict]:
         """Make an HTTP request to the Hatching Triage Sandbox API.
 
         Returns both the response and the deserialized JSON response.
@@ -442,15 +444,15 @@
             If there was an error.
         """
 
         resp, resp_dict = await self._request("get", "/profiles")
 
         return self.convert_resp(base.HatchingProfileResponse, resp, resp_dict)
 
-    async def get_rule(self, rule_name: str) -> base.YaraRule:
+    async def get_rule(self, rule_name: str) -> base.YaraRule | base.ErrorResponse:
         """Get a single Yara rule by name.
 
         Parameters
         ----------
         rule_name : str
             The name of the rule.
 
@@ -460,15 +462,15 @@
             If successful, the returned Yara rule.
         """
 
         resp, resp_dict = await self._request("get", f"/yara/{rule_name}")
 
         return self.convert_resp(base.YaraRule, resp, resp_dict)
 
-    async def get_rules(self) -> base.YaraRules:
+    async def get_rules(self) -> base.YaraRules | base.ErrorResponse:
         """Get all Yara rules tied to your account.
 
         Returns
         -------
         base.YaraRules
             If successful, the returned Yara rules.
         """
@@ -572,16 +574,16 @@
 
         return self.convert_resp(base.SamplesResponse, resp, resp_dict)
 
     async def submit_profile(
         self,
         name: str,
         tags: list[str],
-        timeout: int,
-        network: enums.ProfileNetworkOptions,
+        timeout: int | None,
+        network: enums.ProfileNetworkOptions | None,
     ) -> None | base.ErrorResponse:
         """Add a new sandbox analysis profile to your account.
 
         Parameters
         ----------
         name : str
             The name of the new profile, must not exist already.
@@ -595,14 +597,39 @@
 
         Returns
         -------
         None | base.ErrorResponse
             None if successful, else ``base.ErrorResponse``.
         """
 
+        data = {"name": name, "tags": tags, "timeout": timeout, "network": network}
+
+        resp, resp_dict = await self._request(
+            "post", "/profiles", json={k: v for k, v in data.items() if v is not None}
+        )
+
+        return self.convert_resp(base.HatchingProfileResponse, resp, resp_dict)
+
+    async def _write_rule(self, method: str, name: str, contents: str):
+        """A generic method to create/update a yara rule."""
+
+        data = {"name": name, "rule": contents}
+
+        if method == "put":
+            uri = f"/yara/{name}"
+        else:
+            uri = "/yara"
+
+        resp, resp_dict = await self._request(method, uri, json=data)
+
+        if "error" in resp_dict:
+            return self.convert_resp(base.ErrorResponse, resp, resp_dict)
+
+        return None
+
     async def submit_rule(self, name: str, contents: str) -> base.ErrorResponse | None:
         """Submit a Yara rule to your account.
 
         Parameters
         ----------
         name : str
             The name of the rule - must not exist already.
@@ -611,46 +638,129 @@
 
         Returns
         -------
         base.ErrorResponse | None
             None if successful, otherwise the returned ErrorResponse.
         """
 
-    async def submit_sample(
+        return await self._write_rule("post", name, contents)
+
+    async def _submit_sample(
+        self,
+        json: dict | None = None,
+        data: aiohttp.MultipartWriter | None = None,
+    ):
+        """Actually make the submit sample HTTP request."""
+
+        resp, resp_dict = await self._request("post", "/samples", json=json, data=data)
+        return resp, resp_dict
+
+    async def _submit_fetch(
+        self,
+        submit_req: base.SubmissionRequest,
+    ):
+        """Submit a file hosted at a URL for the sandbox to download and analyze."""
+
+        return await self._submit_sample(json=submit_req.dict(exclude_none=True))
+
+    async def _submit_file(
         self,
         submit_req: base.SubmissionRequest,
         sample: bytes | pathlib.Path | str,
-    ) -> base.SamplesResponse:
+    ):
+        """Submit a file to the sandbox for analysis."""
+
+        mpwriter = aiohttp.MultipartWriter()
+
+        if isinstance(sample, bytes):
+            fpart = mpwriter.append(sample)
+
+            if not submit_req.target:
+                fhash = hashlib.md5(sample).hexdigest()
+                raise errors.PyHatchingValueError(
+                    f"Must specify a filename when passing submitting bytes ({fhash})"
+                )
+
+            fpart.set_content_disposition(
+                "form-data", name="file", filename=submit_req.target
+            )
+
+        else:
+            try:
+                with open(sample, "rb") as fd:
+                    mpwriter.append(fd)
+            except OSError as err:
+                raise errors.PyHatchingFileError(
+                    f"Unable to read {sample}: {err}"
+                ) from err
+
+        jpart = mpwriter.append(submit_req.json(exclude_none=True))
+        jpart.set_content_disposition("form-data", name="_json")
+
+        return await self._submit_sample(data=mpwriter)
+
+    async def _submit_url(self, url: str):
+        """Submit a url to the sandbox for analysis."""
+
+        return await self._submit_sample(json={"url": url})
+
+    async def submit_sample(
+        self,
+        submit_req: base.SubmissionRequest,
+        sample: bytes | pathlib.Path | str | None,
+    ) -> base.SamplesResponse | base.ErrorResponse:
         """Submit a sample to the sandbox based on the given ``SubmissionRequest``.
 
         Parameters
         ----------
         submit_req : base.SubmissionRequest
             The object used to make the request - see this object for details.
         sample : bytes | pathlib.Path | str
             The local file path, url, or raw bytes, to submit to the sandbox.
 
         Returns
         -------
         base.SamplesResponse
             If successful, the newly created sample object.
+        base.ErrorResponse
+            If the API reports an error with the submission.
         """
 
+        if submit_req.kind == "file":
+            if sample is None:
+                raise errors.PyHatchingValueError(
+                    "No file specified for file based submission."
+                )
+            path = os.path.expandvars(os.path.expanduser(sample))
+            resp, resp_dict = await self._submit_file(submit_req, path)
+        else:
+            if submit_req.url is None:
+                raise errors.PyHatchingValueError(
+                    "No URL specified for url based submission."
+                )
+            if submit_req.kind == "url":
+                resp, resp_dict = await self._submit_url(submit_req.url)
+            elif submit_req.kind == "fetch":
+                resp, resp_dict = await self._submit_fetch(submit_req)
+
+        return self.convert_resp(base.SamplesResponse, resp, resp_dict)
+
     async def update_profile(
         self,
         tags: list[str],
         timeout: int,
         network: enums.ProfileNetworkOptions,
-        name: str | None = None,
-        profile_id: str | None = None,
+        name: str,
+        profile_id: str,
     ) -> None | base.ErrorResponse:
         """Update the given profile.
 
-        One of ``name`` or ``profile_id`` must be set. Otherwise, ValueError is raised.
-        Both parameters cannot be used at the same time.
+        See `profile docs`_ for how this endpoint behaves, all args are required.
+
+        Does not support name changes - only updating IDs in place.
 
         Parameters
         ----------
         tags : list[str]
             The tags that match this profile to samples (TODO find documented options).
         timeout : int
             The profiles timeout length in seconds.
@@ -664,19 +774,29 @@
         Returns
         -------
         None | base.ErrorResponse
             None if successful, otherwise a ``base.ErrorResponse``.
 
         Raises
         ------
-        ValueError
+        PyHatchingValueError
             If both ``name`` and ``profile_id`` are not set.
             Or if both parameters are set.
+
+        .. _profile docs: https://tria.ge/docs/cloud-api/profiles/
         """
 
+        data = {"name": name, "tags": tags, "timeout": timeout, "network": network}
+
+        resp, resp_dict = await self._request(
+            "post", f"/profiles/{profile_id}", json=data
+        )
+
+        return self.convert_resp(base.SamplesResponse, resp, resp_dict)
+
     async def update_rule(self, name: str, contents: str) -> base.ErrorResponse | None:
         """Update an existing Yara rule.
 
         Parameters
         ----------
         name : str
             The name of the rule - must exist already.
@@ -684,7 +804,9 @@
             The new contents of the Yara rule.
 
         Returns
         -------
         base.ErrorResponse | None
             None if successful, otherwise the returned ErrorResponse.
         """
+
+        return await self._write_rule("put", name, contents)
```

### Comparing `pyhatching-0.1.0/src/pyhatching/__main__.py` & `pyhatching-0.2.0/src/pyhatching/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 
 
 async def main():
     """Main function for the CLI."""
 
     args = MAIN_PARSER.parse_args()
 
-    if not args.token:
+    if args.token is None:
         if (token := os.environ.get("HATCHING_TOKEN")):
             args.token = token
         else:
             print("No token in $HATCHING_TOKEN or passed with --token!")
             return
 
+    if args.command is None:
+        print("Must specify a command!")
+
     try:
         cmd = getattr(_cmds, f"do_{args.command}")
     except AttributeError as err:
         print(f"Unable to find command func for {args.command}: {err}")
         return
 
     async with PyHatchingClient(api_key=args.token) as client:
         try:
-            cmd(client, args)
+            await cmd(client, args)
         except PyHatchingError as err:
-            print(f"{str(type(err))} while executing {args.command}: {err}")
+            print(f"{err.__class__.__name__} while executing {args.command}: {err}")
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `pyhatching-0.1.0/src/pyhatching/base.py` & `pyhatching-0.2.0/src/pyhatching/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,32 +30,32 @@
 
 class SampleInfo(HatchingResponse):
     """Sample metadata."""
 
     id: str
     status: enums.SubmissionStatuses
     kind: enums.SampleKinds
-    filename: Optional[str]
-    url: Optional[str]
     private: bool
     submitted: datetime.datetime
+    filename: Optional[str] = None
+    url: Optional[str] = None
 
 
 class SamplesResponse(SampleInfo):
     """Response object for POST /samples."""
 
     completed: datetime.datetime
 
 
 class YaraRule(BaseModel):
     """A yara rule."""
 
     name: str
-    warnings: Optional[list[str]]
-    rule: Optional[str]
+    warnings: Optional[list[str]] = None
+    rule: Optional[str] = None
 
 
 class YaraRules(HatchingResponse):
     """A list of yara rules."""
 
     rules: list[YaraRule]
 
@@ -78,145 +78,145 @@
 class HatchingRequest(BaseModel):
     """A request model sent to the Hatching Triage API."""
 
 
 class SubmissionRequestDefaults(BaseModel):
     """Default sandbox paramaters for SubmissionRequest."""
 
-    timeout: Optional[int]
-    network: Optional[enums.SubmssionsRequestNetDefaults]
+    timeout: Optional[int] = None
+    network: Optional[enums.SubmssionsRequestNetDefaults] = None
 
 
 class HatchingProfileSubmission(BaseModel):
     """A sandbox submission profile object."""
 
-    profile: Optional[str]
-    pick: Optional[str]
+    profile: Optional[str] = None
+    pick: Optional[str] = None
 
 
 class SubmissionRequest(HatchingRequest):
     """Request object for POST /samples.
 
     TODO Document the params here as they aren't anywhere else.
     """
 
     kind: enums.SubmissionKinds
-    url: Optional[str]
-    target: Optional[str]
-    interactive: Optional[bool]
-    password: Optional[str]
-    profiles: Optional[list[HatchingProfileSubmission]]
-    user_tags: Optional[list[str]]
-    defaults: SubmissionRequestDefaults
+    url: Optional[str] = None
+    target: Optional[str] = None
+    interactive: Optional[bool] = None
+    password: Optional[str] = None
+    profiles: Optional[list[HatchingProfileSubmission]] = None
+    user_tags: Optional[list[str]] = None
+    defaults: Optional[SubmissionRequestDefaults] = None
 
 
 class TaskSummary(BaseModel):
     """The summary of a task."""
 
     sample: str
-    kind: Optional[str]
-    name: Optional[str]
-    status: Optional[str]
-    ttp: Optional[list[str]]
-    tags: Optional[list[str]]
-    score: Optional[int]
-    target: Optional[str]
-    backend: Optional[str]
-    resource: Optional[str]
-    platform: Optional[str]
-    task_name: Optional[str]
-    failure: Optional[str]
-    queue_id: Optional[int]
-    pick: Optional[str]
+    kind: Optional[str] = None
+    name: Optional[str] = None
+    status: Optional[str] = None
+    ttp: Optional[list[str]] = None
+    tags: Optional[list[str]] = None
+    score: Optional[int] = None
+    target: Optional[str] = None
+    backend: Optional[str] = None
+    resource: Optional[str] = None
+    platform: Optional[str] = None
+    task_name: Optional[str] = None
+    failure: Optional[str] = None
+    queue_id: Optional[int] = None
+    pick: Optional[str] = None
 
 
 class OverviewAnalysis(BaseModel):
     """Quick overview of analysis results."""
 
     score: int
-    family: Optional[list[str]]
-    tags: Optional[list[str]]
+    family: Optional[list[str]] = None
+    tags: Optional[list[str]] = None
 
 
 class ReportedFailure(BaseModel):
     """An API failure."""
 
-    task: Optional[str]
-    backend: Optional[str]
     reason: str
+    task: Optional[str] = None
+    backend: Optional[str] = None
 
 
 class TargetDesc(BaseModel):
     """The description of a target (or analyzed object)."""
 
-    id: Optional[str]
-    score: Optional[int]
-    submitted: Optional[datetime.datetime]
-    completed: Optional[datetime.datetime]
-    target: Optional[str]
-    pick: Optional[str]
-    type: Optional[str]
-    size: Optional[int]
-    md5: Optional[str]
-    sha1: Optional[str]
-    sha256: Optional[str]
-    sha512: Optional[str]
-    filetype: Optional[str]
-    static_tags: Optional[list[str]]
+    id: Optional[str] = None
+    score: Optional[int] = None
+    submitted: Optional[datetime.datetime] = None
+    completed: Optional[datetime.datetime] = None
+    target: Optional[str] = None
+    pick: Optional[str] = None
+    type: Optional[str] = None
+    size: Optional[int] = None
+    md5: Optional[str] = None
+    sha1: Optional[str] = None
+    sha256: Optional[str] = None
+    sha512: Optional[str] = None
+    filetype: Optional[str] = None
+    static_tags: Optional[list[str]] = None
 
 
 class Indicator(BaseModel):
     """A single IOC hit of an analyzed sample."""
 
-    ioc: Optional[str]
-    description: Optional[str]
-    at: Optional[int]  # NOTE These had `uint32` go types, does `int` work?
-    pid: Optional[int]  # NOTE These had `uint64` go types, does `int` work?
-    procid: Optional[int]  # NOTE These had `int32` go types, does `int` work?
-    pid_target: Optional[int]  # NOTE These had `uint64` go types, does `int` work?
-    procid_target: Optional[int]  # NOTE These had `int32` go types, does `int` work?
-    flow: Optional[int]
-    stream: Optional[int]
-    dump_file: Optional[str]
-    resource: Optional[str]
-    yara_rule: Optional[str]
+    ioc: Optional[str] = None
+    description: Optional[str] = None
+    at: Optional[int] = None
+    pid: Optional[int] = None
+    procid: Optional[int] = None
+    pid_target: Optional[int] = None
+    procid_target: Optional[int] = None
+    flow: Optional[int] = None
+    stream: Optional[int] = None
+    dump_file: Optional[str] = None
+    resource: Optional[str] = None
+    yara_rule: Optional[str] = None
 
 
 class Signature(BaseModel):
     """A Yara rule hit."""
 
-    label: Optional[str]
-    name: Optional[str]
-    score: Optional[int]
-    ttp: Optional[list[str]]
-    tags: Optional[list[str]]
-    indicators: Optional[list[Indicator]]
-    yara_rule: Optional[str]
-    desc: Optional[str]
-    url: Optional[str]
+    label: Optional[str] = None
+    name: Optional[str] = None
+    score: Optional[int] = None
+    ttp: Optional[list[str]] = None
+    tags: Optional[list[str]] = None
+    indicators: Optional[list[Indicator]] = None
+    yara_rule: Optional[str] = None
+    desc: Optional[str] = None
+    url: Optional[str] = None
 
 
 class OverviewIOCs(BaseModel):
     """An overview of the IOCs observed during analysis."""
 
-    urls: Optional[list[str]]
-    domains: Optional[list[str]]
-    ips: Optional[list[str]]
+    urls: Optional[list[str]] = None
+    domains: Optional[list[str]] = None
+    ips: Optional[list[str]] = None
 
 
 class Credentials(BaseModel):
     """Credentials captured during analysis."""
 
-    pass_: str
-    flow: Optional[int]
-    protocol: Optional[str]
-    host: Optional[str]
-    port: Optional[int]
     user: str
-    email_to: Optional[str]
+    pass_: str = Field(alias="pass")
+    flow: Optional[int] = None
+    protocol: Optional[str] = None
+    host: Optional[str] = None
+    port: Optional[int] = None
+    email_to: Optional[str] = None
 
     @classmethod
     def parse_obj(cls, obj: Any) -> "Credentials":
         """A custom parsing method to read in "pass" from a dict.
         
         Mostly copies `BaseModel.parse_obj`.
         """
@@ -272,129 +272,129 @@
     key: str
     value: Any
 
 
 class Config(BaseModel):
     """A malware samples's configuration extracted during analysis."""
 
-    family: Optional[str]
-    tags: Optional[list[str]]
-    rule: Optional[str]
-    c2: Optional[list[str]]
-    version: Optional[str]
-    botnet: Optional[str]
-    campaign: Optional[str]
-    mutex: Optional[list[str]]
-    decoy: Optional[list[str]]
-    wallet: Optional[list[str]]
-    dns: Optional[list[str]]
-    keys: Optional[list[Key]]
-    webinject: Optional[list[str]]
-    command_lines: Optional[list[str]]
-    listen_addr: Optional[str]
-    listen_port: Optional[int]
-    listen_for: Optional[list[str]]
-    shellcode: Optional[list[bytes]]
-    extracted_pe: Optional[list[str]]
-    credentials: Optional[list[Credentials]]
-    attr: Optional[dict]
-    raw: Optional[str]
+    family: Optional[str] = None
+    tags: Optional[list[str]] = None
+    rule: Optional[str] = None
+    c2: Optional[list[str]] = None
+    version: Optional[str] = None
+    botnet: Optional[str] = None
+    campaign: Optional[str] = None
+    mutex: Optional[list[str]] = None
+    decoy: Optional[list[str]] = None
+    wallet: Optional[list[str]] = None
+    dns: Optional[list[str]] = None
+    keys: Optional[list[Key]] = None
+    webinject: Optional[list[str]] = None
+    command_lines: Optional[list[str]] = None
+    listen_addr: Optional[str] = None
+    listen_port: Optional[int] = None
+    listen_for: Optional[list[str]] = None
+    shellcode: Optional[list[bytes]] = None
+    extracted_pe: Optional[list[str]] = None
+    credentials: Optional[list[Credentials]] = None
+    attr: Optional[dict] = None
+    raw: Optional[str] = None
 
 
 class Ransom(BaseModel):
     """A ransomware note observed during analysis."""
 
-    family: Optional[str]
-    target: Optional[str]
-    emails: Optional[list[str]]
-    wallets: Optional[list[str]]
-    urls: Optional[list[str]]
-    contact: Optional[list[str]]
     note: str
+    family: Optional[str] = None
+    target: Optional[str] = None
+    emails: Optional[list[str]] = None
+    wallets: Optional[list[str]] = None
+    urls: Optional[list[str]] = None
+    contact: Optional[list[str]] = None
 
 
 class DropperURL(BaseModel):
     """A URL used by a dropper."""
 
     type: str
     url: str
 
 
 class Dropper(BaseModel):
     """A malware that downloads other malware."""
 
-    family: Optional[str]
     language: str
-    source: Optional[str]
-    deobfuscated: Optional[str]
     urls: list[DropperURL]
+    family: Optional[str] = None
+    source: Optional[str] = None
+    deobfuscated: Optional[str] = None
 
 
 class OverviewTarget(BaseModel):
     """A summary of the target (analyzed object) and findings."""
 
     tasks: list[str]
-    id: Optional[str]
-    score: Optional[int]
-    submitted: Optional[datetime.datetime]
-    completed: Optional[datetime.datetime]
-    target: Optional[str]
-    pick: Optional[str]
-    type: Optional[str]
-    size: Optional[int]
-    md5: Optional[str]
-    sha1: Optional[str]
-    sha256: Optional[str]
-    sha512: Optional[str]
-    filetype: Optional[str]
-    static_tags: Optional[list[str]]
-    tags: Optional[list[str]]
-    family: Optional[list[str]]
-    signatures: list[Signature]
-    iocs: Optional[OverviewIOCs]
+    id: Optional[str] = None
+    score: Optional[int] = None
+    submitted: Optional[datetime.datetime] = None
+    completed: Optional[datetime.datetime] = None
+    target: Optional[str] = None
+    pick: Optional[str] = None
+    type: Optional[str] = None
+    size: Optional[int] = None
+    md5: Optional[str] = None
+    sha1: Optional[str] = None
+    sha256: Optional[str] = None
+    sha512: Optional[str] = None
+    filetype: Optional[str] = None
+    static_tags: Optional[list[str]] = None
+    tags: Optional[list[str]] = None
+    family: Optional[list[str]] = None
+    signatures: list[Signature] = None
+    iocs: Optional[OverviewIOCs] = None
 
 
 class OverviewExtracted(BaseModel):
     """Collection of data extracted during analysis."""
 
     tasks: list[str]
-    dumped_file: Optional[str]
-    resource: Optional[str]
-    config: Optional[Config]
-    path: Optional[str]
-    ransom_note: Optional[Ransom]
-    dropper: Optional[Dropper]
-    credentials: Optional[Credentials]
+    dumped_file: Optional[str] = None
+    resource: Optional[str] = None
+    config: Optional[Config] = None
+    path: Optional[str] = None
+    ransom_note: Optional[Ransom] = None
+    dropper: Optional[Dropper] = None
+    credentials: Optional[Credentials] = None
 
 
 class OverviewSample(BaseModel):
     """Information on the analyzed sample, very similar to OverviewTarget but w/o tasks."""
 
-    id: Optional[str]
-    score: Optional[int]
-    target: Optional[str]
-    pick: Optional[str]
-    type: Optional[str]
-    size: Optional[int]
-    md5: Optional[str]
-    sha1: Optional[str]
-    sha256: Optional[str]
-    sha512: Optional[str]
-    filetype: Optional[str]
-    static_tags: Optional[list[str]]
-    submitted: Optional[datetime.datetime]
-    created: datetime.datetime
-    completed: datetime.datetime
-    iocs: Optional[OverviewIOCs]
+    id: Optional[str] = None
+    score: Optional[int] = None
+    target: Optional[str] = None
+    pick: Optional[str] = None
+    type: Optional[str] = None
+    size: Optional[int] = None
+    md5: Optional[str] = None
+    sha1: Optional[str] = None
+    sha256: Optional[str] = None
+    sha512: Optional[str] = None
+    filetype: Optional[str] = None
+    static_tags: Optional[list[str]] = None
+    submitted: Optional[datetime.datetime] = None
+    created: Optional[datetime.datetime] = None
+    completed: Optional[datetime.datetime] = None
+    iocs: Optional[OverviewIOCs] = None
 
 
 class OverviewReport(HatchingResponse):
     """The sandbox's overview report for a single sample."""
 
     version: str
     sample: OverviewSample
-    tasks: Optional[list[TaskSummary]]
     analysis: OverviewAnalysis
     targets: list[OverviewTarget]
-    errors: Optional[list[ReportedFailure]]
-    signatures: Optional[list[Signature]]
-    extracted: Optional[list[OverviewExtracted]]
+    tasks: Optional[list[TaskSummary]] = None
+    errors: Optional[list[ReportedFailure]] = None
+    signatures: Optional[list[Signature]] = None
+    extracted: Optional[list[OverviewExtracted]] = None
```

### Comparing `pyhatching-0.1.0/src/pyhatching/enums.py` & `pyhatching-0.2.0/src/pyhatching/enums.py`

 * *Files identical despite different names*

### Comparing `pyhatching-0.1.0/src/pyhatching/errors.py` & `pyhatching-0.2.0/src/pyhatching/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Errors for pyhatching."""
 
 class PyHatchingError(Exception):
     """An error in the pyhatching library."""
 
 
-class PyHatchingValueError(PyHatchingError):
+class PyHatchingFileError(PyHatchingError, OSError):
+    """An error occured while pyhatching was working with a file."""
+
+
+class PyHatchingValueError(PyHatchingError, ValueError):
     """An unexpected value was encountered by pyhatching."""
 
 
 class PyHatchingValidateError(PyHatchingError):
-    """An error validating a pyhatching JSON response."""
+    """An error validating a pyhatching Pydantic object."""
 
 
 class PyHatchingConnError(PyHatchingError):
     """An error occurred at some point during the connection/request to the sandbox.
     
     The base Exception to catch when there's any errors from the sandbox API,
     including when the response body cannot be cast to a dict, when the API
```

### Comparing `pyhatching-0.1.0/src/pyhatching/utils.py` & `pyhatching-0.2.0/src/pyhatching/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     Returns
     -------
     enums.HashPrefixes | None
         Either the name of the hash type or None if the input is not a hash.
     """
 
     if SHA5RE.search(input_hash):
-        return enums.HashPrefixes.SHA5
+        return enums.HashPrefixes.SHA5.value
     if SHA2RE.search(input_hash):
-        return enums.HashPrefixes.SHA2
+        return enums.HashPrefixes.SHA2.value
     if SHA1RE.search(input_hash):
-        return enums.HashPrefixes.SHA1
+        return enums.HashPrefixes.SHA1.value
     if MD5RE.search(input_hash):
-        return enums.HashPrefixes.MD5
+        return enums.HashPrefixes.MD5.value
 
     return None
```

### Comparing `pyhatching-0.1.0/src/pyhatching.egg-info/PKG-INFO` & `pyhatching-0.2.0/src/pyhatching.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhatching
-Version: 0.1.0
+Version: 0.2.0
 Summary: An async Python client for the Hatching Triage Sandbox.
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

