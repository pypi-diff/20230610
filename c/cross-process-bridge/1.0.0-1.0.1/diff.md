# Comparing `tmp/cross_process_bridge-1.0.0.tar.gz` & `tmp/cross_process_bridge-1.0.1.tar.gz`

## Comparing `cross_process_bridge-1.0.0.tar` & `cross_process_bridge-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/.DS_Store
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/examples/basic.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/examples/extended_inheritance.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/__init__.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/child_process_bridge.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/cross_process_bridge.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/instance_creator.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/src/cross_process_bridge/models.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/LICENSE
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/.DS_Store
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/examples/basic.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/examples/context_example.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/examples/extended_inheritance.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/src/cross_process_bridge/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/src/cross_process_bridge/child_process_bridge.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/src/cross_process_bridge/cross_process_bridge.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/src/cross_process_bridge/instance_creator.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/src/cross_process_bridge/models.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/README.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 cross_process_bridge-1.0.1/PKG-INFO
```

### Comparing `cross_process_bridge-1.0.0/.DS_Store` & `cross_process_bridge-1.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `cross_process_bridge-1.0.0/src/cross_process_bridge/child_process_bridge.py` & `cross_process_bridge-1.0.1/src/cross_process_bridge/child_process_bridge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from multiprocessing import Queue
-from typing import Tuple, Any
 
 from cross_process_bridge.instance_creator import InstanceCreator
 from cross_process_bridge.models import TaskRequest, TaskResult
 
 
 class ChildProcessBridge:
     def __init__(self, task_queue: Queue, response_queue: Queue, instance_creator: InstanceCreator):
```

### Comparing `cross_process_bridge-1.0.0/src/cross_process_bridge/cross_process_bridge.py` & `cross_process_bridge-1.0.1/src/cross_process_bridge/cross_process_bridge.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import os
 from multiprocessing import Queue, Process
+from typing import Optional
 
+from cross_process_bridge.child_process_bridge import run_cross_process
 from cross_process_bridge.instance_creator import InstanceCreator
 from cross_process_bridge.models import TaskResult, TaskRequest
-from cross_process_bridge.child_process_bridge import run_cross_process
 
 
 class CrossProcessMetaclass(type):
     @classmethod
     def _insert_wrapper_functions(cls, dct, base):
         for key, value in base.__dict__.items():
             if callable(value) and key not in ('__init__', 'start', 'stop'):
@@ -23,26 +23,29 @@
         if bases[1] is not CrossProcessBridge:
             raise Exception('must inherit from CrossProcessBridge second')
         if len(bases) != 2:
             raise Exception('must have exactly one base other than CrossProcessBridge')
 
         real_base = bases[0]
         cls._insert_wrapper_functions(dct, real_base)
+        dct['__getattr__'] = CrossProcessBridge.create_cross_process_function('__getattribute__')
+        custom_setattr = CrossProcessBridge.create_cross_process_function('__setattr__')
+        dct['custom_setattr'] = custom_setattr
 
         dct['real_base'] = real_base
         return super().__new__(cls, name, (CrossProcessBridge, real_base), dct)
 
 
 class CrossProcessBridge(metaclass=CrossProcessMetaclass):
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
         self.task_queue = Queue()
         self.response_queue = Queue()
-        self.process: Process = None
+        self.process: Optional[Process] = None
 
     def start(self, *args, **kwargs):
         if self.process is None or not self.process.is_alive():
             instance_creator = InstanceCreator(self.real_base, *self.args, **self.kwargs)
             self.process = Process(target=run_cross_process,
                                    args=(self.task_queue, self.response_queue, instance_creator))
             self.process.start()
@@ -64,7 +67,26 @@
             self.task_queue.put(TaskRequest(item, *args, **kwargs))
             result: TaskResult = self.response_queue.get()
             if result.exception is not None:
                 raise result.exception
             return result.retval
 
         return cross_process_function
+
+    def __del__(self):
+        self.stop()
+
+    def __setattr__(self, key, value):
+        if (key in self.__dict__ or
+                'process' not in self.__dict__ or
+                self.process is None or
+                not self.process.is_alive()):
+            return super().__setattr__(key, value)
+
+        return self.custom_setattr(key, value)
+
+    def __enter__(self):
+        self.start()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.stop()
```

### Comparing `cross_process_bridge-1.0.0/LICENSE` & `cross_process_bridge-1.0.1/LICENSE`

 * *Files identical despite different names*

