# Comparing `tmp/alns-5.1.0.tar.gz` & `tmp/alns-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alns-5.1.0.tar", max compression
+gzip compressed data, was "alns-5.2.0.tar", max compression
```

## Comparing `alns-5.1.0.tar` & `alns-5.2.0.tar`

### file list

```diff
@@ -1,59 +1,61 @@
--rw-r--r--   0        0        0     1095 2023-05-07 11:05:53.026157 alns-5.1.0/LICENSE.md
--rw-r--r--   0        0        0     5392 2023-05-07 11:05:53.026157 alns-5.1.0/README.md
--rw-r--r--   0        0        0    11418 2023-05-07 11:05:53.026157 alns-5.1.0/alns/ALNS.py
--rw-r--r--   0        0        0      495 2023-05-07 11:05:53.026157 alns-5.1.0/alns/Outcome.py
--rw-r--r--   0        0        0     5366 2023-05-07 11:05:53.026157 alns-5.1.0/alns/Result.py
--rw-r--r--   0        0        0      299 2023-05-07 11:05:53.026157 alns-5.1.0/alns/State.py
--rw-r--r--   0        0        0     3975 2023-05-07 11:05:53.026157 alns-5.1.0/alns/Statistics.py
--rw-r--r--   0        0        0       89 2023-05-07 11:05:53.026157 alns-5.1.0/alns/__init__.py
--rw-r--r--   0        0        0      885 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/AcceptanceCriterion.py
--rw-r--r--   0        0        0     1857 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/GreatDeluge.py
--rw-r--r--   0        0        0      276 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/HillClimbing.py
--rw-r--r--   0        0        0     2481 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/LateAcceptanceHillClimbing.py
--rw-r--r--   0        0        0     3545 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/NonLinearGreatDeluge.py
--rw-r--r--   0        0        0      179 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/RandomWalk.py
--rw-r--r--   0        0        0     6082 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/RecordToRecordTravel.py
--rw-r--r--   0        0        0     6400 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/SimulatedAnnealing.py
--rw-r--r--   0        0        0     2214 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/WorseAccept.py
--rw-r--r--   0        0        0      429 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/__init__.py
--rw-r--r--   0        0        0     2311 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_great_deluge.py
--rw-r--r--   0        0        0      820 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_hill_climbing.py
--rw-r--r--   0        0        0     6012 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_late_acceptance_hill_climbing.py
--rw-r--r--   0        0        0     3452 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_non_linear_great_deluge.py
--rw-r--r--   0        0        0      790 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_random_walk.py
--rw-r--r--   0        0        0     5022 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_record_to_record_travel.py
--rw-r--r--   0        0        0     7119 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_simulated_annealing.py
--rw-r--r--   0        0        0     1947 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_threshold_accept.py
--rw-r--r--   0        0        0     1161 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_update.py
--rw-r--r--   0        0        0     4361 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_worse_accept.py
--rw-r--r--   0        0        0      907 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/update.py
--rw-r--r--   0        0        0     5249 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/AlphaUCB.py
--rw-r--r--   0        0        0     3516 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/OperatorSelectionScheme.py
--rw-r--r--   0        0        0      635 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/RandomSelect.py
--rw-r--r--   0        0        0     5090 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/RouletteWheel.py
--rw-r--r--   0        0        0     3598 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/SegmentedRouletteWheel.py
--rw-r--r--   0        0        0      231 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/__init__.py
--rw-r--r--   0        0        0     2358 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_alpha_ucb.py
--rw-r--r--   0        0        0     2180 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_random_select.py
--rw-r--r--   0        0        0     3871 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_roulette_wheel.py
--rw-r--r--   0        0        0     2754 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_segmented_roulette_wheel.py
--rw-r--r--   0        0        0      842 2023-05-07 11:05:53.030156 alns-5.1.0/alns/show_versions.py
--rw-r--r--   0        0        0      663 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/MaxIterations.py
--rw-r--r--   0        0        0      769 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/MaxRuntime.py
--rw-r--r--   0        0        0     1013 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/NoImprovement.py
--rw-r--r--   0        0        0      669 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      166 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/__init__.py
--rw-r--r--   0        0        0     1290 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/test_max_iterations.py
--rw-r--r--   0        0        0     1811 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/test_max_runtime.py
--rw-r--r--   0        0        0     2431 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/test_no_improvement.py
--rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/__init__.py
--rw-r--r--   0        0        0      385 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/conftest.py
--rw-r--r--   0        0        0      355 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/states.py
--rw-r--r--   0        0        0    10367 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/test_alns.py
--rw-r--r--   0        0        0     6962 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/test_result.py
--rw-r--r--   0        0        0     2796 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/test_statistics.py
--rw-r--r--   0        0        0     2664 2023-05-07 11:05:53.050156 alns-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     6690 1970-01-01 00:00:00.000000 alns-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-06-10 09:32:51.231439 alns-5.2.0/LICENSE.md
+-rw-r--r--   0        0        0     5643 2023-06-10 09:32:51.231439 alns-5.2.0/README.md
+-rw-r--r--   0        0        0    11418 2023-06-10 09:32:51.231439 alns-5.2.0/alns/ALNS.py
+-rw-r--r--   0        0        0      495 2023-06-10 09:32:51.231439 alns-5.2.0/alns/Outcome.py
+-rw-r--r--   0        0        0     5366 2023-06-10 09:32:51.231439 alns-5.2.0/alns/Result.py
+-rw-r--r--   0        0        0      637 2023-06-10 09:32:51.231439 alns-5.2.0/alns/State.py
+-rw-r--r--   0        0        0     3975 2023-06-10 09:32:51.231439 alns-5.2.0/alns/Statistics.py
+-rw-r--r--   0        0        0       89 2023-06-10 09:32:51.231439 alns-5.2.0/alns/__init__.py
+-rw-r--r--   0        0        0      885 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/AcceptanceCriterion.py
+-rw-r--r--   0        0        0     1857 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/GreatDeluge.py
+-rw-r--r--   0        0        0      276 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/HillClimbing.py
+-rw-r--r--   0        0        0     2481 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/LateAcceptanceHillClimbing.py
+-rw-r--r--   0        0        0     3545 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/NonLinearGreatDeluge.py
+-rw-r--r--   0        0        0      179 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/RandomWalk.py
+-rw-r--r--   0        0        0     6082 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/RecordToRecordTravel.py
+-rw-r--r--   0        0        0     6400 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/SimulatedAnnealing.py
+-rw-r--r--   0        0        0     2214 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/WorseAccept.py
+-rw-r--r--   0        0        0      429 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/__init__.py
+-rw-r--r--   0        0        0     2311 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_great_deluge.py
+-rw-r--r--   0        0        0      820 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_hill_climbing.py
+-rw-r--r--   0        0        0     6012 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_late_acceptance_hill_climbing.py
+-rw-r--r--   0        0        0     3452 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_non_linear_great_deluge.py
+-rw-r--r--   0        0        0      790 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_random_walk.py
+-rw-r--r--   0        0        0     5022 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_record_to_record_travel.py
+-rw-r--r--   0        0        0     7119 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_simulated_annealing.py
+-rw-r--r--   0        0        0     1947 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_threshold_accept.py
+-rw-r--r--   0        0        0     1161 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_update.py
+-rw-r--r--   0        0        0     4361 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/tests/test_worse_accept.py
+-rw-r--r--   0        0        0      907 2023-06-10 09:32:51.231439 alns-5.2.0/alns/accept/update.py
+-rw-r--r--   0        0        0     5247 2023-06-10 09:32:51.231439 alns-5.2.0/alns/select/AlphaUCB.py
+-rw-r--r--   0        0        0     6509 2023-06-10 09:32:51.231439 alns-5.2.0/alns/select/MABSelector.py
+-rw-r--r--   0        0        0     3516 2023-06-10 09:32:51.231439 alns-5.2.0/alns/select/OperatorSelectionScheme.py
+-rw-r--r--   0        0        0      635 2023-06-10 09:32:51.231439 alns-5.2.0/alns/select/RandomSelect.py
+-rw-r--r--   0        0        0     5090 2023-06-10 09:32:51.231439 alns-5.2.0/alns/select/RouletteWheel.py
+-rw-r--r--   0        0        0     3598 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/SegmentedRouletteWheel.py
+-rw-r--r--   0        0        0      268 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/tests/__init__.py
+-rw-r--r--   0        0        0     2358 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/tests/test_alpha_ucb.py
+-rw-r--r--   0        0        0     4379 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/tests/test_mab_selector.py
+-rw-r--r--   0        0        0     2180 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/tests/test_random_select.py
+-rw-r--r--   0        0        0     3871 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/tests/test_roulette_wheel.py
+-rw-r--r--   0        0        0     2754 2023-06-10 09:32:51.235440 alns-5.2.0/alns/select/tests/test_segmented_roulette_wheel.py
+-rw-r--r--   0        0        0      842 2023-06-10 09:32:51.235440 alns-5.2.0/alns/show_versions.py
+-rw-r--r--   0        0        0      663 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/MaxIterations.py
+-rw-r--r--   0        0        0      769 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/MaxRuntime.py
+-rw-r--r--   0        0        0     1013 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/NoImprovement.py
+-rw-r--r--   0        0        0      669 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      166 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/tests/__init__.py
+-rw-r--r--   0        0        0     1290 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/tests/test_max_iterations.py
+-rw-r--r--   0        0        0     1811 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/tests/test_max_runtime.py
+-rw-r--r--   0        0        0     2431 2023-06-10 09:32:51.235440 alns-5.2.0/alns/stop/tests/test_no_improvement.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:32:51.235440 alns-5.2.0/alns/tests/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-10 09:32:51.235440 alns-5.2.0/alns/tests/conftest.py
+-rw-r--r--   0        0        0      834 2023-06-10 09:32:51.235440 alns-5.2.0/alns/tests/states.py
+-rw-r--r--   0        0        0    10367 2023-06-10 09:32:51.235440 alns-5.2.0/alns/tests/test_alns.py
+-rw-r--r--   0        0        0     6962 2023-06-10 09:32:51.235440 alns-5.2.0/alns/tests/test_result.py
+-rw-r--r--   0        0        0     2796 2023-06-10 09:32:51.235440 alns-5.2.0/alns/tests/test_statistics.py
+-rw-r--r--   0        0        0     2850 2023-06-10 09:32:51.251440 alns-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6772 1970-01-01 00:00:00.000000 alns-5.2.0/PKG-INFO
```

### Comparing `alns-5.1.0/LICENSE.md` & `alns-5.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/README.md` & `alns-5.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 stopping criterion is met. In each iteration, a destroy and repair operator are
 selected, which transform the current solution into a candidate solution. This
 candidate solution is then evaluated by an acceptance criterion, and the
 operator selection scheme is updated based on the evaluation outcome.
 
 `alns` depends only on `numpy` and `matplotlib`. It may be installed in the
 usual way as
-
 ```
 pip install alns
 ```
+Additionally, to enable more advanced operator selection schemes using 
+multi-armed bandit algorithms, `alns` may be installed with the optional 
+[MABWiser][12] dependency:
+```
+pip install alns[mabwiser]
+```
 
 The documentation is available [here][1].
 
 ### Getting started
 
 If you are new to metaheuristics or ALNS, you might benefit from reading
 the [introduction to ALNS][11] page.
@@ -118,7 +123,9 @@
 [8]: https://alns.readthedocs.io/en/latest/examples/capacitated_vehicle_routing_problem.html
 
 [9]: https://alns.readthedocs.io/en/latest/examples/permutation_flow_shop_problem.html
 
 [10]: https://alns.readthedocs.io/en/latest/setup/template.html
 
 [11]: https://alns.readthedocs.io/en/latest/setup/introduction_to_alns.html
+
+[12]: https://github.com/fidelity/mabwiser
```

### Comparing `alns-5.1.0/alns/ALNS.py` & `alns-5.2.0/alns/ALNS.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/Result.py` & `alns-5.2.0/alns/Result.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/Statistics.py` & `alns-5.2.0/alns/Statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/AcceptanceCriterion.py` & `alns-5.2.0/alns/accept/AcceptanceCriterion.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/GreatDeluge.py` & `alns-5.2.0/alns/accept/GreatDeluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/LateAcceptanceHillClimbing.py` & `alns-5.2.0/alns/accept/LateAcceptanceHillClimbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/NonLinearGreatDeluge.py` & `alns-5.2.0/alns/accept/NonLinearGreatDeluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/RecordToRecordTravel.py` & `alns-5.2.0/alns/accept/RecordToRecordTravel.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/SimulatedAnnealing.py` & `alns-5.2.0/alns/accept/SimulatedAnnealing.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/WorseAccept.py` & `alns-5.2.0/alns/accept/WorseAccept.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_great_deluge.py` & `alns-5.2.0/alns/accept/tests/test_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_hill_climbing.py` & `alns-5.2.0/alns/accept/tests/test_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_late_acceptance_hill_climbing.py` & `alns-5.2.0/alns/accept/tests/test_late_acceptance_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_non_linear_great_deluge.py` & `alns-5.2.0/alns/accept/tests/test_non_linear_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_random_walk.py` & `alns-5.2.0/alns/accept/tests/test_random_walk.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_record_to_record_travel.py` & `alns-5.2.0/alns/accept/tests/test_record_to_record_travel.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_simulated_annealing.py` & `alns-5.2.0/alns/accept/tests/test_simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_threshold_accept.py` & `alns-5.2.0/alns/accept/tests/test_threshold_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_update.py` & `alns-5.2.0/alns/accept/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/tests/test_worse_accept.py` & `alns-5.2.0/alns/accept/tests/test_worse_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/accept/update.py` & `alns-5.2.0/alns/accept/update.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/AlphaUCB.py` & `alns-5.2.0/alns/select/AlphaUCB.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         repair operators. Entry (i, j) is True if destroy operator i can be
         used together with repair operator j, and False otherwise.
 
     References
     ----------
     .. [1] Hendel, G. 2022. Adaptive large neighborhood search for mixed
            integer programming. *Mathematical Programming Computation* 14:
-           185 – 221.
+           185 - 221.
     """
 
     def __init__(
         self,
         scores: List[float],
         alpha: float,
         num_destroy: int,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alns-5.1.0/alns/select/OperatorSelectionScheme.py` & `alns-5.2.0/alns/select/OperatorSelectionScheme.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/RandomSelect.py` & `alns-5.2.0/alns/select/RandomSelect.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/RouletteWheel.py` & `alns-5.2.0/alns/select/RouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/SegmentedRouletteWheel.py` & `alns-5.2.0/alns/select/SegmentedRouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/tests/test_alpha_ucb.py` & `alns-5.2.0/alns/select/tests/test_alpha_ucb.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/tests/test_random_select.py` & `alns-5.2.0/alns/select/tests/test_random_select.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/tests/test_roulette_wheel.py` & `alns-5.2.0/alns/select/tests/test_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/select/tests/test_segmented_roulette_wheel.py` & `alns-5.2.0/alns/select/tests/test_segmented_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/show_versions.py` & `alns-5.2.0/alns/show_versions.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/stop/MaxIterations.py` & `alns-5.2.0/alns/stop/MaxIterations.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/stop/MaxRuntime.py` & `alns-5.2.0/alns/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/stop/NoImprovement.py` & `alns-5.2.0/alns/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/stop/StoppingCriterion.py` & `alns-5.2.0/alns/stop/StoppingCriterion.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/stop/tests/test_max_iterations.py` & `alns-5.2.0/alns/stop/tests/test_max_iterations.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/stop/tests/test_max_runtime.py` & `alns-5.2.0/alns/stop/tests/test_max_runtime.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/stop/tests/test_no_improvement.py` & `alns-5.2.0/alns/stop/tests/test_no_improvement.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/tests/test_alns.py` & `alns-5.2.0/alns/tests/test_alns.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/tests/test_result.py` & `alns-5.2.0/alns/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/alns/tests/test_statistics.py` & `alns-5.2.0/alns/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.1.0/pyproject.toml` & `alns-5.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alns"
-version = "5.1.0"
+version = "5.2.0"
 description = "A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/ALNS"
 include = [
     "LICENSE.md",
@@ -29,47 +29,53 @@
 [tool.poetry.urls]
 "Tracker" = "https://github.com/N-Wouda/ALNS/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8, <4.0"
 numpy = ">=1.18.0"
 matplotlib = ">=3.5.0"
+mabwiser = { version = ">=2.7.0", optional = true }
+
+[tool.poetry.extras]
+mabwiser = ["mabwiser"]  # optional integration with MABWiser
 
 # This group is needed to develop the package itself.
 [tool.poetry.group.dev.dependencies]
-vrplib = "^1.0.1"
 pre-commit = "^2.20.0"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.6.1"
 codecov = "*"
+mabwiser = ">=2.7.0"
 
 # This optional docs group is needed to build the documentation. It is not 
 # required by the package itself.
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 tomli = ">=2.0.1"
 nbsphinx = ">=0.8.9"
 ipython = ">=8.6.0"
 numpydoc = ">=1.5.0"
 sphinx_rtd_theme = ">=0.5.1"
 sphinx-autoapi = ">=2.0.1"
 docutils = "==0.16"
+mabwiser = ">=2.7.0"
 
 # This optional examples group is needed to run the example notebooks, but not
 # required for the package itself.
 [tool.poetry.group.examples]
 optional = true
 
 [tool.poetry.group.examples.dependencies]
-cvrplib = "^0.1.1"
+vrplib = "^1.0.1"
 networkx = ">=2.4.0"
 tsplib95 = ">=0.7.0"
 jupyter = "^1.0.0"
+mabwiser = ">=2.7.0"
 
 [tool.black]
 line-length = 79
 
 [tool.isort]
 case_sensitive = true
 line_length = 79
```

### Comparing `alns-5.1.0/PKG-INFO` & `alns-5.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alns
-Version: 5.1.0
+Version: 5.2.0
 Summary: A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm.
 Home-page: https://github.com/N-Wouda/ALNS
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,21 +12,18 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+Provides-Extra: mabwiser
+Requires-Dist: mabwiser (>=2.7.0) ; extra == "mabwiser"
 Requires-Dist: matplotlib (>=3.5.0)
 Requires-Dist: numpy (>=1.18.0)
 Project-URL: Repository, https://github.com/N-Wouda/ALNS
 Project-URL: Tracker, https://github.com/N-Wouda/ALNS/issues
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/alns.svg)](https://badge.fury.io/py/alns)
@@ -42,18 +39,23 @@
 stopping criterion is met. In each iteration, a destroy and repair operator are
 selected, which transform the current solution into a candidate solution. This
 candidate solution is then evaluated by an acceptance criterion, and the
 operator selection scheme is updated based on the evaluation outcome.
 
 `alns` depends only on `numpy` and `matplotlib`. It may be installed in the
 usual way as
-
 ```
 pip install alns
 ```
+Additionally, to enable more advanced operator selection schemes using 
+multi-armed bandit algorithms, `alns` may be installed with the optional 
+[MABWiser][12] dependency:
+```
+pip install alns[mabwiser]
+```
 
 The documentation is available [here][1].
 
 ### Getting started
 
 If you are new to metaheuristics or ALNS, you might benefit from reading
 the [introduction to ALNS][11] page.
@@ -150,7 +152,9 @@
 
 [9]: https://alns.readthedocs.io/en/latest/examples/permutation_flow_shop_problem.html
 
 [10]: https://alns.readthedocs.io/en/latest/setup/template.html
 
 [11]: https://alns.readthedocs.io/en/latest/setup/introduction_to_alns.html
 
+[12]: https://github.com/fidelity/mabwiser
+
```

