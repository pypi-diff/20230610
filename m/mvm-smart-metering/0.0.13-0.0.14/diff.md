# Comparing `tmp/mvm_smart_metering-0.0.13.tar.gz` & `tmp/mvm_smart_metering-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvm_smart_metering-0.0.13.tar", max compression
+gzip compressed data, was "mvm_smart_metering-0.0.14.tar", max compression
```

## Comparing `mvm_smart_metering-0.0.13.tar` & `mvm_smart_metering-0.0.14.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      286 2023-02-28 08:41:47.758152 mvm_smart_metering-0.0.13/README.md
--rw-r--r--   0        0        0       78 2023-02-28 08:41:47.758152 mvm_smart_metering-0.0.13/mvm_smart_meter/__init__.py
--rw-r--r--   0        0        0    16040 2023-02-28 08:41:47.758152 mvm_smart_metering-0.0.13/mvm_smart_meter/smart_meter.py
--rw-r--r--   0        0        0      506 2023-02-28 08:41:47.758152 mvm_smart_metering-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.13/setup.py
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0      286 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/README.md
+-rw-r--r--   0        0        0       78 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/mvm_smart_meter/__init__.py
+-rw-r--r--   0        0        0    16148 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/mvm_smart_meter/smart_meter.py
+-rw-r--r--   0        0        0      501 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.14/setup.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.14/PKG-INFO
```

### Comparing `mvm_smart_metering-0.0.13/mvm_smart_meter/smart_meter.py` & `mvm_smart_metering-0.0.14/mvm_smart_meter/smart_meter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,42 +4,41 @@
 import json
 from datetime import datetime, timedelta
 
 
 from requestium import Session, Keys
 from selenium import webdriver
 from webdriver_manager.firefox import GeckoDriverManager
+from selenium.webdriver.firefox.service import Service
 from selenium.webdriver.firefox.options import Options
 import pandas
 import io
 
 
 class Smart_meter:
     """All the main function to gather date from the smart metering site is gathered here"""
 
     def __init__(self, username: str, password: str):
         self.options = Options()
         self.options.add_argument("--headless")
 
-        gecko_driver_path = os.getenv("GECKO_DRIVER_PATH")
+        agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0"
+        self.options.set_preference("general.useragent.override", agent)
 
-        if gecko_driver_path is None:
-            gecko_executable_path = GeckoDriverManager().install()
-        else:
+        if gecko_driver_path := os.getenv("GECKO_DRIVER_PATH"):
             gecko_executable_path = gecko_driver_path
 
+        else:
+            gecko_executable_path = GeckoDriverManager().install()
+        self.service = Service(executable_path=gecko_executable_path)
         self.firefox_driver = webdriver.Firefox(
-            executable_path=gecko_executable_path, options=self.options
+            service=self.service, options=self.options
         )
+
         self.s = Session(driver=self.firefox_driver)
-        self.s.headers.update(
-            {
-                "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/109.0"
-            }
-        )
         self.base_url = "https://eloszto.mvmemaszhalozat.hu"
         self.username = username
         self.password = password
 
     def get_base_cookies(self):
         """Gets cookies from the main site to be used for later"""
         r = self.s.get(self.base_url)
@@ -113,26 +112,29 @@
         """The smart metering site is on a external site, this function gets thoose links into a list."""
         custumer_meters_url = f"https://eloszto.mvmemaszhalozat.hu/sap/opu/odata/sap/ZGW_UGYFELSZOLGALAT_SRV/Felhelyek(Vevo='{self.custumer_number}',Id='{self.customer_id}')/Okosmero"
         querystring = {"sap-client": "112", "sap-language": "HU"}
         r = self.s.get(custumer_meters_url, headers=self.headers, params=querystring)
         r_list = r.json()["d"]["results"]
         self.meter_ids = r.json()["d"]["results"]
         self.smart_meter_links = []
-
+        print(r_list)
         for link in r_list:
+  
             if link["URL"].find("guid=&") == -1:
                 split_url = link["URL"].split("?")
                 query_string = split_url[1]
 
                 query_string_list = query_string.split("&")
 
                 query_dict = {"url": split_url[0], "meter_id": link["FogyMeroAzon"]}
+  
                 for item in query_string_list:
                     key, value = item.split("=")
                     query_dict[key] = value
+    
                 self.smart_meter_links.append(query_dict)
 
     def get_cookies_smart_meter_site(self):
         """Get cookies from the main site.Need to find a workaround as requestium uses old version of selenium."""
         # TODO get around without using selenium
 
         self.smart_meter_url = f"{self.smart_meter_links[0]['url']}"
```

### Comparing `mvm_smart_metering-0.0.13/setup.py` & `mvm_smart_metering-0.0.14/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 ['mvm_smart_meter']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.11.1,<5.0.0',
- 'pandas>=1.5.3,<2.0.0',
- 'python-dotenv>=0.21.1,<0.22.0',
- 'requestium>=0.1.15,<0.2.0',
+ 'pandas==2.0.2',
+ 'python-dotenv==1.0.0',
+ 'requestium==0.2.1',
  'requests>=2.28.2,<3.0.0',
  'webdriver-manager>=3.8.5,<4.0.0']
 
 setup_kwargs = {
     'name': 'mvm-smart-metering',
-    'version': '0.0.13',
+    'version': '0.0.14',
     'description': 'Script for scraping mvm smart meter data',
     'long_description': '# MVM Smart Metering\nThis is a automation tool for collecting load curve from mvm smart metering site\n\n---\n\nInstallation:\n\n```bash\npip install mvm-smart-metering\n```\n\nor\n\n```bash\npoetry add mvm-smart-metering\n```\n\n\n\n[Documantion](https://ktomi96.github.io/mvm_smart_metering/)\n\n---\n\n\n\n\n',
     'author': 'ktomi96',
     'author_email': 'kokai.tamas.96@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.11,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mvm_smart_metering-0.0.13/PKG-INFO` & `mvm_smart_metering-0.0.14/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: mvm-smart-metering
-Version: 0.0.13
+Version: 0.0.14
 Summary: Script for scraping mvm smart meter data
 Author: ktomi96
 Author-email: kokai.tamas.96@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
-Requires-Dist: requestium (>=0.1.15,<0.2.0)
+Requires-Dist: pandas (==2.0.2)
+Requires-Dist: python-dotenv (==1.0.0)
+Requires-Dist: requestium (==0.2.1)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: webdriver-manager (>=3.8.5,<4.0.0)
 Description-Content-Type: text/markdown
 
 # MVM Smart Metering
 This is a automation tool for collecting load curve from mvm smart metering site
```

