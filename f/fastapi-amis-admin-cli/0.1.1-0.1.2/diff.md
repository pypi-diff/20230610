# Comparing `tmp/fastapi_amis_admin_cli-0.1.1.tar.gz` & `tmp/fastapi_amis_admin_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin_cli-0.1.1.tar", last modified: Tue May  9 08:56:39 2023, max compression
+gzip compressed data, was "fastapi_amis_admin_cli-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_amis_admin_cli-0.1.1.tar` & `fastapi_amis_admin_cli-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1256 2022-05-28 15:32:35.402638 fastapi_amis_admin_cli-0.1.1/README.md
--rw-r--r--   0        0        0      100 2022-05-28 08:45:24.064128 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/cookiecutter.json
--rw-r--r--   0        0        0      422 2023-05-09 01:50:53.209469 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/__init__.py
--rw-r--r--   0        0        0      669 2023-05-09 01:50:53.220445 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py
--rw-r--r--   0        0        0      143 2022-08-13 16:02:30.396212 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/apis.py
--rw-r--r--   0        0        0        0 2022-05-27 06:19:18.767737 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/crud.py
--rw-r--r--   0        0        0      686 2022-05-26 04:36:33.170207 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py
--rw-r--r--   0        0        0      652 2023-05-09 02:10:05.738379 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/models.py
--rw-r--r--   0        0        0       68 2022-05-26 03:27:12.416572 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/schemas.py
--rw-r--r--   0        0        0       26 2022-05-23 09:29:33.512434 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/tests.py
--rw-r--r--   0        0        0      377 2023-05-09 01:22:34.362238 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/cookiecutter.json
--rw-r--r--   0        0        0      391 2022-05-30 13:59:02.924301 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/Dockerfile
--rw-r--r--   0        0        0      911 2023-05-09 08:55:47.865644 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/README.md
--rw-r--r--   0        0        0      464 2023-05-09 01:39:10.888488 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/.env
--rw-r--r--   0        0        0        0 2022-05-12 08:47:40.318000 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/apps/__init__.py
--rw-r--r--   0        0        0      110 2022-05-23 02:16:40.221000 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/__init__.py
--rw-r--r--   0        0        0      435 2022-06-10 14:16:35.825432 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/adminsite.py
--rw-r--r--   0        0        0      490 2022-06-10 14:16:35.798451 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/settings.py
--rw-r--r--   0        0        0     1801 2023-05-09 01:52:17.958788 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py
--rw-r--r--   0        0        0      269 2023-05-09 08:29:07.400258 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/requirements.txt
--rw-r--r--   0        0        0      378 2022-05-30 14:00:21.016996 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/docker-compose.yml
--rw-r--r--   0        0        0     1815 2023-05-09 08:08:21.181729 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/pyproject.toml
--rw-r--r--   0        0        0       83 2023-05-09 08:17:24.867753 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/__init__.py
--rw-r--r--   0        0        0        0 2022-05-26 14:40:55.873535 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/__init__.py
--rw-r--r--   0        0        0     2983 2023-05-09 08:41:28.975785 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/main.py
--rw-r--r--   0        0        0     1674 2022-07-01 06:13:04.760726 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/project.py
--rw-r--r--   0        0        0     2833 2023-05-09 03:37:40.520047 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/utils.py
--rw-r--r--   0        0        0       74 2022-05-28 12:31:29.770843 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/main.py
--rw-r--r--   0        0        0     1494 2023-05-09 07:56:21.864863 fastapi_amis_admin_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 fastapi_amis_admin_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1256 2022-05-28 15:32:35.402638 fastapi_amis_admin_cli-0.1.2/README.md
+-rw-r--r--   0        0        0      100 2022-05-28 08:45:24.064128 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/cookiecutter.json
+-rw-r--r--   0        0        0      422 2023-05-09 01:50:53.209469 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/__init__.py
+-rw-r--r--   0        0        0      669 2023-05-09 01:50:53.220445 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py
+-rw-r--r--   0        0        0      143 2022-08-13 16:02:30.396212 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/apis.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:19:18.767737 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/crud.py
+-rw-r--r--   0        0        0      686 2022-05-26 04:36:33.170207 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py
+-rw-r--r--   0        0        0      652 2023-05-09 02:10:05.738379 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/models.py
+-rw-r--r--   0        0        0       68 2022-05-26 03:27:12.416572 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/schemas.py
+-rw-r--r--   0        0        0       26 2022-05-23 09:29:33.512434 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/tests.py
+-rw-r--r--   0        0        0      377 2023-05-09 01:22:34.362238 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/cookiecutter.json
+-rw-r--r--   0        0        0      391 2022-05-30 13:59:02.924301 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/Dockerfile
+-rw-r--r--   0        0        0      911 2023-05-09 08:55:47.865644 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/README.md
+-rw-r--r--   0        0        0      464 2023-05-09 01:39:10.888488 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/.env
+-rw-r--r--   0        0        0        0 2022-05-12 08:47:40.318000 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/apps/__init__.py
+-rw-r--r--   0        0        0      110 2022-05-23 02:16:40.221000 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/__init__.py
+-rw-r--r--   0        0        0      435 2022-06-10 14:16:35.825432 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/adminsite.py
+-rw-r--r--   0        0        0      490 2022-06-10 14:16:35.798451 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/settings.py
+-rw-r--r--   0        0        0     1801 2023-05-09 01:52:17.958788 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py
+-rw-r--r--   0        0        0      269 2023-05-09 08:29:07.400258 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/requirements.txt
+-rw-r--r--   0        0        0      378 2022-05-30 14:00:21.016996 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/docker-compose.yml
+-rw-r--r--   0        0        0     1815 2023-05-09 08:08:21.181729 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-06-10 09:29:09.418185 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-26 14:40:55.873535 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/commands/__init__.py
+-rw-r--r--   0        0        0     2947 2023-05-09 08:58:29.061351 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/commands/main.py
+-rw-r--r--   0        0        0     1674 2022-07-01 06:13:04.760726 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/commands/project.py
+-rw-r--r--   0        0        0     2975 2023-06-10 09:39:09.984130 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/commands/utils.py
+-rw-r--r--   0        0        0       74 2022-05-28 12:31:29.770843 fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/main.py
+-rw-r--r--   0        0        0     1494 2023-05-09 07:56:21.864863 fastapi_amis_admin_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 fastapi_amis_admin_cli-0.1.2/PKG-INFO
```

### Comparing `fastapi_amis_admin_cli-0.1.1/README.md` & `fastapi_amis_admin_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/models.py` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/README.md` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/pyproject.toml` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/main.py` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/commands/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     app: Annotated[str, typer.Option(default_factory=lambda: get_setting_value("app", "main:app"))],
     host: Annotated[str, typer.Option(default_factory=lambda: get_setting_value("host", "127.0.0.1"))],
     port: Annotated[int, typer.Option(default_factory=lambda: get_setting_value("port", 8000))],
     reload: Annotated[bool, typer.Option(default_factory=lambda: get_setting_value("debug", False))],
     workers: Annotated[int, typer.Option(default_factory=lambda: get_setting_value("workers", 1))],
 ):
     """
-    Run The FastAPI-Amis-Admin Server.
-    To see the complete set of available options, use `uvicorn --help`.
+    Run The FastAPI-Amis-Admin Server. To see the complete set of available options, use `uvicorn --help`.
     """
 
     check_requirement('uvicorn', install=True)
     args = ctx.args.copy()
     if args and args[0] == '--help':
         return os.system('uvicorn ' + ' '.join(args))
     if not args or args[0].startswith('-'):
@@ -57,15 +56,15 @@
     if reload:
         workers = 1
         args.append('--reload')
     args.extend(['--host', host, '--port', str(port), '--workers', str(workers)])
     return os.system('uvicorn ' + ' '.join(args))
 
 
-@app.command(help="Stop Uvicorn Application")
+@app.command()
 def stop(
     port: Annotated[int, typer.Argument(default_factory=lambda: get_setting_value("port", 8000))],  # type: ignore
 ):
     """Stop Uvicorn Application"""
     while True:
         proc = kill_port(port)
         if not proc:
```

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/project.py` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/utils.py` & `fastapi_amis_admin_cli-0.1.2/fastapi_amis_admin_cli/commands/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 import importlib
 import locale
 import os
 import sys
+import time
 from pathlib import Path
 from typing import Optional, List, TypeVar, Dict, Any, Union
 
 import typer
 from click import Choice
 
 
@@ -79,15 +80,18 @@
             return True
         return False
 
 
 def kill_port(port):
     import psutil
 
-    for proc in psutil.process_iter():
-        if proc.name().find("python") == -1:
-            continue
-        for conns in proc.connections(kind="inet"):
-            if conns.laddr.port == port:
-                proc.kill()
+    for conn in psutil.net_connections(kind='inet'):
+        if conn.laddr.port == port:
+            try:
+                proc = psutil.Process(conn.pid)
+                if proc:
+                    proc.kill()
+                    time.sleep(1)
                 return proc
+            except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+                pass
     return None
```

### Comparing `fastapi_amis_admin_cli-0.1.1/pyproject.toml` & `fastapi_amis_admin_cli-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.1/PKG-INFO` & `fastapi_amis_admin_cli-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin_cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: FastAPI-Amis-Admin-Cli is an extended library for quickly building `FastAPI-Amis-Admin` projects.
 Keywords: fastapi-amis-admin-cli,fastapi-amis-admin,fastapi-user-auth,fastapi-APScheduler
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

