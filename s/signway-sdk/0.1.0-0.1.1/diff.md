# Comparing `tmp/signway_sdk-0.1.0.tar.gz` & `tmp/signway_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signway_sdk-0.1.0.tar", max compression
+gzip compressed data, was "signway_sdk-0.1.1.tar", max compression
```

## Comparing `signway_sdk-0.1.0.tar` & `signway_sdk-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      144 2023-06-10 16:06:18.711836 signway_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      387 2023-06-10 16:34:50.648845 signway_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-10 16:24:52.074709 signway_sdk-0.1.0/signway_sdk/__init__.py
--rw-r--r--   0        0        0     1471 2023-06-10 16:23:13.302904 signway_sdk-0.1.0/signway_sdk/sign_url.py
--rw-r--r--   0        0        0     3258 2023-06-02 06:44:04.166807 signway_sdk-0.1.0/signway_sdk/signing_functions.py
--rw-r--r--   0        0        0      832 2023-06-10 16:23:13.315819 signway_sdk-0.1.0/signway_sdk/test_sing_url.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 signway_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      428 2023-06-10 17:21:05.475214 signway_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0      404 2023-06-10 17:21:19.827099 signway_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/__init__.py
+-rw-r--r--   0        0        0     1471 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/sign_url.py
+-rw-r--r--   0        0        0     3292 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/signing_functions.py
+-rw-r--r--   0        0        0      839 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/test_sing_url.py
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 signway_sdk-0.1.1/PKG-INFO
```

### Comparing `signway_sdk-0.1.0/signway_sdk/sign_url.py` & `signway_sdk-0.1.1/signway_sdk/sign_url.py`

 * *Files identical despite different names*

### Comparing `signway_sdk-0.1.0/signway_sdk/signing_functions.py` & `signway_sdk-0.1.1/signway_sdk/signing_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,20 @@
     headers_list = []
     for k in headers:
         headers_list.append(k.lower())
     headers_list.sort()
     return ';'.join(headers_list)
 
 
-def canonical_request(method: str, url: str, headers: dict[str, str], body: str) -> str:
+def canonical_request(
+        method: str,
+        url: str,
+        headers: dict[str, str],
+        body: str
+) -> str:
     return f"{method}\n" \
            f"{canonical_uri_string(url)}\n" \
            f"{canonical_query_string(url)}\n" \
            f"{canonical_header_string(headers)}\n\n" \
            f"{signed_header_string(headers)}\n" \
            f"{body}"
```

### Comparing `signway_sdk-0.1.0/signway_sdk/test_sing_url.py` & `signway_sdk-0.1.1/signway_sdk/test_sing_url.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         expiry=600,
         method='POST',
         host='http://localhost:3000',
         proxy_url='https://github.com/',
         datetime_override=datetime.utcfromtimestamp(0)
     )
 
-    assert url == f'http://localhost:3000/' \
+    assert url == 'http://localhost:3000/' \
                   '?X-Sw-Algorithm=SW1-HMAC-SHA256' \
                   '&X-Sw-Credential=foo%2F19700101' \
                   '&X-Sw-Date=19700101T000000Z' \
                   '&X-Sw-Expires=600' \
                   '&X-Sw-Proxy=https%3A%2F%2Fgithub.com%2F' \
                   '&X-Sw-SignedHeaders=' \
                   '&X-Sw-Body=false' \
-                  '&X-Sw-Signature=ed15db76d806155fd5119e093a0f030063c90d943dfdd27e011a9044a77a90a6'
+                  '&X-Sw-Signature=ed15db76d806155fd5119e093a0f030063c90d943dfdd27e011a9044a77a90a6'  # noqa
```

