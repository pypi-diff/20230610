# Comparing `tmp/PySocketLib-0.1.1.tar.gz` & `tmp/PySocketLib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySocketLib-0.1.1.tar", last modified: Sat Jun 10 12:49:46 2023, max compression
+gzip compressed data, was "PySocketLib-0.2.tar", last modified: Sat Jun 10 14:41:22 2023, max compression
```

## Comparing `PySocketLib-0.1.1.tar` & `PySocketLib-0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 12:49:46.199202 PySocketLib-0.1.1/
--rw-rw-r--   0 igors     (1000) igors     (1000)     1069 2023-06-10 09:19:23.000000 PySocketLib-0.1.1/LICENSE
--rw-rw-r--   0 igors     (1000) igors     (1000)     3680 2023-06-10 12:49:46.199202 PySocketLib-0.1.1/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)     3154 2023-06-10 12:24:08.000000 PySocketLib-0.1.1/README.md
--rw-rw-r--   0 igors     (1000) igors     (1000)      511 2023-06-10 12:49:40.000000 PySocketLib-0.1.1/pyproject.toml
--rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-06-10 12:49:46.199202 PySocketLib-0.1.1/setup.cfg
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 12:49:46.195202 PySocketLib-0.1.1/src/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 12:49:46.195202 PySocketLib-0.1.1/src/PySocketLib/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 12:49:46.195202 PySocketLib-0.1.1/src/PySocketLib/CExceptions/
--rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.1.1/src/PySocketLib/CExceptions/InitExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       74 2023-06-05 14:38:04.000000 PySocketLib-0.1.1/src/PySocketLib/CExceptions/ProtocolExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       61 2023-06-03 17:39:57.000000 PySocketLib-0.1.1/src/PySocketLib/CExceptions/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 12:49:46.195202 PySocketLib-0.1.1/src/PySocketLib/Client/
--rw-rw-r--   0 igors     (1000) igors     (1000)      851 2023-06-10 08:58:56.000000 PySocketLib-0.1.1/src/PySocketLib/Client/Client.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      214 2023-06-02 19:35:46.000000 PySocketLib-0.1.1/src/PySocketLib/Client/ConnectedClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       71 2023-06-03 13:07:20.000000 PySocketLib-0.1.1/src/PySocketLib/Client/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 12:49:46.199202 PySocketLib-0.1.1/src/PySocketLib/Server/
--rw-rw-r--   0 igors     (1000) igors     (1000)     3063 2023-06-10 09:08:01.000000 PySocketLib-0.1.1/src/PySocketLib/Server/Server.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      811 2023-06-10 09:08:01.000000 PySocketLib-0.1.1/src/PySocketLib/Server/TCPServer.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       59 2023-06-03 13:06:22.000000 PySocketLib-0.1.1/src/PySocketLib/Server/__init__.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       67 2023-06-10 06:43:20.000000 PySocketLib-0.1.1/src/PySocketLib/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 12:49:46.195202 PySocketLib-0.1.1/src/PySocketLib.egg-info/
--rw-rw-r--   0 igors     (1000) igors     (1000)     3680 2023-06-10 12:49:46.000000 PySocketLib-0.1.1/src/PySocketLib.egg-info/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)      566 2023-06-10 12:49:46.000000 PySocketLib-0.1.1/src/PySocketLib.egg-info/SOURCES.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-06-10 12:49:46.000000 PySocketLib-0.1.1/src/PySocketLib.egg-info/dependency_links.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)       12 2023-06-10 12:49:46.000000 PySocketLib-0.1.1/src/PySocketLib.egg-info/top_level.txt
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1069 2023-06-10 09:19:23.000000 PySocketLib-0.2/LICENSE
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3678 2023-06-10 14:41:22.517443 PySocketLib-0.2/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3154 2023-06-10 12:24:08.000000 PySocketLib-0.2/README.md
+-rw-rw-r--   0 igors     (1000) igors     (1000)      509 2023-06-10 14:41:12.000000 PySocketLib-0.2/pyproject.toml
+-rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-06-10 14:41:22.517443 PySocketLib-0.2/setup.cfg
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.513443 PySocketLib-0.2/src/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.513443 PySocketLib-0.2/src/PySocketLib/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib/CExceptions/
+-rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.2/src/PySocketLib/CExceptions/InitExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       74 2023-06-05 14:38:04.000000 PySocketLib-0.2/src/PySocketLib/CExceptions/ProtocolExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       61 2023-06-03 17:39:57.000000 PySocketLib-0.2/src/PySocketLib/CExceptions/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib/Client/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      964 2023-06-10 14:30:50.000000 PySocketLib-0.2/src/PySocketLib/Client/Client.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      214 2023-06-02 19:35:46.000000 PySocketLib-0.2/src/PySocketLib/Client/ConnectedClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       71 2023-06-03 13:07:20.000000 PySocketLib-0.2/src/PySocketLib/Client/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib/Server/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3126 2023-06-10 14:30:39.000000 PySocketLib-0.2/src/PySocketLib/Server/Server.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      773 2023-06-10 14:31:48.000000 PySocketLib-0.2/src/PySocketLib/Server/TCPServer.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       59 2023-06-03 13:06:22.000000 PySocketLib-0.2/src/PySocketLib/Server/__init__.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       67 2023-06-10 06:43:20.000000 PySocketLib-0.2/src/PySocketLib/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:41:22.517443 PySocketLib-0.2/src/PySocketLib.egg-info/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3678 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      566 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/SOURCES.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/dependency_links.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)       12 2023-06-10 14:41:22.000000 PySocketLib-0.2/src/PySocketLib.egg-info/top_level.txt
```

### Comparing `PySocketLib-0.1.1/LICENSE` & `PySocketLib-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.1.1/PKG-INFO` & `PySocketLib-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySocketLib
-Version: 0.1.1
+Version: 0.2
 Summary: Library to simplify working with socket
 Author-email: Samsonov Igor <ig.samsonov10@yandex.ru>
 Project-URL: Homepage, https://github.com/Minuta18/PySocketLib
 Project-URL: Bug Tracker, https://github.com/Minuta18/PySocketLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PySocketLib-0.1.1/README.md` & `PySocketLib-0.2/README.md`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.1.1/src/PySocketLib/Client/Client.py` & `PySocketLib-0.2/src/PySocketLib/Client/Client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import socket
 
 class Client:
     '''Simple socket client'''
     def __init__(self, 
-        hostname: str='0.0.0.0', 
-        port: int=8000,
+        addr: tuple,
     ):
-        self.__hostname = hostname
-        self.__port = port
-
-        self.__socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.__socket.connect((self.__hostname, self.__port))
+        self.__socket = None
+        if len(addr) == 2:
+            self.__socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        elif len(addr) == 4:
+            self.__socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
+        else:
+            raise ValueError(f"Invalid address: {addr}")
+        self.__socket.connect(addr)
 
     def __del__(self):
         self.__socket.close()
 
     def __service_connection(self):
         recv_data = self.__socket.recv(1024)
         self.on_receive(recv_data)
```

### Comparing `PySocketLib-0.1.1/src/PySocketLib/Server/Server.py` & `PySocketLib-0.2/src/PySocketLib/Server/Server.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 from PySocketLib.CExceptions.InitExceptions import UnablePort
 from PySocketLib.Client import ConnectedClient
 
 class Server:
     '''Simple socket server'''
     def __init__(self, 
-        host: str='0.0.0.0',
-        port: int=8000,
+        addr: tuple,
     ):
-        if port <= 1023:
-            raise UnablePort("Can't use priviliged port {}" % port)
-        self.__host = host
-        self.__port = port
-        
         self.__socket_selector = selectors.DefaultSelector()
-
-        self.__socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.__socket.bind((host, port))
+        
+        self.__socket = None
+        if len(addr) == 2:
+            self.__socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        elif len(addr) == 4:
+            self.__socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM, 0)
+        else:
+            raise ValueError(f"Invalid address: {addr}")
+        
+        self.__socket.bind(addr)
         self.__socket.listen()
         self.__socket.setblocking(False)
         self.__socket_selector.register(self.__socket, selectors.EVENT_READ)
         self.__clients = dict()
 
     def __del__(self):
         '''Disconnects all clients'''
```

### Comparing `PySocketLib-0.1.1/src/PySocketLib/Server/TCPServer.py` & `PySocketLib-0.2/src/PySocketLib/Server/TCPServer.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from PySocketLib.Server import Server
 from PySocketLib.CExceptions.InitExceptions import UnablePort
 from PySocketLib.Client import ConnectedClient
 
 class TCPServer(Server):
     '''Simple TCP server'''
     def __init__(self, 
-        host: str='0.0.0.0',
-        port: int=8000,
+        addr: tuple,
     ):
-        super().__init__(host, port)
+        super().__init__(addr)
 
     def connect_client(self, sock: socket.socket) -> ConnectedClient:
         return super().connect_client(sock)
     
     def disconnect_client(self, client: ConnectedClient):
         return super().disconnect_client(client)
```

### Comparing `PySocketLib-0.1.1/src/PySocketLib.egg-info/PKG-INFO` & `PySocketLib-0.2/src/PySocketLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySocketLib
-Version: 0.1.1
+Version: 0.2
 Summary: Library to simplify working with socket
 Author-email: Samsonov Igor <ig.samsonov10@yandex.ru>
 Project-URL: Homepage, https://github.com/Minuta18/PySocketLib
 Project-URL: Bug Tracker, https://github.com/Minuta18/PySocketLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PySocketLib-0.1.1/src/PySocketLib.egg-info/SOURCES.txt` & `PySocketLib-0.2/src/PySocketLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

