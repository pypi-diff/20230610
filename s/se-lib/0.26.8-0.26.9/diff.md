# Comparing `tmp/se_lib-0.26.8.tar.gz` & `tmp/se_lib-0.26.9.tar.gz`

## Comparing `se_lib-0.26.8.tar` & `se_lib-0.26.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.8/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.8/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.8/selib/.DS_Store
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 se_lib-0.26.8/selib/__init__.py
--rw-r--r--   0        0        0    80457 2020-02-02 00:00:00.000000 se_lib-0.26.8/selib/selib.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 se_lib-0.26.8/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.8/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 se_lib-0.26.8/pyproject.toml
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 se_lib-0.26.8/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.9/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.9/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.9/selib/.DS_Store
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 se_lib-0.26.9/selib/__init__.py
+-rw-r--r--   0        0        0    80457 2020-02-02 00:00:00.000000 se_lib-0.26.9/selib/selib.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 se_lib-0.26.9/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.9/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 se_lib-0.26.9/pyproject.toml
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 se_lib-0.26.9/PKG-INFO
```

### Comparing `se_lib-0.26.8/.DS_Store` & `se_lib-0.26.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.8/selib/.DS_Store` & `se_lib-0.26.9/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.8/selib/__init__.py` & `se_lib-0.26.9/selib/__init__.py`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.8/selib/selib.py` & `se_lib-0.26.9/selib/selib.py`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.8/LICENSE` & `se_lib-0.26.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-se-lib Version .26.7
+se-lib Version .26.9
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26.8/README.md` & `se_lib-0.26.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Systems Engineering Library (se-lib)
-Version .26.8
+Version .26.9
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26.8/pyproject.toml` & `se_lib-0.26.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "se-lib"
-version = "0.26.8"
+version = "0.26.9"
 authors = [
   { name="se-lib Development Team", email="info@se-lib.org" },
 ]
 description = "Systems Engineering Library (se-lib)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `se_lib-0.26.8/PKG-INFO` & `se_lib-0.26.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.26.8
+Version: 0.26.9
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pysd
 Requires-Dist: simpy
 Description-Content-Type: text/markdown
 
 # Systems Engineering Library (se-lib)
-Version .26.8
+Version .26.9
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

