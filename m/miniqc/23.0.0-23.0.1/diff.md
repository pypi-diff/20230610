# Comparing `tmp/miniqc-23.0.0.tar.gz` & `tmp/miniqc-23.0.1.tar.gz`

## Comparing `miniqc-23.0.0.tar` & `miniqc-23.0.1.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 miniqc-23.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 miniqc-23.0.0/.github/workflows/hatch.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.0.0/miniqc/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 miniqc-23.0.0/miniqc/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 miniqc-23.0.0/miniqc/_version.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 miniqc-23.0.0/miniqc/_version.pyi
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 miniqc-23.0.0/miniqc/nifti.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.0.0/miniqc/py.typed
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 miniqc-23.0.0/miniqc/types.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/__init__.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/conftest.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/test_miniqc.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/test_nifti.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/data/bids_dataset/dataset_description.json
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-dangling_T2w.nii.gz -> does-not-exist
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-good_T1w.nii.gz
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-nii2_T1w.nii.gz
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 miniqc-23.0.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 miniqc-23.0.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 miniqc-23.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 miniqc-23.0.0/README.md
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 miniqc-23.0.0/pyproject.toml
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 miniqc-23.0.0/PKG-INFO
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 miniqc-23.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 miniqc-23.0.1/Dockerfile
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 miniqc-23.0.1/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 miniqc-23.0.1/.github/workflows/hatch.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 miniqc-23.0.1/.maint/local_gitignore
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 miniqc-23.0.1/.maint/make_gitignore
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/__init__.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/_version.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/_version.pyi
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/nifti.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/py.typed
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/types.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/test_miniqc.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/test_nifti.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/dataset_description.json
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-dangling_T2w.nii.gz -> does-not-exist
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-good_T1w.nii.gz
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-nii2_T1w.nii.gz
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 miniqc-23.0.1/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 miniqc-23.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 miniqc-23.0.1/README.md
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 miniqc-23.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 miniqc-23.0.1/PKG-INFO
```

### Comparing `miniqc-23.0.0/.github/workflows/hatch.yml` & `miniqc-23.0.1/.github/workflows/hatch.yml`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.0/miniqc/__main__.py` & `miniqc-23.0.1/miniqc/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import json
 import os
 import re
 import typing as ty
 from enum import Enum
 from pathlib import Path
 
+import nibabel as nb
 import typer
+from typing_extensions import TypeAlias
 
 from . import nifti
 from .types import CheckList, FailedCheck
 
+# Add to this list as file types are added
+SupportedType: TypeAlias = ty.Union[nb.Nifti1Image,]
+
 # Regex patterns paired with checklists to verify on file
 # To avoid multiple reads, only the first matching check is applied to each
 # file
-CHECKS: list[tuple[re.Pattern[str], CheckList]] = [
+CHECKS: list[tuple[re.Pattern[str], CheckList[SupportedType]]] = [
     (re.compile(r'\.nii(\.gz)?$'), nifti.CHECKS),
 ]
 
 app = typer.Typer()
 
 
 class AnalysisLevel(Enum):
```

### Comparing `miniqc-23.0.0/miniqc/nifti.py` & `miniqc-23.0.1/miniqc/nifti.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,19 +14,19 @@
         return nb.Nifti2Image.from_filename(path)
 
 
 def fullsize(img: nb.Nifti1Image) -> CheckResult:
     """Verify NIfTI image has expected length from header"""
     dataobj: nb.arrayproxy.ArrayProxy = img.dataobj  # type: ignore
 
-    expected = dataobj.offset + dataobj.dtype.itemsize * prod(dataobj.shape)
+    expected: int = dataobj.offset + dataobj.dtype.itemsize * prod(dataobj.shape)
 
     with dataobj._get_fileobj() as fobj:
         # Seek beyond end returns end position
-        actual = fobj.seek(expected + 1)
+        actual: int = fobj.seek(expected + 1)
     return CheckResult(
         (actual == expected, f'Expected {expected} bytes; found {actual}')
     )
 
 
 CHECKS = CheckList(
     loader=load,
```

### Comparing `miniqc-23.0.0/tests/conftest.py` & `miniqc-23.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.0/tests/test_miniqc.py` & `miniqc-23.0.1/tests/test_miniqc.py`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.0/tests/test_nifti.py` & `miniqc-23.0.1/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.0/LICENSE.txt` & `miniqc-23.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.0/README.md` & `miniqc-23.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,17 +53,16 @@
   ]
 ]
 ```
 
 ### Outputs
 
 The output of this tool is a JSON array of arrays, each of length 3.
-The each sub-array contains the failed file (relative to dataset root),
-the type of error (`"FailedCheck"` for miniqc-defined failures, or any Python
-exceptions raised while checking the file).
+Each sub-array contains the failed file (relative to dataset root),
+the type of error, and a message with more detail.
 
 ## Testing
 
 With the [hatch](https://hatch.pypa.io) project management tool installed:
 
 ```console
 hatch run test:cov
```

### Comparing `miniqc-23.0.0/pyproject.toml` & `miniqc-23.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "nibabel",
   "typer",
+  "typing_extensions",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/effigies/miniqc#readme"
 Issues = "https://github.com/effigies/miniqc/issues"
 Source = "https://github.com/effigies/miniqc"
```

### Comparing `miniqc-23.0.0/PKG-INFO` & `miniqc-23.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniqc
-Version: 23.0.0
+Version: 23.0.1
 Summary: A BIDS app for performing minimal QC beyond validation
 Project-URL: Documentation, https://github.com/effigies/miniqc#readme
 Project-URL: Issues, https://github.com/effigies/miniqc/issues
 Project-URL: Source, https://github.com/effigies/miniqc
 Author-email: Chris Markiewicz <markiewicz@stanford.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: nibabel
 Requires-Dist: typer
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # miniQC
 
 [![PyPI - Version](https://img.shields.io/pypi/v/miniqc.svg)](https://pypi.org/project/miniqc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/miniqc.svg)](https://pypi.org/project/miniqc)
 
@@ -73,17 +74,16 @@
   ]
 ]
 ```
 
 ### Outputs
 
 The output of this tool is a JSON array of arrays, each of length 3.
-The each sub-array contains the failed file (relative to dataset root),
-the type of error (`"FailedCheck"` for miniqc-defined failures, or any Python
-exceptions raised while checking the file).
+Each sub-array contains the failed file (relative to dataset root),
+the type of error, and a message with more detail.
 
 ## Testing
 
 With the [hatch](https://hatch.pypa.io) project management tool installed:
 
 ```console
 hatch run test:cov
```

