# Comparing `tmp/cs.debug-20221118.tar.gz` & `tmp/cs.debug-20230610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.debug-20221118.tar", last modified: Fri Nov 18 03:52:46 2022, max compression
+gzip compressed data, was "cs.debug-20230610.tar", last modified: Sat Jun 10 05:47:59 2023, max compression
```

## Comparing `cs.debug-20221118.tar` & `cs.debug-20230610.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-11-18 03:52:46.371033 cs.debug-20221118/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2022-11-18 03:52:25.000000 cs.debug-20221118/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     4918 2022-11-18 03:52:46.371250 cs.debug-20221118/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     4249 2022-11-18 03:52:28.000000 cs.debug-20221118/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-11-18 03:52:46.365720 cs.debug-20221118/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-11-18 03:52:46.366029 cs.debug-20221118/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-11-18 03:52:46.368157 cs.debug-20221118/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    15877 2022-11-18 03:52:16.000000 cs.debug-20221118/lib/python/cs/debug.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-11-18 03:52:46.370616 cs.debug-20221118/lib/python/cs.debug.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     4918 2022-11-18 03:52:46.000000 cs.debug-20221118/lib/python/cs.debug.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      292 2022-11-18 03:52:46.000000 cs.debug-20221118/lib/python/cs.debug.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2022-11-18 03:52:46.000000 cs.debug-20221118/lib/python/cs.debug.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      117 2022-11-18 03:52:46.000000 cs.debug-20221118/lib/python/cs.debug.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2022-11-18 03:52:46.000000 cs.debug-20221118/lib/python/cs.debug.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     5225 2022-11-18 03:52:36.000000 cs.debug-20221118/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      955 2022-11-18 03:52:46.372219 cs.debug-20221118/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2022-11-18 03:52:28.000000 cs.debug-20221118/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.380517 cs.debug-20230610/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-10 05:47:37.000000 cs.debug-20230610/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5601 2023-06-10 05:47:59.380653 cs.debug-20230610/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5036 2023-06-10 05:47:40.000000 cs.debug-20230610/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.374218 cs.debug-20230610/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.374569 cs.debug-20230610/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.376742 cs.debug-20230610/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    17739 2023-06-10 05:47:28.000000 cs.debug-20230610/lib/python/cs/debug.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.380220 cs.debug-20230610/lib/python/cs.debug.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5601 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      199 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6018 2023-06-10 05:47:49.000000 cs.debug-20230610/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1041 2023-06-10 05:47:59.381561 cs.debug-20230610/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-10 05:47:40.000000 cs.debug-20230610/setup.py
```

### Comparing `cs.debug-20221118/PKG-INFO` & `cs.debug-20230610/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,15 @@
-Metadata-Version: 2.1
-Name: cs.debug
-Version: 20221118
-Summary: Assorted debugging facilities.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Assorted debugging facilities.
 
-*Latest release 20221118*:
-stack_dump: cope when cs.logutils.setup_logging not run yet.
+*Latest release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -34,54 +18,73 @@
 ## Class `DebuggingLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for `threading.Lock` to trace creation and use.
 
 `cs.threads.Lock()` returns one of these in debug mode or a raw
 `threading.Lock` otherwise.
 
+*Method `DebuggingLock.acquire(self, *a)`*:
+Acquire the lock.
+
+*Method `DebuggingLock.release(self)`*:
+Release the lock.
+
 ## Class `DebuggingRLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for threading.RLock to trace creation and use.
 
 `cs.threads.RLock()` returns on of these in debug mode or a raw
 `threading.RLock` otherwise.
 
 ## Class `DebugShell(cmd.Cmd)`
 
 An interactive prompt for python statements, attached to `/dev/tty` by default.
 
+*Method `DebugShell.default(self, line)`*:
+Default command action.
+
 ## Class `DebugWrapper(types.SimpleNamespace)`
 
 Base class for classes presenting debugging wrappers.
 
 ## Function `DF(func, *a, **kw)`
 
 Wrapper for a function call to debug its use.
 
 This requires rewriting the call from `f(*a,*kw)` to `DF(f,*a,**kw)`.
 Alternatively one could rewrite as `DEBUG(f)(*a,**kw)`.
 
-## Function `Lock()`
+## Class `Lock(DebugWrapper, types.SimpleNamespace)`
+
+Wrapper class for `threading.Lock` to trace creation and use.
+
+`cs.threads.Lock()` returns one of these in debug mode or a raw
+`threading.Lock` otherwise.
+
+*Method `Lock.acquire(self, *a)`*:
+Acquire the lock.
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingLock`, otherwise a `threading.Lock`.
+*Method `Lock.release(self)`*:
+Release the lock.
 
 ## Function `openfiles(substr=None, pid=None)`
 
 Run lsof(8) against process `pid`
 returning paths of open files whose paths contain `substr`.
 
 Parameters:
 * `substr`: default substring to select by; default returns all paths.
 * `pid`: process to examine; default from `os.getpid()`.
 
-## Function `RLock()`
+## Class `RLock(DebugWrapper, types.SimpleNamespace)`
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingRLock`, otherwise a `threading.RLock`.
+Wrapper class for threading.RLock to trace creation and use.
+
+`cs.threads.RLock()` returns on of these in debug mode or a raw
+`threading.RLock` otherwise.
 
 ## Function `selftest(module_name, defaultTest=None, argv=None)`
 
 Called by my unit tests.
 
 ## Function `stack_dump(stack=None, limit=None, logger=None, log_level=None)`
 
@@ -105,26 +108,37 @@
 * `Ts`: the `Thread`s to dump; if unspecified use `threading.enumerate()`.
 * `fp`: the file to which to write; if unspecified use `sys.stderr`.
 
 ## Class `TimingOutLock`
 
 A `Lock` replacement which times out, used for locating deadlock points.
 
+## Function `trace(*da, **dkw)`
+
+Decorator to report the call and return of a function.
+
 ## Function `trace_caller(func)`
 
 Decorator to report the caller of a function when called.
 
 ## Class `TraceSuite`
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
+
 *Release 20221118*:
 stack_dump: cope when cs.logutils.setup_logging not run yet.
 
 *Release 20211208*:
 @trace moved to cs.pyfunc, other minor changes.
 
 *Release 20200318*:
```

### Comparing `cs.debug-20221118/README.md` & `cs.debug-20230610/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,58 @@
+[project]
+name = "cs.debug"
+description = "Assorted debugging facilities."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.deco>=20230331",
+    "cs.fs>=20230401",
+    "cs.lex>=20230401",
+    "cs.logutils>=20230212",
+    "cs.obj>=20220918",
+    "cs.pfx>=20230604",
+    "cs.py.func>=20230331",
+    "cs.py.stack>=20220918",
+    "cs.py3>=20220523",
+    "cs.seq>=20221118",
+    "cs.x>=20230331",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 2",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20230610"
+
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Assorted debugging facilities.
 
-*Latest release 20221118*:
-stack_dump: cope when cs.logutils.setup_logging not run yet.
+*Latest release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -14,63 +61,58 @@
 ## Class `DebuggingLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for `threading.Lock` to trace creation and use.
 
 `cs.threads.Lock()` returns one of these in debug mode or a raw
 `threading.Lock` otherwise.
 
-*Method `DebuggingLock.acquire(self, *a)`*:
-Acquire the lock.
-
-*Method `DebuggingLock.release(self)`*:
-Release the lock.
-
 ## Class `DebuggingRLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for threading.RLock to trace creation and use.
 
 `cs.threads.RLock()` returns on of these in debug mode or a raw
 `threading.RLock` otherwise.
 
 ## Class `DebugShell(cmd.Cmd)`
 
 An interactive prompt for python statements, attached to `/dev/tty` by default.
 
-*Method `DebugShell.default(self, line)`*:
-Default command action.
-
 ## Class `DebugWrapper(types.SimpleNamespace)`
 
 Base class for classes presenting debugging wrappers.
 
 ## Function `DF(func, *a, **kw)`
 
 Wrapper for a function call to debug its use.
 
 This requires rewriting the call from `f(*a,*kw)` to `DF(f,*a,**kw)`.
 Alternatively one could rewrite as `DEBUG(f)(*a,**kw)`.
 
-## Function `Lock()`
+## Class `Lock(DebugWrapper, types.SimpleNamespace)`
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingLock`, otherwise a `threading.Lock`.
+Wrapper class for `threading.Lock` to trace creation and use.
+
+`cs.threads.Lock()` returns one of these in debug mode or a raw
+`threading.Lock` otherwise.
 
 ## Function `openfiles(substr=None, pid=None)`
 
 Run lsof(8) against process `pid`
 returning paths of open files whose paths contain `substr`.
 
 Parameters:
 * `substr`: default substring to select by; default returns all paths.
 * `pid`: process to examine; default from `os.getpid()`.
 
-## Function `RLock()`
+## Class `RLock(DebugWrapper, types.SimpleNamespace)`
+
+Wrapper class for threading.RLock to trace creation and use.
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingRLock`, otherwise a `threading.RLock`.
+`cs.threads.RLock()` returns on of these in debug mode or a raw
+`threading.RLock` otherwise.
 
 ## Function `selftest(module_name, defaultTest=None, argv=None)`
 
 Called by my unit tests.
 
 ## Function `stack_dump(stack=None, limit=None, logger=None, log_level=None)`
 
@@ -94,26 +136,37 @@
 * `Ts`: the `Thread`s to dump; if unspecified use `threading.enumerate()`.
 * `fp`: the file to which to write; if unspecified use `sys.stderr`.
 
 ## Class `TimingOutLock`
 
 A `Lock` replacement which times out, used for locating deadlock points.
 
+## Function `trace(*da, **dkw)`
+
+Decorator to report the call and return of a function.
+
 ## Function `trace_caller(func)`
 
 Decorator to report the caller of a function when called.
 
 ## Class `TraceSuite`
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
+
 *Release 20221118*:
 stack_dump: cope when cs.logutils.setup_logging not run yet.
 
 *Release 20211208*:
 @trace moved to cs.pyfunc, other minor changes.
 
 *Release 20200318*:
@@ -127,17 +180,26 @@
 * Update imports for recentchanges.
 * New context manager TraceSuite to trace start and end of a code suite.
 
 *Release 20160918*:
 selftest(): fix parameter ordering to match unittest.
 
 *Release 20160828*:
-Update metadata with "install_requires" instead of "requires".
+Update metadata with \"install_requires\" instead of \"requires\".
 
 *Release 20160827*:
 * New openfiles() to return selected pathnames of open files via lsof(8).
 * New selftest() to invoke unittests with benefits.
 * DebugShell, a cmd.Cmd subclass for debugging - current use case calls this with self.__dict__ in a test case tearDwon.
 * debug_object_shell: convenience wrapper for DebugShell to call it on an object's attributes.
 
 *Release 20150116*:
-PyPI prep.
+PyPI prep."""
+content-type = "text/markdown"
+
+[build-system]
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+build-backend = "setuptools.build_meta"
```

### Comparing `cs.debug-20221118/lib/python/cs/debug.py` & `cs.debug-20230610/lib/python/cs/debug.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,78 +9,74 @@
 '''
 
 from __future__ import print_function
 from cmd import Cmd
 import inspect
 import logging
 import os
+from pprint import pformat
 from subprocess import Popen, PIPE
 import sys
-import threading
+from threading import (
+    enumerate as enumerate_threads,
+    Lock as threading_Lock,
+    RLock as threading_RLock,
+    Thread as threading_Thread,
+)
 import time
 import traceback
 from types import SimpleNamespace as NS
 
+from cs.deco import decorator
+from cs.fs import shortpath
+from cs.lex import s
 import cs.logutils
 from cs.logutils import debug, error, warning, D, ifdebug, loginfo
 from cs.obj import Proxy
 from cs.pfx import Pfx
+from cs.py.func import funccite, func_a_kw_fmt
 from cs.py.stack import caller
 from cs.py3 import Queue, Queue_Empty, exec_code
 from cs.seq import seq
 from cs.x import X
 
-__version__ = '20221118'
+__version__ = '20230610'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
+        'cs.deco',
+        'cs.fs',
+        'cs.lex',
         'cs.logutils',
         'cs.obj',
         'cs.pfx',
+        'cs.py.func',
         'cs.py.stack',
         'cs.py3',
         'cs.seq',
         'cs.x',
     ],
 }
 
 # @DEBUG dispatches a thread to monitor function elapsed time.
 # This is how often it polls for function completion.
 DEBUG_POLL_RATE = 0.25
 
-def Lock():
-  ''' Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-      then return a `DebuggingLock`, otherwise a `threading.Lock`.
-  '''
-  if not ifdebug():
-    return threading.Lock()
-  filename, lineno = inspect.stack()[1][1:3]
-  return DebuggingLock({'filename': filename, 'lineno': lineno})
-
-def RLock():
-  ''' Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-      then return a `DebuggingRLock`, otherwise a `threading.RLock`.
-  '''
-  if not ifdebug():
-    return threading.RLock()
-  filename, lineno = inspect.stack()[1][1:3]
-  return DebuggingRLock({'filename': filename, 'lineno': lineno})
-
 class TimingOutLock(object):
   ''' A `Lock` replacement which times out, used for locating deadlock points.
   '''
 
   def __init__(self, deadlock_timeout=20.0, recursive=False):
-    self._lock = threading.RLock() if recursive else threading.Lock()
+    self._lock = threading_RLock() if recursive else threading_Lock()
     self._deadlock_timeout = deadlock_timeout
 
   def acquire(self, blocking=True, timeout=-1, name=None):
     if timeout < 0:
       timeout = self._deadlock_timeout
     else:
       timeout = min(timeout, self._deadlock_timeout)
@@ -121,27 +117,27 @@
     X("TraceSuite ENTER %s", self.msg)
 
   def __exit__(self, exc_type, exc_value, exc_tb):
     X("TraceSuite LEAVE %s: exc_value=%s", self.msg, exc_value)
 
 def Thread(*a, **kw):
   if not ifdebug():
-    return threading.Thread(*a, **kw)
+    return threading_Thread(*a, **kw)
   filename, lineno = inspect.stack()[1][1:3]
   return DebuggingThread({'filename': filename, 'lineno': lineno}, *a, **kw)
 
 def thread_dump(Ts=None, fp=None):
   ''' Write thread identifiers and stack traces to the file `fp`.
 
       Parameters:
       * `Ts`: the `Thread`s to dump; if unspecified use `threading.enumerate()`.
       * `fp`: the file to which to write; if unspecified use `sys.stderr`.
   '''
   if Ts is None:
-    Ts = threading.enumerate()
+    Ts = enumerate_threads()
   if fp is None:
     fp = sys.stderr
   with Pfx("thread_dump"):
     frames = sys._current_frames()
     for T in Ts:
       try:
         frame = frames[T.ident]
@@ -186,15 +182,15 @@
 
   def inner(*a, **kw):
     if not force and not ifdebug():
       return f(*a, **kw)
     filename, lineno = inspect.stack()[1][1:3]
     n = seq()
     R = Result()
-    T = threading.Thread(
+    T = threading_Thread(
         target=_debug_watcher, args=(filename, lineno, n, f.__name__, R)
     )
     T.daemon = True
     T.start()
     debug(
         "%s:%d: [%d] call %s(*%r, **%r)", filename, lineno, n, f.__name__, a,
         kw
@@ -264,21 +260,21 @@
 class DebuggingLock(DebugWrapper):
   ''' Wrapper class for `threading.Lock` to trace creation and use.
 
       `cs.threads.Lock()` returns one of these in debug mode or a raw
       `threading.Lock` otherwise.
   '''
 
-  def __init__(self, dkw, slow=2):
+  def __init__(self, *, slow=2, **dkw):
     DebugWrapper.__init__(self, **dkw)
     self.debug("__init__(slow=%r)", slow)
     if slow <= 0:
       raise ValueError("slow must be positive, received: %r" % (slow,))
     self.slow = slow
-    self.lock = threading.Lock()
+    self.lock = threading_Lock()
     self.held = None
 
   def __enter__(self):
     ##self.lock.__enter__()
     self.acquire()
     return self
 
@@ -359,79 +355,96 @@
 class DebuggingRLock(DebugWrapper):
   ''' Wrapper class for threading.RLock to trace creation and use.
 
       `cs.threads.RLock()` returns on of these in debug mode or a raw
       `threading.RLock` otherwise.
   '''
 
-  def __init__(self, dkw):
-    D("dkw = %r", dkw)
-    DebugWrapper.__init__(self, **dkw)
+  def __init__(self, owner=None, **dkw):
+    if owner is None:
+      owner = caller()
+    DebugWrapper.__init__(
+        self, filename=owner.filename, lineno=owner.lineno, **dkw
+    )
     self.debug('__init__')
-    self.lock = threading.RLock()
-    self.stack = None
+    self.lock = threading_RLock()
+    self.stack = []
 
   def __str__(self):
-    return "%s%r" % (
-        type(self).__name__, [
-            "%s:%s:%s" % (f.filename, f.lineno, f.code_context[0].strip())
-            for f in self.stack
-        ] if self.stack else "NO_STACK"
+    return "%s[%s:%s]%s" % (
+        type(self).__name__,
+        shortpath(self.filename),
+        self.lineno,
+        "->".join(
+            ["%s:%s" % filename_lineno for filename_lineno in self.stack]
+        ),
     )
 
-  def __enter__(self):
-    filename, lineno = inspect.stack()[1][1:3]
-    self.debug('from %s:%d: __enter__ ...', filename, lineno)
-    self.lock.__enter__()
-    self.stack = inspect.stack()
-    self.debug('from %s:%d: __enter__ ENTERED', filename, lineno)
-    return self
-
-  def __exit__(self, *a):
-    filename, lineno = inspect.stack()[1][1:3]
-    self.debug('%s:%d: __exit__(*%s) ...', filename, lineno, a)
-    return self.lock.__exit__(*a)
-
-  def acquire(self, blocking=True, timeout=-1):
-    filename, lineno = inspect.stack()[0][1:3]
-    self.debug('%s:%d: acquire(blocking=%s)', filename, lineno, blocking)
+  def __enter__(self, locker=None):
+    if locker is None:
+      locker = caller()
+    filename_lineno = locker.filename, locker.lineno
+    self.debug('from %s:%d: __enter__ ...', locker.filename, locker.lineno)
+    entry = self.lock.__enter__()
+    self.stack.append(filename_lineno)
+    return entry
+
+  def __exit__(self, *a, exiter=None):
+    if exiter is None:
+      exiter = caller()
+    self.debug('%s:%d: __exit__(*%s) ...', exiter.filename, exiter.lineno, a)
+    exited = self.lock.__exit__(*a)
+    self.stack.pop()
+    return exited
+
+  def acquire(self, blocking=True, timeout=-1, acquirer=None):
+    if acquirer is None:
+      acquirer = caller()
+    self.debug(
+        '%s:%d: acquire(blocking=%s)', acquirer.filename, acquirer.lineno,
+        blocking
+    )
     if timeout < 0:
       ret = self.lock.acquire(blocking)
     else:
       ret = self.lock.acquire(blocking, timeout)
     if ret:
-      self.stack = inspect.stack()
+      self.stack.append((acquirer.filename, acquirer.lineno))
     return ret
 
-  def release(self):
-    filename, lineno = inspect.stack()[0][1:3]
-    self.debug('%s:%d: release()', filename, lineno)
+  def release(self, releaser=None):
+    if releaser is None:
+      releaser = caller()
+    self.debug('%s:%d: release()', releaser.filename, releaser.lineno)
     self.lock.release()
-    self.stack = None
+    self.stack.pop()
+
+Lock = DebuggingLock
+RLock = DebuggingRLock
 
 _debug_threads = set()
 
 def dump_debug_threads():
   D("dump_debug_threads:")
   for T in _debug_threads:
     D("dump_debug_threads: thread %r: %r", T.name, T.debug_label)
   D("dump_debug_threads done")
 
-class DebuggingThread(threading.Thread, DebugWrapper):
+class DebuggingThread(threading_Thread, DebugWrapper):
 
   def __init__(self, dkw, *a, **kw):
     DebugWrapper.__init__(self, **dkw)
     self.debug("NEW THREAD(*%r, **%r)", a, kw)
     _debug_threads.add(self)
-    threading.Thread.__init__(self, *a, **kw)
+    threading_Thread.__init__(self, *a, **kw)
 
   @DEBUG
   def join(self, timeout=None):
     self.debug("join(timeout=%r)...", timeout)
-    retval = threading.Thread.join(self, timeout=timeout)
+    retval = threading_Thread.join(self, timeout=timeout)
     self.debug("join(timeout=%r) completed", timeout)
     _debug_threads.discard(self)
     return retval
 
 def trace_caller(func):
   ''' Decorator to report the caller of a function when called.
   '''
@@ -550,14 +563,78 @@
   intro = '\n\n'
   for k in sorted(v.keys()):
     intro += '\n  %s = %r' % (k, v[k])
   intro += '\n'
   C.prompt = prompt
   C.cmdloop(intro)
 
+_trace_indent = ""
+
+@decorator
+# pylint: disable=too-many-arguments
+def trace(
+    func,
+    call=True,
+    retval=False,
+    exception=True,
+    use_pformat=False,
+    with_caller=False,
+    with_pfx=False,
+):
+  ''' Decorator to report the call and return of a function.
+  '''
+
+  citation = funccite(func)
+
+  def traced_function_wrapper(*a, **kw):
+    ''' Wrapper for `func` to trace call and return.
+    '''
+    global _trace_indent  # pylint: disable=global-statement
+    if with_pfx:
+      # late import so that we can use this in modules we import
+      # pylint: disable=import-outside-toplevel
+      try:
+        from cs.pfx import XP as xlog
+      except ImportError:
+        xlog = X
+    else:
+      xlog = X
+    log_cite = citation
+    if with_caller:
+      log_cite = log_cite + "from[%s]" % (caller(),)
+    if call:
+      fmt, av = func_a_kw_fmt(log_cite, *a, **kw)
+      xlog("%sCALL " + fmt, _trace_indent, *av)
+    old_indent = _trace_indent
+    _trace_indent += '  '
+    try:
+      result = func(*a, **kw)
+    except Exception as e:
+      if exception:
+        xlog("%sCALL %s RAISE %r", _trace_indent, log_cite, e)
+      _trace_indent = old_indent
+      raise
+    else:
+      if retval:
+        xlog(
+            "%sCALL %s RETURN %s",
+            _trace_indent,
+            log_cite,
+            (pformat if use_pformat else repr)(result),
+        )
+      else:
+        ##xlog("%sRETURN %s <= %s", _trace_indent, type(result), log_cite)
+        xlog("%sRETURN %s <= %s", _trace_indent, s(result), log_cite)
+      _trace_indent = old_indent
+      return result
+
+  traced_function_wrapper.__name__ = "@trace(%s)" % (citation,)
+  traced_function_wrapper.__doc__ = "@trace(%s)\n\n" + (func.__doc__ or '')
+  return traced_function_wrapper
+
 def selftest(module_name, defaultTest=None, argv=None):
   ''' Called by my unit tests.
   '''
   # pylint: disable=import-outside-toplevel
   if argv is None:
     argv = sys.argv
   import importlib
```

### Comparing `cs.debug-20221118/lib/python/cs.debug.egg-info/PKG-INFO` & `cs.debug-20230610/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.debug
-Version: 20221118
+Version: 20230610
 Summary: Assorted debugging facilities.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,16 +16,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted debugging facilities.
 
-*Latest release 20221118*:
-stack_dump: cope when cs.logutils.setup_logging not run yet.
+*Latest release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -56,32 +60,36 @@
 ## Function `DF(func, *a, **kw)`
 
 Wrapper for a function call to debug its use.
 
 This requires rewriting the call from `f(*a,*kw)` to `DF(f,*a,**kw)`.
 Alternatively one could rewrite as `DEBUG(f)(*a,**kw)`.
 
-## Function `Lock()`
+## Class `Lock(DebugWrapper, types.SimpleNamespace)`
+
+Wrapper class for `threading.Lock` to trace creation and use.
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingLock`, otherwise a `threading.Lock`.
+`cs.threads.Lock()` returns one of these in debug mode or a raw
+`threading.Lock` otherwise.
 
 ## Function `openfiles(substr=None, pid=None)`
 
 Run lsof(8) against process `pid`
 returning paths of open files whose paths contain `substr`.
 
 Parameters:
 * `substr`: default substring to select by; default returns all paths.
 * `pid`: process to examine; default from `os.getpid()`.
 
-## Function `RLock()`
+## Class `RLock(DebugWrapper, types.SimpleNamespace)`
+
+Wrapper class for threading.RLock to trace creation and use.
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingRLock`, otherwise a `threading.RLock`.
+`cs.threads.RLock()` returns on of these in debug mode or a raw
+`threading.RLock` otherwise.
 
 ## Function `selftest(module_name, defaultTest=None, argv=None)`
 
 Called by my unit tests.
 
 ## Function `stack_dump(stack=None, limit=None, logger=None, log_level=None)`
 
@@ -105,26 +113,37 @@
 * `Ts`: the `Thread`s to dump; if unspecified use `threading.enumerate()`.
 * `fp`: the file to which to write; if unspecified use `sys.stderr`.
 
 ## Class `TimingOutLock`
 
 A `Lock` replacement which times out, used for locating deadlock points.
 
+## Function `trace(*da, **dkw)`
+
+Decorator to report the call and return of a function.
+
 ## Function `trace_caller(func)`
 
 Decorator to report the caller of a function when called.
 
 ## Class `TraceSuite`
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
+
 *Release 20221118*:
 stack_dump: cope when cs.logutils.setup_logging not run yet.
 
 *Release 20211208*:
 @trace moved to cs.pyfunc, other minor changes.
 
 *Release 20200318*:
```

### Comparing `cs.debug-20221118/pyproject.toml` & `cs.debug-20230610/lib/python/cs.debug.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,35 @@
-[project]
-name = "cs.debug"
-description = "Assorted debugging facilities."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.logutils>=20220531",
-    "cs.obj>=20220918",
-    "cs.pfx>=20221118",
-    "cs.py.stack>=20220918",
-    "cs.py3>=20220523",
-    "cs.seq>=20221118",
-    "cs.x",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20221118"
+Metadata-Version: 2.1
+Name: cs.debug
+Version: 20230610
+Summary: Assorted debugging facilities.
+Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
+Author: Cameron Simpson
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Assorted debugging facilities.
 
-*Latest release 20221118*:
-stack_dump: cope when cs.logutils.setup_logging not run yet.
+*Latest release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -75,32 +60,36 @@
 ## Function `DF(func, *a, **kw)`
 
 Wrapper for a function call to debug its use.
 
 This requires rewriting the call from `f(*a,*kw)` to `DF(f,*a,**kw)`.
 Alternatively one could rewrite as `DEBUG(f)(*a,**kw)`.
 
-## Function `Lock()`
+## Class `Lock(DebugWrapper, types.SimpleNamespace)`
+
+Wrapper class for `threading.Lock` to trace creation and use.
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingLock`, otherwise a `threading.Lock`.
+`cs.threads.Lock()` returns one of these in debug mode or a raw
+`threading.Lock` otherwise.
 
 ## Function `openfiles(substr=None, pid=None)`
 
 Run lsof(8) against process `pid`
 returning paths of open files whose paths contain `substr`.
 
 Parameters:
 * `substr`: default substring to select by; default returns all paths.
 * `pid`: process to examine; default from `os.getpid()`.
 
-## Function `RLock()`
+## Class `RLock(DebugWrapper, types.SimpleNamespace)`
 
-Factory function: if `cs.logutils.loginfo.level<=logging.DEBUG`
-then return a `DebuggingRLock`, otherwise a `threading.RLock`.
+Wrapper class for threading.RLock to trace creation and use.
+
+`cs.threads.RLock()` returns on of these in debug mode or a raw
+`threading.RLock` otherwise.
 
 ## Function `selftest(module_name, defaultTest=None, argv=None)`
 
 Called by my unit tests.
 
 ## Function `stack_dump(stack=None, limit=None, logger=None, log_level=None)`
 
@@ -124,26 +113,37 @@
 * `Ts`: the `Thread`s to dump; if unspecified use `threading.enumerate()`.
 * `fp`: the file to which to write; if unspecified use `sys.stderr`.
 
 ## Class `TimingOutLock`
 
 A `Lock` replacement which times out, used for locating deadlock points.
 
+## Function `trace(*da, **dkw)`
+
+Decorator to report the call and return of a function.
+
 ## Function `trace_caller(func)`
 
 Decorator to report the caller of a function when called.
 
 ## Class `TraceSuite`
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230610*:
+* DebuggingRLock fixes.
+* Move @trace from cs.py.func to cs.debug.
+* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
+* Rename threading.Thread to threading_Thread.
+* Simplify the debugging lock classes.
+
 *Release 20221118*:
 stack_dump: cope when cs.logutils.setup_logging not run yet.
 
 *Release 20211208*:
 @trace moved to cs.pyfunc, other minor changes.
 
 *Release 20200318*:
@@ -157,26 +157,17 @@
 * Update imports for recentchanges.
 * New context manager TraceSuite to trace start and end of a code suite.
 
 *Release 20160918*:
 selftest(): fix parameter ordering to match unittest.
 
 *Release 20160828*:
-Update metadata with \"install_requires\" instead of \"requires\".
+Update metadata with "install_requires" instead of "requires".
 
 *Release 20160827*:
 * New openfiles() to return selected pathnames of open files via lsof(8).
 * New selftest() to invoke unittests with benefits.
 * DebugShell, a cmd.Cmd subclass for debugging - current use case calls this with self.__dict__ in a test case tearDwon.
 * debug_object_shell: convenience wrapper for DebugShell to call it on an object's attributes.
 
 *Release 20150116*:
-PyPI prep."""
-content-type = "text/markdown"
-
-[build-system]
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-build-backend = "setuptools.build_meta"
+PyPI prep.
```

### Comparing `cs.debug-20221118/setup.cfg` & `cs.debug-20230610/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.debug
-version = 20221118
+version = 20230610
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Assorted debugging facilities.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -19,19 +19,23 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
-	cs.logutils>=20220531
+	cs.deco>=20230331
+	cs.fs>=20230401
+	cs.lex>=20230401
+	cs.logutils>=20230212
 	cs.obj>=20220918
-	cs.pfx>=20221118
+	cs.pfx>=20230604
+	cs.py.func>=20230331
 	cs.py.stack>=20220918
 	cs.py3>=20220523
 	cs.seq>=20221118
-	cs.x
+	cs.x>=20230331
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

