# Comparing `tmp/gitfarts-0.1.0.tar.gz` & `tmp/gitfarts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitfarts-0.1.0.tar", max compression
+gzip compressed data, was "gitfarts-0.1.1.tar", max compression
```

## Comparing `gitfarts-0.1.0.tar` & `gitfarts-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-10 12:31:52.561550 gitfarts-0.1.0/gitfarts/__init__.py
--rw-r--r--   0        0        0     4652 2023-06-10 12:30:20.595885 gitfarts-0.1.0/gitfarts/main.py
--rw-r--r--   0        0        0      315 2023-06-10 12:32:45.330393 gitfarts-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 gitfarts-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-10 12:31:52.561550 gitfarts-0.1.1/gitfarts/__init__.py
+-rw-r--r--   0        0        0     4593 2023-06-10 12:35:12.503966 gitfarts-0.1.1/gitfarts/main.py
+-rw-r--r--   0        0        0      316 2023-06-10 12:35:47.130673 gitfarts-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 gitfarts-0.1.1/PKG-INFO
```

### Comparing `gitfarts-0.1.0/gitfarts/main.py` & `gitfarts-0.1.1/gitfarts/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 __version__ = pkg_resources.require("git-bars")[0].version
 
 def print_bars(items, block=u"\u2580", width=50):
     """Print unicode bar representations of dates and scores."""
     for i in items:
         num = str(items[i]["commits"])
 
-        sys.stdout.write(i)
-        sys.stdout.write(",")
-        sys.stdout.write(num)
+        print(f"{i}, {num}")
         
 
 
 
 def filter(items, periodicity="day", author=""):
     """Filter entries by periodicity and author."""
     bars = OrderedDict()
```

