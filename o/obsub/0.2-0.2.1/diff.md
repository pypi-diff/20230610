# Comparing `tmp/obsub-0.2.tar.gz` & `tmp/obsub-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/obsub-0.2.tar", last modified: Sat Feb 22 11:52:13 2014, max compression
+gzip compressed data, was "obsub-0.2.1.tar", last modified: Sat Jun 10 13:03:56 2023, max compression
```

## Comparing `obsub-0.2.tar` & `obsub-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eduard    (1000) users      (100)        0 2014-02-22 11:52:13.000000 obsub-0.2/
--rwxr-xr-x   0 eduard    (1000) users      (100)     1095 2014-02-06 12:43:47.000000 obsub-0.2/setup.py
--rw-r--r--   0 eduard    (1000) users      (100)     7329 2014-02-06 12:07:58.000000 obsub-0.2/LICENSE.rst
--rw-r--r--   0 eduard    (1000) users      (100)      131 2014-02-22 11:52:13.000000 obsub-0.2/setup.cfg
-drwxr-xr-x   0 eduard    (1000) users      (100)        0 2014-02-22 11:52:13.000000 obsub-0.2/test/
--rw-r--r--   0 eduard    (1000) users      (100)     2037 2014-01-04 15:26:25.000000 obsub-0.2/test/test_weakref.py
--rw-r--r--   0 eduard    (1000) users      (100)     4051 2014-02-06 12:07:58.000000 obsub-0.2/test/test_core.py
--rw-r--r--   0 eduard    (1000) users      (100)      215 2014-01-07 16:21:20.000000 obsub-0.2/test/test_signature.py
-drwxr-xr-x   0 eduard    (1000) users      (100)        0 2014-02-22 11:52:13.000000 obsub-0.2/test/py3/
--rw-r--r--   0 eduard    (1000) users      (100)      803 2014-01-07 16:21:20.000000 obsub-0.2/test/py3/test_signature.py
--rw-r--r--   0 eduard    (1000) users      (100)       85 2014-02-06 12:07:58.000000 obsub-0.2/MANIFEST.in
--rw-r--r--   0 eduard    (1000) users      (100)     7474 2014-02-22 11:52:13.000000 obsub-0.2/PKG-INFO
--rw-r--r--   0 eduard    (1000) users      (100)     1341 2014-02-06 12:07:58.000000 obsub-0.2/CHANGELOG.rst
--rw-r--r--   0 eduard    (1000) users      (100)     7084 2014-02-06 12:07:58.000000 obsub-0.2/obsub.py
--rw-r--r--   0 eduard    (1000) users      (100)     4072 2014-02-06 12:07:58.000000 obsub-0.2/README.rst
-drwxr-xr-x   0 eduard    (1000) users      (100)        0 2014-02-22 11:52:13.000000 obsub-0.2/obsub.egg-info/
--rw-r--r--   0 eduard    (1000) users      (100)      281 2014-02-22 11:52:13.000000 obsub-0.2/obsub.egg-info/SOURCES.txt
--rw-r--r--   0 eduard    (1000) users      (100)     7474 2014-02-22 11:52:13.000000 obsub-0.2/obsub.egg-info/PKG-INFO
--rw-r--r--   0 eduard    (1000) users      (100)        6 2014-02-22 11:52:13.000000 obsub-0.2/obsub.egg-info/top_level.txt
--rw-r--r--   0 eduard    (1000) users      (100)        1 2014-02-22 11:52:13.000000 obsub-0.2/obsub.egg-info/dependency_links.txt
+drwxr-xr-x   0 emilia    (1002) users      (100)        0 2023-06-10 13:03:56.643368 obsub-0.2.1/
+-rw-r--r--   0 emilia    (1002) users      (100)     1340 2023-06-10 12:47:56.000000 obsub-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 emilia    (1002) users      (100)     7329 2023-06-10 12:51:43.000000 obsub-0.2.1/LICENSE.rst
+-rw-r--r--   0 emilia    (1002) users      (100)       85 2023-06-10 12:47:56.000000 obsub-0.2.1/MANIFEST.in
+-rw-r--r--   0 emilia    (1002) users      (100)     5602 2023-06-10 13:03:56.643368 obsub-0.2.1/PKG-INFO
+-rw-r--r--   0 emilia    (1002) users      (100)     3670 2023-06-10 13:03:05.000000 obsub-0.2.1/README.rst
+drwxr-xr-x   0 emilia    (1002) users      (100)        0 2023-06-10 13:03:56.642368 obsub-0.2.1/obsub.egg-info/
+-rw-r--r--   0 emilia    (1002) users      (100)     5602 2023-06-10 13:03:56.000000 obsub-0.2.1/obsub.egg-info/PKG-INFO
+-rw-r--r--   0 emilia    (1002) users      (100)      281 2023-06-10 13:03:56.000000 obsub-0.2.1/obsub.egg-info/SOURCES.txt
+-rw-r--r--   0 emilia    (1002) users      (100)        1 2023-06-10 13:03:56.000000 obsub-0.2.1/obsub.egg-info/dependency_links.txt
+-rw-r--r--   0 emilia    (1002) users      (100)        6 2023-06-10 13:03:56.000000 obsub-0.2.1/obsub.egg-info/top_level.txt
+-rw-r--r--   0 emilia    (1002) users      (100)     7084 2023-06-10 12:47:56.000000 obsub-0.2.1/obsub.py
+-rw-r--r--   0 emilia    (1002) users      (100)      110 2023-06-10 13:03:56.643368 obsub-0.2.1/setup.cfg
+-rwxr-xr-x   0 emilia    (1002) users      (100)     1138 2023-06-10 13:03:47.000000 obsub-0.2.1/setup.py
+drwxr-xr-x   0 emilia    (1002) users      (100)        0 2023-06-10 13:03:56.643368 obsub-0.2.1/test/
+drwxr-xr-x   0 emilia    (1002) users      (100)        0 2023-06-10 13:03:56.643368 obsub-0.2.1/test/py3/
+-rw-r--r--   0 emilia    (1002) users      (100)      803 2023-06-10 12:47:56.000000 obsub-0.2.1/test/py3/test_signature.py
+-rw-r--r--   0 emilia    (1002) users      (100)     4051 2023-06-10 12:47:56.000000 obsub-0.2.1/test/test_core.py
+-rw-r--r--   0 emilia    (1002) users      (100)      215 2023-06-10 12:47:56.000000 obsub-0.2.1/test/test_signature.py
+-rw-r--r--   0 emilia    (1002) users      (100)     2037 2023-06-10 12:47:56.000000 obsub-0.2.1/test/test_weakref.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `obsub-0.2/setup.py` & `obsub-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,21 @@
     # some file is not available
     # just use what we got so far but issue a warning
     logging.warn('documentation files missing')
 
 
 setup(
     name='obsub',
-    version='0.2',
+    version='0.2.1',
     description='Implementation of the observer pattern via a decorator',
     long_description=long_description,
-    author='Eduard Bopp',
-    author_email='eduard.bopp@aepsil0n.de',
-    url='https://github.com/aepsil0n/obsub',
+    long_description_content_type='text/x-rst',
+    author='Emilia Bopp',
+    author_email='contact@ebopp.de',
+    url='https://github.com/milibopp/obsub',
     py_modules=['obsub',],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `obsub-0.2/LICENSE.rst` & `obsub-0.2.1/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 This Python module is licensed under a `CC0
 license <http://creativecommons.org/publicdomain/zero/1.0/>`__.
 
-To the extent possible under law, Eduard Bopp has waived all copyright
+To the extent possible under law, Emilia Bopp has waived all copyright
 and related or neighboring rights to obsub. This work is published from:
 Germany.
 
 Full license text
 =================
 
 CC0 1.0 Universal
```

### Comparing `obsub-0.2/test/test_weakref.py` & `obsub-0.2.1/test/test_weakref.py`

 * *Files identical despite different names*

### Comparing `obsub-0.2/test/test_core.py` & `obsub-0.2.1/test/test_core.py`

 * *Files identical despite different names*

### Comparing `obsub-0.2/test/py3/test_signature.py` & `obsub-0.2.1/test/py3/test_signature.py`

 * *Files identical despite different names*

### Comparing `obsub-0.2/CHANGELOG.rst` & `obsub-0.2.1/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 - Function signatures are now preserved correctly by the event decorator. This
   is true only for python3. On python2 there is no support for default
   arguments, currently
 - Some fixes to memory handling and tests thereof. This includes a more generic
   handling of the garbage collection process within the test suite to make it
   pass on pypy, too.
-- Massive refactoring of test suite from one very long doctest to more focussed
+- Massive refactoring of test suite from one very long doctest to more focused
   unit tests.
 - The documentation has been converted from Markdown to reStructuredText, since
   it is compatible with both PyPI and GitHub.
 - Various improvements and some streamlining of the documentation.
 - Fix package name in license.
 - Continuous integration now includes coveralls.io support.
 - Support for Python 2.5 is no longer tested using Travis CI, since they have
```

### Comparing `obsub-0.2/obsub.py` & `obsub-0.2.1/obsub.py`

 * *Files identical despite different names*

### Comparing `obsub-0.2/README.rst` & `obsub-0.2.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 obsub
 =====
 
-|Build Status| |Coverage| |Version| |Downloads| |License|
+|Version| |License|
 
 Small python module that implements the observer pattern via a
 decorator.
 
+**Deprecation notice**
+
+This module has been unmaintained since around 2014. The authors have
+moved on to other alternatives to event handling. There is also
+`observed <https://github.com/DanielSank/observed>`_ by @DanielSank, which
+was partially inspired by *obsub*, however, has not seen many updates lately.
+@milibopp has been writing with functional reactive programming (FRP), but
+not for Python.
+
+FRP is a higher-level abstraction than the observer pattern, that essentially
+is a purely functional approach to unidirectional dataflow, composing your
+programs of event stream transformations. Experience has shown, that is easier
+to compose and to test than the raw observer pattern. A solid implementation in
+Python is `RxPY <https://github.com/ReactiveX/RxPY>`_, part of the ReactiveX
+project.
+
 
 Description
 -----------
 
 This is based on a `thread on stackoverflow
 <http://stackoverflow.com/questions/1904351/python-observer-pattern-examples-tips>`_
 (the example of C#-like events by Jason Orendorff), so I don't take any
@@ -62,83 +78,41 @@
 
 ::
 
     Stuff foo happens
     Stuff foo is handled
 
 
-Continuous integration
-----------------------
-
-For the fun of it, `Travis CI <https://travis-ci.org/aepsil0n/obsub>`__
-is used for continuous integration. As long as everything is fine, the
-button below should be green and shiny!
-
-|Build Status|
-
-The continuous integration ensures that our tests run on the following
-platforms:
-
--  Python 2.6, 2.7
--  Python 3.2, 3.3
--  pypy
-
-It might also work on Python 2.5, but is not automatically tested with this
-version.
-
-We also track the coverage of our tests with coveralls.io
-
-|Coverage|
-
-Use `coverage <https://pypi.python.org/pypi/coverage>`__ to generate local
-coverage reports like this:
-
-::
-
-    coverage run setup.py nosetests
-
-Note: on some platforms (e.g. Ubuntu) the executable is called
-``python-coverage``.
-
-
 Contribution and feedback
 -------------------------
 
-*obsub* is developed on `github <https://github.com/aepsil0n/obsub>`__.
+*obsub* is developed on `github <https://github.com/milibopp/obsub>`__.
 
 If you have any questions about this software or encounter bugs, you're welcome
-to open a `new issue on github <https://github.com/aepsil0n/obsub/issues/new>`__.
+to open a `new issue on github <https://github.com/milibopp/obsub/issues/new>`__.
 
 In case you do not want to use github for some reason, you can alternatively
 send an email one of us:
 
-- `Eduard Bopp <eduard.bopp@aepsil0n.de>`__
+- `Emilia Bopp <contact@ebopp.de>`__
 - `André-Patrick Bubel <code@andre-bubel.de>`__
 - `Thomas Gläßle <t_glaessle@gmx.de>`__
 
 Feel free to contribute patches as pull requests as you see fit. Try to be
 consistent with PEP 8 guidelines as far as possible and test everything.
 Otherwise, your commit messages should start with a capitalized verb for
 consistency. Unless your modification is completely trivial, also add a message
 body to your commit.
 
 
-
 Credits
 -------
 
 Thanks to Jason Orendorff on for the idea on stackoverflow. I also want
 to thank @coldfix and @Moredread for contributions and feedback.
 
-.. |Downloads| image:: https://pypip.in/d/obsub/badge.png
-   :target: https://pypi.python.org/pypi/obsub/
-   :alt: Downloads
-.. |Version| image:: https://pypip.in/v/obsub/badge.png
+.. |Version| image:: https://img.shields.io/pypi/v/obsub.svg
    :target: https://pypi.python.org/pypi/obsub/
    :alt: Latest Version
-.. |License| image:: https://pypip.in/license/obsub/badge.png
+.. |License| image:: https://img.shields.io/pypi/l/obsub.svg
    :target: https://pypi.python.org/pypi/obsub/
    :alt: License
-.. |Build Status| image:: https://api.travis-ci.org/aepsil0n/obsub.png?branch=master
-   :target: https://travis-ci.org/aepsil0n/obsub
-.. |Coverage| image:: https://coveralls.io/repos/aepsil0n/obsub/badge.png?branch=master
-   :target: https://coveralls.io/r/aepsil0n/obsub
```

