# Comparing `tmp/cross_process_bridge-0.0.1.tar.gz` & `tmp/cross_process_bridge-1.0.0.tar.gz`

## Comparing `cross_process_bridge-0.0.1.tar` & `cross_process_bridge-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/examples/example.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/src/cross_process_bridge/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/src/cross_process_bridge/cross_process_bridge.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/src/cross_process_bridge/instance_creator.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/src/cross_process_bridge/models.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/src/cross_process_bridge/run_cross_process.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/LICENSE
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 cross_process_bridge-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/.DS_Store
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/examples/basic.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/examples/extended_inheritance.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/__init__.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/child_process_bridge.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/cross_process_bridge.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/instance_creator.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/models.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/PKG-INFO
```

### Comparing `cross_process_bridge-0.0.1/examples/example.py` & `cross_process_bridge-1.0.0/examples/extended_inheritance.py`

 * *Files identical despite different names*

### Comparing `cross_process_bridge-0.0.1/src/cross_process_bridge/cross_process_bridge.py` & `cross_process_bridge-1.0.0/src/cross_process_bridge/cross_process_bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from multiprocessing import Queue, Process
 
 from cross_process_bridge.instance_creator import InstanceCreator
 from cross_process_bridge.models import TaskResult, TaskRequest
-from cross_process_bridge.run_cross_process import run_cross_process
+from cross_process_bridge.child_process_bridge import run_cross_process
 
 
 class CrossProcessMetaclass(type):
     @classmethod
     def _insert_wrapper_functions(cls, dct, base):
         for key, value in base.__dict__.items():
             if callable(value) and key not in ('__init__', 'start', 'stop'):
```

### Comparing `cross_process_bridge-0.0.1/src/cross_process_bridge/run_cross_process.py` & `cross_process_bridge-1.0.0/src/cross_process_bridge/child_process_bridge.py`

 * *Files identical despite different names*

### Comparing `cross_process_bridge-0.0.1/LICENSE` & `cross_process_bridge-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cross_process_bridge-0.0.1/README.md` & `cross_process_bridge-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Cross Process
+# Cross Process Bridge
 
 This package is a utility for creating an instance of a class in a new process and seamlessly calling its functions from
 the original process  
   
 ## Background
 ### multiprocessing
 let's say I have a class that needs to do something that affects the whole process - for example changing the working 
@@ -57,27 +57,27 @@
 new process.  
 when I am done i can call `stop()` which will stop the process
 
 #### Complete example:
 
 ```python
 import os
-from cross_process_bridge.cross_process_bridge import CrossProcessBridge
+from cross_process_bridge import CrossProcessBridge
 
 
 class A:
     def a(self):
         print('a', os.getpid())
 
 
 class B(A, CrossProcessBridge):
     pass
 
 
 if __name__ == '__main__':
     pid = os.getpid()
     print(pid)  # print the pid of the original process
-    b = B()  # create the bridge instance
-    b.start()  # start the process and create an instance in it
-    b.a()  # call the `a()` function - will print a different pid
-    b.stop()  # stop the process
+    b = B()     # create the bridge instance
+    b.start()   # start the process and create an instance in it
+    b.a()       # call the `a()` function - will print a different pid
+    b.stop()    # stop the process
 ```
```

### Comparing `cross_process_bridge-0.0.1/pyproject.toml` & `cross_process_bridge-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cross_process_bridge"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Avi Mayer", email="mayeravraham@gmail.com" },
 ]
 description = "A utility to create an instance in another process and call its functions seamlessly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cross_process_bridge-0.0.1/PKG-INFO` & `cross_process_bridge-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: cross_process_bridge
-Version: 0.0.1
+Version: 1.0.0
 Summary: A utility to create an instance in another process and call its functions seamlessly
 Project-URL: Homepage, https://github.com/avraham-mayer/python-cross-process-bridge
 Author-email: Avi Mayer <mayeravraham@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Cross Process
+# Cross Process Bridge
 
 This package is a utility for creating an instance of a class in a new process and seamlessly calling its functions from
 the original process  
   
 ## Background
 ### multiprocessing
 let's say I have a class that needs to do something that affects the whole process - for example changing the working 
@@ -70,27 +70,27 @@
 new process.  
 when I am done i can call `stop()` which will stop the process
 
 #### Complete example:
 
 ```python
 import os
-from cross_process_bridge.cross_process_bridge import CrossProcessBridge
+from cross_process_bridge import CrossProcessBridge
 
 
 class A:
     def a(self):
         print('a', os.getpid())
 
 
 class B(A, CrossProcessBridge):
     pass
 
 
 if __name__ == '__main__':
     pid = os.getpid()
     print(pid)  # print the pid of the original process
-    b = B()  # create the bridge instance
-    b.start()  # start the process and create an instance in it
-    b.a()  # call the `a()` function - will print a different pid
-    b.stop()  # stop the process
+    b = B()     # create the bridge instance
+    b.start()   # start the process and create an instance in it
+    b.a()       # call the `a()` function - will print a different pid
+    b.stop()    # stop the process
 ```
```

