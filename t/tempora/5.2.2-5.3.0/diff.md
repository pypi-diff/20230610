# Comparing `tmp/tempora-5.2.2.tar.gz` & `tmp/tempora-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempora-5.2.2.tar", last modified: Mon Apr 10 14:47:19 2023, max compression
+gzip compressed data, was "tempora-5.3.0.tar", last modified: Sat Jun 10 16:01:54 2023, max compression
```

## Comparing `tempora-5.2.2.tar` & `tempora-5.3.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.522996 tempora-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 14:46:59.000000 tempora-5.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 14:46:59.000000 tempora-5.2.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-10 14:46:59.000000 tempora-5.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 14:46:59.000000 tempora-5.2.2/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 14:46:59.000000 tempora-5.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-10 14:46:59.000000 tempora-5.2.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 14:46:59.000000 tempora-5.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 14:46:59.000000 tempora-5.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-10 14:46:59.000000 tempora-5.2.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-10 14:46:59.000000 tempora-5.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-10 14:47:19.522996 tempora-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-10 14:46:59.000000 tempora-5.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-10 14:46:59.000000 tempora-5.2.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 14:46:59.000000 tempora-5.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 14:46:59.000000 tempora-5.2.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-10 14:46:59.000000 tempora-5.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 14:46:59.000000 tempora-5.2.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-10 14:46:59.000000 tempora-5.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-10 14:46:59.000000 tempora-5.2.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-10 14:47:19.522996 tempora-5.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/tempora/
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/utc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.522996 tempora-5.2.2/tempora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.522996 tempora-5.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-10 14:46:59.000000 tempora-5.2.2/tests/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-10 14:46:59.000000 tempora-5.2.2/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-10 14:46:59.000000 tempora-5.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-10 16:01:34.000000 tempora-5.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-10 16:01:34.000000 tempora-5.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.637063 tempora-5.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-10 16:01:34.000000 tempora-5.3.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-10 16:01:34.000000 tempora-5.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.637063 tempora-5.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-10 16:01:34.000000 tempora-5.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 16:01:34.000000 tempora-5.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-10 16:01:34.000000 tempora-5.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-10 16:01:34.000000 tempora-5.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-10 16:01:34.000000 tempora-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-10 16:01:54.641063 tempora-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-10 16:01:34.000000 tempora-5.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-10 16:01:34.000000 tempora-5.3.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.637063 tempora-5.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-10 16:01:34.000000 tempora-5.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 16:01:34.000000 tempora-5.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-10 16:01:34.000000 tempora-5.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-10 16:01:34.000000 tempora-5.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-10 16:01:34.000000 tempora-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-10 16:01:34.000000 tempora-5.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-10 16:01:54.645063 tempora-5.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/tempora/
+-rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/utc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/tempora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-10 16:01:34.000000 tempora-5.3.0/tests/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-10 16:01:34.000000 tempora-5.3.0/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-10 16:01:34.000000 tempora-5.3.0/tox.ini
```

### Comparing `tempora-5.2.2/.github/workflows/main.yml` & `tempora-5.3.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -100,14 +103,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `tempora-5.2.2/CHANGES.rst` & `tempora-5.3.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v5.3.0
+======
+
+#24: Removed use of ``datetime.utc**`` functions
+deprecated in Python 3.12.
+
 v5.2.2
 ======
 
 #22: Fixed bug in tests that would fail when a leap year
 was about a year away.
 
 v5.2.1
```

### Comparing `tempora-5.2.2/LICENSE` & `tempora-5.3.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tempora-5.2.2/PKG-INFO` & `tempora-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempora
-Version: 5.2.2
+Version: 5.3.0
 Summary: Objects and routines pertaining to date and time (tempora)
 Home-page: https://github.com/jaraco/tempora
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tempora-5.2.2/README.rst` & `tempora-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `tempora-5.2.2/docs/conf.py` & `tempora-5.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.2/docs/index.rst` & `tempora-5.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tempora-5.2.2/pytest.ini` & `tempora-5.3.0/pytest.ini`

 * *Files 24% similar despite different names*

```diff
@@ -3,33 +3,25 @@
 addopts=--doctest-modules
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
-	
-	# ktosiek/pytest-freezegun#35
-	ignore:distutils Version classes are deprecated:DeprecationWarning
```

### Comparing `tempora-5.2.2/setup.cfg` & `tempora-5.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -27,28 +27,24 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	backports.unittest_mock
-	freezegun
-	pytest-freezegun
-	types-freezegun
+	pytest-freezer
 	types-pytz
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```

### Comparing `tempora-5.2.2/tempora/__init__.py` & `tempora-5.3.0/tempora/__init__.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.2/tempora/schedule.py` & `tempora-5.3.0/tempora/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 def now():
     """
     Provide the current timezone-aware datetime.
 
     A client may override this function to change the default behavior,
     such as to use local time or timezone-naïve times.
     """
-    return datetime.datetime.utcnow().replace(tzinfo=pytz.utc)
+    return datetime.datetime.now(pytz.utc)
 
 
 def from_timestamp(ts):
     """
     Convert a numeric timestamp to a timezone-aware datetime.
 
     A client may override this function to change the default behavior,
     such as to use local time or timezone-naïve times.
     """
-    return datetime.datetime.utcfromtimestamp(ts).replace(tzinfo=pytz.utc)
+    return datetime.datetime.fromtimestamp(ts, pytz.utc)
 
 
 class DelayedCommand(datetime.datetime):
     """
     A command to be executed after some delay (seconds or timedelta).
     """
```

### Comparing `tempora-5.2.2/tempora/timing.py` & `tempora-5.3.0/tempora/timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,24 +47,24 @@
 
     def reset(self):
         self.elapsed = datetime.timedelta(0)
         with contextlib.suppress(AttributeError):
             del self.start_time
 
     def start(self):
-        self.start_time = datetime.datetime.utcnow()
+        self.start_time = datetime.datetime.now(datetime.timezone.utc)
 
     def stop(self):
-        stop_time = datetime.datetime.utcnow()
+        stop_time = datetime.datetime.now(datetime.timezone.utc)
         self.elapsed += stop_time - self.start_time
         del self.start_time
         return self.elapsed
 
     def split(self):
-        local_duration = datetime.datetime.utcnow() - self.start_time
+        local_duration = datetime.datetime.now(datetime.timezone.utc) - self.start_time
         return self.elapsed + local_duration
 
     # context manager support
     def __enter__(self):
         self.start()
         return self
```

### Comparing `tempora-5.2.2/tempora/utc.py` & `tempora-5.3.0/tempora/utc.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.2/tempora.egg-info/PKG-INFO` & `tempora-5.3.0/tempora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempora
-Version: 5.2.2
+Version: 5.3.0
 Summary: Objects and routines pertaining to date and time (tempora)
 Home-page: https://github.com/jaraco/tempora
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tempora-5.2.2/tempora.egg-info/SOURCES.txt` & `tempora-5.3.0/tempora.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 LICENSE
 README.rst
 conftest.py
 mypy.ini
```

### Comparing `tempora-5.2.2/tests/test_schedule.py` & `tempora-5.3.0/tests/test_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         sched.run_pending()
         callback.assert_called_once_with(target)
 
     def test_periodic_command(self):
         sched = schedule.InvokeScheduler()
         target = mock.MagicMock()
 
-        before = datetime.datetime.utcnow()
+        before = datetime.datetime.now(tz=datetime.timezone.utc)
 
         cmd = schedule.PeriodicCommand.after(10, target)
         sched.add(cmd)
         sched.run_pending()
         target.assert_not_called()
 
         with freezegun.freeze_time(before + datetime.timedelta(seconds=15)):
```

### Comparing `tempora-5.2.2/tests/test_timing.py` & `tempora-5.3.0/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.2/tox.ini` & `tempora-5.3.0/tox.ini`

 * *Files identical despite different names*

