# Comparing `tmp/cabinet-2023.6.10.1.tar.gz` & `tmp/cabinet-2023.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.6.10.1.tar", last modified: Sat Jun 10 19:51:08 2023, max compression
+gzip compressed data, was "cabinet-2023.6.8.1.tar", last modified: Fri Jun  9 04:30:15 2023, max compression
```

## Comparing `cabinet-2023.6.10.1.tar` & `cabinet-2023.6.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-10 19:51:08.450486 cabinet-2023.6.10.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.6.10.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6583 2023-06-10 19:51:08.450486 cabinet-2023.6.10.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6231 2023-06-09 04:51:16.000000 cabinet-2023.6.10.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.10.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-10 19:51:08.450486 cabinet-2023.6.10.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-10 19:51:08.446486 cabinet-2023.6.10.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-10 19:51:08.450486 cabinet-2023.6.10.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.10.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.10.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    26253 2023-06-10 19:50:00.000000 cabinet-2023.6.10.1/src/cabinet/cabinet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.10.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-10 19:51:08.450486 cabinet-2023.6.10.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6583 2023-06-10 19:51:08.000000 cabinet-2023.6.10.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-10 19:51:08.000000 cabinet-2023.6.10.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-10 19:51:08.000000 cabinet-2023.6.10.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-10 19:51:08.000000 cabinet-2023.6.10.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-10 19:51:08.000000 cabinet-2023.6.10.1/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-10 19:51:08.450486 cabinet-2023.6.10.1/test/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.10.1/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.6.8.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.8.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.8.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.8.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26147 2023-06-09 04:29:47.000000 cabinet-2023.6.8.1/src/cabinet/cabinet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.8.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/test/test___init__.py
```

### Comparing `cabinet-2023.6.10.1/LICENSE` & `cabinet-2023.6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.6.10.1/PKG-INFO` & `cabinet-2023.6.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.6.10.1
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -237,19 +237,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.10.1/README.md` & `cabinet-2023.6.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -225,19 +225,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.10.1/setup.cfg` & `cabinet-2023.6.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.06.10.1
+version = 2023.06.08.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.6.10.1/src/cabinet/cabinet.py` & `cabinet-2023.6.8.1/src/cabinet/cabinet.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         return logger
 
     def _ifprint(self, message: str, is_print: bool):
         """
         Prints a string if `print` is true.
         """
         if is_print:
-            print(json.dumps(message, indent=2))
+            print(message)
 
     def configure(self):
         """
         Configures the Cabinet instance based on command line arguments or user input.
         """
 
         message = f"""
@@ -468,33 +468,30 @@
         for index, item in enumerate(attribute_max_attribute_index):
             if item not in partition:
                 try:
                     partition[item] = value if index == len(
                         attribute) + maximum_attribute_index - 1 else {}
                     partition = partition[item]
                     self.log(
-                        f"Adding key: {{'{item}': {partition}}} \
-to \"{attribute_max_attribute_index[index-1] if index > 0 else path_full}\"",
+                        f"Adding new key '{item}' to {partition if index > 0 else path_full}",
                         is_quiet=self.new_setup)
                 except TypeError as error:
                     self.log(f"{error}\n\n{attribute[index-1]} is currently a string, so it cannot \
 be treated as an object with multiple properties.", level="error")
             else:
                 if index == len(attribute) + maximum_attribute_index - 1:
                     partition[item] = value
                 else:
                     partition = partition[item]
 
         with open(path_full, 'w+', encoding="utf8") as file:
             json.dump(_settings, file, indent=4)
 
-        self.log(
-            f"{' -> '.join(attribute[:-1])} set to {value}",
-            level='info', is_quiet=not is_print)
-
+        self._ifprint(
+            f"{' -> '.join(attribute[:-1])} set to {value}", is_print)
         return value
 
     def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
                           ignore_not_found: bool = False):
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
```

### Comparing `cabinet-2023.6.10.1/src/cabinet/mail.py` & `cabinet-2023.6.8.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.6.10.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.6.10.1
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -237,19 +237,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.10.1/test/test___init__.py` & `cabinet-2023.6.8.1/test/test___init__.py`

 * *Files identical despite different names*

