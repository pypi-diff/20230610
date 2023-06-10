# Comparing `tmp/hstsparser-1.1.9.tar.gz` & `tmp/hstsparser-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstsparser-1.1.9.tar", max compression
+gzip compressed data, was "hstsparser-1.2.0.tar", max compression
```

## Comparing `hstsparser-1.1.9.tar` & `hstsparser-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-06-03 23:16:54.445967 hstsparser-1.1.9/LICENSE
--rw-r--r--   0        0        0     3180 2023-06-03 23:16:54.445967 hstsparser-1.1.9/README.md
--rwxr-xr-x   0        0        0     7678 2023-06-03 23:16:54.449967 hstsparser-1.1.9/hstsparser.py
--rw-r--r--   0        0        0     1407 2023-06-03 23:17:17.338171 hstsparser-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     4086 1970-01-01 00:00:00.000000 hstsparser-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-10 13:42:01.762057 hstsparser-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3180 2023-06-10 13:42:01.762057 hstsparser-1.2.0/README.md
+-rwxr-xr-x   0        0        0     8252 2023-06-10 13:42:01.762057 hstsparser-1.2.0/hstsparser.py
+-rw-r--r--   0        0        0     1407 2023-06-10 13:42:25.506419 hstsparser-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4086 1970-01-01 00:00:00.000000 hstsparser-1.2.0/PKG-INFO
```

### Comparing `hstsparser-1.1.9/LICENSE` & `hstsparser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hstsparser-1.1.9/README.md` & `hstsparser-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hstsparser-1.1.9/hstsparser.py` & `hstsparser-1.2.0/hstsparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,32 @@
 def date_round(date: datetime.datetime) -> datetime.datetime:
     """Round `datetime` object"""
     return date - datetime.timedelta(
         minutes=date.minute % 10, seconds=date.second, microseconds=date.microsecond
     )
 
 
+def parse_chrome_record(data: dict, database: list, host: str, args: Namespace) -> None:
+    if "expect_ct" not in data:
+        if bool(data["sts_include_subdomains"]):
+            subdomains = "Yes"
+        else:
+            subdomains = "No"
+        record = [
+            host,
+            datetime.datetime.fromtimestamp(data["expiry"]),
+            subdomains,
+            datetime.datetime.fromtimestamp(data["sts_observed"]),
+        ]
+        if args.csv_file:
+            record[1] = date_round(record[1])
+            record[3] = date_round(record[3])
+        database.append(record)
+
+
 parser = ArgumentParser(prog="hstsparser", description="Process HSTS databases")
 parser.add_argument(
     dest="database_file",
     help="The path to the database to be processed",
     metavar="FILE",
     type=lambda x: is_valid_file(parser, x),
 )
@@ -133,15 +151,15 @@
 group.add_argument("--chrome", action="store_true", help="Process a Chrome database")
 
 try:
     __version__ = importlib.metadata.version("hstsparser")
 except importlib.metadata.PackageNotFoundError:
     __version__ = "0.0.1"
 
-parser.add_argument('--version', action='version', version=f'%(prog)s {__version__}')
+parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
 
 
 def main() -> None:
     """Entry point for command line alias."""
     args = parser.parse_args()
 
     dirtydb = args.database_file.read()
@@ -173,31 +191,32 @@
             args,
             database,
             ["URL", "Visits", "Last Accessed", "Expiry", "Type", "Include Subdomains"],
         )
 
     if args.chrome:
         dirtydb = json.loads(dirtydb)
-        for i in dirtydb:
-            current = dirtydb[i]
-            if "expect_ct" not in current:
-                if bool(current["sts_include_subdomains"]):
-                    subdomains = "Yes"
-                else:
-                    subdomains = "No"
-                record = [
-                    i,
-                    datetime.datetime.fromtimestamp(current["expiry"]),
-                    subdomains,
-                    datetime.datetime.fromtimestamp(current["sts_observed"]),
-                ]
-                if args.csv_file:
-                    record[1] = date_round(record[1])
-                    record[3] = date_round(record[3])
-                database.append(record)
+
+        # v1 of this file did not specify a version number
+        chrome_version: int = dirtydb.get("version", 1)
+
+        match chrome_version:
+            case 1:
+                for i in dirtydb:
+                    parse_chrome_record(dirtydb[i], database, i, args)
+            case 2:
+                for i in dirtydb.get("sts", []):
+                    parse_chrome_record(i, database, i.get("host", ""), args)
+            case _:
+                print(
+                    "Unrecognised Chrome file version. "
+                    "Please raise an issue on https://github.com/thebeanogamer/hstsparser"
+                )
+                raise NotImplementedError
+
         if args.wordlist_file:
             wordlist = args.wordlist_file.read().splitlines()
             rainbow = []
             for i in wordlist:
                 rainbow.append(convert_domain(i))
             for i in database:
                 for j in range(0, len(rainbow)):
```

### Comparing `hstsparser-1.1.9/pyproject.toml` & `hstsparser-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstsparser"
-version = "1.1.9"
+version = "1.2.0"
 description = "A tool to parse Firefox and Chrome HSTS databases into forensic artifacts."
 authors = ["Daniel Milnes <daniel@daniel-milnes.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thebeanogamer/hstsparser"
 repository = "https://github.com/thebeanogamer/hstsparser"
 documentation = "https://github.com/thebeanogamer/hstsparser"
```

### Comparing `hstsparser-1.1.9/PKG-INFO` & `hstsparser-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstsparser
-Version: 1.1.9
+Version: 1.2.0
 Summary: A tool to parse Firefox and Chrome HSTS databases into forensic artifacts.
 Home-page: https://github.com/thebeanogamer/hstsparser
 License: MIT
 Keywords: chrome,firefox,dfir,forensics,hsts
 Author: Daniel Milnes
 Author-email: daniel@daniel-milnes.uk
 Requires-Python: >=3.9
```

