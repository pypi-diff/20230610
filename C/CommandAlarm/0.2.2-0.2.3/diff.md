# Comparing `tmp/CommandAlarm-0.2.2.tar.gz` & `tmp/CommandAlarm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommandAlarm-0.2.2.tar", last modified: Mon Jun  5 22:18:21 2023, max compression
+gzip compressed data, was "CommandAlarm-0.2.3.tar", last modified: Sat Jun 10 13:05:55 2023, max compression
```

## Comparing `CommandAlarm-0.2.2.tar` & `CommandAlarm-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-05 22:18:21.959043 CommandAlarm-0.2.2/
--rw-r--r--   0 testuser  (1002) testuser  (1003)      201 2023-06-05 21:59:54.000000 CommandAlarm-0.2.2/CHANGELOG.md
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-05 22:18:21.955043 CommandAlarm-0.2.2/CommandAlarm.egg-info/
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-05 22:18:21.000000 CommandAlarm-0.2.2/CommandAlarm.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)      288 2023-06-05 22:18:21.000000 CommandAlarm-0.2.2/CommandAlarm.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-05 22:18:21.000000 CommandAlarm-0.2.2/CommandAlarm.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-05 22:18:21.000000 CommandAlarm-0.2.2/CommandAlarm.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-05 22:18:21.000000 CommandAlarm-0.2.2/CommandAlarm.egg-info/top_level.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2017-09-30 07:16:26.000000 CommandAlarm-0.2.2/LICENSE
--rw-r--r--   0 testuser  (1002) testuser  (1003)       29 2023-06-04 13:17:50.000000 CommandAlarm-0.2.2/MANIFEST.in
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-05 22:18:21.959043 CommandAlarm-0.2.2/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2306 2023-06-03 22:05:16.000000 CommandAlarm-0.2.2/README.md
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-05 22:18:21.959043 CommandAlarm-0.2.2/commandalarm/
--rw-r--r--   0 testuser  (1002) testuser  (1003)       46 2023-06-05 22:11:52.000000 CommandAlarm-0.2.2/commandalarm/__init__.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)     7110 2023-06-05 14:05:28.000000 CommandAlarm-0.2.2/commandalarm/commandalarm.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-05 22:18:21.959043 CommandAlarm-0.2.2/setup.cfg
--rw-r--r--   0 testuser  (1002) testuser  (1003)      863 2023-06-05 22:11:42.000000 CommandAlarm-0.2.2/setup.py
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-10 13:05:55.618416 CommandAlarm-0.2.3/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      349 2023-06-10 10:08:09.000000 CommandAlarm-0.2.3/CHANGELOG.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-10 13:05:55.618416 CommandAlarm-0.2.3/CommandAlarm.egg-info/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2827 2023-06-10 13:05:55.000000 CommandAlarm-0.2.3/CommandAlarm.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      288 2023-06-10 13:05:55.000000 CommandAlarm-0.2.3/CommandAlarm.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-10 13:05:55.000000 CommandAlarm-0.2.3/CommandAlarm.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-10 13:05:55.000000 CommandAlarm-0.2.3/CommandAlarm.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-10 13:05:55.000000 CommandAlarm-0.2.3/CommandAlarm.egg-info/top_level.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2023-06-09 19:46:38.000000 CommandAlarm-0.2.3/LICENSE
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       29 2023-06-09 19:46:38.000000 CommandAlarm-0.2.3/MANIFEST.in
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2827 2023-06-10 13:05:55.618416 CommandAlarm-0.2.3/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2304 2023-06-09 19:49:31.000000 CommandAlarm-0.2.3/README.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-10 13:05:55.618416 CommandAlarm-0.2.3/commandalarm/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       46 2023-06-10 10:03:08.000000 CommandAlarm-0.2.3/commandalarm/__init__.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     7219 2023-06-09 22:16:23.000000 CommandAlarm-0.2.3/commandalarm/commandalarm.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-10 13:05:55.618416 CommandAlarm-0.2.3/setup.cfg
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      863 2023-06-10 10:02:37.000000 CommandAlarm-0.2.3/setup.py
```

### Comparing `CommandAlarm-0.2.2/CommandAlarm.egg-info/PKG-INFO` & `CommandAlarm-0.2.3/CommandAlarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -84,8 +84,8 @@
 
 **Ethereum (ETH):** 0x2B29d1A7d94501b6491a26DF54550b0AF793235F
 
 **Litecoin (LTC):** ltc1qhvyfnayhwk3udakyynppc2uy2y2fv97lnt8y7w
 
 ## License
 
-CommandAlarm is licensed under the [GPL License](https://github.com/alofgren/commandalarm/blob/master/LICENSE).
+CommandAlarm is licensed under the [GPL License](https://github.com/alofgren/commandalarm/blob/main/LICENSE).
```

### Comparing `CommandAlarm-0.2.2/LICENSE` & `CommandAlarm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CommandAlarm-0.2.2/PKG-INFO` & `CommandAlarm-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -84,8 +84,8 @@
 
 **Ethereum (ETH):** 0x2B29d1A7d94501b6491a26DF54550b0AF793235F
 
 **Litecoin (LTC):** ltc1qhvyfnayhwk3udakyynppc2uy2y2fv97lnt8y7w
 
 ## License
 
-CommandAlarm is licensed under the [GPL License](https://github.com/alofgren/commandalarm/blob/master/LICENSE).
+CommandAlarm is licensed under the [GPL License](https://github.com/alofgren/commandalarm/blob/main/LICENSE).
```

### Comparing `CommandAlarm-0.2.2/README.md` & `CommandAlarm-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,8 +70,8 @@
 
 **Ethereum (ETH):** 0x2B29d1A7d94501b6491a26DF54550b0AF793235F
 
 **Litecoin (LTC):** ltc1qhvyfnayhwk3udakyynppc2uy2y2fv97lnt8y7w
 
 ## License
 
-CommandAlarm is licensed under the [GPL License](https://github.com/alofgren/commandalarm/blob/master/LICENSE).
+CommandAlarm is licensed under the [GPL License](https://github.com/alofgren/commandalarm/blob/main/LICENSE).
```

### Comparing `CommandAlarm-0.2.2/commandalarm/commandalarm.py` & `CommandAlarm-0.2.3/commandalarm/commandalarm.py`

 * *Files 7% similar despite different names*

```diff
@@ -184,33 +184,33 @@
                                         capture_output=True,
                                         shell=args.shell,
                                         timeout=args.timeout,
                                         check=args.check,
                                         text=True)
                 print(result.stdout)
             except FileNotFoundError:
-                print("Command not found")
+                print("Command not found", file=sys.stderr)
             except subprocess.CalledProcessError as called_process_err:
                 print(
-                    f"Command returned non-zero exit status {called_process_err.returncode}"
-                )
-                print(f"stderr: {called_process_err.stderr}")
+                    f"Command returned non-zero exit status {called_process_err.returncode}",
+                    file=sys.stderr)
+                print(f"stderr: {called_process_err.stderr}", file=sys.stderr)
             except PermissionError as permission_err:
-                print(f"Permission error: {permission_err}")
+                print(f"Permission error: {permission_err}", file=sys.stderr)
             except subprocess.TimeoutExpired as timeout_expired:
                 print(
-                    f"Command timed out after {timeout_expired.timeout} seconds"
-                )
+                    f"Command timed out after {timeout_expired.timeout} seconds",
+                    file=sys.stderr)
             if args.repeat:
                 ALARM_FIRED = False
                 time.sleep(1)
                 set_alarm(args.time, args.day)
             else:
                 break
     except KeyboardInterrupt:
-        print("Alarm stopped manually.")
+        print("Alarm stopped manually.", file=sys.stderr)
         signal.alarm(0)
-        sys.exit()
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `CommandAlarm-0.2.2/setup.py` & `CommandAlarm-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CommandAlarm",
-    version="0.2.2",
+    version="0.2.3",
     author="alofgren",
     author_email="drelofren@outlook.com",
     description="A simple command line program that allows users to set an alarm with a custom command.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alofgren/commandalarm",
     packages=setuptools.find_packages(),
```

