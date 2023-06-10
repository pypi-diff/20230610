# Comparing `tmp/mfhpo_benchmark_api-1.0.3-py3-none-any.whl.zip` & `tmp/mfhpo_benchmark_api-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 23101 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      663 b- defN 23-Jun-10 11:52 benchmark_apis/__init__.py
--rw-rw-r--  2.0 unx     2235 b- defN 23-Jun-10 09:44 benchmark_apis/abstract_bench.py
+Zip file size: 23875 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx      663 b- defN 23-Jun-10 12:11 benchmark_apis/__init__.py
+-rw-rw-r--  2.0 unx     2294 b- defN 23-Jun-10 12:10 benchmark_apis/abstract_bench.py
 -rw-rw-r--  2.0 unx     4633 b- defN 23-Jun-10 09:49 benchmark_apis/abstract_func.py
 -rw-rw-r--  2.0 unx     2492 b- defN 23-Jun-10 11:57 benchmark_apis/abstract_interface.py
+-rw-rw-r--  2.0 unx     2981 b- defN 23-Jun-09 14:33 benchmark_apis/discrete_search_spaces.json
 -rw-rw-r--  2.0 unx     6075 b- defN 23-Jun-10 09:47 benchmark_apis/hpobench/hpobench.py
 -rw-rw-r--  2.0 unx     5817 b- defN 23-Jun-10 09:48 benchmark_apis/hpolib/hpolib.py
 -rw-rw-r--  2.0 unx     7561 b- defN 23-Jun-10 11:57 benchmark_apis/jahs/jahs.py
 -rw-rw-r--  2.0 unx     8611 b- defN 23-Jun-10 11:58 benchmark_apis/lcbench/lcbench.py
 -rw-rw-r--  2.0 unx     3717 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/branin.py
 -rw-rw-r--  2.0 unx     4583 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/hartmann.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx      129 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1337 b- defN 23-Jun-10 12:00 mfhpo_benchmark_api-1.0.3.dist-info/RECORD
-15 files, 59269 bytes uncompressed, 20859 bytes compressed:  64.8%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      129 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1436 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/RECORD
+16 files, 62408 bytes uncompressed, 21473 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: benchmark_apis/abstract_func.py
 Comment: 
 
 Filename: benchmark_apis/abstract_interface.py
 Comment: 
 
+Filename: benchmark_apis/discrete_search_spaces.json
+Comment: 
+
 Filename: benchmark_apis/hpobench/hpobench.py
 Comment: 
 
 Filename: benchmark_apis/hpolib/hpolib.py
 Comment: 
 
 Filename: benchmark_apis/jahs/jahs.py
@@ -24,23 +27,23 @@
 
 Filename: benchmark_apis/synthetic/branin.py
 Comment: 
 
 Filename: benchmark_apis/synthetic/hartmann.py
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.3.dist-info/LICENSE
+Filename: mfhpo_benchmark_api-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.3.dist-info/METADATA
+Filename: mfhpo_benchmark_api-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.3.dist-info/WHEEL
+Filename: mfhpo_benchmark_api-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.3.dist-info/top_level.txt
+Filename: mfhpo_benchmark_api-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.3.dist-info/RECORD
+Filename: mfhpo_benchmark_api-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_apis/__init__.py

```diff
@@ -2,15 +2,15 @@
 from benchmark_apis.hpolib.hpolib import HPOLib
 from benchmark_apis.jahs.jahs import JAHSBench201
 from benchmark_apis.lcbench.lcbench import LCBench
 from benchmark_apis.synthetic.branin import MFBranin
 from benchmark_apis.synthetic.hartmann import MFHartmann
 
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-benchmark-api/"
```

## benchmark_apis/abstract_bench.py

```diff
@@ -6,16 +6,17 @@
 from typing import ClassVar, Final
 
 import ConfigSpace as CS
 
 from benchmark_apis.abstract_interface import AbstractHPOData, AbstractInterface
 
 
+curdir = os.path.dirname(os.path.abspath(__file__))
 DATA_DIR_NAME: Final[str] = os.path.join(os.environ["HOME"], "hpo_benchmarks")
-SEARCH_SPACE_PATH: Final[str] = "benchmark_apis/discrete_search_spaces.json"
+SEARCH_SPACE_PATH: Final[str] = os.path.join(curdir, "discrete_search_spaces.json")
 VALUE_RANGES: Final[dict[str, dict[str, list[int | float | str | bool]]]] = json.load(open(SEARCH_SPACE_PATH))
 
 
 class AbstractBench(AbstractInterface):
     _BENCH_TYPE: ClassVar[str] = "HPO"
     _TARGET_METRIC_KEYS: ClassVar[list[str]]
     _N_DATASETS: ClassVar[int]
```

## Comparing `mfhpo_benchmark_api-1.0.3.dist-info/LICENSE` & `mfhpo_benchmark_api-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_benchmark_api-1.0.3.dist-info/METADATA` & `mfhpo_benchmark_api-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfhpo-benchmark-api
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/nabenabe0928/mfhpo-benchmark-api
 Author: nabenabe0928
 Author-email: shuhei.watanabe.utokyo@gmail.com
 Platform: Linux
 Platform: Darwin
 Requires-Python: >=3.8
 License-File: LICENSE
```

## Comparing `mfhpo_benchmark_api-1.0.3.dist-info/RECORD` & `mfhpo_benchmark_api-1.0.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-benchmark_apis/__init__.py,sha256=QdLy7Byts7HOErMi7mIbt1sHB-ObLpL4LJh6rRNeH3s,663
-benchmark_apis/abstract_bench.py,sha256=EEM9Or2BY5KU-PFD5WEnPye4FaKywhhtpI_AV2OghMo,2235
+benchmark_apis/__init__.py,sha256=NsQBdArefiTKodTt2LptICOOgu4iUCtwTAwqEZjtRmk,663
+benchmark_apis/abstract_bench.py,sha256=9kNF_E1jO8z1fA4EHQT1yufsAJ9e5MbgHtQSLQQXkjQ,2294
 benchmark_apis/abstract_func.py,sha256=x5qIi-g9EwKR37-TRGmudqeaRXF6vheGx1hfvhvnX3Y,4633
 benchmark_apis/abstract_interface.py,sha256=A9WPFCgxW3eij7g1j-6TnWVysBxsHspQLb-B9Tg8_Xg,2492
+benchmark_apis/discrete_search_spaces.json,sha256=w8J23jbT3u5qdQUba8MCe8cQ69ZVeSc1oy6mDaSzLXY,2981
 benchmark_apis/hpobench/hpobench.py,sha256=m8BMQEsDVgKKQYh1WSQIT63xNbJ9rjx8_bgSAdwWzQs,6075
 benchmark_apis/hpolib/hpolib.py,sha256=ATD6ZO1cOxQo66MmvfydvSQznYZFAlhgO1fLpz6wISQ,5817
 benchmark_apis/jahs/jahs.py,sha256=oAYt1cjV5VtVzx-OT8E5UGjyhLkpJQPJ6BrVq1nPkoQ,7561
 benchmark_apis/lcbench/lcbench.py,sha256=13K5vbgK_-KguOxtEv77j4uM7GAqVMD2de3LbbrpD08,8611
 benchmark_apis/synthetic/branin.py,sha256=HZC4Yq4KOmb91pSKAJCosAL_W_whiPAEInrkNhVuh58,3717
 benchmark_apis/synthetic/hartmann.py,sha256=-wcPvr-vaE5qmlV58bInwdHDksrX4KxDuPtwTT10tnE,4583
-mfhpo_benchmark_api-1.0.3.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_benchmark_api-1.0.3.dist-info/METADATA,sha256=F1IRnjH-q0VBcB2cDoGlWF6WC6yeIC8P4VVi0RCAvtU,564
-mfhpo_benchmark_api-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_benchmark_api-1.0.3.dist-info/top_level.txt,sha256=iPvqaBSsSXa6C3RgpKBBQEwUK8Sava3jgYaJJvP159w,129
-mfhpo_benchmark_api-1.0.3.dist-info/RECORD,,
+mfhpo_benchmark_api-1.0.4.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_benchmark_api-1.0.4.dist-info/METADATA,sha256=bptrSiem1BBwWXfDuZpyhJo2fsKsdxhpyy2OgfiSXtA,564
+mfhpo_benchmark_api-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_benchmark_api-1.0.4.dist-info/top_level.txt,sha256=iPvqaBSsSXa6C3RgpKBBQEwUK8Sava3jgYaJJvP159w,129
+mfhpo_benchmark_api-1.0.4.dist-info/RECORD,,
```

