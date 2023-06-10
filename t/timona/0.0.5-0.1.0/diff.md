# Comparing `tmp/timona-0.0.5.tar.gz` & `tmp/timona-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timona-0.0.5.tar", max compression
+gzip compressed data, was "timona-0.1.0.tar", max compression
```

## Comparing `timona-0.0.5.tar` & `timona-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.5/LICENSE
--rw-r--r--   0        0        0      104 2023-05-30 12:02:34.562872 timona-0.0.5/README.md
--rw-r--r--   0        0        0      542 2023-06-08 07:15:04.719193 timona-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.5/timona/__init__.py
--rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.5/timona/__main__.py
--rw-r--r--   0        0        0       38 2023-06-08 07:15:04.719193 timona-0.0.5/timona/__version__.py
--rw-r--r--   0        0        0     1228 2023-05-30 14:40:01.114338 timona-0.0.5/timona/config.py
--rw-r--r--   0        0        0     2715 2023-05-31 07:56:35.415665 timona-0.0.5/timona/helm.py
--rw-r--r--   0        0        0     2730 2023-05-31 09:39:19.195374 timona-0.0.5/timona/main.py
--rw-r--r--   0        0        0     5236 2023-05-30 14:50:19.327125 timona-0.0.5/timona/releases.py
--rw-r--r--   0        0        0     2541 2023-06-08 07:06:35.419053 timona-0.0.5/timona/template/__init__.py
--rw-r--r--   0        0        0      282 2023-06-08 07:07:37.075544 timona-0.0.5/timona/template/module_jinja2.py
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 timona-0.0.5/setup.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 timona-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 18:54:15.243204 timona-0.1.0/LICENSE
+-rw-r--r--   0        0        0      104 2023-06-10 18:54:15.243204 timona-0.1.0/README.md
+-rw-r--r--   0        0        0      542 2023-06-10 18:54:32.167343 timona-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-06-10 18:54:15.243204 timona-0.1.0/timona/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-10 18:54:15.243204 timona-0.1.0/timona/__main__.py
+-rw-r--r--   0        0        0       38 2023-06-10 18:54:32.167343 timona-0.1.0/timona/__version__.py
+-rw-r--r--   0        0        0     1228 2023-06-10 18:54:15.243204 timona-0.1.0/timona/config.py
+-rw-r--r--   0        0        0     2715 2023-06-10 18:54:15.243204 timona-0.1.0/timona/helm.py
+-rw-r--r--   0        0        0     2882 2023-06-10 18:54:15.243204 timona-0.1.0/timona/main.py
+-rw-r--r--   0        0        0     5236 2023-06-10 18:54:15.243204 timona-0.1.0/timona/releases.py
+-rw-r--r--   0        0        0     2541 2023-06-10 18:54:15.243204 timona-0.1.0/timona/template/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-10 18:54:15.243204 timona-0.1.0/timona/template/module_jinja2.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 timona-0.1.0/PKG-INFO
```

### Comparing `timona-0.0.5/LICENSE` & `timona-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timona-0.0.5/pyproject.toml` & `timona-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timona"
-version = "0.0.5"
+version = "0.1.0"
 description = "Tool to automate Helm deployments"
 authors = ["mihaiush <mihaiush@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mihaiush/timona"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `timona-0.0.5/timona/config.py` & `timona-0.1.0/timona/config.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.5/timona/helm.py` & `timona-0.1.0/timona/helm.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.5/timona/main.py` & `timona-0.1.0/timona/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 def usage():
     print()
     print("timona COMAND [RELEASE]")
     print()
     print("COMMANDS:")
+    print("  config           - dump config")
     print("  releases         - list releases")
     print("  env RELEASE      - show environment")
     print("  template RELEASE - render template")
     print("  debug RELEASE    - dry-run")
     print("  diff RELEASE     - diff between running and config")
     print("  deploy RELEASE   - deploy")
     print("  status RELEASE   - status")
@@ -30,34 +31,39 @@
 
 
 def main():
     if len(sys.argv) == 1:
         usage()
     CMD = sys.argv[1]
     valid_commands = [
+        'config',
         'releases',
         'env',
         'template',
         'debug',
         'diff',
         'deploy',
         'status',
         'delete',
         'version'
     ]
     if CMD not in valid_commands:
         usage()
     R = None
-    if CMD != 'releases' and CMD != 'version':
+    if CMD not in ['config', 'releases', 'version']:
         if len(sys.argv) == 2:
             usage()
         R = sys.argv[2]
 
     CONFIG = load_config()
 
+    if CMD == 'config':
+        print(yaml.safe_dump(CONFIG))
+        sys.exit()
+
     TMP = '{}/.timona'.format(CONFIG['config']['tmp'])
     os.makedirs(TMP, exist_ok=True)
     T = Template(CONFIG['config']['template'], TMP)
     H = Helm(CONFIG['config']['helm'], T, TMP)
 
     if CMD == 'version':
         print('timona: {}'.format(version))
```

### Comparing `timona-0.0.5/timona/releases.py` & `timona-0.1.0/timona/releases.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.5/timona/template/__init__.py` & `timona-0.1.0/timona/template/__init__.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.5/PKG-INFO` & `timona-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timona
-Version: 0.0.5
+Version: 0.1.0
 Summary: Tool to automate Helm deployments
 Home-page: https://github.com/mihaiush/timona
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

