# Comparing `tmp/mfhpo_benchmark_api-1.0.4-py3-none-any.whl.zip` & `tmp/mfhpo_benchmark_api-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23875 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      663 b- defN 23-Jun-10 12:11 benchmark_apis/__init__.py
+Zip file size: 24096 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx      663 b- defN 23-Jun-10 14:00 benchmark_apis/__init__.py
 -rw-rw-r--  2.0 unx     2294 b- defN 23-Jun-10 12:10 benchmark_apis/abstract_bench.py
 -rw-rw-r--  2.0 unx     4633 b- defN 23-Jun-10 09:49 benchmark_apis/abstract_func.py
--rw-rw-r--  2.0 unx     2492 b- defN 23-Jun-10 11:57 benchmark_apis/abstract_interface.py
--rw-rw-r--  2.0 unx     2981 b- defN 23-Jun-09 14:33 benchmark_apis/discrete_search_spaces.json
--rw-rw-r--  2.0 unx     6075 b- defN 23-Jun-10 09:47 benchmark_apis/hpobench/hpobench.py
--rw-rw-r--  2.0 unx     5817 b- defN 23-Jun-10 09:48 benchmark_apis/hpolib/hpolib.py
--rw-rw-r--  2.0 unx     7561 b- defN 23-Jun-10 11:57 benchmark_apis/jahs/jahs.py
--rw-rw-r--  2.0 unx     8611 b- defN 23-Jun-10 11:58 benchmark_apis/lcbench/lcbench.py
+-rw-rw-r--  2.0 unx     2628 b- defN 23-Jun-10 13:49 benchmark_apis/abstract_interface.py
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-10 13:46 benchmark_apis/discrete_search_spaces.json
+-rw-rw-r--  2.0 unx     6318 b- defN 23-Jun-10 13:53 benchmark_apis/hpobench/hpobench.py
+-rw-rw-r--  2.0 unx     6157 b- defN 23-Jun-10 13:53 benchmark_apis/hpolib/hpolib.py
+-rw-rw-r--  2.0 unx     7631 b- defN 23-Jun-10 13:52 benchmark_apis/jahs/jahs.py
+-rw-rw-r--  2.0 unx     8655 b- defN 23-Jun-10 13:59 benchmark_apis/lcbench/lcbench.py
 -rw-rw-r--  2.0 unx     3717 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/branin.py
 -rw-rw-r--  2.0 unx     4583 b- defN 23-Jun-10 05:21 benchmark_apis/synthetic/hartmann.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx      129 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1436 b- defN 23-Jun-10 12:17 mfhpo_benchmark_api-1.0.4.dist-info/RECORD
-16 files, 62408 bytes uncompressed, 21473 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 14:01 mfhpo_benchmark_api-1.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 14:01 mfhpo_benchmark_api-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 14:01 mfhpo_benchmark_api-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      129 b- defN 23-Jun-10 14:01 mfhpo_benchmark_api-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1436 b- defN 23-Jun-10 14:01 mfhpo_benchmark_api-1.1.0.dist-info/RECORD
+16 files, 63235 bytes uncompressed, 21694 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: benchmark_apis/synthetic/branin.py
 Comment: 
 
 Filename: benchmark_apis/synthetic/hartmann.py
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.4.dist-info/LICENSE
+Filename: mfhpo_benchmark_api-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.4.dist-info/METADATA
+Filename: mfhpo_benchmark_api-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.4.dist-info/WHEEL
+Filename: mfhpo_benchmark_api-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.4.dist-info/top_level.txt
+Filename: mfhpo_benchmark_api-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.0.4.dist-info/RECORD
+Filename: mfhpo_benchmark_api-1.1.0.dist-info/RECORD
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
 
 
-__version__ = "1.0.4"
+__version__ = "1.1.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-benchmark-api/"
```

## benchmark_apis/abstract_interface.py

```diff
@@ -36,24 +36,33 @@
 
 
 RESULT_KEYS = _ResultKeys()
 
 
 class AbstractHPOData(metaclass=ABCMeta):
     _data_url: str
+    _data_dir: str
 
-    def _check_benchdata_availability(self, benchdata_path: str, additional_info: str) -> None:
-        if not os.path.exists(benchdata_path):
-            raise FileNotFoundError(
-                f"Could not find the dataset at {benchdata_path}.\n"
-                f"Download the dataset and place the file at {benchdata_path}.\n"
-                "You can download the dataset via:\n"
-                f"\t$ wget {self._data_url}\n\n"
-                f"{additional_info}"
-            )
+    @property
+    def full_install_instruction(self) -> str:
+        return (
+            f"Could not find the dataset at {self._data_dir}.\n"
+            f"Download the dataset and place the file at {self._data_dir}.\n"
+            "You can download the dataset via:\n"
+            f"{self.install_instruction}"
+        )
+
+    @property
+    @abstractmethod
+    def install_instruction(self) -> str:
+        raise NotImplementedError
+
+    def _check_benchdata_availability(self) -> None:
+        if not os.path.exists(self._data_dir):
+            raise FileNotFoundError(self.full_install_instruction)
 
 
 class AbstractInterface(metaclass=ABCMeta):
     _BENCH_TYPE: ClassVar[str]
 
     def __init__(self, seed: int | None):
         self._rng = np.random.RandomState(seed)
```

## benchmark_apis/discrete_search_spaces.json

### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'jahs'": "OrderedDict([('Activation', ['ReLU', 'Hardswish', 'Mish']), ('TrivialAugment', [True, "*

 * *           "False]), ('N', [1, 3, 5]), ('W', [4, 8, 16]), ('Op1', ['0', '1', '2', '3', '4']), "*

 * *           "('Op2', ['0', '1', '2', '3', '4']), ('Op3', ['0', '1', '2', '3', '4']), ('Op4', ['0', "*

 * *           "'1', '2', '3', '4']), ('Op5', ['0', '1', '2', '3', '4']), ('Op6', ['0', '1', '2', '3', "*

 * *           "'4'])])",*

 * * 'delete': "['jahs-bench']"}*

```diff
@@ -104,15 +104,15 @@
             32,
             64,
             128,
             256,
             512
         ]
     },
-    "jahs-bench": {
+    "jahs": {
         "Activation": [
             "ReLU",
             "Hardswish",
             "Mish"
         ],
         "N": [
             1,
```

## benchmark_apis/hpobench/hpobench.py

```diff
@@ -20,35 +20,44 @@
     precision: str = "precision"
     f1: str = "f1"
 
 
 _TARGET_KEYS = _TargetMetricKeys()
 _FIDEL_KEY = "epoch"
 _KEY_ORDER = ["alpha", "batch_size", "depth", "learning_rate_init", "width"]
+_DATA_DIR = os.path.join(DATA_DIR_NAME, "hpobench")
 
 
 class RowDataType(TypedDict):
     loss: list[dict[int, float]]
     runtime: list[dict[int, float]]
     precision: list[dict[int, float]]
     f1: list[dict[int, float]]
 
 
 class HPOBenchDatabase(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
     _data_url = "https://ndownloader.figshare.com/files/30379005/"
+    _data_dir = _DATA_DIR
 
     def __init__(self, dataset_name: str):
-        benchdata_path = os.path.join(DATA_DIR_NAME, "hpobench", f"{dataset_name}.pkl")
-        additional_info = (
-            "\t$ unzip nn.zip\n\n" "Then extract the pkl file using https://github.com/nabenabe0928/hpolib-extractor/."
+        self._benchdata_path = os.path.join(self._data_dir, f"{dataset_name}.pkl")
+        self._check_benchdata_availability()
+        self._db = pickle.load(open(self._benchdata_path, "rb"))
+
+    @property
+    def install_instruction(self) -> str:
+        return (
+            f"\t$ cd {self._data_dir}\n"
+            f"\t$ wget {self._data_url}\n"
+            "\t$ unzip nn.zip\n\n"
+            "Then extract the pkl file using https://github.com/nabenabe0928/hpolib-extractor/.\n"
+            f"You should get `{self._benchdata_path}` in the end."
         )
-        self._check_benchdata_availability(benchdata_path, additional_info=additional_info)
-        self._db = pickle.load(open(benchdata_path, "rb"))
 
     def __getitem__(self, key: str) -> RowDataType:
         return self._db[key]
 
 
 class HPOBench(AbstractBench):
     """The class for HPOlib.
```

## benchmark_apis/hpolib/hpolib.py

```diff
@@ -29,35 +29,45 @@
     "dropout_1",
     "dropout_2",
     "init_lr",
     "lr_schedule",
     "n_units_1",
     "n_units_2",
 ]
+_DATA_DIR = os.path.join(DATA_DIR_NAME, "hpolib")
 
 
 class RowDataType(TypedDict):
     valid_mse: list[dict[int, float]]
     runtime: list[float]
     n_params: int
 
 
 class HPOLibDatabase(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
     _data_url = "http://ml4aad.org/wp-content/uploads/2019/01/fcnet_tabular_benchmarks.tar.gz"
+    _data_dir = _DATA_DIR
 
     def __init__(self, dataset_name: str):
-        benchdata_path = os.path.join(DATA_DIR_NAME, "hpolib", f"{dataset_name}.pkl")
-        additional_info = (
-            "\t$ tar xf fcnet_tabular_benchmarks.tar.gz\n\n"
-            "Then extract the pkl file using https://github.com/nabenabe0928/hpolib-extractor/."
+        self._benchdata_path = os.path.join(self._data_dir, f"{dataset_name}.pkl")
+        self._check_benchdata_availability()
+        self._db = pickle.load(open(self._benchdata_path, "rb"))
+
+    @property
+    def install_instruction(self) -> str:
+        return (
+            f"\t$ cd {self._data_dir}\n"
+            f"\t$ wget {self._data_url}\n"
+            "\t$ tar xf fcnet_tabular_benchmarks.tar.gz\n"
+            "\t$ mv fcnet_tabular_benchmarks/*.hdf5 .\n"
+            "\t$ rm -r fcnet_tabular_benchmarks/\n\n"
+            "Then extract the pkl file using https://github.com/nabenabe0928/hpolib-extractor/.\n"
+            f"You should get `{self._benchdata_path}` in the end."
         )
-        self._check_benchdata_availability(benchdata_path, additional_info=additional_info)
-        self._db = pickle.load(open(benchdata_path, "rb"))
 
     def __getitem__(self, key: str) -> RowDataType:
         return self._db[key]
 
 
 class HPOLib(AbstractBench):
     """The class for HPOlib.
```

## benchmark_apis/jahs/jahs.py

```diff
@@ -26,30 +26,39 @@
 class _FidelKeys:
     epoch: str = "epoch"
     resol: str = "Resolution"
 
 
 _FIDEL_KEYS = _FidelKeys()
 _TARGET_KEYS = _TargetMetricKeys()
+_DATA_DIR = os.path.join(DATA_DIR_NAME, "jahs")
 
 
 class JAHSBenchSurrogate(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
     _data_url = (
         "https://ml.informatik.uni-freiburg.de/research-artifacts/jahs_bench_201/v1.1.0/assembled_surrogates.tar"
     )
+    _data_dir = _DATA_DIR
 
-    def __init__(self, data_dir: str, dataset_name: str, target_metrics: list[str]):
-        additional_info = f"Then untar the file in {data_dir}."
-        self._check_benchdata_availability(data_dir, additional_info=additional_info)
+    def __init__(self, dataset_name: str, target_metrics: list[str]):
+        self._check_benchdata_availability()
         self._target_metrics = target_metrics[:]
         _metrics = [getattr(_TARGET_KEYS, tm) for tm in self._target_metrics]
         metrics = list(set(_metrics + [_TARGET_KEYS.runtime]))
-        self._surrogate = jahs_bench.Benchmark(task=dataset_name, download=False, save_dir=data_dir, metrics=metrics)
+        self._surrogate = jahs_bench.Benchmark(task=dataset_name, download=False, save_dir=_DATA_DIR, metrics=metrics)
+
+    @property
+    def install_instruction(self) -> str:
+        return (
+            f"$ cd {self._data_dir}\n"
+            f"$ wget {self._data_url}\n\n"
+            f"Then untar `assembled_surrogates.tar` in {self._data_dir}."
+        )
 
     def __call__(self, eval_config: dict[str, int | float | str | bool], fidels: dict[str, int | float]) -> ResultType:
         _fidels = fidels.copy()
         nepochs = _fidels.pop(_FIDEL_KEYS.epoch)
 
         eval_config.update({"Optimizer": "SGD", **_fidels})  # type: ignore
         eval_config = {k: int(v) if k[:-1] == "Op" else v for k, v in eval_config.items()}
@@ -110,16 +119,15 @@
         min_epoch: int = 22,
         max_epoch: int = 200,
         min_resol: float = 0.1,
         max_resol: float = 1.0,
         keep_benchdata: bool = True,
     ):
         self.dataset_name = ["cifar10", "fashion_mnist", "colorectal_histology"][dataset_id]
-        self._data_dir = os.path.join(DATA_DIR_NAME, "jahs_bench_data")
-        self._value_range = VALUE_RANGES["jahs-bench"]
+        self._value_range = VALUE_RANGES["jahs"]
         self._target_metrics = target_metrics[:]
         self._min_epoch, self._max_epoch = min_epoch, max_epoch
         self._min_resol, self._max_resol = min_resol, max_resol
         self._surrogate = self.get_benchdata() if keep_benchdata else None
 
         self._validate_target_metrics()
         self._validate_epochs()
@@ -129,17 +137,15 @@
         min_resol, max_resol = self._min_resol, self._max_resol
         if min_resol <= 0 or max_resol > 1.0:
             raise ValueError(f"Resolution must be in [0.0, 1.0], but got {min_resol=} and {max_resol=}")
         if min_resol >= max_resol:
             raise ValueError(f"min_resol < max_resol must hold, but got {min_resol=} and {max_resol=}")
 
     def get_benchdata(self) -> JAHSBenchSurrogate:
-        return JAHSBenchSurrogate(
-            data_dir=self._data_dir, dataset_name=self.dataset_name, target_metrics=self._target_metrics
-        )
+        return JAHSBenchSurrogate(dataset_name=self.dataset_name, target_metrics=self._target_metrics)
 
     def __call__(  # type: ignore[override]
         self,
         eval_config: dict[str, int | float | str | bool],
         *,
         fidels: dict[str, int | float] = {},
         seed: int | None = None,
```

## benchmark_apis/lcbench/lcbench.py

```diff
@@ -19,32 +19,39 @@
 class _TargetMetricKeys:
     loss: str = "val_balanced_accuracy"
     runtime: str = "time"
 
 
 _TARGET_KEYS = _TargetMetricKeys()
 _FIDEL_KEY = "epoch"
+_DATA_DIR = os.path.join(DATA_DIR_NAME, "lcbench")
 
 
 class LCBenchSurrogate(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
     _data_url = "https://syncandshare.lrz.de/getlink/fiCMkzqj1bv1LfCUyvZKmLvd/"
+    _data_dir = _DATA_DIR
 
     def __init__(self, dataset_id: str, target_metrics: list[str]):
-        benchdata_path = os.path.join(DATA_DIR_NAME, "lcbench")
-        additional_info = f"Then unzip the file in {DATA_DIR_NAME}."
-        self._check_benchdata_availability(benchdata_path, additional_info=additional_info)
+        self._check_benchdata_availability()
         self._dataset_id = dataset_id
         self._target_metrics = target_metrics[:]
         # active_session=False is necessary for parallel computing.
         self._surrogate = benchmark_set.BenchmarkSet("lcbench", instance=dataset_id, active_session=False)
 
-    def _check_benchdata_availability(self, benchdata_path: str, additional_info: str) -> None:
-        super()._check_benchdata_availability(benchdata_path=benchdata_path, additional_info=additional_info)
+    @property
+    def install_instruction(self) -> str:
+        return (
+            f"\tAccess to {self._data_url} and download `lcbench.zip` from the website.\n\n"
+            f"After that, please unzip `lcbench.zip` in {self._data_dir}."
+        )
+
+    def _check_benchdata_availability(self) -> None:
+        super()._check_benchdata_availability()
         local_config.init_config()
         local_config.set_data_path(DATA_DIR_NAME)
 
     def __call__(self, eval_config: dict[str, int | float], fidel: int) -> ResultType:
         _eval_config: dict[str, int | float | str] = eval_config.copy()  # type: ignore
         _eval_config["OpenML_task_id"] = self._dataset_id
         _eval_config[_FIDEL_KEY] = fidel
```

## Comparing `mfhpo_benchmark_api-1.0.4.dist-info/LICENSE` & `mfhpo_benchmark_api-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_benchmark_api-1.0.4.dist-info/METADATA` & `mfhpo_benchmark_api-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfhpo-benchmark-api
-Version: 1.0.4
+Version: 1.1.0
 Home-page: https://github.com/nabenabe0928/mfhpo-benchmark-api
 Author: nabenabe0928
 Author-email: shuhei.watanabe.utokyo@gmail.com
 Platform: Linux
 Platform: Darwin
 Requires-Python: >=3.8
 License-File: LICENSE
```

## Comparing `mfhpo_benchmark_api-1.0.4.dist-info/RECORD` & `mfhpo_benchmark_api-1.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-benchmark_apis/__init__.py,sha256=NsQBdArefiTKodTt2LptICOOgu4iUCtwTAwqEZjtRmk,663
+benchmark_apis/__init__.py,sha256=wUgR2afDcIktbROzYVWKRSKrcSCSZpk2T3rOP860nqY,663
 benchmark_apis/abstract_bench.py,sha256=9kNF_E1jO8z1fA4EHQT1yufsAJ9e5MbgHtQSLQQXkjQ,2294
 benchmark_apis/abstract_func.py,sha256=x5qIi-g9EwKR37-TRGmudqeaRXF6vheGx1hfvhvnX3Y,4633
-benchmark_apis/abstract_interface.py,sha256=A9WPFCgxW3eij7g1j-6TnWVysBxsHspQLb-B9Tg8_Xg,2492
-benchmark_apis/discrete_search_spaces.json,sha256=w8J23jbT3u5qdQUba8MCe8cQ69ZVeSc1oy6mDaSzLXY,2981
-benchmark_apis/hpobench/hpobench.py,sha256=m8BMQEsDVgKKQYh1WSQIT63xNbJ9rjx8_bgSAdwWzQs,6075
-benchmark_apis/hpolib/hpolib.py,sha256=ATD6ZO1cOxQo66MmvfydvSQznYZFAlhgO1fLpz6wISQ,5817
-benchmark_apis/jahs/jahs.py,sha256=oAYt1cjV5VtVzx-OT8E5UGjyhLkpJQPJ6BrVq1nPkoQ,7561
-benchmark_apis/lcbench/lcbench.py,sha256=13K5vbgK_-KguOxtEv77j4uM7GAqVMD2de3LbbrpD08,8611
+benchmark_apis/abstract_interface.py,sha256=pkJDlCE8GMbhlG36vubE88YW2-spy0YrlbHKLvLcFhI,2628
+benchmark_apis/discrete_search_spaces.json,sha256=S8gLxrA_vweXVuPHU-TNfq8C4GrLSQQsxgeMdxEjz58,2975
+benchmark_apis/hpobench/hpobench.py,sha256=-EK5g0ZZ3cEX6X9VYdlZK4mh_SAN7JANO24XodYzo1c,6318
+benchmark_apis/hpolib/hpolib.py,sha256=zXT7DHbdra8gqyXQwo7el3-y2fTLBKr63LTfe_rZb0o,6157
+benchmark_apis/jahs/jahs.py,sha256=zE7g-196tixDr8w_jbqfNqG4qmtco73JKwEm1ItIXas,7631
+benchmark_apis/lcbench/lcbench.py,sha256=pJDUzIefx5aMBXFADeefgygjD128uDYe7jLWEEIG4WY,8655
 benchmark_apis/synthetic/branin.py,sha256=HZC4Yq4KOmb91pSKAJCosAL_W_whiPAEInrkNhVuh58,3717
 benchmark_apis/synthetic/hartmann.py,sha256=-wcPvr-vaE5qmlV58bInwdHDksrX4KxDuPtwTT10tnE,4583
-mfhpo_benchmark_api-1.0.4.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_benchmark_api-1.0.4.dist-info/METADATA,sha256=bptrSiem1BBwWXfDuZpyhJo2fsKsdxhpyy2OgfiSXtA,564
-mfhpo_benchmark_api-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_benchmark_api-1.0.4.dist-info/top_level.txt,sha256=iPvqaBSsSXa6C3RgpKBBQEwUK8Sava3jgYaJJvP159w,129
-mfhpo_benchmark_api-1.0.4.dist-info/RECORD,,
+mfhpo_benchmark_api-1.1.0.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_benchmark_api-1.1.0.dist-info/METADATA,sha256=gf8pHmOICMEs3GGqv14w2rLPf8s2UniDmc7JvNty39w,564
+mfhpo_benchmark_api-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_benchmark_api-1.1.0.dist-info/top_level.txt,sha256=iPvqaBSsSXa6C3RgpKBBQEwUK8Sava3jgYaJJvP159w,129
+mfhpo_benchmark_api-1.1.0.dist-info/RECORD,,
```

