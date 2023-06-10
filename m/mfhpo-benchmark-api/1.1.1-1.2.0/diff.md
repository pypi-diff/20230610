# Comparing `tmp/mfhpo_benchmark_api-1.1.1-py3-none-any.whl.zip` & `tmp/mfhpo_benchmark_api-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 24373 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      663 b- defN 23-Jun-10 15:19 benchmark_apis/__init__.py
--rw-rw-r--  2.0 unx     2294 b- defN 23-Jun-10 15:10 benchmark_apis/abstract_bench.py
--rw-rw-r--  2.0 unx     4701 b- defN 23-Jun-10 15:12 benchmark_apis/abstract_func.py
+Zip file size: 24371 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx      650 b- defN 23-Jun-10 21:32 benchmark_apis/__init__.py
 -rw-rw-r--  2.0 unx     2689 b- defN 23-Jun-10 15:11 benchmark_apis/abstract_interface.py
--rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-10 13:46 benchmark_apis/discrete_search_spaces.json
--rw-rw-r--  2.0 unx     6394 b- defN 23-Jun-10 15:17 benchmark_apis/hpobench/hpobench.py
--rw-rw-r--  2.0 unx     6265 b- defN 23-Jun-10 15:17 benchmark_apis/hpolib/hpolib.py
--rw-rw-r--  2.0 unx     7779 b- defN 23-Jun-10 15:17 benchmark_apis/jahs/jahs.py
--rw-rw-r--  2.0 unx     8487 b- defN 23-Jun-10 15:16 benchmark_apis/lcbench/lcbench.py
--rw-rw-r--  2.0 unx     3717 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/branin.py
--rw-rw-r--  2.0 unx     4583 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/hartmann.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 15:21 mfhpo_benchmark_api-1.1.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 15:21 mfhpo_benchmark_api-1.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 15:21 mfhpo_benchmark_api-1.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx      129 b- defN 23-Jun-10 15:21 mfhpo_benchmark_api-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1436 b- defN 23-Jun-10 15:21 mfhpo_benchmark_api-1.1.1.dist-info/RECORD
-16 files, 63528 bytes uncompressed, 21971 bytes compressed:  65.4%
+-rw-rw-r--  2.0 unx     2294 b- defN 23-Jun-10 21:27 benchmark_apis/hpo/abstract_bench.py
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-10 13:46 benchmark_apis/hpo/discrete_search_spaces.json
+-rw-rw-r--  2.0 unx     6398 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/hpobench.py
+-rw-rw-r--  2.0 unx     6269 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/hpolib.py
+-rw-rw-r--  2.0 unx     7783 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/jahs.py
+-rw-rw-r--  2.0 unx     8491 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/lcbench.py
+-rw-rw-r--  2.0 unx     4701 b- defN 23-Jun-10 15:12 benchmark_apis/synthetic/abstract_func.py
+-rw-rw-r--  2.0 unx     3727 b- defN 23-Jun-10 21:22 benchmark_apis/synthetic/branin.py
+-rw-rw-r--  2.0 unx     4593 b- defN 23-Jun-10 21:22 benchmark_apis/synthetic/hartmann.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       59 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/RECORD
+16 files, 63485 bytes uncompressed, 21959 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,49 +1,49 @@
 Filename: benchmark_apis/__init__.py
 Comment: 
 
-Filename: benchmark_apis/abstract_bench.py
+Filename: benchmark_apis/abstract_interface.py
 Comment: 
 
-Filename: benchmark_apis/abstract_func.py
+Filename: benchmark_apis/hpo/abstract_bench.py
 Comment: 
 
-Filename: benchmark_apis/abstract_interface.py
+Filename: benchmark_apis/hpo/discrete_search_spaces.json
 Comment: 
 
-Filename: benchmark_apis/discrete_search_spaces.json
+Filename: benchmark_apis/hpo/hpobench.py
 Comment: 
 
-Filename: benchmark_apis/hpobench/hpobench.py
+Filename: benchmark_apis/hpo/hpolib.py
 Comment: 
 
-Filename: benchmark_apis/hpolib/hpolib.py
+Filename: benchmark_apis/hpo/jahs.py
 Comment: 
 
-Filename: benchmark_apis/jahs/jahs.py
+Filename: benchmark_apis/hpo/lcbench.py
 Comment: 
 
-Filename: benchmark_apis/lcbench/lcbench.py
+Filename: benchmark_apis/synthetic/abstract_func.py
 Comment: 
 
 Filename: benchmark_apis/synthetic/branin.py
 Comment: 
 
 Filename: benchmark_apis/synthetic/hartmann.py
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.1.1.dist-info/LICENSE
+Filename: mfhpo_benchmark_api-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.1.1.dist-info/METADATA
+Filename: mfhpo_benchmark_api-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.1.1.dist-info/WHEEL
+Filename: mfhpo_benchmark_api-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.1.1.dist-info/top_level.txt
+Filename: mfhpo_benchmark_api-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.1.1.dist-info/RECORD
+Filename: mfhpo_benchmark_api-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_apis/__init__.py

```diff
@@ -1,16 +1,16 @@
-from benchmark_apis.hpobench.hpobench import HPOBench
-from benchmark_apis.hpolib.hpolib import HPOLib
-from benchmark_apis.jahs.jahs import JAHSBench201
-from benchmark_apis.lcbench.lcbench import LCBench
+from benchmark_apis.hpo.hpobench import HPOBench
+from benchmark_apis.hpo.hpolib import HPOLib
+from benchmark_apis.hpo.jahs import JAHSBench201
+from benchmark_apis.hpo.lcbench import LCBench
 from benchmark_apis.synthetic.branin import MFBranin
 from benchmark_apis.synthetic.hartmann import MFHartmann
 
 
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-benchmark-api/"
```

## benchmark_apis/synthetic/branin.py

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import ClassVar
 
-from benchmark_apis.abstract_func import MFAbstractFunc
+from benchmark_apis.synthetic.abstract_func import MFAbstractFunc
 
 import numpy as np
 
 
 @dataclass(frozen=True)
 class _BraninCoefficients:
     a: float
```

## benchmark_apis/synthetic/hartmann.py

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import ClassVar, Literal
 
-from benchmark_apis.abstract_func import MFAbstractFunc
+from benchmark_apis.synthetic.abstract_func import MFAbstractFunc
 
 import numpy as np
 
 
 class MFHartmann(MFAbstractFunc):
     """
     Multi-fidelity Hartmann Function.
```

## Comparing `benchmark_apis/abstract_bench.py` & `benchmark_apis/hpo/abstract_bench.py`

 * *Files identical despite different names*

## Comparing `benchmark_apis/abstract_func.py` & `benchmark_apis/synthetic/abstract_func.py`

 * *Files identical despite different names*

## Comparing `benchmark_apis/discrete_search_spaces.json` & `benchmark_apis/hpo/discrete_search_spaces.json`

 * *Files identical despite different names*

## Comparing `benchmark_apis/hpobench/hpobench.py` & `benchmark_apis/hpo/hpobench.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 import pickle
 from dataclasses import dataclass
 from typing import ClassVar, Literal, TypedDict
 
 import ConfigSpace as CS
 
-from benchmark_apis.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
 from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType
+from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
 
 import numpy as np
 
 
 @dataclass(frozen=True)
 class _TargetMetricKeys:
     loss: str = "bal_acc"
```

## Comparing `benchmark_apis/hpolib/hpolib.py` & `benchmark_apis/hpo/hpolib.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 import pickle
 from dataclasses import dataclass
 from typing import ClassVar, Literal, TypedDict
 
 import ConfigSpace as CS
 
-from benchmark_apis.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
 from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType
+from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
 
 import numpy as np
 
 
 @dataclass(frozen=True)
 class _TargetMetricKeys:
     loss: str = "valid_mse"
```

## Comparing `benchmark_apis/jahs/jahs.py` & `benchmark_apis/hpo/jahs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import os
 from dataclasses import dataclass
 from typing import ClassVar
 
 import ConfigSpace as CS
 
-from benchmark_apis.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
 from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType, _warn_not_found_module
+from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
 
 try:
     import jahs_bench
 except ModuleNotFoundError:  # We cannot use jahs with smac
     _warn_not_found_module(bench_name="jahs")
```

## Comparing `benchmark_apis/lcbench/lcbench.py` & `benchmark_apis/hpo/lcbench.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import os
 from dataclasses import dataclass
 from typing import ClassVar
 
 import ConfigSpace as CS
 
-from benchmark_apis.abstract_bench import AbstractBench, DATA_DIR_NAME
 from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType, _warn_not_found_module
+from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME
 
 try:
     from yahpo_gym import benchmark_set, local_config
 except ModuleNotFoundError:
     _warn_not_found_module(bench_name="lcbench")
 
 
@@ -181,15 +181,15 @@
         benchdata: LCBenchSurrogate | None = None,
     ) -> ResultType:
         if benchdata is None and self._surrogate is None:
             raise ValueError("data must be provided when `keep_benchdata` is False")
 
         surrogate = benchdata if self._surrogate is None else self._surrogate
         assert surrogate is not None  # mypy redefinition
-        fidel = int(fidels.get(_FIDEL_KEY, min(self._max_epoch, self._TRUE_MAX_EPOCH)))
+        fidel = int(min(self._TRUE_MAX_EPOCH, fidels.get(_FIDEL_KEY, self._max_epoch)))
         self._validate_config(eval_config=eval_config)
         return surrogate(eval_config=eval_config, fidel=fidel)
 
     @property
     def config_space(self) -> CS.ConfigurationSpace:
         config_space = CS.ConfigurationSpace()
         config_space.add_hyperparameters(
```

## Comparing `mfhpo_benchmark_api-1.1.1.dist-info/LICENSE` & `mfhpo_benchmark_api-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_benchmark_api-1.1.1.dist-info/METADATA` & `mfhpo_benchmark_api-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfhpo-benchmark-api
-Version: 1.1.1
+Version: 1.2.0
 Home-page: https://github.com/nabenabe0928/mfhpo-benchmark-api
 Author: nabenabe0928
 Author-email: shuhei.watanabe.utokyo@gmail.com
 Platform: Linux
 Platform: Darwin
 Requires-Python: >=3.8
 License-File: LICENSE
```

