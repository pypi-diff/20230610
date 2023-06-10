# Comparing `tmp/PySocketLib-0.2.1.tar.gz` & `tmp/PySocketLib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySocketLib-0.2.1.tar", last modified: Sat Jun 10 14:46:23 2023, max compression
+gzip compressed data, was "PySocketLib-0.2.2.tar", last modified: Sat Jun 10 15:05:21 2023, max compression
```

## Comparing `PySocketLib-0.2.1.tar` & `PySocketLib-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/
--rw-rw-r--   0 igors     (1000) igors     (1000)     1069 2023-06-10 09:19:23.000000 PySocketLib-0.2.1/LICENSE
--rw-rw-r--   0 igors     (1000) igors     (1000)     3661 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)     3135 2023-06-10 14:44:47.000000 PySocketLib-0.2.1/README.md
--rw-rw-r--   0 igors     (1000) igors     (1000)      511 2023-06-10 14:46:14.000000 PySocketLib-0.2.1/pyproject.toml
--rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/setup.cfg
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.053643 PySocketLib-0.2.1/src/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/CExceptions/
--rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.2.1/src/PySocketLib/CExceptions/InitExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       74 2023-06-05 14:38:04.000000 PySocketLib-0.2.1/src/PySocketLib/CExceptions/ProtocolExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       61 2023-06-03 17:39:57.000000 PySocketLib-0.2.1/src/PySocketLib/CExceptions/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/Client/
--rw-rw-r--   0 igors     (1000) igors     (1000)      964 2023-06-10 14:30:50.000000 PySocketLib-0.2.1/src/PySocketLib/Client/Client.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      214 2023-06-02 19:35:46.000000 PySocketLib-0.2.1/src/PySocketLib/Client/ConnectedClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       71 2023-06-03 13:07:20.000000 PySocketLib-0.2.1/src/PySocketLib/Client/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib/Server/
--rw-rw-r--   0 igors     (1000) igors     (1000)     3126 2023-06-10 14:30:39.000000 PySocketLib-0.2.1/src/PySocketLib/Server/Server.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      773 2023-06-10 14:31:48.000000 PySocketLib-0.2.1/src/PySocketLib/Server/TCPServer.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       59 2023-06-03 13:06:22.000000 PySocketLib-0.2.1/src/PySocketLib/Server/__init__.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       67 2023-06-10 06:43:20.000000 PySocketLib-0.2.1/src/PySocketLib/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 14:46:23.057643 PySocketLib-0.2.1/src/PySocketLib.egg-info/
--rw-rw-r--   0 igors     (1000) igors     (1000)     3661 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)      566 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/SOURCES.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/dependency_links.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)       12 2023-06-10 14:46:23.000000 PySocketLib-0.2.1/src/PySocketLib.egg-info/top_level.txt
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.779314 PySocketLib-0.2.2/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1069 2023-06-10 09:19:23.000000 PySocketLib-0.2.2/LICENSE
+-rw-rw-r--   0 igors     (1000) igors     (1000)      966 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      439 2023-06-10 15:03:43.000000 PySocketLib-0.2.2/README.md
+-rw-rw-r--   0 igors     (1000) igors     (1000)      511 2023-06-10 15:04:25.000000 PySocketLib-0.2.2/pyproject.toml
+-rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-06-10 15:05:21.779314 PySocketLib-0.2.2/setup.cfg
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      409 2023-06-10 14:30:53.000000 PySocketLib-0.2.2/src/ExampleClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1143 2023-06-10 14:30:45.000000 PySocketLib-0.2.2/src/ExampleServer.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/CExceptions/
+-rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.2.2/src/PySocketLib/CExceptions/InitExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       74 2023-06-05 14:38:04.000000 PySocketLib-0.2.2/src/PySocketLib/CExceptions/ProtocolExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       61 2023-06-03 17:39:57.000000 PySocketLib-0.2.2/src/PySocketLib/CExceptions/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/Client/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      964 2023-06-10 14:30:50.000000 PySocketLib-0.2.2/src/PySocketLib/Client/Client.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      214 2023-06-02 19:35:46.000000 PySocketLib-0.2.2/src/PySocketLib/Client/ConnectedClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       71 2023-06-03 13:07:20.000000 PySocketLib-0.2.2/src/PySocketLib/Client/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/Server/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3126 2023-06-10 14:30:39.000000 PySocketLib-0.2.2/src/PySocketLib/Server/Server.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      773 2023-06-10 14:31:48.000000 PySocketLib-0.2.2/src/PySocketLib/Server/TCPServer.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       59 2023-06-03 13:06:22.000000 PySocketLib-0.2.2/src/PySocketLib/Server/__init__.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       67 2023-06-10 06:43:20.000000 PySocketLib-0.2.2/src/PySocketLib/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib.egg-info/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      966 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      608 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/SOURCES.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/dependency_links.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)       40 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/top_level.txt
```

### Comparing `PySocketLib-0.2.1/LICENSE` & `PySocketLib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.2.1/src/PySocketLib/Client/Client.py` & `PySocketLib-0.2.2/src/PySocketLib/Client/Client.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.2.1/src/PySocketLib/Server/Server.py` & `PySocketLib-0.2.2/src/PySocketLib/Server/Server.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.2.1/src/PySocketLib/Server/TCPServer.py` & `PySocketLib-0.2.2/src/PySocketLib/Server/TCPServer.py`

 * *Files identical despite different names*

