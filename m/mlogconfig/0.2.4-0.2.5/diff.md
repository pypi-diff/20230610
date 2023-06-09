# Comparing `tmp/mlogconfig-0.2.4.tar.gz` & `tmp/mlogconfig-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlogconfig-0.2.4.tar", max compression
+gzip compressed data, was "mlogconfig-0.2.5.tar", max compression
```

## Comparing `mlogconfig-0.2.4.tar` & `mlogconfig-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/LICENSE.md
--rw-r--r--   0        0        0     2614 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/README.md
--rw-r--r--   0        0        0     3145 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/mlogconfig/mlogconfig.py
--rw-r--r--   0        0        0      901 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/mlogconfig/modules/validate.py
--rw-r--r--   0        0        0      557 2023-06-09 21:42:01.078083 mlogconfig-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 mlogconfig-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-06-09 22:22:53.696492 mlogconfig-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0     2614 2023-06-09 22:22:53.696492 mlogconfig-0.2.5/README.md
+-rw-r--r--   0        0        0     3487 2023-06-09 22:22:53.696492 mlogconfig-0.2.5/mlogconfig/mlogconfig.py
+-rw-r--r--   0        0        0      901 2023-06-09 22:22:53.696492 mlogconfig-0.2.5/mlogconfig/modules/validate.py
+-rw-r--r--   0        0        0      557 2023-06-09 22:23:08.976701 mlogconfig-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 mlogconfig-0.2.5/PKG-INFO
```

### Comparing `mlogconfig-0.2.4/LICENSE.md` & `mlogconfig-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.4/README.md` & `mlogconfig-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.4/mlogconfig/mlogconfig.py` & `mlogconfig-0.2.5/mlogconfig/mlogconfig.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,21 @@
     console_logging: bool = False,
     syslog_logging: bool = False,
     log_level: Union[int, str] = logging.INFO,
     file_mode: str = "a",
 ) -> None:
     """
     Sets up logging configuration for an application.
+
+    :param file_path: Path to the log file.
+    :param error_log_file_path: Path to the error log file.
+    :param console_logging: Whether to enable logging to console.
+    :param syslog_logging: Whether to enable logging to syslog.
+    :param log_level: Logging level to use.
+    :param file_mode: File mode to use when opening log files.
     """
     file_handler, file_path = validate_file(file_path, mode=file_mode)
 
     root_logger = getLogger()
     root_logger.setLevel(log_level)
 
     format_str = "%(asctime)s - %(levelname)s: %(message)s"
```

### Comparing `mlogconfig-0.2.4/mlogconfig/modules/validate.py` & `mlogconfig-0.2.5/mlogconfig/modules/validate.py`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.4/pyproject.toml` & `mlogconfig-0.2.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlogconfig"
-version = "v0.2.4"
+version = "v0.2.5"
 description = "This module provides a configurable logging setup for Python applications. It supports logging to console, file, syslog (for Linux and macOS), and Windows Event Log. The user can enable or disable each logging method as needed."
 authors = ["Matt <matt@mattwyen.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `mlogconfig-0.2.4/PKG-INFO` & `mlogconfig-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlogconfig
-Version: 0.2.4
+Version: 0.2.5
 Summary: This module provides a configurable logging setup for Python applications. It supports logging to console, file, syslog (for Linux and macOS), and Windows Event Log. The user can enable or disable each logging method as needed.
 License: MIT
 Author: Matt
 Author-email: matt@mattwyen.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

