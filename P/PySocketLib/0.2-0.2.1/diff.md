# Comparing `tmp/PySocketLib-0.2.tar.gz` & `tmp/PySocketLib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySocketLib-0.2.tar", last modified: Sat Jun 10 14:41:22 2023, max compression
+gzip compressed data, was "PySocketLib-0.2.1.tar", last modified: Sat Jun 10 14:46:23 2023, max compression
```

## Comparing `PySocketLib-0.2.tar` & `PySocketLib-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/
--rw-rw-r--   0 igors     (1000) igors     (1000)     1069 2023-06-10 09:19:23.000000 PySocketLib-0.2/LICENSE
--rw-rw-r--   0 igors     (1000) igors     (1000)     3678 2023-06-10 14:41:22.517443 PySocketLib-0.2/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)     3154 2023-06-10 12:24:08.000000 PySocketLib-0.2/README.md
--rw-rw-r--   0 igors     (1000) igors     (1000)      509 2023-06-10 14:41:12.000000 PySocketLib-0.2/pyproject.toml
--rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-06-10 14:41:22.517443 PySocketLib-0.2/setup.cfg
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.513443 PySocketLib-0.2/src/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.513443 PySocketLib-0.2/src/PySocketLib/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib/CExceptions/
--rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.2/src/PySocketLib/CExceptions/InitExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       74 2023-06-05 14:38:04.000000 PySocketLib-0.2/src/PySocketLib/CExceptions/ProtocolExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       61 2023-06-03 17:39:57.000000 PySocketLib-0.2/src/PySocketLib/CExceptions/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib/Client/
--rw-rw-r--   0 igors     (1000) igors     (1000)      964 2023-06-10 14:30:50.000000 PySocketLib-0.2/src/PySocketLib/Client/Client.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      214 2023-06-02 19:35:46.000000 PySocketLib-0.2/src/PySocketLib/Client/ConnectedClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       71 2023-06-03 13:07:20.000000 PySocketLib-0.2/src/PySocketLib/Client/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib/Server/
--rw-rw-r--   0 igors     (1000) igors     (1000)     3126 2023-06-10 14:30:39.000000 PySocketLib-0.2/src/PySocketLib/Server/Server.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      773 2023-06-10 14:31:48.000000 PySocketLib-0.2/src/PySocketLib/Server/TCPServer.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       59 2023-06-03 13:06:22.000000 PySocketLib-0.2/src/PySocketLib/Server/__init__.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       67 2023-06-10 06:43:20.000000 PySocketLib-0.2/src/PySocketLib/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib.egg-info/
--rw-rw-r--   0 igors     (1000) igors     (1000)     3678 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)      566 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/SOURCES.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/dependency_links.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)       12 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/top_level.txt
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1069 2023-06-10 09:19:23.000000 PySocketLib-0.2.1/LICENSE
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3661 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3135 2023-06-10 14:44:47.000000 PySocketLib-0.2.1/README.md
+-rw-rw-r--   0 igors     (1000) igors     (1000)      511 2023-06-10 14:46:14.000000 PySocketLib-0.2.1/pyproject.toml
+-rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/setup.cfg
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.053643 PySocketLib-0.2.1/src/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/CExceptions/
+-rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.2.1/src/PySocketLib/CExceptions/InitExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       74 2023-06-05 14:38:04.000000 PySocketLib-0.2.1/src/PySocketLib/CExceptions/ProtocolExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       61 2023-06-03 17:39:57.000000 PySocketLib-0.2.1/src/PySocketLib/CExceptions/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/Client/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      964 2023-06-10 14:30:50.000000 PySocketLib-0.2.1/src/PySocketLib/Client/Client.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      214 2023-06-02 19:35:46.000000 PySocketLib-0.2.1/src/PySocketLib/Client/ConnectedClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       71 2023-06-03 13:07:20.000000 PySocketLib-0.2.1/src/PySocketLib/Client/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/Server/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3126 2023-06-10 14:30:39.000000 PySocketLib-0.2.1/src/PySocketLib/Server/Server.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      773 2023-06-10 14:31:48.000000 PySocketLib-0.2.1/src/PySocketLib/Server/TCPServer.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       59 2023-06-03 13:06:22.000000 PySocketLib-0.2.1/src/PySocketLib/Server/__init__.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       67 2023-06-10 06:43:20.000000 PySocketLib-0.2.1/src/PySocketLib/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib.egg-info/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3661 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      566 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/SOURCES.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/dependency_links.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)       12 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/top_level.txt
```

### Comparing `PySocketLib-0.2/LICENSE` & `PySocketLib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.2/PKG-INFO` & `PySocketLib-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySocketLib
-Version: 0.2
+Version: 0.2.1
 Summary: Library to simplify working with socket
 Author-email: Samsonov Igor <ig.samsonov10@yandex.ru>
 Project-URL: Homepage, https://github.com/Minuta18/PySocketLib
 Project-URL: Bug Tracker, https://github.com/Minuta18/PySocketLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,15 +47,15 @@
     def on_receive(self):
         ...
 
     def on_send(self):
         ...
 
 if __name__ == '__main__':
-    server = EchoServer(port=5678)
+    server = EchoServer(('', 3000))
     
     while True:
         server.proceed()
 ```
 
 Methods:
 `connect_client` - Actions to do when client connects,
@@ -92,15 +92,15 @@
             print(f'[INFO] Sent data {message}')
             self.client_messages[client] = None
             return message
         else:
             return b''
 
 if __name__ == '__main__':
-    server = EchoServer(port=5678)
+    server = EchoServer(('', 3000))
     
     while True:
         server.proceed()
 ```
 
 ## Client
 
@@ -117,15 +117,15 @@
     
     def on_receive(self, data: bytes):
         print('Server: ' + str(data))
 
         return super().on_receive(data)
     
 if __name__ == '__main__':
-    cl = MyClient(hostname='127.0.0.1', port=5678)
+    cl = MyClient(('', 3000))
     while True:
         cl.send(b'')
         cl.proceed()
 ```
 
 ## Result
```

### Comparing `PySocketLib-0.2/README.md` & `PySocketLib-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def on_receive(self):
         ...
 
     def on_send(self):
         ...
 
 if __name__ == '__main__':
-    server = EchoServer(port=5678)
+    server = EchoServer(('', 3000))
     
     while True:
         server.proceed()
 ```
 
 Methods:
 `connect_client` - Actions to do when client connects,
@@ -78,15 +78,15 @@
             print(f'[INFO] Sent data {message}')
             self.client_messages[client] = None
             return message
         else:
             return b''
 
 if __name__ == '__main__':
-    server = EchoServer(port=5678)
+    server = EchoServer(('', 3000))
     
     while True:
         server.proceed()
 ```
 
 ## Client
 
@@ -103,15 +103,15 @@
     
     def on_receive(self, data: bytes):
         print('Server: ' + str(data))
 
         return super().on_receive(data)
     
 if __name__ == '__main__':
-    cl = MyClient(hostname='127.0.0.1', port=5678)
+    cl = MyClient(('', 3000))
     while True:
         cl.send(b'')
         cl.proceed()
 ```
 
 ## Result
```

### Comparing `PySocketLib-0.2/src/PySocketLib/Client/Client.py` & `PySocketLib-0.2.1/src/PySocketLib/Client/Client.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.2/src/PySocketLib/Server/Server.py` & `PySocketLib-0.2.1/src/PySocketLib/Server/Server.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.2/src/PySocketLib/Server/TCPServer.py` & `PySocketLib-0.2.1/src/PySocketLib/Server/TCPServer.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.2/src/PySocketLib.egg-info/PKG-INFO` & `PySocketLib-0.2.1/src/PySocketLib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySocketLib
-Version: 0.2
+Version: 0.2.1
 Summary: Library to simplify working with socket
 Author-email: Samsonov Igor <ig.samsonov10@yandex.ru>
 Project-URL: Homepage, https://github.com/Minuta18/PySocketLib
 Project-URL: Bug Tracker, https://github.com/Minuta18/PySocketLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,15 +47,15 @@
     def on_receive(self):
         ...
 
     def on_send(self):
         ...
 
 if __name__ == '__main__':
-    server = EchoServer(port=5678)
+    server = EchoServer(('', 3000))
     
     while True:
         server.proceed()
 ```
 
 Methods:
 `connect_client` - Actions to do when client connects,
@@ -92,15 +92,15 @@
             print(f'[INFO] Sent data {message}')
             self.client_messages[client] = None
             return message
         else:
             return b''
 
 if __name__ == '__main__':
-    server = EchoServer(port=5678)
+    server = EchoServer(('', 3000))
     
     while True:
         server.proceed()
 ```
 
 ## Client
 
@@ -117,15 +117,15 @@
     
     def on_receive(self, data: bytes):
         print('Server: ' + str(data))
 
         return super().on_receive(data)
     
 if __name__ == '__main__':
-    cl = MyClient(hostname='127.0.0.1', port=5678)
+    cl = MyClient(('', 3000))
     while True:
         cl.send(b'')
         cl.proceed()
 ```
 
 ## Result
```

### Comparing `PySocketLib-0.2/src/PySocketLib.egg-info/SOURCES.txt` & `PySocketLib-0.2.1/src/PySocketLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

