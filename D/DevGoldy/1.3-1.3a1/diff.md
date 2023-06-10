# Comparing `tmp/DevGoldy-1.3.tar.gz` & `tmp/DevGoldy-1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DevGoldy-1.3.tar", last modified: Sat Jun 10 15:45:59 2023, max compression
+gzip compressed data, was "DevGoldy-1.3a1.tar", last modified: Sun Oct 30 14:32:32 2022, max compression
```

## Comparing `DevGoldy-1.3.tar` & `DevGoldy-1.3a1.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-06-10 15:45:59.833548 DevGoldy-1.3/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       61 2023-06-10 15:35:24.000000 DevGoldy-1.3/.gitignore
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-06-10 15:45:59.817247 DevGoldy-1.3/DevGoldy/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      325 2023-06-10 15:24:45.000000 DevGoldy-1.3/DevGoldy/__init__.py
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-06-10 15:45:59.825201 DevGoldy-1.3/DevGoldy/cli/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1839 2023-06-10 15:30:59.000000 DevGoldy-1.3/DevGoldy/cli/__init__.py
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-06-10 15:45:59.828703 DevGoldy-1.3/DevGoldy/cli/commands/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       55 2023-06-10 15:32:33.000000 DevGoldy-1.3/DevGoldy/cli/commands/__init__.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      570 2023-06-10 15:45:29.000000 DevGoldy-1.3/DevGoldy/cli/commands/reload.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      659 2023-06-10 15:43:54.000000 DevGoldy-1.3/DevGoldy/cli/commands/usb.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      573 2023-06-09 20:45:41.000000 DevGoldy-1.3/DevGoldy/errors.py
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-06-10 15:45:59.830924 DevGoldy-1.3/DevGoldy/utils/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      345 2022-11-23 13:01:15.000000 DevGoldy-1.3/DevGoldy/utils/__init__.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      403 2023-06-09 20:58:04.000000 DevGoldy-1.3/DevGoldy/utils/powershell.py
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-06-10 15:45:59.824149 DevGoldy-1.3/DevGoldy.egg-info/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     2309 2023-06-10 15:45:59.000000 DevGoldy-1.3/DevGoldy.egg-info/PKG-INFO
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      470 2023-06-10 15:45:59.000000 DevGoldy-1.3/DevGoldy.egg-info/SOURCES.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)        1 2023-06-10 15:45:59.000000 DevGoldy-1.3/DevGoldy.egg-info/dependency_links.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       87 2023-06-10 15:45:59.000000 DevGoldy-1.3/DevGoldy.egg-info/entry_points.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       87 2023-06-10 15:45:59.000000 DevGoldy-1.3/DevGoldy.egg-info/requires.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)        9 2023-06-10 15:45:59.000000 DevGoldy-1.3/DevGoldy.egg-info/top_level.txt
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       13 2023-06-09 20:06:53.000000 DevGoldy-1.3/Makefile
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     2309 2023-06-10 15:45:59.833019 DevGoldy-1.3/PKG-INFO
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     1471 2023-06-09 20:00:52.000000 DevGoldy-1.3/README.md
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)     2748 2023-06-10 15:41:43.000000 DevGoldy-1.3/pyproject.toml
-drwxrwxrwx   0 goldy     (1001) goldy     (1001)        0 2023-06-10 15:45:59.831972 DevGoldy-1.3/scripts/
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)      294 2023-06-10 15:35:59.000000 DevGoldy-1.3/scripts/demo.py
--rwxrwxrwx   0 goldy     (1001) goldy     (1001)       38 2023-06-10 15:45:59.833691 DevGoldy-1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-10-30 14:32:32.285601 DevGoldy-1.3a1/
+drwxrwxrwx   0        0        0        0 2022-10-30 14:32:32.229657 DevGoldy-1.3a1/DevGoldy/
+-rw-rw-rw-   0        0        0        0 2022-07-28 21:39:02.000000 DevGoldy-1.3a1/DevGoldy/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-30 14:32:32.275597 DevGoldy-1.3a1/DevGoldy/dev_goldy/
+-rw-rw-rw-   0        0        0     1855 2022-10-30 14:30:20.000000 DevGoldy-1.3a1/DevGoldy/dev_goldy/__init__.py
+-rw-rw-rw-   0        0        0      199 2022-07-28 21:39:02.000000 DevGoldy-1.3a1/DevGoldy/dev_goldy/start.py
+-rw-rw-rw-   0        0        0      574 2022-10-30 14:20:32.000000 DevGoldy-1.3a1/DevGoldy/dev_goldy/usb.py
+drwxrwxrwx   0        0        0        0 2022-10-30 14:32:32.280599 DevGoldy-1.3a1/DevGoldy/dev_goldy/utils/
+-rw-rw-rw-   0        0        0      286 2022-10-30 13:27:39.000000 DevGoldy-1.3a1/DevGoldy/dev_goldy/utils/__init__.py
+-rw-rw-rw-   0        0        0      396 2022-10-30 13:30:10.000000 DevGoldy-1.3a1/DevGoldy/dev_goldy/utils/powershell.py
+-rw-rw-rw-   0        0        0       99 2022-10-30 13:18:55.000000 DevGoldy-1.3a1/DevGoldy/info.py
+-rw-rw-rw-   0        0        0       76 2022-07-28 21:39:02.000000 DevGoldy-1.3a1/DevGoldy/run.py
+drwxrwxrwx   0        0        0        0 2022-10-30 14:32:32.265597 DevGoldy-1.3a1/DevGoldy.egg-info/
+-rw-rw-rw-   0        0        0      392 2022-10-30 14:32:31.000000 DevGoldy-1.3a1/DevGoldy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2022-10-30 14:32:32.000000 DevGoldy-1.3a1/DevGoldy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-30 14:32:31.000000 DevGoldy-1.3a1/DevGoldy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2022-10-30 14:32:31.000000 DevGoldy-1.3a1/DevGoldy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2022-10-30 14:32:31.000000 DevGoldy-1.3a1/DevGoldy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-10-30 14:32:31.000000 DevGoldy-1.3a1/DevGoldy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       32 2022-04-26 10:34:03.000000 DevGoldy-1.3a1/MANIFEST.in
+-rw-rw-rw-   0        0        0      392 2022-10-30 14:32:32.283601 DevGoldy-1.3a1/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2022-07-28 21:39:02.000000 DevGoldy-1.3a1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-10-30 14:32:32.286600 DevGoldy-1.3a1/setup.cfg
+-rw-rw-rw-   0        0        0      724 2022-10-30 13:26:03.000000 DevGoldy-1.3a1/setup.py
```

### Comparing `DevGoldy-1.3/DevGoldy/cli/__init__.py` & `DevGoldy-1.3a1/DevGoldy/dev_goldy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-import click
-from devgoldyutils import Colours
-from .. import __version__, dev_goldy_logger
-
-@click.group(invoke_without_command = True)
-@click.pass_context
-def dev_goldy(ctx: click.Context):
-    if ctx.invoked_subcommand is None:
-        print(f"""
-██████╗░███████╗██╗░░░██╗  ░██████╗░░█████╗░██╗░░░░░██████╗░██╗░░░██╗
-██╔══██╗██╔════╝██║░░░██║  ██╔════╝░██╔══██╗██║░░░░░██╔══██╗╚██╗░██╔╝
-██║░░██║█████╗░░╚██╗░██╔╝  ██║░░██╗░██║░░██║██║░░░░░██║░░██║░╚████╔╝░
-██║░░██║██╔══╝░░░╚████╔╝░  ██║░░╚██╗██║░░██║██║░░░░░██║░░██║░░╚██╔╝░░
-██████╔╝███████╗░░╚██╔╝░░  ╚██████╔╝╚█████╔╝███████╗██████╔╝░░░██║░░░
-╚═════╝░╚══════╝░░░╚═╝░░░  ░╚═════╝░░╚════╝░╚══════╝╚═════╝░░░░╚═╝░░░
-
-    Version: [ {__version__} ]
-        """)
-
-        print(Colours.BLUE.apply("Do 'devgoldy --help' for a list of available commands."))
-
-    else:
-        dev_goldy_logger.info(Colours.BLUE.apply(f"Running command {ctx.invoked_subcommand}..."))
-        print("")
-
-
-# Register sub commands.
-# -----------------------
-from .commands import *
+import click
+import devgoldyutils
+
+try:
+    from .. import info
+except ValueError:
+    import info
+
+console = devgoldyutils.Console()
+
+@click.group(invoke_without_command=True)
+@click.pass_context
+def devgoldy(ctx:click.Context):
+    if ctx.invoked_subcommand is None:
+        print(f"""
+██████╗░███████╗██╗░░░██╗  ░██████╗░░█████╗░██╗░░░░░██████╗░██╗░░░██╗
+██╔══██╗██╔════╝██║░░░██║  ██╔════╝░██╔══██╗██║░░░░░██╔══██╗╚██╗░██╔╝
+██║░░██║█████╗░░╚██╗░██╔╝  ██║░░██╗░██║░░██║██║░░░░░██║░░██║░╚████╔╝░
+██║░░██║██╔══╝░░░╚████╔╝░  ██║░░╚██╗██║░░██║██║░░░░░██║░░██║░░╚██╔╝░░
+██████╔╝███████╗░░╚██╔╝░░  ╚██████╔╝╚█████╔╝███████╗██████╔╝░░░██║░░░
+╚═════╝░╚══════╝░░░╚═╝░░░  ░╚═════╝░░╚════╝░╚══════╝╚═════╝░░░░╚═╝░░░
+
+    Version: [ {info.VERSION} ]
+        """)
+
+        print(console.BLUE("Do 'devgoldy --help' for a list of available commands."))
+
+    else:
+        print(console.BLUE(f"Running command {ctx.invoked_subcommand}..."))
+        print("")
+    
+from . import utils
+from . import start, usb
```

### Comparing `DevGoldy-1.3/DevGoldy/cli/commands/usb.py` & `DevGoldy-1.3a1/DevGoldy/dev_goldy/usb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-import os
-import sys
+import sys, os
 
-import click
-from click import Context
+from click import Argument, Context
 
-from . import dev_goldy
-from ... import utils, errors
+from . import click, utils, devgoldy
 
-@dev_goldy.group(invoke_without_command = True)
+@devgoldy.group(invoke_without_command=True)
 @click.pass_context
 def usb(ctx:Context):
     """Allows you to list all and specific usb devices."""
     if ctx.invoked_subcommand is not None:
         pass
     else:
         all.invoke(ctx)
 
 @usb.command()
 def all():
     if sys.platform == "win32":
-        return utils.PowerShell("Get-PnpDevice -PresentOnly | Where-Object { $_.InstanceId -match '^USB' }").run()
+        utils.PowerShell("Get-PnpDevice -PresentOnly | Where-Object { $_.InstanceId -match '^USB' }").run()
 
-    elif sys.platform == "linux":
-        return os.system("lsusb")
-
-    raise errors.OSNotSupported()
+    if sys.platform == "linux":
+        os.system("lsusb")
```

