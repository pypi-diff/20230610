# Comparing `tmp/counterplots-0.0.4.tar.gz` & `tmp/counterplots-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "counterplots-0.0.4.tar", last modified: Sat Jun 10 20:15:21 2023, max compression
+gzip compressed data, was "counterplots-0.0.5.tar", last modified: Sat Jun 10 20:24:10 2023, max compression
```

## Comparing `counterplots-0.0.4.tar` & `counterplots-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:15:21.324859 counterplots-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-10 20:14:45.000000 counterplots-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-10 20:15:21.324859 counterplots-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-10 20:14:45.000000 counterplots-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:15:21.320859 counterplots-0.0.4/counterplots/
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-10 20:14:45.000000 counterplots-0.0.4/counterplots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:15:21.324859 counterplots-0.0.4/counterplots/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:14:45.000000 counterplots-0.0.4/counterplots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-10 20:14:45.000000 counterplots-0.0.4/counterplots/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-10 20:14:45.000000 counterplots-0.0.4/counterplots/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-10 20:14:45.000000 counterplots-0.0.4/counterplots/utils/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:15:21.320859 counterplots-0.0.4/counterplots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-10 20:15:21.000000 counterplots-0.0.4/counterplots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-10 20:15:21.000000 counterplots-0.0.4/counterplots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:15:21.000000 counterplots-0.0.4/counterplots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-10 20:15:21.000000 counterplots-0.0.4/counterplots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 20:15:21.000000 counterplots-0.0.4/counterplots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:15:21.324859 counterplots-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-10 20:14:45.000000 counterplots-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:15:21.324859 counterplots-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:14:45.000000 counterplots-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-10 20:14:45.000000 counterplots-0.0.4/tests/test____init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:15:21.324859 counterplots-0.0.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:14:45.000000 counterplots-0.0.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-10 20:14:45.000000 counterplots-0.0.4/tests/utils/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-10 20:14:45.000000 counterplots-0.0.4/tests/utils/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-10 20:14:45.000000 counterplots-0.0.4/tests/utils/test_verification.py
+drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 20:24:10.623233 counterplots-0.0.5/
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     1067 2023-06-10 15:01:31.000000 counterplots-0.0.5/LICENSE.txt
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     5712 2023-06-10 20:24:10.623233 counterplots-0.0.5/PKG-INFO
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     5230 2023-06-10 19:13:31.000000 counterplots-0.0.5/README.md
+drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 20:24:10.619233 counterplots-0.0.5/counterplots/
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     7742 2023-06-08 13:25:54.000000 counterplots-0.0.5/counterplots/__init__.py
+drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 20:24:10.623233 counterplots-0.0.5/counterplots/utils/
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-08 12:29:34.000000 counterplots-0.0.5/counterplots/utils/__init__.py
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)    10947 2023-06-10 12:25:27.000000 counterplots-0.0.5/counterplots/utils/plots.py
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     8868 2023-06-10 12:25:34.000000 counterplots-0.0.5/counterplots/utils/process.py
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     1631 2023-06-10 12:25:46.000000 counterplots-0.0.5/counterplots/utils/verification.py
+drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 20:24:10.619233 counterplots-0.0.5/counterplots.egg-info/
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     5712 2023-06-10 20:24:10.000000 counterplots-0.0.5/counterplots.egg-info/PKG-INFO
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)      511 2023-06-10 20:24:10.000000 counterplots-0.0.5/counterplots.egg-info/SOURCES.txt
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)        1 2023-06-10 20:24:10.000000 counterplots-0.0.5/counterplots.egg-info/dependency_links.txt
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)       17 2023-06-10 20:24:10.000000 counterplots-0.0.5/counterplots.egg-info/requires.txt
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)       19 2023-06-10 20:24:10.000000 counterplots-0.0.5/counterplots.egg-info/top_level.txt
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)       38 2023-06-10 20:24:10.623233 counterplots-0.0.5/setup.cfg
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)      940 2023-06-10 20:21:09.000000 counterplots-0.0.5/setup.py
+drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 20:24:10.623233 counterplots-0.0.5/tests/
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-08 11:50:57.000000 counterplots-0.0.5/tests/__init__.py
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     4530 2023-06-10 12:29:17.000000 counterplots-0.0.5/tests/test____init__.py
+drwxrwxr-x   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-10 20:24:10.623233 counterplots-0.0.5/tests/utils/
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)        0 2023-06-08 12:24:10.000000 counterplots-0.0.5/tests/utils/__init__.py
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     3095 2023-06-10 12:40:22.000000 counterplots-0.0.5/tests/utils/test_plots.py
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     5550 2023-06-10 12:29:50.000000 counterplots-0.0.5/tests/utils/test_process.py
+-rw-rw-r--   0 rmazzine  (1000) rmazzine  (1000)     2868 2023-06-10 12:30:25.000000 counterplots-0.0.5/tests/utils/test_verification.py
```

### Comparing `counterplots-0.0.4/LICENSE.txt` & `counterplots-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/PKG-INFO` & `counterplots-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,172 +1,173 @@
 Metadata-Version: 2.1
 Name: counterplots
-Version: 0.0.4
+Version: 0.0.5
 Summary: Plotting tool for counterfactual explanations
 Home-page: https://github.com/ADMAntwerp/CounterPlots
+Download-URL: https://pypi.org/project/counterplots/
 Author: Raphael Mazzine Barbosa de Oliveira, Bjorge Meulemeester
 License: MIT
-Download-URL: https://pypi.org/project/counterplots/
-Description: <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_logo.svg"><br>
-        
-        --------------------------------------
-        
-        CounterPlots: Plotting tool for counterfactuals
-        =======================================
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![example workflow](https://github.com/ADMAntwerp/CounterPlots/actions/workflows/deployment.yml/badge.svg)](https://github.com/ADMAntwerp/CounterPlots/actions)
-        [![Code Coverage](https://codecov.io/gh/rmazzine/counterplotcoverage/branch/main/graph/badge.svg?token=TQYJSGEMP1)](https://codecov.io/gh/rmazzine/counterplotcoverage)
-        [![Known Vulnerabilities](https://snyk.io/test/github/ADMAntwerp/CounterPlots/badge.svg)](https://snyk.io/test/github/ADMAntwerp/CounterPlots)
-        
-        Counterplots is a Python package that allows you to plot counterfactuals with easy integration with any counterfactual generation algorithm.
-        
-        ## Plot examples
-        
-        ### Greedy Plot
-        
-        The greedy plot shows the greediest (feature change with the highest impact towards the opposite class) path from the factual instance until it reaches the counterfactual.
-        
-        <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_greedy.png">
-        
-        ### CounterShapley Plot
-        
-        This chart shows each counterfactual feature change contribution to the counterfactual prediction. It uses Shapley values to calculate the contribution of each feature change.
-        
-        <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_countershapley.png">
-        
-        ### Constellation Plot
-        
-        This chart shows the prediction score change for all possible feature change combinations.
-        
-        <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_constellation.png">
-        
-        ## Installation
-        With pip:
-        ```bash
-        pip install counterplots
-        ```
-        
-        ## Usage
-        To use CounterPlots, you just need the machine learning model predictor, and the factual and counterfactual points.
-        The example below uses a simple mock model:
-        ```python
-        from counterplots import CreatePlot
-        import numpy as np
-        
-        # Simple mock model for the predict_proba function which returns a probability for each input instance
-        def mock_predict_proba(data):
-            out = []
-            for x in data:
-                if list(x) == [0.0, 0.0, 0.0]:
-                    out.append(0.0)
-                elif list(x) == [1.0, 0.0, 0.0]:
-                    out.append(0.44)
-                elif list(x) == [0.0, 1.0, 0.0]:
-                    out.append(0.4)
-                elif list(x) == [0.0, 0.0, 1.0]:
-                    out.append(0.2)
-                elif list(x) == [1.0, 1.0, 0.0]:
-                    out.append(0.3)
-                elif list(x) == [0.0, 1.0, 1.0]:
-                    out.append(0.25)
-                elif list(x) == [1.0, 0.0, 1.0]:
-                    out.append(0.4)
-                elif list(x) == [1.0, 1.0, 1.0]:
-                    out.append(1.0)
-            return np.array(out)
-        
-        # Factual Instance
-        factual = np.array([0, 0, 0])
-        # Counterfactual Instance
-        cf = np.array([1, 1, 1])
-        
-        # Create the plot object
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            mock_predict_proba)
-        
-        # Create the greedy plot
-        cf_plots.greedy('greedy_plot.png')
-        # Create the countershapley plot
-        cf_plots.countershapley('countershapley_plot.png')
-        # Create the constellation plot
-        cf_plots.constellation('constellation_plot.png')
-        
-        # Print the countershapley values
-        print(cf_plots.countershapley_values())
-        ```
-        
-        In case you want to add custom names to the features, use the optional argument `feature_names`:
-        ```python
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            mock_predict_proba,
-            feature_names=['feature1', 'feature2', 'feature3'])
-        ```
-        
-        In case you want to add custom labels to the factual and counterfactual points, use the optional argument `class_names`:
-        ```python
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            mock_predict_proba,
-            class_names=['Factual', 'Counterfactual'])
-        ```
-        
-        ## Using with Scikit-Learn
-        
-        CounterPlots can be used with any machine learning model that has a `predict_proba` function. For example, with Scikit-Learn:
-        <details>
-        
-        ```python
-        import numpy as np
-        from sklearn.ensemble import RandomForestClassifier
-        from sklearn.datasets import load_iris
-        
-        from counterplots import CreatePlot
-        
-        iris = load_iris()
-        
-        X = iris.data
-        y = [0 if l == 0 else 1 for l in iris.target] # Makes it a binary classification problem
-        
-        clf = RandomForestClassifier(max_depth=2, random_state=0)
-        clf.fit(X, y)
-        
-        preds = clf.predict(X)
-        
-        # For the factual point, takes an instance with 0 classification
-        factual = X[np.argwhere(preds == 0)[0]][0]
-        # For the counterfactual point, takes an instance with 1 classification
-        cf = X[np.argwhere(preds == 1)[0]][0]
-        
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            clf.predict_proba,
-            feature_names=iris.feature_names,
-            class_names={0: 'Setosa', 1: 'Non-Setosa'}
-        )
-        
-        
-        # Create the greedy plot
-        cf_plots.greedy('iris_greedy_plot.png')
-        # Create the countershapley plot
-        cf_plots.countershapley('iris_countershapley_plot.png')
-        # Create the constellation plot
-        cf_plots.constellation('iris_constellation_plot.png')
-        
-        # Print the countershapley values
-        print(cf_plots.countershapley_values())
-        ```
-        </details>
-        
-        ## Citation
-        If you use CounterPlots in your research, please cite the following paper:
-        ```bibtex
-        ```
 Keywords: Counterfactual Explanations,Visualization,Plotting,Explainable Artificial Intelligence,XAI,Machine Learning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_logo.svg"><br>
+
+--------------------------------------
+
+CounterPlots: Plotting tool for counterfactuals
+=======================================
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![example workflow](https://github.com/ADMAntwerp/CounterPlots/actions/workflows/deployment.yml/badge.svg)](https://github.com/ADMAntwerp/CounterPlots/actions)
+[![Code Coverage](https://codecov.io/gh/rmazzine/counterplotcoverage/branch/main/graph/badge.svg?token=TQYJSGEMP1)](https://codecov.io/gh/rmazzine/counterplotcoverage)
+[![Known Vulnerabilities](https://snyk.io/test/github/ADMAntwerp/CounterPlots/badge.svg)](https://snyk.io/test/github/ADMAntwerp/CounterPlots)
+
+Counterplots is a Python package that allows you to plot counterfactuals with easy integration with any counterfactual generation algorithm.
+
+## Plot examples
+
+### Greedy Plot
+
+The greedy plot shows the greediest (feature change with the highest impact towards the opposite class) path from the factual instance until it reaches the counterfactual.
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_greedy.png">
+
+### CounterShapley Plot
+
+This chart shows each counterfactual feature change contribution to the counterfactual prediction. It uses Shapley values to calculate the contribution of each feature change.
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_countershapley.png">
+
+### Constellation Plot
+
+This chart shows the prediction score change for all possible feature change combinations.
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_constellation.png">
+
+## Installation
+With pip:
+```bash
+pip install counterplots
+```
+
+## Usage
+To use CounterPlots, you just need the machine learning model predictor, and the factual and counterfactual points.
+The example below uses a simple mock model:
+```python
+from counterplots import CreatePlot
+import numpy as np
+
+# Simple mock model for the predict_proba function which returns a probability for each input instance
+def mock_predict_proba(data):
+    out = []
+    for x in data:
+        if list(x) == [0.0, 0.0, 0.0]:
+            out.append(0.0)
+        elif list(x) == [1.0, 0.0, 0.0]:
+            out.append(0.44)
+        elif list(x) == [0.0, 1.0, 0.0]:
+            out.append(0.4)
+        elif list(x) == [0.0, 0.0, 1.0]:
+            out.append(0.2)
+        elif list(x) == [1.0, 1.0, 0.0]:
+            out.append(0.3)
+        elif list(x) == [0.0, 1.0, 1.0]:
+            out.append(0.25)
+        elif list(x) == [1.0, 0.0, 1.0]:
+            out.append(0.4)
+        elif list(x) == [1.0, 1.0, 1.0]:
+            out.append(1.0)
+    return np.array(out)
+
+# Factual Instance
+factual = np.array([0, 0, 0])
+# Counterfactual Instance
+cf = np.array([1, 1, 1])
+
+# Create the plot object
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    mock_predict_proba)
+
+# Create the greedy plot
+cf_plots.greedy('greedy_plot.png')
+# Create the countershapley plot
+cf_plots.countershapley('countershapley_plot.png')
+# Create the constellation plot
+cf_plots.constellation('constellation_plot.png')
+
+# Print the countershapley values
+print(cf_plots.countershapley_values())
+```
+
+In case you want to add custom names to the features, use the optional argument `feature_names`:
+```python
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    mock_predict_proba,
+    feature_names=['feature1', 'feature2', 'feature3'])
+```
+
+In case you want to add custom labels to the factual and counterfactual points, use the optional argument `class_names`:
+```python
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    mock_predict_proba,
+    class_names=['Factual', 'Counterfactual'])
+```
+
+## Using with Scikit-Learn
+
+CounterPlots can be used with any machine learning model that has a `predict_proba` function. For example, with Scikit-Learn:
+<details>
+
+```python
+import numpy as np
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.datasets import load_iris
+
+from counterplots import CreatePlot
+
+iris = load_iris()
+
+X = iris.data
+y = [0 if l == 0 else 1 for l in iris.target] # Makes it a binary classification problem
+
+clf = RandomForestClassifier(max_depth=2, random_state=0)
+clf.fit(X, y)
+
+preds = clf.predict(X)
+
+# For the factual point, takes an instance with 0 classification
+factual = X[np.argwhere(preds == 0)[0]][0]
+# For the counterfactual point, takes an instance with 1 classification
+cf = X[np.argwhere(preds == 1)[0]][0]
+
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    clf.predict_proba,
+    feature_names=iris.feature_names,
+    class_names={0: 'Setosa', 1: 'Non-Setosa'}
+)
+
+
+# Create the greedy plot
+cf_plots.greedy('iris_greedy_plot.png')
+# Create the countershapley plot
+cf_plots.countershapley('iris_countershapley_plot.png')
+# Create the constellation plot
+cf_plots.constellation('iris_constellation_plot.png')
+
+# Print the countershapley values
+print(cf_plots.countershapley_values())
+```
+</details>
+
+## Citation
+If you use CounterPlots in your research, please cite the following paper:
+```bibtex
+```
```

### Comparing `counterplots-0.0.4/README.md` & `counterplots-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/counterplots/__init__.py` & `counterplots-0.0.5/counterplots/__init__.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/counterplots/utils/plots.py` & `counterplots-0.0.5/counterplots/utils/plots.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/counterplots/utils/process.py` & `counterplots-0.0.5/counterplots/utils/process.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/counterplots/utils/verification.py` & `counterplots-0.0.5/counterplots/utils/verification.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/counterplots.egg-info/PKG-INFO` & `counterplots-0.0.5/counterplots.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,172 +1,173 @@
 Metadata-Version: 2.1
 Name: counterplots
-Version: 0.0.4
+Version: 0.0.5
 Summary: Plotting tool for counterfactual explanations
 Home-page: https://github.com/ADMAntwerp/CounterPlots
+Download-URL: https://pypi.org/project/counterplots/
 Author: Raphael Mazzine Barbosa de Oliveira, Bjorge Meulemeester
 License: MIT
-Download-URL: https://pypi.org/project/counterplots/
-Description: <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_logo.svg"><br>
-        
-        --------------------------------------
-        
-        CounterPlots: Plotting tool for counterfactuals
-        =======================================
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![example workflow](https://github.com/ADMAntwerp/CounterPlots/actions/workflows/deployment.yml/badge.svg)](https://github.com/ADMAntwerp/CounterPlots/actions)
-        [![Code Coverage](https://codecov.io/gh/rmazzine/counterplotcoverage/branch/main/graph/badge.svg?token=TQYJSGEMP1)](https://codecov.io/gh/rmazzine/counterplotcoverage)
-        [![Known Vulnerabilities](https://snyk.io/test/github/ADMAntwerp/CounterPlots/badge.svg)](https://snyk.io/test/github/ADMAntwerp/CounterPlots)
-        
-        Counterplots is a Python package that allows you to plot counterfactuals with easy integration with any counterfactual generation algorithm.
-        
-        ## Plot examples
-        
-        ### Greedy Plot
-        
-        The greedy plot shows the greediest (feature change with the highest impact towards the opposite class) path from the factual instance until it reaches the counterfactual.
-        
-        <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_greedy.png">
-        
-        ### CounterShapley Plot
-        
-        This chart shows each counterfactual feature change contribution to the counterfactual prediction. It uses Shapley values to calculate the contribution of each feature change.
-        
-        <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_countershapley.png">
-        
-        ### Constellation Plot
-        
-        This chart shows the prediction score change for all possible feature change combinations.
-        
-        <img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_constellation.png">
-        
-        ## Installation
-        With pip:
-        ```bash
-        pip install counterplots
-        ```
-        
-        ## Usage
-        To use CounterPlots, you just need the machine learning model predictor, and the factual and counterfactual points.
-        The example below uses a simple mock model:
-        ```python
-        from counterplots import CreatePlot
-        import numpy as np
-        
-        # Simple mock model for the predict_proba function which returns a probability for each input instance
-        def mock_predict_proba(data):
-            out = []
-            for x in data:
-                if list(x) == [0.0, 0.0, 0.0]:
-                    out.append(0.0)
-                elif list(x) == [1.0, 0.0, 0.0]:
-                    out.append(0.44)
-                elif list(x) == [0.0, 1.0, 0.0]:
-                    out.append(0.4)
-                elif list(x) == [0.0, 0.0, 1.0]:
-                    out.append(0.2)
-                elif list(x) == [1.0, 1.0, 0.0]:
-                    out.append(0.3)
-                elif list(x) == [0.0, 1.0, 1.0]:
-                    out.append(0.25)
-                elif list(x) == [1.0, 0.0, 1.0]:
-                    out.append(0.4)
-                elif list(x) == [1.0, 1.0, 1.0]:
-                    out.append(1.0)
-            return np.array(out)
-        
-        # Factual Instance
-        factual = np.array([0, 0, 0])
-        # Counterfactual Instance
-        cf = np.array([1, 1, 1])
-        
-        # Create the plot object
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            mock_predict_proba)
-        
-        # Create the greedy plot
-        cf_plots.greedy('greedy_plot.png')
-        # Create the countershapley plot
-        cf_plots.countershapley('countershapley_plot.png')
-        # Create the constellation plot
-        cf_plots.constellation('constellation_plot.png')
-        
-        # Print the countershapley values
-        print(cf_plots.countershapley_values())
-        ```
-        
-        In case you want to add custom names to the features, use the optional argument `feature_names`:
-        ```python
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            mock_predict_proba,
-            feature_names=['feature1', 'feature2', 'feature3'])
-        ```
-        
-        In case you want to add custom labels to the factual and counterfactual points, use the optional argument `class_names`:
-        ```python
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            mock_predict_proba,
-            class_names=['Factual', 'Counterfactual'])
-        ```
-        
-        ## Using with Scikit-Learn
-        
-        CounterPlots can be used with any machine learning model that has a `predict_proba` function. For example, with Scikit-Learn:
-        <details>
-        
-        ```python
-        import numpy as np
-        from sklearn.ensemble import RandomForestClassifier
-        from sklearn.datasets import load_iris
-        
-        from counterplots import CreatePlot
-        
-        iris = load_iris()
-        
-        X = iris.data
-        y = [0 if l == 0 else 1 for l in iris.target] # Makes it a binary classification problem
-        
-        clf = RandomForestClassifier(max_depth=2, random_state=0)
-        clf.fit(X, y)
-        
-        preds = clf.predict(X)
-        
-        # For the factual point, takes an instance with 0 classification
-        factual = X[np.argwhere(preds == 0)[0]][0]
-        # For the counterfactual point, takes an instance with 1 classification
-        cf = X[np.argwhere(preds == 1)[0]][0]
-        
-        cf_plots = CreatePlot(
-            factual,
-            cf,
-            clf.predict_proba,
-            feature_names=iris.feature_names,
-            class_names={0: 'Setosa', 1: 'Non-Setosa'}
-        )
-        
-        
-        # Create the greedy plot
-        cf_plots.greedy('iris_greedy_plot.png')
-        # Create the countershapley plot
-        cf_plots.countershapley('iris_countershapley_plot.png')
-        # Create the constellation plot
-        cf_plots.constellation('iris_constellation_plot.png')
-        
-        # Print the countershapley values
-        print(cf_plots.countershapley_values())
-        ```
-        </details>
-        
-        ## Citation
-        If you use CounterPlots in your research, please cite the following paper:
-        ```bibtex
-        ```
 Keywords: Counterfactual Explanations,Visualization,Plotting,Explainable Artificial Intelligence,XAI,Machine Learning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_logo.svg"><br>
+
+--------------------------------------
+
+CounterPlots: Plotting tool for counterfactuals
+=======================================
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![example workflow](https://github.com/ADMAntwerp/CounterPlots/actions/workflows/deployment.yml/badge.svg)](https://github.com/ADMAntwerp/CounterPlots/actions)
+[![Code Coverage](https://codecov.io/gh/rmazzine/counterplotcoverage/branch/main/graph/badge.svg?token=TQYJSGEMP1)](https://codecov.io/gh/rmazzine/counterplotcoverage)
+[![Known Vulnerabilities](https://snyk.io/test/github/ADMAntwerp/CounterPlots/badge.svg)](https://snyk.io/test/github/ADMAntwerp/CounterPlots)
+
+Counterplots is a Python package that allows you to plot counterfactuals with easy integration with any counterfactual generation algorithm.
+
+## Plot examples
+
+### Greedy Plot
+
+The greedy plot shows the greediest (feature change with the highest impact towards the opposite class) path from the factual instance until it reaches the counterfactual.
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_greedy.png">
+
+### CounterShapley Plot
+
+This chart shows each counterfactual feature change contribution to the counterfactual prediction. It uses Shapley values to calculate the contribution of each feature change.
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_countershapley.png">
+
+### Constellation Plot
+
+This chart shows the prediction score change for all possible feature change combinations.
+
+<img src="https://raw.githubusercontent.com/ADMAntwerp/CounterPlots/main/_static/counterplots_example_constellation.png">
+
+## Installation
+With pip:
+```bash
+pip install counterplots
+```
+
+## Usage
+To use CounterPlots, you just need the machine learning model predictor, and the factual and counterfactual points.
+The example below uses a simple mock model:
+```python
+from counterplots import CreatePlot
+import numpy as np
+
+# Simple mock model for the predict_proba function which returns a probability for each input instance
+def mock_predict_proba(data):
+    out = []
+    for x in data:
+        if list(x) == [0.0, 0.0, 0.0]:
+            out.append(0.0)
+        elif list(x) == [1.0, 0.0, 0.0]:
+            out.append(0.44)
+        elif list(x) == [0.0, 1.0, 0.0]:
+            out.append(0.4)
+        elif list(x) == [0.0, 0.0, 1.0]:
+            out.append(0.2)
+        elif list(x) == [1.0, 1.0, 0.0]:
+            out.append(0.3)
+        elif list(x) == [0.0, 1.0, 1.0]:
+            out.append(0.25)
+        elif list(x) == [1.0, 0.0, 1.0]:
+            out.append(0.4)
+        elif list(x) == [1.0, 1.0, 1.0]:
+            out.append(1.0)
+    return np.array(out)
+
+# Factual Instance
+factual = np.array([0, 0, 0])
+# Counterfactual Instance
+cf = np.array([1, 1, 1])
+
+# Create the plot object
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    mock_predict_proba)
+
+# Create the greedy plot
+cf_plots.greedy('greedy_plot.png')
+# Create the countershapley plot
+cf_plots.countershapley('countershapley_plot.png')
+# Create the constellation plot
+cf_plots.constellation('constellation_plot.png')
+
+# Print the countershapley values
+print(cf_plots.countershapley_values())
+```
+
+In case you want to add custom names to the features, use the optional argument `feature_names`:
+```python
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    mock_predict_proba,
+    feature_names=['feature1', 'feature2', 'feature3'])
+```
+
+In case you want to add custom labels to the factual and counterfactual points, use the optional argument `class_names`:
+```python
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    mock_predict_proba,
+    class_names=['Factual', 'Counterfactual'])
+```
+
+## Using with Scikit-Learn
+
+CounterPlots can be used with any machine learning model that has a `predict_proba` function. For example, with Scikit-Learn:
+<details>
+
+```python
+import numpy as np
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.datasets import load_iris
+
+from counterplots import CreatePlot
+
+iris = load_iris()
+
+X = iris.data
+y = [0 if l == 0 else 1 for l in iris.target] # Makes it a binary classification problem
+
+clf = RandomForestClassifier(max_depth=2, random_state=0)
+clf.fit(X, y)
+
+preds = clf.predict(X)
+
+# For the factual point, takes an instance with 0 classification
+factual = X[np.argwhere(preds == 0)[0]][0]
+# For the counterfactual point, takes an instance with 1 classification
+cf = X[np.argwhere(preds == 1)[0]][0]
+
+cf_plots = CreatePlot(
+    factual,
+    cf,
+    clf.predict_proba,
+    feature_names=iris.feature_names,
+    class_names={0: 'Setosa', 1: 'Non-Setosa'}
+)
+
+
+# Create the greedy plot
+cf_plots.greedy('iris_greedy_plot.png')
+# Create the countershapley plot
+cf_plots.countershapley('iris_countershapley_plot.png')
+# Create the constellation plot
+cf_plots.constellation('iris_constellation_plot.png')
+
+# Print the countershapley values
+print(cf_plots.countershapley_values())
+```
+</details>
+
+## Citation
+If you use CounterPlots in your research, please cite the following paper:
+```bibtex
+```
```

### Comparing `counterplots-0.0.4/setup.py` & `counterplots-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = f.read()
 
 with open('LICENSE.txt') as f:
     LICENSE = f.read()
 
 setup_args = dict(
     name='counterplots',
-    version='0.0.4',
+    version='0.0.5',
     description='Plotting tool for counterfactual explanations',
     long_description_content_type='text/markdown',
     long_description=README,
     license='MIT',
     packages=find_packages(exclude=('tests\*', 'exp_notebooks\*', '_static\*')),
     author='Raphael Mazzine Barbosa de Oliveira, Bjorge Meulemeester',
     keywords=['Counterfactual Explanations', 'Visualization', 'Plotting', 'Explainable Artificial Intelligence', 'XAI', 'Machine Learning'],
```

### Comparing `counterplots-0.0.4/tests/test____init__.py` & `counterplots-0.0.5/tests/test____init__.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/tests/utils/test_plots.py` & `counterplots-0.0.5/tests/utils/test_plots.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/tests/utils/test_process.py` & `counterplots-0.0.5/tests/utils/test_process.py`

 * *Files identical despite different names*

### Comparing `counterplots-0.0.4/tests/utils/test_verification.py` & `counterplots-0.0.5/tests/utils/test_verification.py`

 * *Files identical despite different names*

