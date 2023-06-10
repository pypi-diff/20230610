# Comparing `tmp/twema-0.5.1.tar.gz` & `tmp/twema-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/twema-0.5.1.tar", last modified: Sat Feb  1 11:13:17 2020, max compression
+gzip compressed data, was "twema-0.5.2.tar", last modified: Sat Jun 10 17:54:01 2023, max compression
```

## Comparing `twema-0.5.1.tar` & `twema-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2020-02-01 11:13:17.000000 twema-0.5.1/
--rw-r--r--   0 dottedmag   (501) staff       (20)       60 2020-01-30 23:21:50.000000 twema-0.5.1/MANIFEST.in
--rw-r--r--   0 dottedmag   (501) staff       (20)      246 2020-02-01 11:13:17.000000 twema-0.5.1/PKG-INFO
--rw-r--r--   0 dottedmag   (501) staff       (20)      772 2020-01-30 23:21:50.000000 twema-0.5.1/README.md
-drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2020-02-01 11:13:17.000000 twema-0.5.1/docs/
--rw-r--r--   0 dottedmag   (501) staff       (20)    34523 2020-01-18 14:52:09.000000 twema-0.5.1/docs/COPYING
--rw-r--r--   0 dottedmag   (501) staff       (20)      350 2020-01-18 15:06:21.000000 twema-0.5.1/docs/config.toml.example
--rw-r--r--   0 dottedmag   (501) staff       (20)       38 2020-02-01 11:13:17.000000 twema-0.5.1/setup.cfg
--rw-r--r--   0 dottedmag   (501) staff       (20)      693 2020-02-01 11:12:56.000000 twema-0.5.1/setup.py
-drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2020-02-01 11:13:17.000000 twema-0.5.1/twema/
--rw-r--r--   0 dottedmag   (501) staff       (20)     1922 2020-01-30 23:30:15.000000 twema-0.5.1/twema/__init__.py
--rw-r--r--   0 dottedmag   (501) staff       (20)     1283 2020-01-30 20:14:13.000000 twema-0.5.1/twema/cli.py
--rw-r--r--   0 dottedmag   (501) staff       (20)     1426 2020-01-31 09:47:07.000000 twema-0.5.1/twema/config.py
--rw-r--r--   0 dottedmag   (501) staff       (20)     1310 2020-01-30 12:51:05.000000 twema-0.5.1/twema/db.py
--rw-r--r--   0 dottedmag   (501) staff       (20)     1611 2020-01-31 09:47:17.000000 twema-0.5.1/twema/formatting.py
--rw-r--r--   0 dottedmag   (501) staff       (20)      498 2020-01-30 12:45:06.000000 twema-0.5.1/twema/mail.py
--rw-r--r--   0 dottedmag   (501) staff       (20)     8119 2020-01-31 09:47:51.000000 twema-0.5.1/twema/parse.py
-drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2020-02-01 11:13:17.000000 twema-0.5.1/twema/templates/
--rw-r--r--   0 dottedmag   (501) staff       (20)     2115 2020-02-01 11:12:04.000000 twema-0.5.1/twema/templates/thread.jinja
--rw-r--r--   0 dottedmag   (501) staff       (20)     1113 2020-01-31 09:57:47.000000 twema-0.5.1/twema/twitter.py
-drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2020-02-01 11:13:17.000000 twema-0.5.1/twema.egg-info/
--rw-r--r--   0 dottedmag   (501) staff       (20)      246 2020-02-01 11:13:17.000000 twema-0.5.1/twema.egg-info/PKG-INFO
--rw-r--r--   0 dottedmag   (501) staff       (20)      398 2020-02-01 11:13:17.000000 twema-0.5.1/twema.egg-info/SOURCES.txt
--rw-r--r--   0 dottedmag   (501) staff       (20)        1 2020-02-01 11:13:17.000000 twema-0.5.1/twema.egg-info/dependency_links.txt
--rw-r--r--   0 dottedmag   (501) staff       (20)       42 2020-02-01 11:13:17.000000 twema-0.5.1/twema.egg-info/entry_points.txt
--rw-r--r--   0 dottedmag   (501) staff       (20)       55 2020-02-01 11:13:17.000000 twema-0.5.1/twema.egg-info/requires.txt
--rw-r--r--   0 dottedmag   (501) staff       (20)        6 2020-02-01 11:13:17.000000 twema-0.5.1/twema.egg-info/top_level.txt
+drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2023-06-10 17:54:01.115282 twema-0.5.2/
+-rw-r--r--   0 dottedmag   (501) staff       (20)       60 2023-06-10 17:52:12.000000 twema-0.5.2/MANIFEST.in
+-rw-r--r--   0 dottedmag   (501) staff       (20)      207 2023-06-10 17:54:01.115160 twema-0.5.2/PKG-INFO
+-rw-r--r--   0 dottedmag   (501) staff       (20)      772 2023-06-10 17:52:12.000000 twema-0.5.2/README.md
+drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2023-06-10 17:54:01.112936 twema-0.5.2/docs/
+-rw-r--r--   0 dottedmag   (501) staff       (20)    34523 2023-06-10 17:52:12.000000 twema-0.5.2/docs/COPYING
+-rw-r--r--   0 dottedmag   (501) staff       (20)      350 2023-06-10 17:52:12.000000 twema-0.5.2/docs/config.toml.example
+-rw-r--r--   0 dottedmag   (501) staff       (20)       30 2023-06-10 17:52:12.000000 twema-0.5.2/pyproject.toml
+-rw-r--r--   0 dottedmag   (501) staff       (20)       38 2023-06-10 17:54:01.115330 twema-0.5.2/setup.cfg
+-rw-r--r--   0 dottedmag   (501) staff       (20)      692 2023-06-10 17:52:38.000000 twema-0.5.2/setup.py
+drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2023-06-10 17:54:01.114077 twema-0.5.2/twema/
+-rw-r--r--   0 dottedmag   (501) staff       (20)     1922 2023-06-10 17:52:12.000000 twema-0.5.2/twema/__init__.py
+-rw-r--r--   0 dottedmag   (501) staff       (20)     1283 2023-06-10 17:52:12.000000 twema-0.5.2/twema/cli.py
+-rw-r--r--   0 dottedmag   (501) staff       (20)     1426 2023-06-10 17:52:12.000000 twema-0.5.2/twema/config.py
+-rw-r--r--   0 dottedmag   (501) staff       (20)     1310 2023-06-10 17:52:12.000000 twema-0.5.2/twema/db.py
+-rw-r--r--   0 dottedmag   (501) staff       (20)     1611 2023-06-10 17:52:12.000000 twema-0.5.2/twema/formatting.py
+-rw-r--r--   0 dottedmag   (501) staff       (20)      498 2023-06-10 17:52:12.000000 twema-0.5.2/twema/mail.py
+-rw-r--r--   0 dottedmag   (501) staff       (20)     8119 2023-06-10 17:52:12.000000 twema-0.5.2/twema/parse.py
+drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2023-06-10 17:54:01.114983 twema-0.5.2/twema/templates/
+-rw-r--r--   0 dottedmag   (501) staff       (20)     2136 2023-06-10 17:52:12.000000 twema-0.5.2/twema/templates/thread.jinja
+-rw-r--r--   0 dottedmag   (501) staff       (20)     1113 2023-06-10 17:52:12.000000 twema-0.5.2/twema/twitter.py
+drwxr-xr-x   0 dottedmag   (501) staff       (20)        0 2023-06-10 17:54:01.114849 twema-0.5.2/twema.egg-info/
+-rw-r--r--   0 dottedmag   (501) staff       (20)      207 2023-06-10 17:54:01.000000 twema-0.5.2/twema.egg-info/PKG-INFO
+-rw-r--r--   0 dottedmag   (501) staff       (20)      413 2023-06-10 17:54:01.000000 twema-0.5.2/twema.egg-info/SOURCES.txt
+-rw-r--r--   0 dottedmag   (501) staff       (20)        1 2023-06-10 17:54:01.000000 twema-0.5.2/twema.egg-info/dependency_links.txt
+-rw-r--r--   0 dottedmag   (501) staff       (20)       41 2023-06-10 17:54:01.000000 twema-0.5.2/twema.egg-info/entry_points.txt
+-rw-r--r--   0 dottedmag   (501) staff       (20)       54 2023-06-10 17:54:01.000000 twema-0.5.2/twema.egg-info/requires.txt
+-rw-r--r--   0 dottedmag   (501) staff       (20)        6 2023-06-10 17:54:01.000000 twema-0.5.2/twema.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `twema-0.5.1/README.md` & `twema-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/docs/COPYING` & `twema-0.5.2/docs/COPYING`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/setup.py` & `twema-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # This file is a part of twema and licensed under AGPLv3. See doc/COPYING at the
 # root of the repository for the details.
 #
 from setuptools import setup
 
 setup(
     name="twema",
-    version="0.5.1",
+    version="0.5.2",
     description="Twitter-to-email gateway",
     url="https://github.com/dottedmag/twema",
     author="Mikhail Gusarov",
     author_email="dottedmag@dottedmag.net",
     license="AGPLv3",
     packages=["twema"],
     entry_points={"console_scripts": ["twema=twema.cli:main"]},
     include_package_data=True,
     install_requires=[
-        "Jinja2==2.11.0",
+        "Jinja2==3.1.2",
         "toml==0.10.0",
         "twitter==1.18.0",
         "xdg==4.0.1",
     ],
 )
```

### Comparing `twema-0.5.1/twema/__init__.py` & `twema-0.5.2/twema/__init__.py`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/twema/cli.py` & `twema-0.5.2/twema/cli.py`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/twema/config.py` & `twema-0.5.2/twema/config.py`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/twema/db.py` & `twema-0.5.2/twema/db.py`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/twema/formatting.py` & `twema-0.5.2/twema/formatting.py`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/twema/parse.py` & `twema-0.5.2/twema/parse.py`

 * *Files identical despite different names*

### Comparing `twema-0.5.1/twema/templates/thread.jinja` & `twema-0.5.2/twema/templates/thread.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   </div>
 {% endmacro %}
 <html>
   <head>
     <style>
       * { font-family: sans-serif; }
       .retweet { margin-left: 50px; margin-bottom: 20px; }
-      .quote { margin-left: 50px; }
+      .quote { margin-left: 50px; margin-bottom: 20px; }
       .header {
         margin-bottom: 10px;
       }
       a {
         color: #656565;
       }
       .tweet_date { font-size: 50%; }
```

### Comparing `twema-0.5.1/twema/twitter.py` & `twema-0.5.2/twema/twitter.py`

 * *Files identical despite different names*

