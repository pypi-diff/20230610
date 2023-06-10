# Comparing `tmp/irisml-tasks-fiftyone-0.0.0.tar.gz` & `tmp/irisml-tasks-fiftyone-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/shono/repos/irisml-tasks-fiftyone/dist/tmprryrkwve/irisml-tasks-fiftyone-0.0.0.tar", last modified: Wed Jul  6 19:58:18 2022, max compression
+gzip compressed data, was "irisml-tasks-fiftyone-0.0.1.tar", last modified: Sat Jun 10 02:23:55 2023, max compression
```

## Comparing `irisml-tasks-fiftyone-0.0.0.tar` & `irisml-tasks-fiftyone-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-07-06 19:58:18.289982 irisml-tasks-fiftyone-0.0.0/
--rw-r--r--   0 shono     (1000) shono     (1000)     1030 2022-07-06 19:58:18.289982 irisml-tasks-fiftyone-0.0.0/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)      837 2022-07-06 19:14:03.000000 irisml-tasks-fiftyone-0.0.0/README.md
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-07-06 19:58:18.289982 irisml-tasks-fiftyone-0.0.0/irisml/
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-07-06 19:58:18.289982 irisml-tasks-fiftyone-0.0.0/irisml/tasks/
--rw-r--r--   0 shono     (1000) shono     (1000)     4572 2022-07-06 19:46:50.000000 irisml-tasks-fiftyone-0.0.0/irisml/tasks/launch_fiftyone.py
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-07-06 19:58:18.289982 irisml-tasks-fiftyone-0.0.0/irisml_tasks_fiftyone.egg-info/
--rw-r--r--   0 shono     (1000) shono     (1000)     1030 2022-07-06 19:58:18.000000 irisml-tasks-fiftyone-0.0.0/irisml_tasks_fiftyone.egg-info/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)      319 2022-07-06 19:58:18.000000 irisml-tasks-fiftyone-0.0.0/irisml_tasks_fiftyone.egg-info/SOURCES.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        1 2022-07-06 19:58:18.000000 irisml-tasks-fiftyone-0.0.0/irisml_tasks_fiftyone.egg-info/dependency_links.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       24 2022-07-06 19:58:18.000000 irisml-tasks-fiftyone-0.0.0/irisml_tasks_fiftyone.egg-info/requires.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        7 2022-07-06 19:58:18.000000 irisml-tasks-fiftyone-0.0.0/irisml_tasks_fiftyone.egg-info/top_level.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       81 2022-07-01 21:21:00.000000 irisml-tasks-fiftyone-0.0.0/pyproject.toml
--rw-r--r--   0 shono     (1000) shono     (1000)      438 2022-07-06 19:58:18.289982 irisml-tasks-fiftyone-0.0.0/setup.cfg
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-07-06 19:58:18.289982 irisml-tasks-fiftyone-0.0.0/test/
--rw-r--r--   0 shono     (1000) shono     (1000)     1976 2022-07-01 23:06:10.000000 irisml-tasks-fiftyone-0.0.0/test/test_launch_fiftyone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/irisml/tasks/launch_fiftyone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/test/test_launch_fiftyone.py
```

### Comparing `irisml-tasks-fiftyone-0.0.0/PKG-INFO` & `irisml-tasks-fiftyone-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-fiftyone
-Version: 0.0.0
+Version: 0.0.1
 Summary: IrisML tasks for fiftyone
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # irisml-tasks-fiftyone
 
 IrisML tasks for fiftyone-related integration. Using these tasks, you can view datasets and prediction results on the fiftyone interface.
 
 For the detail of fiftyone, please visit [their repository](https://github.com/voxel51/fiftyone).
 
@@ -24,14 +25,15 @@
 
 ### launch_fiftyone
 
 ```python
 class Inputs:
     dataset: torch.utils.data.Dataset
     predictions: Optional[List]
+    class_names: Optional[List[str]]
 
 class Config:
     task_type: Literal['multiclass_classification', 'multilabel_classification', 'object_detection']
     duration: int
 ```
 
 This task launches a fiftyone app, then sleeps for config.duration seconds. Currently Image Classification and Object Detection tasks are supported.
```

### Comparing `irisml-tasks-fiftyone-0.0.0/README.md` & `irisml-tasks-fiftyone-0.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 ### launch_fiftyone
 
 ```python
 class Inputs:
     dataset: torch.utils.data.Dataset
     predictions: Optional[List]
+    class_names: Optional[List[str]]
 
 class Config:
     task_type: Literal['multiclass_classification', 'multilabel_classification', 'object_detection']
     duration: int
 ```
 
 This task launches a fiftyone app, then sleeps for config.duration seconds. Currently Image Classification and Object Detection tasks are supported.
```

### Comparing `irisml-tasks-fiftyone-0.0.0/irisml/tasks/launch_fiftyone.py` & `irisml-tasks-fiftyone-0.0.1/irisml/tasks/launch_fiftyone.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,57 +16,64 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Task(irisml.core.TaskBase):
     """Launch a fiftyone app.
 
-    This task will wait for the specified time, then returns an output. You can also finish the task by sending a SIGINT signal."""
-    VERSION = '0.1.0'
+    This task will wait for the specified time, then returns an output. You can also finish the task by sending a SIGINT signal.
+
+    Config:
+        task_type (str): The type of the task. One of ``multiclass_classification``, ``multilabel_classification``, or ``object_detection``.
+        duration (int): The duration of the task in seconds.
+    """
+    VERSION = '0.2.0'
     CACHE_ENABLED = False
 
     @dataclasses.dataclass
     class Inputs:
         dataset: torch.utils.data.Dataset
-        predictions: typing.List[torch.Tensor] = None
+        predictions: typing.Optional[typing.List[torch.Tensor]] = None
+        class_names: typing.Optional[typing.List[str]] = None
 
     @dataclasses.dataclass
     class Config:
         task_type: typing.Literal['multiclass_classification', 'multilabel_classification', 'object_detection'] = 'object_detection'
         duration: int = 180
 
     def execute(self, inputs):
         if inputs.predictions:
             if len(inputs.dataset) != len(inputs.predictions):
                 raise RuntimeError(f"The number of samples and prediction results doesn't match: Expected: {len(inputs.dataset)} Actual: {len(inputs.predictions)}.")
 
         with tempfile.TemporaryDirectory() as temp_dir:
-            dataset = Task.convert_to_fiftyone_dataset(inputs.dataset, inputs.predictions, self.config.task_type, pathlib.Path(temp_dir))
+            dataset = Task.convert_to_fiftyone_dataset(inputs.dataset, inputs.predictions, inputs.class_names, self.config.task_type, pathlib.Path(temp_dir))
             session = fiftyone.launch_app(dataset)
             # session.wait()  # This method blocks forever on WSL.
             try:
                 logger.info(f"Sleeping for {self.config.duration} seconds. Press Ctrl-C to finish the task now.")
                 time.sleep(self.config.duration)
             except KeyboardInterrupt:
                 logger.info("Received a SIGINT. Finishing the task.")
             session.close()
 
         return self.Outputs()
 
     @staticmethod
-    def convert_to_fiftyone_dataset(input_dataset, predictions, task_type, directory):
-        label_names = getattr(input_dataset, 'labels', [])
+    def convert_to_fiftyone_dataset(input_dataset, predictions, class_names, task_type, directory):
+        if not class_names:
+            class_names = getattr(input_dataset, 'labels', [])
         dataset = fiftyone.Dataset()
 
         for i, (image, targets) in enumerate(input_dataset):
             image_filepath = directory / f'{i}.jpg'
             image.save(image_filepath)
-            sample = fiftyone.Sample(image_filepath, ground_truth=Task._make_fo_labels(targets, task_type, label_names))
+            sample = fiftyone.Sample(image_filepath, ground_truth=Task._make_fo_labels(targets, task_type, class_names))
             if predictions:
-                sample['prediction'] = Task._make_fo_predictions(predictions[i], task_type, label_names)
+                sample['prediction'] = Task._make_fo_predictions(predictions[i], task_type, class_names)
             dataset.add_sample(sample)
 
         return dataset
 
     @staticmethod
     def _make_fo_labels(targets, task_type, label_names):
         def get_name(class_id: typing.Union[int, float]):
```

### Comparing `irisml-tasks-fiftyone-0.0.0/irisml_tasks_fiftyone.egg-info/PKG-INFO` & `irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-fiftyone
-Version: 0.0.0
+Version: 0.0.1
 Summary: IrisML tasks for fiftyone
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # irisml-tasks-fiftyone
 
 IrisML tasks for fiftyone-related integration. Using these tasks, you can view datasets and prediction results on the fiftyone interface.
 
 For the detail of fiftyone, please visit [their repository](https://github.com/voxel51/fiftyone).
 
@@ -24,14 +25,15 @@
 
 ### launch_fiftyone
 
 ```python
 class Inputs:
     dataset: torch.utils.data.Dataset
     predictions: Optional[List]
+    class_names: Optional[List[str]]
 
 class Config:
     task_type: Literal['multiclass_classification', 'multilabel_classification', 'object_detection']
     duration: int
 ```
 
 This task launches a fiftyone app, then sleeps for config.duration seconds. Currently Image Classification and Object Detection tasks are supported.
```

### Comparing `irisml-tasks-fiftyone-0.0.0/test/test_launch_fiftyone.py` & `irisml-tasks-fiftyone-0.0.1/test/test_launch_fiftyone.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,31 @@
     def test_load_classification_dataset(self):
         fake_dataset = [(PIL.Image.new('RGB', (100, 100)), 1),
                         (PIL.Image.new('RGB', (100, 100)), 2),
                         (PIL.Image.new('RGB', (100, 100)), 3)]
         predictions = [[0, 1, 0, 0], [0, 0, 1, 0], [0, 1, 1, 1]]
 
         with tempfile.TemporaryDirectory() as temp_dir:
-            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, None, 'multiclass_classification', pathlib.Path(temp_dir))
+            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, None, None, 'multiclass_classification', pathlib.Path(temp_dir))
             self._assert_dataset(dataset)
         with tempfile.TemporaryDirectory() as temp_dir:
-            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, predictions, 'multiclass_classification', pathlib.Path(temp_dir))
+            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, predictions, None, 'multiclass_classification', pathlib.Path(temp_dir))
             self._assert_dataset(dataset)
 
     def test_load_detection_dataset(self):
         fake_dataset = [(PIL.Image.new('RGB', (100, 100)), [[0, 0.1, 0.1, 1, 1]]),
                         (PIL.Image.new('RGB', (100, 100)), []),
                         (PIL.Image.new('RGB', (100, 100)), [[0, 0.1, 0.1, 1, 1], [1, 0.2, 0.2, 0.8, 0.8]])]
         predictions = [[[0, 0.5, 0.1, 0.1, 1, 1]],
                        [[0, 0.1, 0.2, 0.2, 0.8, 0.8]],
                        []]
         with tempfile.TemporaryDirectory() as temp_dir:
-            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, None, 'object_detection', pathlib.Path(temp_dir))
+            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, None, None, 'object_detection', pathlib.Path(temp_dir))
             self._assert_dataset(dataset)
         with tempfile.TemporaryDirectory() as temp_dir:
-            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, predictions, 'object_detection', pathlib.Path(temp_dir))
+            dataset = Task.convert_to_fiftyone_dataset(fake_dataset, predictions, None, 'object_detection', pathlib.Path(temp_dir))
             self._assert_dataset(dataset)
 
     def _assert_dataset(self, dataset):
         self.assertEqual(dataset.media_type, 'image')
         for s in dataset:
             self.assertTrue(pathlib.Path(s.filepath).exists())
```

