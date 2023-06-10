# Comparing `tmp/KapoorLabs-Lightning-5.1.1.tar.gz` & `tmp/KapoorLabs-Lightning-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-rorsfp6o/KapoorLabs-Lightning-5.1.1.tar", last modified: Fri Jun  9 17:47:25 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-58jgomt_/KapoorLabs-Lightning-5.2.0.tar", last modified: Sat Jun 10 14:13:24 2023, max compression
```

## Comparing `KapoorLabs-Lightning-5.1.1.tar` & `KapoorLabs-Lightning-5.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:25.437089 KapoorLabs-Lightning-5.1.1/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.473457 KapoorLabs-Lightning-5.1.1/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.631779 KapoorLabs-Lightning-5.1.1/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.1.1/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/.gitignore
--rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.1.1/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-09 17:47:25.438096 KapoorLabs-Lightning-5.1.1/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.796703 KapoorLabs-Lightning-5.1.1/licenses/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/Apache-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/BSD-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/GPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/LGPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/MIT
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/MPL-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-09 17:47:25.443458 KapoorLabs-Lightning-5.1.1/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.490638 KapoorLabs-Lightning-5.1.1/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.945895 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-09 17:47:24.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:25.334430 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/__init__.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:25.410187 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/caped.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/graph_functions.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/kapoorlabs.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)    34543 2023-06-09 17:46:49.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/lightning_trainer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/optimizers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_datasets.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_loggers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_losses.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_transforms.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/schedulers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:24.519758 KapoorLabs-Lightning-5.2.0/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:23.310536 KapoorLabs-Lightning-5.2.0/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:23.468436 KapoorLabs-Lightning-5.2.0/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.2.0/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.0/.gitignore
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.2.0/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.0/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.0/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-10 14:13:24.521755 KapoorLabs-Lightning-5.2.0/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.0/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:23.647959 KapoorLabs-Lightning-5.2.0/licenses/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.0/licenses/Apache-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.0/licenses/BSD-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.0/licenses/GPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.0/licenses/LGPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.0/licenses/MIT
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.0/licenses/MPL-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.0/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-10 14:13:24.532420 KapoorLabs-Lightning-5.2.0/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:23.327025 KapoorLabs-Lightning-5.2.0/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:23.812581 KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-10 14:13:22.000000 KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-10 14:13:23.000000 KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-10 14:13:22.000000 KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-10 14:13:22.000000 KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-10 14:13:22.000000 KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-10 14:13:22.000000 KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:24.357242 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-10 14:13:24.470141 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-10 14:13:22.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/caped.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/graph_functions.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    34560 2023-06-10 14:12:48.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/lightning_trainer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/optimizers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_datasets.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_loggers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_losses.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_transforms.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/schedulers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.0/tox.ini
```

### Comparing `KapoorLabs-Lightning-5.1.1/.github/workflows/test_and_deploy.yml` & `KapoorLabs-Lightning-5.2.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/.gitignore` & `KapoorLabs-Lightning-5.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/.pre-commit-config.yaml` & `KapoorLabs-Lightning-5.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/LICENSE` & `KapoorLabs-Lightning-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/PKG-INFO` & `KapoorLabs-Lightning-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.1.1
+Version: 5.2.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.1.1/README.md` & `KapoorLabs-Lightning-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/licenses/Apache-2` & `KapoorLabs-Lightning-5.2.0/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/licenses/BSD-3` & `KapoorLabs-Lightning-5.2.0/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/licenses/GPL-3` & `KapoorLabs-Lightning-5.2.0/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/licenses/LGPL-3` & `KapoorLabs-Lightning-5.2.0/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/licenses/MIT` & `KapoorLabs-Lightning-5.2.0/licenses/MIT`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/licenses/MPL-2` & `KapoorLabs-Lightning-5.2.0/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/setup.cfg` & `KapoorLabs-Lightning-5.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.1.1
+Version: 5.2.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `KapoorLabs-Lightning-5.2.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/__init__.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/graph_functions.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/lightning_trainer.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         optim_func: optim,
         train_dataloaders_inf,
         cluster_distribution,
         accelerator,
         devices,
         scheduler: schedulers = None,
         gamma: int = 1,
-        update_interval: int = 5,
+        update_interval: int = 1,
         divergence_tolerance: float = 1e-2,
         mem_percent: int = 40,
         q_power: int = 2,
         n_init: int = 20,
     ):
         super().__init__()
         self.save_hyperparameters(
@@ -339,14 +339,15 @@
                 "cluster_loss_func",
                 "train_dataloaders_inf",
                 "optim_func",
                 "scheduler",
             ]
         )
 
+        # params
         self.network = network
         self.loss_func = loss_func
         self.cluster_loss_func = cluster_loss_func
         self.optim_func = optim_func
         self.scheduler = scheduler
         self.accelerator = accelerator
         self.devices = devices
```

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/optimizers.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_datasets.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_loggers.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_losses.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_models.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_transforms.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/schedulers.py` & `KapoorLabs-Lightning-5.2.0/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.1/tox.ini` & `KapoorLabs-Lightning-5.2.0/tox.ini`

 * *Files identical despite different names*

