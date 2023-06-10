# Comparing `tmp/mfhpo_benchmark_api-1.0.2-py3-none-any.whl.zip` & `tmp/mfhpo_benchmark_api-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 22926 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      944 b- defN 23-Jun-10 11:33 benchmark_apis/__init__.py
+Zip file size: 23101 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      663 b- defN 23-Jun-10 11:52 benchmark_apis/__init__.py
 -rw-rw-r--  2.0 unx     2235 b- defN 23-Jun-10 09:44 benchmark_apis/abstract_bench.py
 -rw-rw-r--  2.0 unx     4633 b- defN 23-Jun-10 09:49 benchmark_apis/abstract_func.py
--rw-rw-r--  2.0 unx     2236 b- defN 23-Jun-10 10:05 benchmark_apis/abstract_interface.py
+-rw-rw-r--  2.0 unx     2492 b- defN 23-Jun-10 11:57 benchmark_apis/abstract_interface.py
 -rw-rw-r--  2.0 unx     6075 b- defN 23-Jun-10 09:47 benchmark_apis/hpobench/hpobench.py
 -rw-rw-r--  2.0 unx     5817 b- defN 23-Jun-10 09:48 benchmark_apis/hpolib/hpolib.py
--rw-rw-r--  2.0 unx     7500 b- defN 23-Jun-10 09:49 benchmark_apis/jahs/jahs.py
--rw-rw-r--  2.0 unx     8501 b- defN 23-Jun-10 09:49 benchmark_apis/lcbench/lcbench.py
+-rw-rw-r--  2.0 unx     7561 b- defN 23-Jun-10 11:57 benchmark_apis/jahs/jahs.py
+-rw-rw-r--  2.0 unx     8611 b- defN 23-Jun-10 11:58 benchmark_apis/lcbench/lcbench.py
 -rw-rw-r--  2.0 unx     3717 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/branin.py
 -rw-rw-r--  2.0 unx     4583 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/hartmann.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 11:33 mfhpo_benchmark_api-1.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      456 b- defN 23-Jun-10 11:33 mfhpo_benchmark_api-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 11:33 mfhpo_benchmark_api-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx      129 b- defN 23-Jun-10 11:33 mfhpo_benchmark_api-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1337 b- defN 23-Jun-10 11:33 mfhpo_benchmark_api-1.0.2.dist-info/RECORD
-15 files, 59015 bytes uncompressed, 20684 bytes compressed:  65.0%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      129 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1337 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/RECORD
+15 files, 59269 bytes uncompressed, 20859 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: benchmark_apis/synthetic/branin.py
 Comment: 
 
 Filename: benchmark_apis/synthetic/hartmann.py
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.2.dist-info/LICENSE
+Filename: mfhpo_benchmark_api-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.2.dist-info/METADATA
+Filename: mfhpo_benchmark_api-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.2.dist-info/WHEEL
+Filename: mfhpo_benchmark_api-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.2.dist-info/top_level.txt
+Filename: mfhpo_benchmark_api-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.2.dist-info/RECORD
+Filename: mfhpo_benchmark_api-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_apis/__init__.py

```diff
@@ -1,39 +1,16 @@
-try:
-    from benchmark_apis.hpobench.hpobench import HPOBench
-except ModuleNotFoundError:
-    pass
+from benchmark_apis.hpobench.hpobench import HPOBench
+from benchmark_apis.hpolib.hpolib import HPOLib
+from benchmark_apis.jahs.jahs import JAHSBench201
+from benchmark_apis.lcbench.lcbench import LCBench
+from benchmark_apis.synthetic.branin import MFBranin
+from benchmark_apis.synthetic.hartmann import MFHartmann
 
-try:
-    from benchmark_apis.hpolib.hpolib import HPOLib
-except ModuleNotFoundError:
-    pass
 
-try:
-    from benchmark_apis.jahs.jahs import JAHSBench201
-except ModuleNotFoundError:
-    pass
-
-try:
-    from benchmark_apis.lcbench.lcbench import LCBench
-except ModuleNotFoundError:
-    pass
-
-try:
-    from benchmark_apis.synthetic.branin import MFBranin
-except ModuleNotFoundError:
-    pass
-
-try:
-    from benchmark_apis.synthetic.hartmann import MFHartmann
-except ModuleNotFoundError:
-    pass
-
-
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-benchmark-api/"
```

## benchmark_apis/abstract_interface.py

```diff
@@ -1,19 +1,27 @@
 from __future__ import annotations
 
 import os
+import warnings
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from typing import ClassVar, Optional, TypedDict
 
 import ConfigSpace as CS
 
 import numpy as np
 
 
+def _warn_not_found_module(bench_name: str) -> None:
+    cmd = "pip install mfhpo-benchmark-api"
+    warnings.warn(
+        f"{bench_name} requirements not found. Use `{cmd}[full]` or `{cmd}[{bench_name}]` when using {bench_name}."
+    )
+
+
 @dataclass(frozen=True)
 class _ResultKeys:
     loss: str = "loss"
     runtime: str = "runtime"
     model_size: str = "model_size"
     f1: str = "f1"
     precision: str = "precision"
```

## benchmark_apis/jahs/jahs.py

```diff
@@ -3,20 +3,20 @@
 import os
 from dataclasses import dataclass
 from typing import ClassVar
 
 import ConfigSpace as CS
 
 from benchmark_apis.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
-from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType
+from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType, _warn_not_found_module
 
 try:
     import jahs_bench
 except ModuleNotFoundError:  # We cannot use jahs with smac
-    pass
+    _warn_not_found_module(bench_name="jahs")
 
 
 @dataclass(frozen=True)
 class _TargetMetricKeys:
     loss: str = "valid-acc"
     runtime: str = "runtime"
     model_size: str = "size_MB"
```

## benchmark_apis/lcbench/lcbench.py

```diff
@@ -3,17 +3,20 @@
 import os
 from dataclasses import dataclass
 from typing import ClassVar
 
 import ConfigSpace as CS
 
 from benchmark_apis.abstract_bench import AbstractBench, DATA_DIR_NAME
-from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType
+from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType, _warn_not_found_module
 
-from yahpo_gym import benchmark_set, local_config
+try:
+    from yahpo_gym import benchmark_set, local_config
+except ModuleNotFoundError:
+    _warn_not_found_module(bench_name="lcbench")
 
 
 @dataclass(frozen=True)
 class _TargetMetricKeys:
     loss: str = "val_balanced_accuracy"
     runtime: str = "time"
```

## Comparing `mfhpo_benchmark_api-1.0.2.dist-info/LICENSE` & `mfhpo_benchmark_api-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_benchmark_api-1.0.2.dist-info/RECORD` & `mfhpo_benchmark_api-1.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-benchmark_apis/__init__.py,sha256=nIl2Zp_Ffy9ngOXzEkwwMqam1VYJ222M5ZtiKHt7NQs,944
+benchmark_apis/__init__.py,sha256=QdLy7Byts7HOErMi7mIbt1sHB-ObLpL4LJh6rRNeH3s,663
 benchmark_apis/abstract_bench.py,sha256=EEM9Or2BY5KU-PFD5WEnPye4FaKywhhtpI_AV2OghMo,2235
 benchmark_apis/abstract_func.py,sha256=x5qIi-g9EwKR37-TRGmudqeaRXF6vheGx1hfvhvnX3Y,4633
-benchmark_apis/abstract_interface.py,sha256=JuSFxCWzn22ZX0bP9-lQc4aN9GX0IqRlDnhHPPp0Kq4,2236
+benchmark_apis/abstract_interface.py,sha256=A9WPFCgxW3eij7g1j-6TnWVysBxsHspQLb-B9Tg8_Xg,2492
 benchmark_apis/hpobench/hpobench.py,sha256=m8BMQEsDVgKKQYh1WSQIT63xNbJ9rjx8_bgSAdwWzQs,6075
 benchmark_apis/hpolib/hpolib.py,sha256=ATD6ZO1cOxQo66MmvfydvSQznYZFAlhgO1fLpz6wISQ,5817
-benchmark_apis/jahs/jahs.py,sha256=pyFuH4c22xOXwM_WwX8ryyPI4E1U_OWZbQ0rm1A55z4,7500
-benchmark_apis/lcbench/lcbench.py,sha256=KXWP_Dc1my42LEx6wr7cl_FZqsVqoJan6a6Y0YgfsuU,8501
+benchmark_apis/jahs/jahs.py,sha256=oAYt1cjV5VtVzx-OT8E5UGjyhLkpJQPJ6BrVq1nPkoQ,7561
+benchmark_apis/lcbench/lcbench.py,sha256=13K5vbgK_-KguOxtEv77j4uM7GAqVMD2de3LbbrpD08,8611
 benchmark_apis/synthetic/branin.py,sha256=HZC4Yq4KOmb91pSKAJCosAL_W_whiPAEInrkNhVuh58,3717
 benchmark_apis/synthetic/hartmann.py,sha256=-wcPvr-vaE5qmlV58bInwdHDksrX4KxDuPtwTT10tnE,4583
-mfhpo_benchmark_api-1.0.2.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_benchmark_api-1.0.2.dist-info/METADATA,sha256=f-o8ofGxtvwS_UXAGuVCZ78J6L5HNz9dMbzI6lKAp6Y,456
-mfhpo_benchmark_api-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_benchmark_api-1.0.2.dist-info/top_level.txt,sha256=iPvqaBSsSXa6C3RgpKBBQEwUK8Sava3jgYaJJvP159w,129
-mfhpo_benchmark_api-1.0.2.dist-info/RECORD,,
+mfhpo_benchmark_api-1.0.3.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_benchmark_api-1.0.3.dist-info/METADATA,sha256=F1IRnjH-q0VBcB2cDoGlWF6WC6yeIC8P4VVi0RCAvtU,564
+mfhpo_benchmark_api-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_benchmark_api-1.0.3.dist-info/top_level.txt,sha256=iPvqaBSsSXa6C3RgpKBBQEwUK8Sava3jgYaJJvP159w,129
+mfhpo_benchmark_api-1.0.3.dist-info/RECORD,,
```

