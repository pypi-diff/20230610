# Comparing `tmp/yagooglesearch-1.6.1.tar.gz` & `tmp/yagooglesearch-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yagooglesearch-1.6.1.tar", last modified: Sat Jul 30 22:04:18 2022, max compression
+gzip compressed data, was "yagooglesearch-1.7.0.tar", last modified: Sat Jun 10 20:22:24 2023, max compression
```

## Comparing `yagooglesearch-1.6.1.tar` & `yagooglesearch-1.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/
--rw-rw-r--   0 brennon   (1000) brennon   (1000)     1515 2021-08-25 20:22:21.000000 yagooglesearch-1.6.1/LICENSE
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    10658 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/PKG-INFO
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    10213 2022-01-21 04:52:13.000000 yagooglesearch-1.6.1/README.md
--rw-rw-r--   0 brennon   (1000) brennon   (1000)       38 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/setup.cfg
--rw-rw-r--   0 brennon   (1000) brennon   (1000)      827 2022-07-30 21:59:49.000000 yagooglesearch-1.6.1/setup.py
-drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/yagooglesearch/
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    23523 2022-07-30 21:53:40.000000 yagooglesearch-1.6.1/yagooglesearch/__init__.py
--rw-r--r--   0 brennon   (1000) brennon   (1000)    94251 2021-08-23 21:04:38.000000 yagooglesearch-1.6.1/yagooglesearch/user_agents.txt
-drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/yagooglesearch.egg-info/
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    10658 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/yagooglesearch.egg-info/PKG-INFO
--rw-rw-r--   0 brennon   (1000) brennon   (1000)      273 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/yagooglesearch.egg-info/SOURCES.txt
--rw-rw-r--   0 brennon   (1000) brennon   (1000)        1 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/yagooglesearch.egg-info/dependency_links.txt
--rw-rw-r--   0 brennon   (1000) brennon   (1000)       55 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/yagooglesearch.egg-info/requires.txt
--rw-rw-r--   0 brennon   (1000) brennon   (1000)       15 2022-07-30 22:04:18.000000 yagooglesearch-1.6.1/yagooglesearch.egg-info/top_level.txt
+drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)     1515 2021-08-25 20:22:21.000000 yagooglesearch-1.7.0/LICENSE
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    10959 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/PKG-INFO
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    10494 2023-06-10 19:53:41.000000 yagooglesearch-1.7.0/README.md
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)       38 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/setup.cfg
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)      827 2023-06-10 20:20:26.000000 yagooglesearch-1.7.0/setup.py
+drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/yagooglesearch/
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    24042 2023-06-10 19:53:41.000000 yagooglesearch-1.7.0/yagooglesearch/__init__.py
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    94251 2021-08-23 21:04:38.000000 yagooglesearch-1.7.0/yagooglesearch/user_agents.txt
+drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/yagooglesearch.egg-info/
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    10959 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/PKG-INFO
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)      273 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/SOURCES.txt
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)        1 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/dependency_links.txt
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)       55 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/requires.txt
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)       15 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yagooglesearch-1.6.1/LICENSE` & `yagooglesearch-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yagooglesearch-1.6.1/PKG-INFO` & `yagooglesearch-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: yagooglesearch
-Version: 1.6.1
+Version: 1.7.0
 Summary: A Python library for executing intelligent, realistic-looking, and tunable Google searches.
 Home-page: https://github.com/opsdisk/yagooglesearch
 Author: Brennon Thomas
 Author-email: info@opsdisk.com
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: python google search googlesearch
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yagooglesearch - Yet another googlesearch
 
 ## Overview
@@ -251,14 +252,19 @@
     urls_list = client.search()
 
     print(urls_list)
 
     proxy_rotation_index += 1
 ```
 
+## GOOGLE_ABUSE_EXEMPTION cookie
+
+If you have a `GOOGLE_ABUSE_EXEMPTION` cookie value, it can be passed into `google_exemption` when instantiating the
+`SearchClient` object.
+
 ## &tbs= URL filter clarification
 
 The `&tbs=` parameter is used to specify either verbatim or time-based filters.
 
 ### Verbatim search
 
 ```none
@@ -300,7 +306,10 @@
 
 * [Mario Vilas](https://github.com/MarioVilas) for his amazing work on the original
   [googlesearch](https://github.com/MarioVilas/googlesearch) library.
 
 ## Contributors
 
 * [KennBro](https://github.com/KennBro) - <https://github.com/opsdisk/yagooglesearch/pull/9>
+* [ArshansGithub](https://github.com/ArshansGithub) - <https://github.com/opsdisk/yagooglesearch/pull/21>
+
+
```

### Comparing `yagooglesearch-1.6.1/README.md` & `yagooglesearch-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,19 @@
     urls_list = client.search()
 
     print(urls_list)
 
     proxy_rotation_index += 1
 ```
 
+## GOOGLE_ABUSE_EXEMPTION cookie
+
+If you have a `GOOGLE_ABUSE_EXEMPTION` cookie value, it can be passed into `google_exemption` when instantiating the
+`SearchClient` object.
+
 ## &tbs= URL filter clarification
 
 The `&tbs=` parameter is used to specify either verbatim or time-based filters.
 
 ### Verbatim search
 
 ```none
@@ -287,7 +292,8 @@
 
 * [Mario Vilas](https://github.com/MarioVilas) for his amazing work on the original
   [googlesearch](https://github.com/MarioVilas/googlesearch) library.
 
 ## Contributors
 
 * [KennBro](https://github.com/KennBro) - <https://github.com/opsdisk/yagooglesearch/pull/9>
+* [ArshansGithub](https://github.com/ArshansGithub) - <https://github.com/opsdisk/yagooglesearch/pull/21>
```

### Comparing `yagooglesearch-1.6.1/setup.py` & `yagooglesearch-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yagooglesearch",
-    version="1.6.1",
+    version="1.7.0",
     author="Brennon Thomas",
     author_email="info@opsdisk.com",
     description="A Python library for executing intelligent, realistic-looking, and tunable Google searches.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/opsdisk/yagooglesearch",
     packages=setuptools.find_packages(),
     package_data={"yagooglesearch": ["user_agents.txt"]},
     install_requires=[
         "beautifulsoup4>=4.9.3",
-        "requests>=2.26.0",
+        "requests>=2.31.0",
         "requests[socks]",
     ],
     python_requires=">=3.6",
     license='BSD 3-Clause "New" or "Revised" License',
     keywords="python google search googlesearch",
 )
```

### Comparing `yagooglesearch-1.6.1/yagooglesearch/__init__.py` & `yagooglesearch-1.7.0/yagooglesearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Third party Python libraries.
 from bs4 import BeautifulSoup
 import requests
 
 # Custom Python libraries.
 
-__version__ = "1.6.1"
+__version__ = "1.7.0"
 
 # Logging
 ROOT_LOGGER = logging.getLogger("yagooglesearch")
 # ISO 8601 datetime format by default.
 LOG_FORMATTER = logging.Formatter("%(asctime)s [%(threadName)-12.12s] [%(levelname)s] %(message)s")
 
 # Setup file logging.
@@ -82,16 +82,16 @@
         yagooglesearch_manages_http_429s=True,
         http_429_cool_off_time_in_minutes=60,
         http_429_cool_off_factor=1.1,
         proxy="",
         verify_ssl=True,
         verbosity=5,
         verbose_output=False,
+        google_exemption=None,
     ):
-
         """
         SearchClient
         :param str query: Query string.  Must NOT be url-encoded.
         :param str tld: Top level domain.
         :param str lang: Language.
         :param str tbs: Verbatim search or time limits (e.g., "qdr:h" => last hour, "qdr:d" => last 24 hours, "qdr:m"
             => last month).
@@ -114,14 +114,16 @@
         :param float http_429_cool_off_factor: Factor to multiply by http_429_cool_off_time_in_minutes for each HTTP 429
             detected.
         :param str proxy: HTTP(S) or SOCKS5 proxy to use.
         :param bool verify_ssl: Verify the SSL certificate to prevent traffic interception attacks.  Defaults to True.
             This may need to be disabled in some HTTPS proxy instances.
         :param int verbosity: Logging and console output verbosity.
         :param bool verbose_output: False (only URLs) or True (rank, title, description, and URL).  Defaults to False.
+        :param str google_exemption: Google cookie exemption string.  This is a string that Google uses to allow certain
+            google searches. Defaults to None.
 
         :rtype: List of str
         :return: List of URLs found or list of {"rank", "title", "description", "url"}
         """
 
         self.query = urllib.parse.quote_plus(query)
         self.tld = tld
@@ -138,25 +140,30 @@
         self.yagooglesearch_manages_http_429s = yagooglesearch_manages_http_429s
         self.http_429_cool_off_time_in_minutes = http_429_cool_off_time_in_minutes
         self.http_429_cool_off_factor = http_429_cool_off_factor
         self.proxy = proxy
         self.verify_ssl = verify_ssl
         self.verbosity = verbosity
         self.verbose_output = verbose_output
+        self.google_exemption = google_exemption
 
         # Assign log level.
         ROOT_LOGGER.setLevel((6 - self.verbosity) * 10)
 
         # Argument checks.
         if self.num > 100:
             ROOT_LOGGER.warning("The largest value allowed by Google for num is 100.  Setting num to 100.")
             self.num = 100
 
-        # Initialize cookies to None, will be updated with each request in get_page().
-        self.cookies = None
+        # Populate cookies with GOOGLE_ABUSE_EXEMPTION if it is provided.  Otherwise, initialize cookies to None.
+        # It will be updated with each request in get_page().
+        if self.google_exemption:
+            self.cookies = {"GOOGLE_ABUSE_EXEMPTION": self.google_exemption}
+        else:
+            self.cookies = None
 
         # Used later to ensure there are not any URL parameter collisions.
         self.url_parameters = (
             "btnG",
             "cr",
             "hl",
             "num",
@@ -174,15 +181,14 @@
         self.update_urls()
 
         # Initialize proxy_dict.
         self.proxy_dict = {}
 
         # Update proxy_dict if a proxy is provided.
         if proxy:
-
             # Standardize case since the scheme will be checked against a hard-coded list.
             self.proxy = proxy.lower()
 
             urllib_object = urllib.parse.urlparse(self.proxy)
             scheme = urllib_object.scheme
 
             if scheme not in ["http", "https", "socks5", "socks5h"]:
@@ -317,15 +323,20 @@
 
         headers = {
             "User-Agent": self.user_agent,
         }
 
         ROOT_LOGGER.info(f"Requesting URL: {url}")
         response = requests.get(
-            url, proxies=self.proxy_dict, headers=headers, cookies=self.cookies, timeout=15, verify=self.verify_ssl
+            url,
+            proxies=self.proxy_dict,
+            headers=headers,
+            cookies=self.cookies,
+            timeout=15,
+            verify=self.verify_ssl,
         )
 
         # Update the cookies.
         self.cookies = response.cookies
 
         # Extract the HTTP response code.
         http_response_code = response.status_code
@@ -337,15 +348,14 @@
         ROOT_LOGGER.debug(f"    proxy: {self.proxy}")
         ROOT_LOGGER.debug(f"    verify_ssl: {self.verify_ssl}")
 
         # Google throws up a consent page for searches sourcing from a European Union country IP location.
         # See https://github.com/benbusby/whoogle-search/issues/311
         try:
             if response.cookies["CONSENT"].startswith("PENDING+"):
-
                 ROOT_LOGGER.warning(
                     "Looks like your IP address is sourcing from a European Union location...your search results may "
                     "vary, but I'll try and work around this by updating the cookie."
                 )
 
                 # Convert the cookiejar data structure to a Python dict.
                 cookie_dict = requests.utils.dict_from_cookiejar(self.cookies)
@@ -377,15 +387,14 @@
 
         html = ""
 
         if http_response_code == 200:
             html = response.text
 
         elif http_response_code == 429:
-
             ROOT_LOGGER.warning("Google is blocking your IP for making too many requests in a specific time period.")
 
             # Calling script does not want yagooglesearch to handle HTTP 429 cool off and retry.  Just return a
             # notification string.
             if not self.yagooglesearch_manages_http_429s:
                 ROOT_LOGGER.info("Since yagooglesearch_manages_http_429s=False, yagooglesearch is done.")
                 return "HTTP_429_DETECTED"
@@ -427,15 +436,14 @@
 
         # Simulates browsing to the https://www.google.com home page and retrieving the initial cookie.
         html = self.get_page(self.url_home)
 
         # Loop until we reach the maximum result results found or there are no more search results found to reach
         # max_search_result_urls_to_return.
         while total_valid_links_found <= self.max_search_result_urls_to_return:
-
             ROOT_LOGGER.info(
                 f"Stats: start={self.start}, num={self.num}, total_valid_links_found={total_valid_links_found} / "
                 f"max_search_result_urls_to_return={self.max_search_result_urls_to_return}"
             )
 
             # Prepare the URL for the search request.
             if self.start:
@@ -480,29 +488,27 @@
                 anchors = soup.find_all("a")
 
             # Tracks number of valid URLs found on a search page.
             valid_links_found_in_this_search = 0
 
             # Process every anchored URL.
             for a in anchors:
-
                 # Get the URL from the anchor tag.
                 try:
                     link = a["href"]
                 except KeyError:
                     ROOT_LOGGER.warning(f"No href for link: {link}")
                     continue
 
                 # Filter invalid links and links pointing to Google itself.
                 link = self.filter_search_result_urls(link)
                 if not link:
                     continue
 
                 if self.verbose_output:
-
                     # Extract the URL title.
                     try:
                         title = a.get_text()
                     except Exception:
                         ROOT_LOGGER.warning(f"No title for link: {link}")
                         title = ""
 
@@ -516,15 +522,14 @@
 
                     except Exception:
                         ROOT_LOGGER.warning(f"No description for link: {link}")
                         description = ""
 
                 # Check if URL has already been found.
                 if link not in self.search_result_list:
-
                     # Increase the counters.
                     valid_links_found_in_this_search += 1
                     total_valid_links_found += 1
 
                     ROOT_LOGGER.info(f"Found unique URL #{total_valid_links_found}: {link}")
 
                     if self.verbose_output:
```

### Comparing `yagooglesearch-1.6.1/yagooglesearch/user_agents.txt` & `yagooglesearch-1.7.0/yagooglesearch/user_agents.txt`

 * *Files identical despite different names*

### Comparing `yagooglesearch-1.6.1/yagooglesearch.egg-info/PKG-INFO` & `yagooglesearch-1.7.0/yagooglesearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: yagooglesearch
-Version: 1.6.1
+Version: 1.7.0
 Summary: A Python library for executing intelligent, realistic-looking, and tunable Google searches.
 Home-page: https://github.com/opsdisk/yagooglesearch
 Author: Brennon Thomas
 Author-email: info@opsdisk.com
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: python google search googlesearch
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yagooglesearch - Yet another googlesearch
 
 ## Overview
@@ -251,14 +252,19 @@
     urls_list = client.search()
 
     print(urls_list)
 
     proxy_rotation_index += 1
 ```
 
+## GOOGLE_ABUSE_EXEMPTION cookie
+
+If you have a `GOOGLE_ABUSE_EXEMPTION` cookie value, it can be passed into `google_exemption` when instantiating the
+`SearchClient` object.
+
 ## &tbs= URL filter clarification
 
 The `&tbs=` parameter is used to specify either verbatim or time-based filters.
 
 ### Verbatim search
 
 ```none
@@ -300,7 +306,10 @@
 
 * [Mario Vilas](https://github.com/MarioVilas) for his amazing work on the original
   [googlesearch](https://github.com/MarioVilas/googlesearch) library.
 
 ## Contributors
 
 * [KennBro](https://github.com/KennBro) - <https://github.com/opsdisk/yagooglesearch/pull/9>
+* [ArshansGithub](https://github.com/ArshansGithub) - <https://github.com/opsdisk/yagooglesearch/pull/21>
+
+
```

