# Comparing `tmp/crossfiledialog-0.1.1.tar.gz` & `tmp/crossfiledialog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossfiledialog-0.1.1.tar", last modified: Mon Jan 31 20:11:21 2022, max compression
+gzip compressed data, was "crossfiledialog-0.1.2.tar", last modified: Sat Jun 10 11:37:08 2023, max compression
```

## Comparing `crossfiledialog-0.1.1.tar` & `crossfiledialog-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2022-01-31 20:11:21.382603 crossfiledialog-0.1.1/
--rw-r--r--   0 maikel    (1000) maikel    (1000)      871 2022-01-31 20:11:21.382603 crossfiledialog-0.1.1/PKG-INFO
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2022-01-31 20:11:21.382603 crossfiledialog-0.1.1/crossfiledialog/
--rw-r--r--   0 maikel    (1000) maikel    (1000)       39 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/crossfiledialog/__init__.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)      117 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/crossfiledialog/exceptions.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     2339 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/crossfiledialog/kdialog.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)      157 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/crossfiledialog/strings.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     2708 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/crossfiledialog/win32.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     1005 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/crossfiledialog/wrapper.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     2308 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/crossfiledialog/zenity.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)       62 2022-01-31 20:08:46.928306 crossfiledialog-0.1.1/setup.cfg
--rw-r--r--   0 maikel    (1000) maikel    (1000)     1103 2022-01-31 20:08:56.496449 crossfiledialog-0.1.1/setup.py
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-10 11:37:07.997761 crossfiledialog-0.1.2/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)    32473 2022-01-31 20:08:46.000000 crossfiledialog-0.1.2/LICENSE
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1465 2023-06-10 11:37:07.997761 crossfiledialog-0.1.2/PKG-INFO
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      564 2023-06-10 11:35:13.000000 crossfiledialog-0.1.2/README.md
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-10 11:37:07.997761 crossfiledialog-0.1.2/crossfiledialog/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       39 2022-01-31 20:08:46.000000 crossfiledialog-0.1.2/crossfiledialog/__init__.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      117 2022-01-31 20:08:46.000000 crossfiledialog-0.1.2/crossfiledialog/exceptions.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     2339 2022-01-31 20:08:46.000000 crossfiledialog-0.1.2/crossfiledialog/kdialog.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      157 2022-01-31 20:08:46.000000 crossfiledialog-0.1.2/crossfiledialog/strings.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     2708 2022-01-31 20:08:46.000000 crossfiledialog-0.1.2/crossfiledialog/win32.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1005 2022-01-31 20:08:46.000000 crossfiledialog-0.1.2/crossfiledialog/wrapper.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     2309 2023-06-10 11:21:47.000000 crossfiledialog-0.1.2/crossfiledialog/zenity.py
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-10 11:37:07.997761 crossfiledialog-0.1.2/crossfiledialog.egg-info/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1465 2023-06-10 11:37:07.000000 crossfiledialog-0.1.2/crossfiledialog.egg-info/PKG-INFO
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      382 2023-06-10 11:37:07.000000 crossfiledialog-0.1.2/crossfiledialog.egg-info/SOURCES.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)        1 2023-06-10 11:37:07.000000 crossfiledialog-0.1.2/crossfiledialog.egg-info/dependency_links.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       16 2023-06-10 11:37:07.000000 crossfiledialog-0.1.2/crossfiledialog.egg-info/top_level.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       79 2023-06-10 11:37:07.997761 crossfiledialog-0.1.2/setup.cfg
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1319 2023-06-10 11:37:02.000000 crossfiledialog-0.1.2/setup.py
```

### Comparing `crossfiledialog-0.1.1/crossfiledialog/kdialog.py` & `crossfiledialog-0.1.2/crossfiledialog/kdialog.py`

 * *Files identical despite different names*

### Comparing `crossfiledialog-0.1.1/crossfiledialog/win32.py` & `crossfiledialog-0.1.2/crossfiledialog/win32.py`

 * *Files identical despite different names*

### Comparing `crossfiledialog-0.1.1/crossfiledialog/wrapper.py` & `crossfiledialog-0.1.2/crossfiledialog/wrapper.py`

 * *Files identical despite different names*

### Comparing `crossfiledialog-0.1.1/crossfiledialog/zenity.py` & `crossfiledialog-0.1.2/crossfiledialog/zenity.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,18 +41,19 @@
 
     process = Popen(cmdlist, stdout=PIPE, stderr=PIPE, **extra_kwargs)
     stdout, stderr = process.communicate()
 
     if process.returncode == -1:
         raise ZenityException("Unexpected error during zenity call")
 
+    stdout, stderr = stdout.decode(), stderr.decode()
+
     if stderr.strip():
         sys.stderr.write(stderr)
 
-    stdout, stderr = stdout.decode(), stderr.decode()
     return stdout.strip()
 
 
 def open_file(title=strings.open_file, filter=None):
     zenity_kwargs = dict(title=title)
 
     if filter:
```

