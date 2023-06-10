# Comparing `tmp/watlow-0.5.2.tar.gz` & `tmp/watlow-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watlow-0.5.2.tar", last modified: Mon Jun  5 21:33:22 2023, max compression
+gzip compressed data, was "watlow-0.5.3.tar", last modified: Sat Jun 10 16:16:25 2023, max compression
```

## Comparing `watlow-0.5.2.tar` & `watlow-0.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:33:22.256345 watlow-0.5.2/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-06-05 17:03:36.000000 watlow-0.5.2/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-06-05 17:03:36.000000 watlow-0.5.2/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-05 21:33:22.256409 watlow-0.5.2/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2031 2022-11-16 23:55:15.000000 watlow-0.5.2/README.md
--rw-r--r--   0 a.ruddick   (502) staff       (20)      110 2023-06-05 21:33:22.256599 watlow-0.5.2/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1990 2023-06-05 21:32:55.000000 watlow-0.5.2/setup.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:33:22.255332 watlow-0.5.2/watlow/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1830 2023-06-05 15:40:30.000000 watlow-0.5.2/watlow/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     9120 2023-06-05 17:03:36.000000 watlow-0.5.2/watlow/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2120 2023-06-05 21:32:01.000000 watlow-0.5.2/watlow/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     6071 2023-06-05 21:32:01.000000 watlow-0.5.2/watlow/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:33:22.256214 watlow-0.5.2/watlow.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      295 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      270 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/top_level.txt
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-10 16:16:25.773151 watlow-0.5.3/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-06-07 16:19:52.000000 watlow-0.5.3/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-06-07 16:19:52.000000 watlow-0.5.3/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-10 16:16:25.773212 watlow-0.5.3/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2031 2022-11-16 23:55:15.000000 watlow-0.5.3/README.md
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      159 2023-06-10 16:16:25.773419 watlow-0.5.3/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2020 2023-06-10 16:15:06.000000 watlow-0.5.3/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-10 16:16:25.772333 watlow-0.5.3/watlow/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1830 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     9120 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2120 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5586 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-10 16:16:25.773053 watlow-0.5.3/watlow.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      295 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      285 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/top_level.txt
```

### Comparing `watlow-0.5.2/LICENSE` & `watlow-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watlow-0.5.2/PKG-INFO` & `watlow-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watlow
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python driver for Watlow EZ-Zone temperature controllers.
 Home-page: https://github.com/numat/watlow/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
```

### Comparing `watlow-0.5.2/README.md` & `watlow-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `watlow-0.5.2/setup.py` & `watlow-0.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     raise ImportError("This module requires Python >=3.7.  Use 0.3.1 for Python3.6")
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="watlow",
-    version="0.5.2",
+    version="0.5.3",
     description="Python driver for Watlow EZ-Zone temperature controllers.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/watlow/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     maintainer="Alex Ruddick",
@@ -30,15 +30,16 @@
         "crcmod"],
     extras_require={
         'test': [
             'mypy==1.3.0',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'ruff==0.0.270',
+            'ruff==0.0.272',
+            'types-pyserial',
         ],
     },
     entry_points={
         "console_scripts": [("watlow = watlow:command_line")]
     },
     license="GPLv2",
     classifiers=[
```

### Comparing `watlow-0.5.2/watlow/__init__.py` & `watlow-0.5.3/watlow/__init__.py`

 * *Files identical despite different names*

### Comparing `watlow-0.5.2/watlow/driver.py` & `watlow-0.5.3/watlow/driver.py`

 * *Files identical despite different names*

### Comparing `watlow-0.5.2/watlow/mock.py` & `watlow-0.5.3/watlow/mock.py`

 * *Files identical despite different names*

### Comparing `watlow-0.5.2/watlow/util.py` & `watlow-0.5.3/watlow/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,17 +73,17 @@
             r = await self._request('read_holding_registers', address, 124)
             registers += r.registers
             address, count = address + 124, count - 124
         r = await self._request('read_holding_registers', address, count)
         registers += r.registers
         return registers
 
-    async def read_holding_registers(self, address, value):
+    async def read_holding_registers(self, address, count):
         """Read modbus holding registers."""
-        await self._request('read_holding_registers', address, value)
+        await self._request('read_holding_registers', address, count)
 
     async def write_coil(self, address, value):
         """Write modbus coils."""
         await self._request('write_coil', address, value)
 
     async def write_coils(self, address, values):
         """Write modbus coils."""
@@ -116,29 +116,22 @@
         request sent while it's processing something). The driver handles this
         by assuming there is only one client instance. If other clients
         exist, other logic will have to be added to either prevent or manage
         race conditions.
         """
         await self.connectTask
         async with self.lock:
-            if not self.client.connected:
-                raise TimeoutError("Not connected to Watlow gateway.")
-            future = getattr(self.client.protocol, method)(*args, **kwargs)
             try:
-                return await asyncio.wait_for(future, timeout=self.timeout)
-            except asyncio.TimeoutError as e:
-                if self.client.connected and hasattr(self, 'modbus'):
-                    # This came from reading through the pymodbus@python3 source
-                    # Problem was that the driver was not detecting disconnect
-                    self.client.protocol_lost_connection(self.modbus)
-                raise TimeoutError(e)
-            except pymodbus.exceptions.ConnectionException as e:
-                if self.client.connected and hasattr(self, 'modbus'):
-                    self.client.protocol_lost_connection(self.modbus)
-                raise ConnectionError(e)
+                if self.pymodbus32plus:
+                    future = getattr(self.client, method)
+                else:
+                    future = getattr(self.client.protocol, method)  # type: ignore
+                return await future(*args, **kwargs)
+            except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException):
+                raise TimeoutError("Not connected to Watlow gateway")
 
     async def _close(self) -> None:
         """Close the TCP connection."""
         if self.pymodbus33plus:
             self.client.close()  # 3.3.x
         elif self.pymodbus30plus:
             await self.client.close()  # type: ignore  # 3.0.x - 3.2.x
```

### Comparing `watlow-0.5.2/watlow.egg-info/PKG-INFO` & `watlow-0.5.3/watlow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watlow
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python driver for Watlow EZ-Zone temperature controllers.
 Home-page: https://github.com/numat/watlow/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
```

