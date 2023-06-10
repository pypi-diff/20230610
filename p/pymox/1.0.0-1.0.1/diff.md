# Comparing `tmp/pymox-1.0.0.tar.gz` & `tmp/pymox-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymox-1.0.0.tar", last modified: Tue Apr 18 12:50:20 2023, max compression
+gzip compressed data, was "pymox-1.0.1.tar", max compression
```

## Comparing `pymox-1.0.0.tar` & `pymox-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,6 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.613649 pymox-1.0.0/
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.585655 pymox-1.0.0/.github/
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.599577 pymox-1.0.0/.github/workflows/
--rw-r--r--   0 ivan       (501) staff       (20)     1072 2023-04-18 12:46:52.000000 pymox-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 ivan       (501) staff       (20)      593 2023-04-18 11:46:42.000000 pymox-1.0.0/.gitignore
--rw-r--r--   0 ivan       (501) staff       (20)     1632 2023-04-18 11:55:35.000000 pymox-1.0.0/CHANGELOG.rst
--rw-r--r--   0 ivan       (501) staff       (20)    11358 2023-04-18 11:36:57.000000 pymox-1.0.0/COPYING
--rw-r--r--   0 ivan       (501) staff       (20)      170 2023-04-18 11:36:57.000000 pymox-1.0.0/MANIFEST.in
--rw-r--r--   0 ivan       (501) staff       (20)     3981 2023-04-18 12:50:20.613979 pymox-1.0.0/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      991 2023-04-18 11:46:42.000000 pymox-1.0.0/README.rst
--rw-r--r--   0 ivan       (501) staff       (20)    38183 2023-04-18 12:08:17.000000 pymox-1.0.0/coverage.xml
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.607957 pymox-1.0.0/docs/
--rw-r--r--   0 ivan       (501) staff       (20)      605 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/Makefile
--rw-r--r--   0 ivan       (501) staff       (20)     5485 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/conf.py
--rw-r--r--   0 ivan       (501) staff       (20)    24561 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/examples.rst
--rw-r--r--   0 ivan       (501) staff       (20)     1590 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/index.rst
--rw-r--r--   0 ivan       (501) staff       (20)      232 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/install.rst
--rw-r--r--   0 ivan       (501) staff       (20)      803 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/make.bat
--rw-r--r--   0 ivan       (501) staff       (20)     2621 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/reference.rst
--rw-r--r--   0 ivan       (501) staff       (20)    22290 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/tutorial.rst
--rw-r--r--   0 ivan       (501) staff       (20)     6431 2023-04-18 11:36:57.000000 pymox-1.0.0/docs/why.rst
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.593443 pymox-1.0.0/mox/
--rw-r--r--   0 ivan       (501) staff       (20)      738 2023-04-18 12:21:18.000000 pymox-1.0.0/mox/__init__.py
--rwxr-xr-x   0 ivan       (501) staff       (20)    74474 2023-04-18 11:36:57.000000 pymox-1.0.0/mox/mox.py
--rw-r--r--   0 ivan       (501) staff       (20)     5579 2023-04-18 11:36:57.000000 pymox-1.0.0/mox/stubout.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.612177 pymox-1.0.0/pymox.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)     3981 2023-04-18 12:50:20.000000 pymox-1.0.0/pymox.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     1055 2023-04-18 12:50:20.000000 pymox-1.0.0/pymox.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-04-18 12:50:20.000000 pymox-1.0.0/pymox.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-04-18 11:38:02.000000 pymox-1.0.0/pymox.egg-info/not-zip-safe
--rw-r--r--   0 ivan       (501) staff       (20)       12 2023-04-18 12:50:20.000000 pymox-1.0.0/pymox.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)        9 2023-04-18 12:50:20.000000 pymox-1.0.0/pymox.egg-info/top_level.txt
--rw-r--r--   0 ivan       (501) staff       (20)       12 2023-04-18 11:36:57.000000 pymox-1.0.0/requirements.txt
--rw-r--r--   0 ivan       (501) staff       (20)      189 2023-04-18 12:50:20.614986 pymox-1.0.0/setup.cfg
--rwxr-xr-x   0 ivan       (501) staff       (20)     2781 2023-04-18 11:58:17.000000 pymox-1.0.0/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.596146 pymox-1.0.0/test/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-18 11:36:57.000000 pymox-1.0.0/test/__init__.py
--rwxr-xr-x   0 ivan       (501) staff       (20)    95793 2023-04-18 11:36:57.000000 pymox-1.0.0/test/mox_test.py
--rwxr-xr-x   0 ivan       (501) staff       (20)     5534 2023-04-18 11:36:57.000000 pymox-1.0.0/test/mox_test_helper.py
--rw-r--r--   0 ivan       (501) staff       (20)     1309 2023-04-18 11:36:57.000000 pymox-1.0.0/test/stubout_test.py
--rw-r--r--   0 ivan       (501) staff       (20)      649 2023-04-18 11:36:57.000000 pymox-1.0.0/test/stubout_testee.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.597448 pymox-1.0.0/test/test_helpers/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-18 11:36:57.000000 pymox-1.0.0/test/test_helpers/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-18 11:36:57.000000 pymox-1.0.0/test/test_helpers/first_import.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-18 12:50:20.598451 pymox-1.0.0/test/test_helpers/subpackage/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-18 11:36:57.000000 pymox-1.0.0/test/test_helpers/subpackage/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)       71 2023-04-18 11:36:57.000000 pymox-1.0.0/test/test_helpers/subpackage/faraway.py
--rw-r--r--   0 ivan       (501) staff       (20)      446 2023-04-18 12:00:17.000000 pymox-1.0.0/tox.ini
+-rw-r--r--   0        0        0      991 2023-06-10 12:41:09.548531 pymox-1.0.1/README.rst
+-rw-r--r--   0        0        0      732 2023-06-10 12:36:46.185084 pymox-1.0.1/mox/__init__.py
+-rwxr-xr-x   0        0        0    73306 2023-06-10 12:36:46.186655 pymox-1.0.1/mox/mox.py
+-rw-r--r--   0        0        0     5368 2023-06-10 12:36:46.188124 pymox-1.0.1/mox/stubout.py
+-rw-r--r--   0        0        0     2271 2023-06-10 12:41:16.705049 pymox-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 pymox-1.0.1/PKG-INFO
```

### Comparing `pymox-1.0.0/README.rst` & `pymox-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymox-1.0.0/mox/mox.py` & `pymox-1.0.1/mox/mox.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,26 +61,24 @@
   my_mox.VerifyAll()
 """
 
 try:
     import abc
 except ImportError:
     abc = None  # Python 2.5 and earlier
-from collections import deque
 import difflib
 import inspect
 import re
-import six
 import types
 import unittest
+from collections import deque
+from re import search as re_search
 
 from . import stubout
 
-from re import search as re_search
-
 
 class Error(AssertionError):
     """Base exception for this module."""
 
     pass
 
 
@@ -104,16 +102,15 @@
 
         if not expected_methods:
             raise ValueError("There must be at least one expected method")
         Error.__init__(self)
         self._expected_methods = expected_methods
 
     def __str__(self):
-        calls = "\n".join(["%3d.  %s" % (i, m)
-                           for i, m in enumerate(self._expected_methods)])
+        calls = "\n".join(["%3d.  %s" % (i, m) for i, m in enumerate(self._expected_methods)])
         return "Verify: Expected methods never called:\n%s" % (calls,)
 
 
 class UnexpectedMethodCallError(Error):
     """Raised when an unexpected method is called.
 
     This can occur if a method is called with incorrect parameters, or out of
@@ -133,19 +130,17 @@
         """
 
         Error.__init__(self)
         if expected is None:
             self._str = "Unexpected method call %s" % (unexpected_method,)
         else:
             differ = difflib.Differ()
-            diff = differ.compare(str(unexpected_method).splitlines(True),
-                                  str(expected).splitlines(True))
-            self._str = (
-                "Unexpected method call.  unexpected:-  expected:+\n%s"
-                % ("\n".join(line.rstrip() for line in diff),)
+            diff = differ.compare(str(unexpected_method).splitlines(True), str(expected).splitlines(True))
+            self._str = "Unexpected method call.  unexpected:-  expected:+\n%s" % (
+                "\n".join(line.rstrip() for line in diff),
             )
 
     def __str__(self):
         return self._str
 
 
 class UnknownMethodCallError(Error):
@@ -160,30 +155,28 @@
           unknown_method_name: str
         """
 
         Error.__init__(self)
         self._unknown_method_name = unknown_method_name
 
     def __str__(self):
-        return "Method called is not a member of the object: %s" % \
-               self._unknown_method_name
+        return "Method called is not a member of the object: %s" % self._unknown_method_name
 
 
 class PrivateAttributeError(Error):
     """
     Raised if a MockObject is passed a private additional attribute name.
     """
 
     def __init__(self, attr):
         Error.__init__(self)
         self._attr = attr
 
     def __str__(self):
-        return ("Attribute '%s' is private and should not be available in a "
-                " mock object." % self._attr)
+        return "Attribute '%s' is private and should not be available in a " " mock object." % self._attr
 
 
 class ExpectedMockCreationError(Error):
     """Raised if mocks should have been created by StubOutClassWithMocks."""
 
     def __init__(self, expected_mocks):
         """Init exception.
@@ -198,16 +191,15 @@
 
         if not expected_mocks:
             raise ValueError("There must be at least one expected method")
         Error.__init__(self)
         self._expected_mocks = expected_mocks
 
     def __str__(self):
-        mocks = "\n".join(["%3d.  %s" % (i, m)
-                           for i, m in enumerate(self._expected_mocks)])
+        mocks = "\n".join(["%3d.  %s" % (i, m) for i, m in enumerate(self._expected_mocks)])
         return "Verify: Expected mocks never created:\n%s" % (mocks,)
 
 
 class UnexpectedMockCreationError(Error):
     """Raised if too many mocks were created by StubOutClassWithMocks."""
 
     def __init__(self, instance, *params, **named_params):
@@ -225,16 +217,15 @@
         self._named_params = named_params
 
     def __str__(self):
         args = ", ".join(["%s" % v for i, v in enumerate(self._params)])
         error = "Unexpected mock creation: %s(%s" % (self._instance, args)
 
         if self._named_params:
-            error += ", " + ", ".join(["%s=%s" % (k, v) for k, v in
-                                       six.iteritems(self._named_params)])
+            error += ", " + ", ".join(["%s=%s" % (k, v) for k, v in self._named_params.items()])
 
         error += ")"
         return error
 
 
 class SwallowedExceptionError(Error):
     """Raised when Verify() is called after something already threw an
@@ -252,42 +243,41 @@
           previous_exceptions: [Error]
         """
 
         Error.__init__(self)
         self._previous_exceptions = previous_exceptions
 
     def __str__(self):
-        exceptions = "\n".join([
-            "%3d.  %s: %s" % (i, e.__class__.__name__, e)
-            for i, e in enumerate(self._previous_exceptions)
-        ])
+        exceptions = "\n".join(
+            ["%3d.  %s: %s" % (i, e.__class__.__name__, e) for i, e in enumerate(self._previous_exceptions)]
+        )
         return "Previous exceptions thrown:\n%s" % (exceptions,)
 
 
 class Mox(object):
     """Mox: a factory for creating mock objects."""
 
     # A list of types that should be stubbed out with MockObjects (as
     # opposed to MockAnythings).
     _USE_MOCK_OBJECT = [
-        getattr(types, 'ClassType', type),
+        getattr(types, "ClassType", type),
         types.FunctionType,
-        getattr(types, 'InstanceType', object),
+        getattr(types, "InstanceType", object),
         types.ModuleType,
-        getattr(types, 'ObjectType', object),
-        getattr(types, 'TypeType', type),
+        getattr(types, "ObjectType", object),
+        getattr(types, "TypeType", type),
         types.MethodType,
-        getattr(types, 'UnboundMethodType', types.FunctionType),
+        getattr(types, "UnboundMethodType", types.FunctionType),
     ]
 
     # A list of types that may be stubbed out with a MockObjectFactory.
     _USE_MOCK_FACTORY = [
-        getattr(types, 'ClassType', type),
-        getattr(types, 'ObjectType', object),
-        getattr(types, 'TypeType', type),
+        getattr(types, "ClassType", type),
+        getattr(types, "ObjectType", object),
+        getattr(types, "TypeType", type),
     ]
     if abc:
         _USE_MOCK_FACTORY.append(abc.ABCMeta)
 
     def __init__(self):
         """Initialize a new Mox."""
 
@@ -358,26 +348,26 @@
             regardless of the type of attribute.
         """
 
         attr_to_replace = getattr(obj, attr_name)
         attr_type = type(attr_to_replace)
 
         if attr_type == MockAnything or attr_type == MockObject:
-            raise TypeError('Cannot mock a MockAnything! Did you remember to '
-                            'call UnsetStubs in your previous test?')
+            raise TypeError("Cannot mock a MockAnything! Did you remember to " "call UnsetStubs in your previous test?")
 
-        if (attr_type in self._USE_MOCK_OBJECT or
-                # isinstance(attr_type, tuple(self._USE_MOCK_OBJECT)) or
-                isinstance(attr_to_replace, object) or
-                inspect.isclass(attr_to_replace)) and not use_mock_anything:
+        if (
+            attr_type in self._USE_MOCK_OBJECT
+            or
+            # isinstance(attr_type, tuple(self._USE_MOCK_OBJECT)) or
+            isinstance(attr_to_replace, object)
+            or inspect.isclass(attr_to_replace)
+        ) and not use_mock_anything:
             stub = self.CreateMock(attr_to_replace)
         else:
-            stub = self.CreateMockAnything(
-                description='Stub for %s' % attr_to_replace
-            )
+            stub = self.CreateMockAnything(description="Stub for %s" % attr_to_replace)
             stub.__name__ = attr_name
 
         self.stubs.Set(obj, attr_name, stub)
 
     def StubOutClassWithMocks(self, obj, attr_name):
         """Replace a class with a "mock factory" that will create mock objects.
 
@@ -416,19 +406,18 @@
         my_import.FooClass(9, 10)  # Returns mock2 again.
         mox.VerifyAll()
         """
         attr_to_replace = getattr(obj, attr_name)
         attr_type = type(attr_to_replace)
 
         if attr_type == MockAnything or attr_type == MockObject:
-            raise TypeError('Cannot mock a MockAnything! Did you remember to '
-                            'call UnsetStubs in your previous test?')
+            raise TypeError("Cannot mock a MockAnything! Did you remember to " "call UnsetStubs in your previous test?")
 
         if not inspect.isclass(attr_to_replace):
-            raise TypeError('Given attr is not a Class.  Use StubOutWithMock.')
+            raise TypeError("Given attr is not a Class.  Use StubOutWithMock.")
 
         factory = _MockObjectFactory(attr_to_replace, self)
         self._mock_objects.append(factory)
         self.stubs.Set(obj, attr_name, factory)
 
     def UnsetStubs(self):
         """Restore stubs to their original state."""
@@ -493,26 +482,26 @@
         pass
 
     def __methods__(self):
         pass
 
     def __repr__(self):
         if self._description:
-            return '<MockAnything instance of %s>' % self._description
+            return "<MockAnything instance of %s>" % self._description
         else:
-            return '<MockAnything instance>'
+            return "<MockAnything instance>"
 
     def __str__(self):
-        return self._CreateMockMethod('__str__')()
+        return self._CreateMockMethod("__str__")()
 
     def __call__(self, *args, **kwargs):
-        return self._CreateMockMethod('__call__')(*args, **kwargs)
+        return self._CreateMockMethod("__call__")(*args, **kwargs)
 
     def __getitem__(self, i):
-        return self._CreateMockMethod('__getitem__')(i)
+        return self._CreateMockMethod("__getitem__")(i)
 
     def __getattr__(self, method_name):
         """Intercept method calls on this object.
 
          A new MockMethod is returned that is aware of the MockAnything's
          state (record or replay).  The call will be recorded or replayed
          by the MockMethod's __call__.
@@ -520,15 +509,15 @@
         Args:
           # method name: the name of the method being called.
           method_name: str
 
         Returns:
           A new MockMethod aware of MockAnything's state (record or replay).
         """
-        if method_name == '__dir__':
+        if method_name == "__dir__":
             return self.__class__.__dir__.__get__(self, self.__class__)
 
         return self._CreateMockMethod(method_name)
 
     def _CreateMockMethod(self, method_name, method_to_mock=None):
         """Create a new mock method call and return it.
 
@@ -539,30 +528,36 @@
           method_name: str
           method_to_mock: a method object
 
         Returns:
           A new MockMethod aware of MockAnything's state (record or replay).
         """
 
-        return MockMethod(method_name, self._expected_calls_queue,
-                          self._exceptions_thrown, self._replay_mode,
-                          method_to_mock=method_to_mock,
-                          description=self._description)
+        return MockMethod(
+            method_name,
+            self._expected_calls_queue,
+            self._exceptions_thrown,
+            self._replay_mode,
+            method_to_mock=method_to_mock,
+            description=self._description,
+        )
 
     def __nonzero__(self):
         """Return 1 for nonzero so the mock can be used as a conditional."""
 
         return 1
 
     def __eq__(self, rhs):
         """Provide custom logic to compare objects."""
 
-        return (isinstance(rhs, MockAnything) and
-                self._replay_mode == rhs._replay_mode and
-                self._expected_calls_queue == rhs._expected_calls_queue)
+        return (
+            isinstance(rhs, MockAnything)
+            and self._replay_mode == rhs._replay_mode
+            and self._expected_calls_queue == rhs._expected_calls_queue
+        )
 
     def __ne__(self, rhs):
         """Provide custom logic to compare objects."""
 
         return not self == rhs
 
     def _Replay(self):
@@ -584,22 +579,21 @@
         # happen if the original exception was swallowed, in which case it's
         # necessary to re-raise it so that the test will fail.  See Issue #16.)
         if self._exceptions_thrown:
             raise SwallowedExceptionError(self._exceptions_thrown)
         # If the list of expected calls is not empty, raise an exception
         if self._expected_calls_queue:
             # The last MultipleTimesGroup is not popped from the queue.
-            is_multiple_times_group = isinstance(
-                self._expected_calls_queue[0],
-                MultipleTimesGroup
-            )
+            is_multiple_times_group = isinstance(self._expected_calls_queue[0], MultipleTimesGroup)
 
-            if (len(self._expected_calls_queue) == 1 and
-                    is_multiple_times_group and
-                    self._expected_calls_queue[0].IsSatisfied()):
+            if (
+                len(self._expected_calls_queue) == 1
+                and is_multiple_times_group
+                and self._expected_calls_queue[0].IsSatisfied()
+            ):
                 pass
             else:
                 raise ExpectedMethodCallsError(self._expected_calls_queue)
 
     def _Reset(self):
         """Reset the state of this mock to record mode with an empty queue."""
 
@@ -607,16 +601,15 @@
         self._expected_calls_queue = deque()
 
         # Make sure we are in setup mode, not replay mode
         self._replay_mode = False
 
 
 class MockObject(MockAnything, object):
-    """A mock object that simulates the public/protected interface of a class.
-    """
+    """A mock object that simulates the public/protected interface of a class."""
 
     def __init__(self, class_to_mock, attrs=None):
         """Initialize a mock object.
 
         This determines the methods and properties of the class and stores
         them.
 
@@ -631,54 +624,46 @@
           ValueError: if an attribute would mask an existing method.
         """
         if attrs is None:
             attrs = {}
 
         # This is used to hack around the mixin/inheritance of MockAnything,
         # which is not a proper object (it can be anything. :-)
-        MockAnything.__dict__['__init__'](self)
+        MockAnything.__dict__["__init__"](self)
 
         # Get a list of all the public and special methods we should mock.
         self._known_methods = set()
         self._known_vars = set()
         self._class_to_mock = class_to_mock
         try:
             if inspect.isclass(self._class_to_mock):
                 self._description = class_to_mock.__name__
             elif inspect.ismethod(self._class_to_mock):
-                if six.PY2:
-                    method_name = class_to_mock.im_func.__name__
-                    class_name = class_to_mock.im_class.__name__
-                else:
-                    method_name = class_to_mock.__func__.__name__
-                    class_name = class_to_mock.__self__.__class__.__name__
-                if class_name == 'type':
+                method_name = class_to_mock.__func__.__name__
+                class_name = class_to_mock.__self__.__class__.__name__
+                if class_name == "type":
                     class_name = class_to_mock.__self__.__name__
-                self._description = '{}.{}'.format(
-                    class_name, method_name)
+                self._description = "{}.{}".format(class_name, method_name)
             else:
                 search_string = (
-                    '<(?P<extra>function|((un)?bound )?method) (?P<class>\w*)'
-                    '(\.(?P<method>\w*))?( at \w+)?>')
+                    r"<(?P<extra>function|((un)?bound )?method) (?P<class>\w*)" r"(\.(?P<method>\w*))?( at \w+)?>"
+                )
                 search = re_search(search_string, str(repr(class_to_mock)))
 
-                self._description = '{}.{}'.format(
-                    search.group('class'), search.group('method'))
+                self._description = "{}.{}".format(search.group("class"), search.group("method"))
 
-                if (search.group('extra') == 'function' and not
-                        search.group('class') or not search.group('method')):
-                    to_use = search.group('class') or search.group('method')
+                if search.group("extra") == "function" and not search.group("class") or not search.group("method"):
+                    to_use = search.group("class") or search.group("method")
                     if inspect.isfunction(self._class_to_mock):
-                        self._description = 'function {}.{}'.format(
-                            self._class_to_mock.__module__, to_use)
+                        self._description = "function {}.{}".format(self._class_to_mock.__module__, to_use)
         except Exception:
             try:
                 self._description = type(class_to_mock).__name__
             except Exception:
-                pass
+                self._description = "Unknown description"
 
         for method in dir(class_to_mock):
             try:
                 attr = getattr(class_to_mock, method)
             except AttributeError:
                 continue
             if callable(attr):
@@ -690,17 +675,15 @@
         # Set additional attributes at instantiation time; this is quicker
         # than manually setting attributes that are normally created in
         # __init__.
         for attr, value in attrs.items():
             if attr.startswith("_"):
                 raise PrivateAttributeError(attr)
             elif attr in self._known_methods:
-                raise ValueError(
-                    "'%s' is a method of '%s' objects." %
-                    (attr, class_to_mock))
+                raise ValueError("'%s' is a method of '%s' objects." % (attr, class_to_mock))
             else:
                 setattr(self, attr, value)
 
     def __getattr__(self, name):
         """Intercept attribute request on this object.
 
         If the attribute is a public class variable, it will be returned and
@@ -725,29 +708,29 @@
               method.
         """
 
         if name in self._known_vars:
             return getattr(self._class_to_mock, name)
 
         if name in self._known_methods:
-            return self._CreateMockMethod(
-                name,
-                method_to_mock=getattr(self._class_to_mock, name))
+            return self._CreateMockMethod(name, method_to_mock=getattr(self._class_to_mock, name))
 
         exception = UnknownMethodCallError(name)
         self._exceptions_thrown.append(exception)
         raise exception
 
     def __eq__(self, rhs):
         """Provide custom logic to compare objects."""
 
-        return (isinstance(rhs, MockObject) and
-                self._class_to_mock == rhs._class_to_mock and
-                self._replay_mode == rhs._replay_mode and
-                self._expected_calls_queue == rhs._expected_calls_queue)
+        return (
+            isinstance(rhs, MockObject)
+            and self._class_to_mock == rhs._class_to_mock
+            and self._replay_mode == rhs._replay_mode
+            and self._expected_calls_queue == rhs._expected_calls_queue
+        )
 
     def __setitem__(self, key, value):
         """Provide custom logic for mocking classes that support item
         assignment.
 
         Args:
           key: Key to set the value for.
@@ -761,30 +744,29 @@
         Raises:
           TypeError if the underlying class does not support item assignment.
           UnexpectedMethodCallError if the object does not expect the call to
             __setitem__.
 
         """
         # Verify the class supports item assignment.
-        if '__setitem__' not in dir(self._class_to_mock):
-            raise TypeError('object does not support item assignment')
+        if "__setitem__" not in dir(self._class_to_mock):
+            raise TypeError("object does not support item assignment")
 
         # If we are in replay mode then simply call the mock __setitem__
         # method.
         if self._replay_mode:
             return MockMethod(
-                '__setitem__',
+                "__setitem__",
                 self._expected_calls_queue,
                 self._exceptions_thrown,
-                self._replay_mode)(
-                key,
-                value)
+                self._replay_mode,
+            )(key, value)
 
         # Otherwise, create a mock method __setitem__.
-        return self._CreateMockMethod('__setitem__')(key, value)
+        return self._CreateMockMethod("__setitem__")(key, value)
 
     def __getitem__(self, key):
         """Provide custom logic for mocking classes that are subscriptable.
 
         Args:
           key: Key to return the value for.
 
@@ -796,25 +778,29 @@
         Raises:
           TypeError if the underlying class is not subscriptable.
           UnexpectedMethodCallError if the object does not expect the call to
             __getitem__.
 
         """
         # Verify the class supports item assignment.
-        if '__getitem__' not in dir(self._class_to_mock):
-            raise TypeError('unsubscriptable object')
+        if "__getitem__" not in dir(self._class_to_mock):
+            raise TypeError("unsubscriptable object")
 
         # If we are in replay mode then simply call the mock __getitem__
         # method.
         if self._replay_mode:
-            return MockMethod('__getitem__', self._expected_calls_queue,
-                              self._exceptions_thrown, self._replay_mode)(key)
+            return MockMethod(
+                "__getitem__",
+                self._expected_calls_queue,
+                self._exceptions_thrown,
+                self._replay_mode,
+            )(key)
 
         # Otherwise, create a mock method __getitem__.
-        return self._CreateMockMethod('__getitem__')(key)
+        return self._CreateMockMethod("__getitem__")(key)
 
     def __iter__(self):
         """Provide custom logic for mocking classes that are iterable.
 
         Returns:
           Expected return value in replay mode.  A MockMethod object for the
           __iter__ method that has already been called if not in replay mode.
@@ -824,36 +810,40 @@
           UnexpectedMethodCallError if the object does not expect the call to
             __iter__.
 
         """
         methods = dir(self._class_to_mock)
 
         # Verify the class supports iteration.
-        if '__iter__' not in methods:
+        if "__iter__" not in methods:
             # If it doesn't have iter method and we are in replay method, then
             # try to iterate using subscripts.
-            if '__getitem__' not in methods or not self._replay_mode:
-                raise TypeError('not iterable object')
+            if "__getitem__" not in methods or not self._replay_mode:
+                raise TypeError("not iterable object")
             else:
                 results = []
                 index = 0
                 try:
                     while True:
                         results.append(self[index])
                         index += 1
                 except IndexError:
                     return iter(results)
 
         # If we are in replay mode then simply call the mock __iter__ method.
         if self._replay_mode:
-            return MockMethod('__iter__', self._expected_calls_queue,
-                              self._exceptions_thrown, self._replay_mode)()
+            return MockMethod(
+                "__iter__",
+                self._expected_calls_queue,
+                self._exceptions_thrown,
+                self._replay_mode,
+            )()
 
         # Otherwise, create a mock method __iter__.
-        return self._CreateMockMethod('__iter__')()
+        return self._CreateMockMethod("__iter__")()
 
     def __contains__(self, key):
         """Provide custom logic for mocking classes that contain items.
 
         Args:
           key: Key to look in container for.
 
@@ -864,49 +854,53 @@
 
         Raises:
           TypeError if the underlying class does not implement __contains__
           UnexpectedMethodCaller if the object does not expect the call to
           __contains__.
 
         """
-        contains = getattr(self._class_to_mock, '__contains__', None)
+        contains = getattr(self._class_to_mock, "__contains__", None)
 
         if contains is None:
-            raise TypeError('unsubscriptable object')
+            raise TypeError("unsubscriptable object")
 
         if self._replay_mode:
-            return MockMethod('__contains__', self._expected_calls_queue,
-                              self._exceptions_thrown, self._replay_mode)(key)
+            return MockMethod(
+                "__contains__",
+                self._expected_calls_queue,
+                self._exceptions_thrown,
+                self._replay_mode,
+            )(key)
 
-        return self._CreateMockMethod('__contains__')(key)
+        return self._CreateMockMethod("__contains__")(key)
 
     def __call__(self, *params, **named_params):
         """Provide custom logic for mocking classes that are callable."""
 
         # Verify the class we are mocking is callable.
-        callable = hasattr(self._class_to_mock, '__call__')
+        callable = hasattr(self._class_to_mock, "__call__")
         # callable = callable and str(
         #     type(self._class_to_mock.__call__)) not in [
         #         "<class 'method-wrapper'>",  # python 3
         #         "<type 'method-wrapper'>"  # python 2
         #     ]
         if not callable:
-            raise TypeError('Not callable')
+            raise TypeError("Not callable")
 
         # Because the call is happening directly on this object instead of a
         # method, the call on the mock method is made right here
 
         # If we are mocking a Function, then use the function, and not the
         # __call__ method
         method = None
         if type(self._class_to_mock) in (types.FunctionType, types.MethodType):
             method = self._class_to_mock
         else:
-            method = getattr(self._class_to_mock, '__call__')
-        mock_method = self._CreateMockMethod('__call__', method_to_mock=method)
+            method = getattr(self._class_to_mock, "__call__")
+        mock_method = self._CreateMockMethod("__call__", method_to_mock=method)
 
         return mock_method(*params, **named_params)
 
     @property
     def __class__(self):
         """Return the class that is being mocked."""
 
@@ -935,23 +929,22 @@
         MockObject.__init__(self, class_to_mock)
         self._mox = mox_instance
         self._instance_queue = deque()
 
     def __call__(self, *params, **named_params):
         """Instantiate and record that a new mock has been created."""
 
-        method = getattr(self._class_to_mock, '__init__')
-        mock_method = self._CreateMockMethod('__init__', method_to_mock=method)
+        method = getattr(self._class_to_mock, "__init__")
+        mock_method = self._CreateMockMethod("__init__", method_to_mock=method)
         # Note: calling mock_method() is deferred in order to catch the
         # empty instance_queue first.
 
         if self._replay_mode:
             if not self._instance_queue:
-                exception = UnexpectedMockCreationError(
-                    self._class_to_mock, *params, **named_params)
+                exception = UnexpectedMockCreationError(self._class_to_mock, *params, **named_params)
                 self._exceptions_thrown.append(exception)
                 raise exception
 
             mock_method(*params, **named_params)
 
             return self._instance_queue.pop()
         else:
@@ -981,36 +974,29 @@
           method: function
 
         Raises:
           ValueError: method could not be inspected, so checks aren't possible.
             Some methods and functions like built-ins can't be inspected.
         """
         try:
-            signature_fn = 'getargspec' if six.PY2 else 'getfullargspec'
-            self._args, varargs, varkw, defaults = getattr(
-                inspect, signature_fn)(method)[:4]
+            self._args, varargs, varkw, defaults = getattr(inspect, "getfullargspec")(method)[:4]
         except TypeError:
-            raise ValueError('Could not get argument specification for %r'
-                             % (method,))
+            raise ValueError("Could not get argument specification for %r" % (method,))
         self._method = method
-        if inspect.ismethod(
-            self._method) or (
-            '.' in repr(
-                self._method)) or (
-                self._args and self._args[0] == 'self'):
+        if inspect.ismethod(self._method) or ("." in repr(self._method)) or (self._args and self._args[0] == "self"):
             self._args = self._args[1:]  # Skip 'self'.
         self._instance = None  # May contain the instance this is bound to.
 
         self._has_varargs = varargs is not None
         self._has_varkw = varkw is not None
         if defaults is None:
             self._required_args = self._args
             self._default_args = []
         else:
-            self._required_args = self._args[:-len(defaults)]
+            self._required_args = self._args[: -len(defaults)]
             self._default_args = self._args[-len(defaults):]
 
     def _RecordArgumentGiven(self, arg_name, arg_status):
         """Mark an argument as being given.
 
         Args:
           # arg_name: The name of the argument to mark in arg_status.
@@ -1019,15 +1005,15 @@
           arg_name: string
           arg_status: dict
 
         Raises:
           AttributeError: arg_name is already marked as _GIVEN.
         """
         if arg_status.get(arg_name, None) == MethodSignatureChecker._GIVEN:
-            raise AttributeError('%s provided more than once' % (arg_name,))
+            raise AttributeError("%s provided more than once" % (arg_name,))
         arg_status[arg_name] = MethodSignatureChecker._GIVEN
 
     def Check(self, params, named_params):
         """Ensures that the parameters used while recording a call are valid.
 
         Args:
           # params: A list of positional parameters.
@@ -1035,124 +1021,121 @@
           params: list
           named_params: dict
 
         Raises:
           AttributeError: the given parameters don't work with the given
           method.
         """
-        arg_status = dict((a, MethodSignatureChecker._NEEDED)
-                          for a in self._required_args)
+        arg_status = dict((a, MethodSignatureChecker._NEEDED) for a in self._required_args)
         for arg in self._default_args:
             arg_status[arg] = MethodSignatureChecker._DEFAULT
 
         # WARNING: Suspect hack ahead.
         #
         # Check to see if this is an unbound method, where the instance
         # should be bound as the first argument.  We try to determine if
         # the first argument (param[0]) is an instance of the class, or it
         # is equivalent to the class (used to account for Comparators).
         #
         # NOTE: If a Func() comparator is used, and the signature is not
         # correct, this will cause extra executions of the function.
         # NOTE: '.' in repr(self._method) is very bad way to check if it's a
         # bound method. Improve it as soon as possible.
-        if inspect.ismethod(self._method) or '.' in repr(self._method):
+        if inspect.ismethod(self._method) or "." in repr(self._method):
             # The extra param accounts for the bound instance.
             if len(params) > len(self._required_args):
-                expected = getattr(self._method, 'im_class', None)
+                expected = getattr(self._method, "im_class", None)
                 if not expected:
                     search = re_search(
-                        '<(function|method) (?P<class>\w+)\.\w+ at \w+>',
-                        str(repr(self._method)))
+                        r"<(function|method) (?P<class>\w+)\.\w+ at \w+>",
+                        str(repr(self._method)),
+                    )
                     if search:
-                        class_ = search.group('class')
+                        class_ = search.group("class")
                         members = dict(inspect.getmembers(self._method))
-                        expected = members.get(
-                            class_, members.get('__globals__', {})
-                        ).get(class_, None)
+                        expected = members.get(class_, members.get("__globals__", {})).get(class_, None)
                 if not expected:
                     search = re_search(
-                        '<(?P<method>((un)?bound method ))(?P<class>\w+)'
-                        '\.\w+ of <?(?P<module>\w+\.)(?P<class2>\w+) object '
-                        'at [A-Za-z0-9]+>?>',
-                        str(repr(self._method))
+                        r"<(?P<method>((un)?bound method ))(?P<class>\w+)"
+                        r"\.\w+ of <?(?P<module>\w+\.)(?P<class2>\w+) object "
+                        r"at [A-Za-z0-9]+>?>",
+                        str(repr(self._method)),
                     )
 
                     if search:
                         for _, class_ in search.groupdict().items():
                             members = dict(inspect.getmembers(self._method))
-                            expected = members.get(
-                                class_, members.get('__globals__', {})
-                            ).get(class_, None)
+                            expected = members.get(class_, members.get("__globals__", {})).get(class_, None)
                             if expected:
                                 break
-                if not expected and six.PY3:
-                    expected = dict(
-                        inspect.getmembers(self._method))['__self__'].__class__
+                if not expected:
+                    expected = dict(inspect.getmembers(self._method))["__self__"].__class__
 
                 # Check if the param is an instance of the expected class,
                 # or check equality (useful for checking Comparators).
 
                 # This is a hack to work around the fact that the first
                 # parameter can be a Comparator, and the comparison may raise
                 # an exception during this comparison, which is OK.
                 try:
-                    param_equality = (params[0] == expected)
+                    param_equality = params[0] == expected
                 except BaseException:
                     param_equality = False
 
                 if isinstance(params[0], expected) or param_equality:
                     params = params[1:]
                 # If the IsA() comparator is being used, we need to check the
                 # inverse of the usual case - that the given instance is a
                 # subclass of the expected class.  For example, the code under
                 # test does late binding to a subclass.
-                elif (isinstance(params[0], IsA) and
-                        params[0]._IsSubClass(expected)):
+                elif isinstance(params[0], IsA) and params[0]._IsSubClass(expected):
                     params = params[1:]
 
         # Check that each positional param is valid.
         for i in range(len(params)):
             try:
                 arg_name = self._args[i]
             except IndexError:
                 if not self._has_varargs:
                     raise AttributeError(
-                        '%s does not take %d or more positional '
-                        'arguments' %
-                        (self._method.__name__, i))
+                        "%s does not take %d or more positional " "arguments" % (self._method.__name__, i)
+                    )
             else:
                 self._RecordArgumentGiven(arg_name, arg_status)
 
         # Check each keyword argument.
         for arg_name in named_params:
             if arg_name not in arg_status and not self._has_varkw:
-                raise AttributeError('%s is not expecting keyword argument %s'
-                                     % (self._method.__name__, arg_name))
+                raise AttributeError("%s is not expecting keyword argument %s" % (self._method.__name__, arg_name))
             self._RecordArgumentGiven(arg_name, arg_status)
 
         # Ensure all the required arguments have been given.
-        still_needed = [k for k, v in six.iteritems(arg_status)
-                        if v == MethodSignatureChecker._NEEDED]
+        still_needed = [k for k, v in arg_status.items() if v == MethodSignatureChecker._NEEDED]
         if still_needed:
-            raise AttributeError('No values given for arguments: %s'
-                                 % (' '.join(sorted(still_needed))))
+            raise AttributeError("No values given for arguments: %s" % (" ".join(sorted(still_needed))))
 
 
 class MockMethod(object):
     """Callable mock method.
 
     A MockMethod should act exactly like the method it mocks, accepting
     parameters and returning a value, or throwing an exception (as specified).
     When this method is called, it can optionally verify whether the called
     method (name and signature) matches the expected method.
     """
 
-    def __init__(self, method_name, call_queue, exception_list, replay_mode,
-                 method_to_mock=None, description=None):
+    def __init__(
+        self,
+        method_name,
+        call_queue,
+        exception_list,
+        replay_mode,
+        method_to_mock=None,
+        description=None,
+    ):
         """Construct a new mock method.
 
         Args:
           # method_name: the name of the method
           # call_queue: deque of calls, verify this call against the head, or
           #     add this call to the queue.
           # exception_list: list of exceptions; any exceptions thrown by this
@@ -1226,27 +1209,24 @@
 
         return expected_method._return_value
 
     def __getattr__(self, name):
         """Raise an AttributeError with a helpful message."""
 
         raise AttributeError(
-            'MockMethod has no attribute "%s". '
-            'Did you remember to put your mocks in replay mode?' %
-            name)
+            'MockMethod has no attribute "%s". ' "Did you remember to put your mocks in replay mode?" % name
+        )
 
     def __iter__(self):
         """Raise a TypeError with a helpful message."""
-        raise TypeError('MockMethod cannot be iterated. '
-                        'Did you remember to put your mocks in replay mode?')
+        raise TypeError("MockMethod cannot be iterated. " "Did you remember to put your mocks in replay mode?")
 
     def __next__(self):
         """Raise a TypeError with a helpful message."""
-        raise TypeError('MockMethod cannot be iterated. '
-                        'Did you remember to put your mocks in replay mode?')
+        raise TypeError("MockMethod cannot be iterated. " "Did you remember to put your mocks in replay mode?")
 
     next = __next__
 
     def _PopNextMethod(self):
         """Pop the next method from our call queue."""
         try:
             return self._call_queue.popleft()
@@ -1281,34 +1261,36 @@
             exception = UnexpectedMethodCallError(self, expected)
             self._exception_list.append(exception)
             raise exception
 
         return expected
 
     def __str__(self):
-        params = ', '.join(
-            [repr(p) for p in self._params or []] +
-            ['%s=%r' % x for x in sorted((self._named_params or {}).items())])
+        params = ", ".join(
+            [repr(p) for p in self._params or []] + ["%s=%r" % x for x in sorted((self._named_params or {}).items())]
+        )
         full_desc = "%s(%s) -> %r" % (self._name, params, self._return_value)
         if self._description:
             full_desc = "%s.%s" % (self._description, full_desc)
         return full_desc
 
     def __eq__(self, rhs):
         """Test whether this MockMethod is equivalent to another MockMethod.
 
         Args:
           # rhs: the right hand side of the test
           rhs: MockMethod
         """
 
-        return (isinstance(rhs, MockMethod) and
-                self._name == rhs._name and
-                self._params == rhs._params and
-                self._named_params == rhs._named_params)
+        return (
+            isinstance(rhs, MockMethod)
+            and self._name == rhs._name
+            and self._params == rhs._params
+            and self._named_params == rhs._named_params
+        )
 
     def __hash__(self):
         return id(self)
 
     def __ne__(self, rhs):
         """Test whether this MockMethod is not equivalent to another MockMethod.
 
@@ -1323,15 +1305,16 @@
         """Returns a possible group from the end of the call queue or None if no
         other methods are on the stack.
         """
 
         # Remove this method from the tail of the queue so we can add it to a
         # group.
         this_method = self._call_queue.pop()
-        assert this_method == self
+        if this_method != self:
+            raise Error("Current method is not at the end of the call queue.")
 
         # Determine if the tail of the queue is a group, or just a regular
         # ordered mock method.
         group = None
         try:
             group = self._call_queue[-1]
         except IndexError:
@@ -1530,15 +1513,15 @@
             return issubclass(self._class_name, clazz)
         except TypeError:
             # Check raw types if there was a type error.  This is helpful for
             # things like cStringIO.StringIO.
             return isinstance(clazz, type(self._class_name))
 
     def __repr__(self):
-        return 'mox.IsA(%s) ' % str(self._class_name)
+        return "mox.IsA(%s) " % str(self._class_name)
 
 
 class IsAlmost(Comparator):
     """Comparison class used to check whether a parameter is nearly equal
     to a given value.  Generally useful for floating point numbers.
 
     Example mock_dao.SetTimeout((IsAlmost(3.9)))
@@ -1608,15 +1591,15 @@
 
         try:
             return rhs.find(self._search_string) > -1
         except Exception:
             return False
 
     def __repr__(self):
-        return '<str containing \'%s\'>' % self._search_string
+        return "<str containing '%s'>" % self._search_string
 
 
 class Regex(Comparator):
     """Checks if a string matches a regular expression.
 
     This uses a given regular expression to determine equality.
     """
@@ -1643,20 +1626,20 @@
         try:
             return self.regex.search(rhs) is not None
         except Exception:
             return False
 
     def __repr__(self):
         pattern = self.regex.pattern
-        if isinstance(pattern, six.binary_type):
+        if isinstance(pattern, bytes):
             pattern = pattern.decode()
-        s = '<regular expression \'{}\''.format(pattern)
+        s = "<regular expression '{}'".format(pattern)
         if self.regex.flags:
-            s += ', flags=%d' % self.regex.flags
-        s += '>'
+            s += ", flags=%d" % self.regex.flags
+        s += ">"
         return s
 
 
 class In(Comparator):
     """Checks whether an item (or key) is in a list (or dict) parameter.
 
     Example:
@@ -1684,15 +1667,15 @@
 
         try:
             return self._key in rhs
         except Exception:
             return False
 
     def __repr__(self):
-        return '<sequence or map containing \'%s\'>' % str(self._key)
+        return "<sequence or map containing '%s'>" % str(self._key)
 
 
 class Not(Comparator):
     """Checks whether a predicates is False.
 
     Example:
       mock_dao.UpdateUsers(Not(ContainsKeyValue('stevepm', stevepm_user_info)))
@@ -1701,16 +1684,16 @@
     def __init__(self, predicate):
         """Initialize.
 
         Args:
           # predicate: a Comparator instance.
         """
 
-        assert isinstance(predicate, Comparator), ("predicate %r must be a"
-                                                   " Comparator." % predicate)
+        if not isinstance(predicate, Comparator):
+            raise Error("predicate %r must be a" " Comparator." % predicate)
         self._predicate = predicate
 
     def equals(self, rhs):
         """Check to see whether the predicate is False.
 
         Args:
           rhs: A value that will be given in argument of the predicate.
@@ -1721,15 +1704,15 @@
 
         try:
             return not self._predicate.equals(rhs)
         except Exception:
             return False
 
     def __repr__(self):
-        return '<not \'%s\'>' % self._predicate
+        return "<not '%s'>" % self._predicate
 
 
 class ContainsKeyValue(Comparator):
     """Checks whether a key/value pair is in a dict parameter.
 
     Example:
     mock_dao.UpdateUsers(ContainsKeyValue('stevepm', stevepm_user_info))
@@ -1755,16 +1738,18 @@
 
         try:
             return rhs[self._key] == self._value
         except Exception:
             return False
 
     def __repr__(self):
-        return '<map containing the entry \'%s: %s\'>' % (str(self._key),
-                                                          str(self._value))
+        return "<map containing the entry '%s: %s'>" % (
+            str(self._key),
+            str(self._value),
+        )
 
 
 class ContainsAttributeValue(Comparator):
     """Checks whether a passed parameter contains attributes with a given
     value.
 
     Example:
@@ -1829,16 +1814,15 @@
             # actual_seq cannot be read as a sequence.
             #
             # This happens because Mox uses __eq__ both to check object
             # equality (in MethodSignatureChecker) and to invoke Comparators.
             return False
 
         try:
-            expected = dict([(element, None)
-                             for element in self._expected_list])
+            expected = dict([(element, None) for element in self._expected_list])
             actual = dict([(element, None) for element in actual_list])
         except TypeError:
             # Fall back to slower list-compare if any of the objects are
             # unhashable.
             expected = self._expected_list
             actual = actual_list
             for element in actual:
@@ -1848,15 +1832,15 @@
                 if element not in actual:
                     return False
             return True
         else:
             return set(actual_list) == set(self._expected_list)
 
     def __repr__(self):
-        return '<sequence with same elements as \'%s\'>' % self._expected_list
+        return "<sequence with same elements as '%s'>" % self._expected_list
 
 
 class And(Comparator):
     """Evaluates one or more Comparators on RHS and returns an AND of the
     results.
     """
 
@@ -1882,15 +1866,15 @@
         for comparator in self._comparators:
             if not comparator.equals(rhs):
                 return False
 
         return True
 
     def __repr__(self):
-        return '<AND %s>' % str(self._comparators)
+        return "<AND %s>" % str(self._comparators)
 
 
 class Or(Comparator):
     """Evaluates one or more Comparators on RHS and returns an OR of the
     results.
     """
 
@@ -1916,15 +1900,15 @@
         for comparator in self._comparators:
             if comparator.equals(rhs):
                 return True
 
         return False
 
     def __repr__(self):
-        return '<OR %s>' % str(self._comparators)
+        return "<OR %s>" % str(self._comparators)
 
 
 class Func(Comparator):
     """Call a function that should verify the parameter passed in is correct.
 
     You may need the ability to perform more advanced operations on the
     parameter in order to validate it.  You can use this to have a callable
@@ -1986,15 +1970,15 @@
         Returns:
           always returns True
         """
 
         return True
 
     def __repr__(self):
-        return '<IgnoreArg>'
+        return "<IgnoreArg>"
 
 
 class Value(Comparator):
     """Compares argument against a remembered value.
 
     To be used in conjunction with Remember comparator.  See Remember()
     for example.
@@ -2033,16 +2017,15 @@
 
     # Check argument against remembered value.
     mock_dao.ReportUsers(users_list)
     """
 
     def __init__(self, value_store):
         if not isinstance(value_store, Value):
-            raise TypeError(
-                "value_store is not an instance of the Value class")
+            raise TypeError("value_store is not an instance of the Value class")
         self._value_store = value_store
 
     def equals(self, rhs):
         self._value_store.store_value(rhs)
         return True
 
     def __repr__(self):
@@ -2092,15 +2075,16 @@
         super(UnorderedGroup, self).__init__(group_name, exception_list)
         self._methods = []
 
     def __str__(self):
         return '%s "%s" pending calls:\n%s' % (
             self.__class__.__name__,
             self._group_name,
-            "\n".join(str(method) for method in self._methods))
+            "\n".join(str(method) for method in self._methods),
+        )
 
     def AddMethod(self, mock_method):
         """Add a method to this group.
 
         Args:
           mock_method: A mock method to be added to this group.
         """
@@ -2208,47 +2192,43 @@
             return next_method, None
         else:
             exception = UnexpectedMethodCallError(mock_method, self)
             self._exception_list.append(exception)
             raise exception
 
     def IsSatisfied(self):
-        """Return True if all methods in this group are called at least once.
-        """
+        """Return True if all methods in this group are called at least once."""
         return len(self._methods_left) == 0
 
 
 class MoxMetaTestBase(type):
     """Metaclass to add mox cleanup and verification to every test.
     As the mox unit testing class is being constructed (MoxTestBase or a
     subclass), this metaclass will modify all test functions to call the
     CleanUpMox method of the test class after they finish. This means that
     unstubbing and verifying will happen for every test with no additional
     code, and any failures will result in test failures as opposed to errors.
     """
 
     def __init__(cls, name, bases, d):
-        if six.PY3:  # pragma: nocover
-            super().__init__(name, bases, d)
-        else:
-            super(MoxMetaTestBase, cls).__init__(name, bases, d)
+        super().__init__(name, bases, d)
         # type.__init__(cls, name, bases, d)
 
         # also get all the attributes from the base classes to account
         # for a case when test class is not the immediate child of MoxTestBase
         for base in bases:
             for attr_name in dir(base):
                 if attr_name not in d:
                     try:  # pragma: nocover
                         d[attr_name] = getattr(base, attr_name)
                     except AttributeError:
                         continue
 
         for func_name, func in d.items():
-            if func_name.startswith('test') and callable(func):
+            if func_name.startswith("test") and callable(func):
                 setattr(cls, func_name, MoxMetaTestBase.CleanUpTest(cls, func))
 
     @staticmethod
     def CleanUpTest(cls, func):
         """Adds Mox cleanup code to any MoxTestBase method.
         Always unsets stubs after a test. Will verify all mocks for tests that
         otherwise pass.
@@ -2258,22 +2238,21 @@
           func: method; the method of the MoxTestBase test class we wish to
             alter.
         Returns:
           The modified method.
         """
 
         def new_method(self, *args, **kwargs):
-            mox_obj = getattr(self, 'mox', None)
-            stubout_obj = getattr(self, 'stubs', None)
+            mox_obj = getattr(self, "mox", None)
+            stubout_obj = getattr(self, "stubs", None)
             cleanup_mox = False
             cleanup_stubout = False
             if mox_obj and isinstance(mox_obj, Mox):
                 cleanup_mox = True
-            if stubout_obj and isinstance(
-                    stubout_obj, stubout.StubOutForTesting):
+            if stubout_obj and isinstance(stubout_obj, stubout.StubOutForTesting):
                 cleanup_stubout = True
             try:
                 func(self, *args, **kwargs)
             finally:
                 if cleanup_mox:
                     mox_obj.UnsetStubs()
                 if cleanup_stubout:
@@ -2284,15 +2263,15 @@
 
         new_method.__name__ = func.__name__
         new_method.__doc__ = func.__doc__
         new_method.__module__ = func.__module__
         return new_method
 
 
-_MoxTestBase = MoxMetaTestBase('_MoxTestBase', (unittest.TestCase,), {})
+_MoxTestBase = MoxMetaTestBase("_MoxTestBase", (unittest.TestCase,), {})
 
 
 class MoxTestBase(_MoxTestBase):
     """Convenience test class to make stubbing easier.
     Sets up a "mox" attribute which is an instance of Mox (any mox tests will
     want this), and a "stubs" attribute that is an instance of
     StubOutForTesting (needed at times). Also automatically unsets any stubs
```

### Comparing `pymox-1.0.0/mox/stubout.py` & `pymox-1.0.1/mox/stubout.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,62 +11,62 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
-import six
 
 
 class StubOutForTesting:
     """Sample Usage:
-       You want os.path.exists() to always return true during testing.
+    You want os.path.exists() to always return true during testing.
 
-       stubs = StubOutForTesting()
-       stubs.Set(os.path, 'exists', lambda x: 1)
-         ...
-       stubs.UnsetAll()
-
-       The above changes os.path.exists into a lambda that returns 1.  Once
-       the ... part of the code finishes, the UnsetAll() looks up the old value
-       of os.path.exists and restores it.
+    stubs = StubOutForTesting()
+    stubs.Set(os.path, 'exists', lambda x: 1)
+      ...
+    stubs.UnsetAll()
+
+    The above changes os.path.exists into a lambda that returns 1.  Once
+    the ... part of the code finishes, the UnsetAll() looks up the old value
+    of os.path.exists and restores it.
 
     """
 
     def __init__(self):
         self.cache = []
         self.stubs = []
 
     def __del__(self):
         self.SmartUnsetAll()
         self.UnsetAll()
 
     def SmartSet(self, obj, attr_name, new_attr):
         """Replace obj.attr_name with new_attr. This method is smart and works
-           at the module, class, and instance level while preserving proper
-           inheritance. It will not stub out C types however unless that has
-           been explicitly allowed by the type.
-
-           This method supports the case where attr_name is a staticmethod or a
-           classmethod of obj.
-
-           Notes:
-          - If obj is an instance, then it is its class that will actually be
-            stubbed. Note that the method Set() does not do that: if obj is
-            an instance, it (and not its class) will be stubbed.
-          - The stubbing is using the builtin getattr and setattr. So, the
-            __get__ and __set__ will be called when stubbing (TODO: A better
-            idea would probably be to manipulate obj.__dict__ instead of
-            getattr() and setattr()).
+         at the module, class, and instance level while preserving proper
+         inheritance. It will not stub out C types however unless that has
+         been explicitly allowed by the type.
+
+         This method supports the case where attr_name is a staticmethod or a
+         classmethod of obj.
+
+         Notes:
+        - If obj is an instance, then it is its class that will actually be
+          stubbed. Note that the method Set() does not do that: if obj is
+          an instance, it (and not its class) will be stubbed.
+        - The stubbing is using the builtin getattr and setattr. So, the
+          __get__ and __set__ will be called when stubbing (TODO: A better
+          idea would probably be to manipulate obj.__dict__ instead of
+          getattr() and setattr()).
 
-           Raises AttributeError if the attribute cannot be found.
+         Raises AttributeError if the attribute cannot be found.
         """
-        if (inspect.ismodule(obj) or
-                (not inspect.isclass(obj) and attr_name in obj.__dict__)):
+        if inspect.ismodule(obj) or (
+            not inspect.isclass(obj) and attr_name in obj.__dict__
+        ):
             orig_obj = obj
             orig_attr = getattr(obj, attr_name)
 
         else:
             if not inspect.isclass(obj):
                 mro = list(inspect.getmro(obj.__class__))
             else:
@@ -85,17 +85,15 @@
 
         if orig_attr is None:
             raise AttributeError("Attribute not found.")
 
         # Calling getattr() on a staticmethod transforms it to a 'normal'
         # function. We need to ensure that we put it back as a staticmethod.
         old_attribute = obj.__dict__.get(attr_name)
-        if old_attribute is not None and isinstance(
-                old_attribute,
-                staticmethod):
+        if old_attribute is not None and isinstance(old_attribute, staticmethod):
             orig_attr = staticmethod(orig_attr)
 
         self.stubs.append((orig_obj, attr_name, orig_attr))
         setattr(orig_obj, attr_name, new_attr)
 
     def SmartUnsetAll(self):
         """Reverses all the SmartSet() calls, restoring things to their
@@ -124,18 +122,15 @@
         old_child = getattr(parent, child_name)
 
         old_attribute = parent.__dict__.get(child_name)
         if old_attribute is not None:
             if isinstance(old_attribute, staticmethod):
                 old_child = staticmethod(old_child)
             elif isinstance(old_attribute, classmethod):
-                if six.PY2:
-                    old_child = classmethod(old_child.im_func)
-                else:
-                    old_child = classmethod(old_child.__func__)
+                old_child = classmethod(old_child.__func__)
 
         self.cache.append((parent, old_child, child_name))
         setattr(parent, child_name, new_child)
 
     def UnsetAll(self):
         """Reverses all the Set() calls, restoring things to their original
         definition.  Its okay to call UnsetAll() repeatedly, as later calls
@@ -143,10 +138,10 @@
 
         """
         # Undo calls to Set() in reverse order, in case Set() was called on the
         # same arguments repeatedly (want the original call to be last one
         # undone)
         self.cache.reverse()
 
-        for (parent, old_child, child_name) in self.cache:
+        for parent, old_child, child_name in self.cache:
             setattr(parent, child_name, old_child)
         self.cache = []
```

