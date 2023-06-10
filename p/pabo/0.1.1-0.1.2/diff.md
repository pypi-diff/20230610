# Comparing `tmp/pabo-0.1.1.tar.gz` & `tmp/pabo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pabo-0.1.1.tar", last modified: Fri Feb 10 14:04:58 2023, max compression
+gzip compressed data, was "pabo-0.1.2.tar", last modified: Sat Jun 10 13:48:17 2023, max compression
```

## Comparing `pabo-0.1.1.tar` & `pabo-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.536481 pabo-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.532481 pabo-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.536481 pabo-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-02-10 14:04:49.000000 pabo-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-10 14:04:49.000000 pabo-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-10 14:04:49.000000 pabo-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-10 14:04:49.000000 pabo-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-10 14:04:49.000000 pabo-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-02-10 14:04:58.536481 pabo-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-02-10 14:04:49.000000 pabo-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.536481 pabo-0.1.1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-02-10 14:04:49.000000 pabo-0.1.1/assets/doc_cov.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.536481 pabo-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-10 14:04:49.000000 pabo-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-10 14:04:49.000000 pabo-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.536481 pabo-0.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-10 14:04:49.000000 pabo-0.1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-10 14:04:49.000000 pabo-0.1.1/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-10 14:04:49.000000 pabo-0.1.1/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-10 14:04:49.000000 pabo-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-10 14:04:58.536481 pabo-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-10 14:04:49.000000 pabo-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.532481 pabo-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.536481 pabo-0.1.1/src/pabo/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-10 14:04:58.000000 pabo-0.1.1/src/pabo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/bits.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/core.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/specify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-02-10 14:04:49.000000 pabo-0.1.1/src/pabo/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:04:58.536481 pabo-0.1.1/src/pabo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-02-10 14:04:58.000000 pabo-0.1.1/src/pabo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-10 14:04:58.000000 pabo-0.1.1/src/pabo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:04:58.000000 pabo-0.1.1/src/pabo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:04:58.000000 pabo-0.1.1/src/pabo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 14:04:58.000000 pabo-0.1.1/src/pabo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-10 14:04:58.000000 pabo-0.1.1/src/pabo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.890246 pabo-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-10 13:48:06.000000 pabo-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-10 13:48:06.000000 pabo-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 13:48:06.000000 pabo-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-10 13:48:06.000000 pabo-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-10 13:48:06.000000 pabo-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-10 13:48:17.890246 pabo-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-10 13:48:06.000000 pabo-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-10 13:48:06.000000 pabo-0.1.2/assets/doc_cov.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-10 13:48:06.000000 pabo-0.1.2/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-10 13:48:06.000000 pabo-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-10 13:48:17.890246 pabo-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-10 13:48:06.000000 pabo-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.890246 pabo-0.1.2/src/pabo/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/core.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/specify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.890246 pabo-0.1.2/src/pabo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/top_level.txt
```

### Comparing `pabo-0.1.1/.github/workflows/release.yml` & `pabo-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/LICENSE` & `pabo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/PKG-INFO` & `pabo-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pabo
-Version: 0.1.1
+Version: 0.1.2
 Summary: "Binary parsing for dummies!"
 Home-page: https://github.com/astrogewgaw/pabo
 Author: "Ujjwal Panda"
 Author-email: "ujjwalpanda97@gmail.com"
 License: MIT License
 Project-URL: Source Code, https://github.com/astrogewgaw/pabo
 Project-URL: Documentation, https://pabo.readthedocs.io/en/latest
```

### Comparing `pabo-0.1.1/README.md` & `pabo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/assets/doc_cov.svg` & `pabo-0.1.2/assets/doc_cov.svg`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/justfile` & `pabo-0.1.2/justfile`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/pyproject.toml` & `pabo-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/setup.cfg` & `pabo-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo/__init__.py` & `pabo-0.1.2/src/pabo/__init__.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo/base.py` & `pabo-0.1.2/src/pabo/base.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo/bits.py` & `pabo-0.1.2/src/pabo/bits.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo/bytes.py` & `pabo-0.1.2/src/pabo/bytes.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo/core.cpp` & `pabo-0.1.2/src/pabo/core.cpp`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo/numeric.py` & `pabo-0.1.2/src/pabo/numeric.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,21 +89,21 @@
 
     def __size__(self):
         return self.count
 
     def __build__(self, data, stream):
         if len(data) < self.count:
             raise PaboError("Not enough data to build.")
-        data = data[: self.count] if self.count != -1 else data
+        data = data[: self.count] if self.count > 0 else data
         array = np.asarray(data, dtype=self.main.__format__)
         if self.packing is not None:
             array = pack(array.flatten(), nbits=self.packing)
         stream.write(array.tobytes())
 
     def __parse__(self, stream):
-        data = stream.read(self.count)
+        data = stream.read(self.count * self.main.width if self.count > 0 else -1)
         if len(data) < self.count:
             raise PaboError("Not enough data to parse.")
         array = np.frombuffer(data, dtype=self.main.__format__)
         if self.packing is not None:
             array = unpack(array, nbits=self.packing)
         return array
```

### Comparing `pabo-0.1.1/src/pabo/specify.py` & `pabo-0.1.2/src/pabo/specify.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo/strings.py` & `pabo-0.1.2/src/pabo/strings.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,18 +55,15 @@
         raise PaboError("A PascalString has no fixed size.")
 
     def __build__(self, data, stream) -> None:
         raw = data.encode(self.code)
         Prefixed(self.pre, Bytes(-1)).__build__(raw, stream)
 
     def __parse__(self, stream):
-        main = Prefixed(self.pre, Bytes(-1))
-        raw = main.__parse__(stream)
-        data = raw.decode(self.code)
-        return data
+        return Prefixed(self.pre, Bytes(-1)).__parse__(stream).decode(self.code)
 
 
 @define
 class PaddedString(Construct):
 
     """
     Represents a string padded by null bytes (\x00).
```

### Comparing `pabo-0.1.1/src/pabo/wrappers.py` & `pabo-0.1.2/src/pabo/wrappers.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.1/src/pabo.egg-info/PKG-INFO` & `pabo-0.1.2/src/pabo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pabo
-Version: 0.1.1
+Version: 0.1.2
 Summary: "Binary parsing for dummies!"
 Home-page: https://github.com/astrogewgaw/pabo
 Author: "Ujjwal Panda"
 Author-email: "ujjwalpanda97@gmail.com"
 License: MIT License
 Project-URL: Source Code, https://github.com/astrogewgaw/pabo
 Project-URL: Documentation, https://pabo.readthedocs.io/en/latest
```

### Comparing `pabo-0.1.1/src/pabo.egg-info/SOURCES.txt` & `pabo-0.1.2/src/pabo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

