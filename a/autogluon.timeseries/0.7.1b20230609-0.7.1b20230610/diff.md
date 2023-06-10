# Comparing `tmp/autogluon.timeseries-0.7.1b20230609.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230609.tar", last modified: Fri Jun  9 09:04:12 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230610.tar", last modified: Sat Jun 10 09:04:14 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230609.tar` & `autogluon.timeseries-0.7.1b20230610.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:04:12.162212 autogluon.timeseries-0.7.1b20230609/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49409 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48405 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 09:04:11.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.360252 autogluon.timeseries-0.7.1b20230610/
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-10 09:04:14.360252 autogluon.timeseries-0.7.1b20230610/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:04:14.360252 autogluon.timeseries-0.7.1b20230610/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.352252 autogluon.timeseries-0.7.1b20230610/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.352252 autogluon.timeseries-0.7.1b20230610/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.356252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.360252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.360252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49409 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.360252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48405 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.360252 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-10 09:03:29.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:14.352252 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:04:14.000000 autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230609/PKG-INFO` & `autogluon.timeseries-0.7.1b20230610/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230609
+Version: 0.7.1b20230610
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230609/setup.py` & `autogluon.timeseries-0.7.1b20230610/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,40 +18,38 @@
 ITEMID = "item_id"
 TIMESTAMP = "timestamp"
 
 IRREGULAR_TIME_INDEX_FREQSTR = "IRREG"
 
 
 class TimeSeriesDataFrame(pd.DataFrame):
-    """``TimeSeriesDataFrame`` s represent a collection of time series, where each row
-    identifies the values of an (``item_id``, ``timestamp``) pair.
+    """A collection of univariate time series, where each row is identified by an (``item_id``, ``timestamp``) pair.
 
-    For example, a time series data frame could represent the daily sales of a collection
-    of products, where each ``item_id`` identifies a product and ``timestamp`` s correspond to
-    the days.
+    For example, a time series data frame could represent the daily sales of a collection of products, where each
+    ``item_id`` corresponds to a product and ``timestamp`` corresponds to the day of the record.
 
     Parameters
     ----------
     data : Any
-        Time-series data to construct a ``TimeSeriesDataFrame``. The class currently supports four input formats.
+        Time series data to construct a ``TimeSeriesDataFrame``. The class currently supports four input formats.
 
-        1. Time-series data in a pandas DataFrame format without multi-index. For example::
+        1. Time series data in a pandas DataFrame format without multi-index. For example::
 
                    item_id  timestamp  target
                 0        0 2019-01-01       0
                 1        0 2019-01-02       1
                 2        0 2019-01-03       2
                 3        1 2019-01-01       3
                 4        1 2019-01-02       4
                 5        1 2019-01-03       5
                 6        2 2019-01-01       6
                 7        2 2019-01-02       7
                 8        2 2019-01-03       8
 
-        2. Time-series data in pandas DataFrame format with multi-index on item_id and timestamp. For example::
+        2. Time series data in pandas DataFrame format with multi-index on ``item_id`` and ``timestamp``. For example::
 
                                         target
                 item_id timestamp
                 0       2019-01-01       0
                         2019-01-02       1
                         2019-01-03       2
                 1       2019-01-01       3
@@ -59,20 +57,20 @@
                         2019-01-03       5
                 2       2019-01-01       6
                         2019-01-02       7
                         2019-01-03       8
 
         3. Path to a data file in CSV or Parquet format. The file must contain columns ``item_id`` and ``timestamp``, as well as columns with time series values. This is similar to Option 1 above (pandas DataFrame format without multi-index). Both remote (e.g., S3) and local paths are accepted.
 
-        4. Time-series data in Iterable format. For example::
+        4. Time series data in Iterable format. For example::
 
                 iterable_dataset = [
-                    {"target": [0, 1, 2], "start": pd.Timestamp("01-01-2019", freq='D')},
-                    {"target": [3, 4, 5], "start": pd.Timestamp("01-01-2019", freq='D')},
-                    {"target": [6, 7, 8], "start": pd.Timestamp("01-01-2019", freq='D')}
+                    {"target": [0, 1, 2], "start": pd.Period("01-01-2019", freq='D')},
+                    {"target": [3, 4, 5], "start": pd.Period("01-01-2019", freq='D')},
+                    {"target": [6, 7, 8], "start": pd.Period("01-01-2019", freq='D')}
                 ]
 
     static_features : Optional[pd.DataFrame]
         An optional data frame describing the metadata attributes of individual items in the item index. These
         may be categorical or real valued attributes for each item. For example, if the item index refers to
         time series data of individual households, static features may refer to time-independent demographic
         features. When provided during ``fit``, the ``TimeSeriesPredictor`` expects the same metadata to be available
@@ -81,16 +79,17 @@
 
         ``TimeSeriesDataFrame`` will ensure consistency of static features during serialization/deserialization,
         copy and slice operations although these features should be considered experimental.
 
     Attributes
     ----------
     freq : str
-        A pandas and gluon-ts compatible string describing the frequency of the time series. For example
-        "D" is daily data, etc. Also see,
+        A pandas-compatible string describing the frequency of the time series. For example ``"D"`` for daily data,
+        ``"H"`` for hourly data, etc. This attribute is determined automatically based on the timestamps. For the full
+        list of possible values, see
         https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
     num_items : int
         Number of items (time series) in the data set.
     item_ids : pd.Index
         List of unique time series IDs contained in the data set.
     """
```

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from autogluon.timeseries.models.local.abstract_local_model import AG_DEFAULT_N_JOBS
 from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
 
 logger = logging.getLogger(__name__)
 
 
 class DirectTabularModel(AbstractTimeSeriesModel):
-    """Predict future time series values using autogluon.tabular.TabularPredictor.
+    """Predict all future time series values simultaneously using TabularPredictor from AutoGluon-Tabular.
 
-    A single predictor is used to forecast all future time series values using the following features:
+    A single TabularPredictor is used to forecast all future time series values using the following features:
 
     - lag features (observed time series values) based on ``freq`` of the data
     - time features (e.g., day of the week) based on the timestamp of the measurement
     - lagged known and past covariates (if available)
     - static features of each item (if available)
 
     Features not known during the forecast horizon (e.g., future target values) are replaced by NaNs.
```

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import math
 import os
 import re
 import warnings
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
@@ -45,17 +46,17 @@
 
     def predict(self, X: pd.DataFrame) -> np.ndarray:
         assert isinstance(X, pd.DataFrame)
         return self.predictor.predict(X).values
 
 
 class RecursiveTabularModel(AbstractTimeSeriesModel):
-    """Predict time series values one by one using TabularPredictor.
+    """Predict future time series values one by one using TabularPredictor from AutoGluon-Tabular.
 
-    Based on the `mlforecast`<https://github.com/Nixtla/mlforecast>_ library.
+    Based on the `mlforecast <https://github.com/Nixtla/mlforecast>`_ library.
 
 
     Other Parameters
     ----------------
     lags : List[int], default = None
         Lags of the target that will be used as features for predictions. If None, will be determined automatically
         based on the frequency of the data.
@@ -71,14 +72,18 @@
         Hyperparameters dictionary passed to ``TabularPredictor.fit``. Contains the names of models that should be fit.
         Defaults to ``{"GBM": {}}``.
     tabular_fit_kwargs : Dict[str, Any], optional
         Additional keyword arguments passed to ``TabularPredictor.fit``. Defaults to an empty dict.
     max_num_samples : int, default = 1_000_000
         If given, training and validation datasets will contain at most this many rows (starting from the end of each
         series).
+    subsampling_strategy : {"items", "timesteps", None}, default = "items"
+        Strategy used to limit memory consumption of the model if the dataset is too large. Use "items" if the dataset
+        contains many time series, "timesteps" if the dataset contains a few very long time series, or None to disable
+        subsampling. Only applies to datasets with > 20_000_000 rows.
 
     """
 
     # TODO: Use sample_weight to align metrics with Tabular
     # TODO: Add lag_transforms
 
     TIMESERIES_METRIC_TO_TABULAR_METRIC = {
@@ -193,70 +198,98 @@
         # FIXME: If unique_id column is not sorted, MLForecast will assign incorrect IDs to forecasts
         return df.rename(columns=column_name_mapping).sort_values(by="unique_id", kind="stable")
 
     def _get_features_dataframe(
         self,
         data: TimeSeriesDataFrame,
         last_k_values: Optional[int] = None,
-        max_num_samples: Optional[int] = None,
     ) -> Tuple[pd.DataFrame, pd.Series]:
         """Construct feature matrix containing lags, covariates, and target time series values.
 
         Rows where the regression target equals NaN are dropped, but rows where the features are missing are kept.
 
         Parameters
         ----------
         data : TimeSeriesDataFrame
             Time series data that needs to be converted.
         last_k_values : int, optional
             If given, only last `last_k_values` rows will be kept for each time series.
-        max_num_samples : int, optional
-            If given, the output will contain at most this many rows.
         """
         item_ids_to_exclude = data.item_ids[data.num_timesteps_per_item() < self.required_ts_length]
         if len(item_ids_to_exclude) > 0:
             data = data.drop(item_ids_to_exclude, level=0)
         df = self._to_mlforecast_df(data, data.static_features)
         # FIXME: keep_last_n produces a bug if time series too short -> manually select tail of each series
         features = self.mlf.preprocess(
             df,
             dropna=False,
             static_features=None,  # we handle static features in `_to_mlforecast_df`, without relying on MLForecast
         )
+        del self.mlf.ts.features_
         if last_k_values is not None:
             features = features.groupby("unique_id", sort=False).tail(last_k_values)
         features.dropna(subset=self.mlf.ts.target_col, inplace=True)
-        if max_num_samples is not None and len(features) > max_num_samples:
-            rows_per_item = int(max_num_samples / data.num_items) + 1
-            features = features.groupby("unique_id", sort=False).tail(rows_per_item)
         features = features.reset_index(drop=True)
         return features[self.mlf.ts.features_order_], features[self.mlf.ts.target_col]
 
+    @staticmethod
+    def _subsample_data_to_avoid_oom(
+        data: TimeSeriesDataFrame,
+        strategy: Optional[str] = "items",
+        max_num_rows: int = 20_000_000,
+    ) -> TimeSeriesDataFrame:
+        """Subsample time series from the dataset to avoid out of memory errors inside MLForecast.preprocess."""
+        # TODO: Find a better way to ensure that the model does not run out of memory. E.g., by estimating the expected
+        # memory usage & comparing it to currently available RAM
+        if len(data) > max_num_rows:
+            if strategy == "items":
+                item_ids = data.item_ids
+                num_items_to_keep = math.ceil(len(item_ids) * max_num_rows / len(data))
+                items_to_keep = np.random.choice(item_ids, num_items_to_keep, replace=False)
+                logger.debug(
+                    f"\tRandomly selected {num_items_to_keep} ({num_items_to_keep / len(item_ids):.1%}) time series "
+                    "to limit peak memory usage"
+                )
+                data = data.query("item_id in @items_to_keep")
+            elif strategy == "timesteps":
+                num_timesteps_to_remove = math.floor((len(data) - max_num_rows) / data.num_items)
+                logger.debug(
+                    f"\tRemoving {num_timesteps_to_remove} from the start of each time series to limit peak memory usage"
+                )
+                data = data.slice_by_timestep(num_timesteps_to_remove, None)
+        return data
+
     def _fit(
         self,
         train_data: TimeSeriesDataFrame,
         val_data: Optional[TimeSeriesDataFrame] = None,
         time_limit: Optional[int] = None,
         verbosity: int = 2,
         **kwargs,
     ) -> None:
         self._check_fit_params()
         from mlforecast import MLForecast
 
         # TabularEstimator is passed to MLForecast later to include tuning_data
         model_params = self._get_model_params().copy()
+
+        subsampling_strategy = model_params.pop("subsampling_strategy", "items")
+        train_data = self._subsample_data_to_avoid_oom(train_data, strategy=subsampling_strategy)
+
         mlforecast_init_args = self._get_mlforecast_init_args(train_data, model_params)
         self.mlf = MLForecast(models={}, freq=self.freq, **mlforecast_init_args)
 
         # Do not use external val_data as tuning_data to avoid overfitting
-        max_num_samples = model_params.get("max_num_samples", 1_000_000)
         train_subset, val_subset = train_data.train_test_split(self.prediction_length)
-        X_train, y_train = self._get_features_dataframe(train_subset, max_num_samples=max_num_samples)
+
+        max_num_samples = model_params.get("max_num_samples", 1_000_000)
+        max_rows_per_item = math.ceil(max_num_samples / train_data.num_items)
+        X_train, y_train = self._get_features_dataframe(train_subset, last_k_values=max_rows_per_item)
         X_val, y_val = self._get_features_dataframe(
-            val_subset, last_k_values=self.prediction_length, max_num_samples=max_num_samples
+            val_subset, last_k_values=min(self.prediction_length, max_rows_per_item)
         )
 
         estimator = TabularEstimator(
             predictor_init_kwargs={
                 "path": self.path + os.sep + "point_predictor",
                 "problem_type": ag.constants.REGRESSION,
                 "eval_metric": self.TIMESERIES_METRIC_TO_TABULAR_METRIC[self.eval_metric],
```

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -137,20 +137,18 @@
             forecast_keys=forecast_keys,
             item_id=str(forecast.item_id),
         )
         return QuantileForecast(**forecast_init_args)
 
 
 class DeepARModel(AbstractGluonTSPyTorchModel):
-    """DeepAR model from GluonTS based on the PyTorch backend.
-
-    The model consists of an LSTM encoder and a decoder that outputs the
-    distribution of the next target value. Close to the model described in [Salinas2020]_.
+    """Autoregressive forecasting model based on a recurrent neural network [Salinas2020]_.
 
     Based on `gluonts.torch.model.deepar.DeepAREstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.deepar.html>`_.
+    See GluonTS documentation for additional hyperparameters.
 
 
     References
     ----------
     .. [Salinas2020] Salinas, David, et al.
         "DeepAR: Probabilistic forecasting with autoregressive recurrent networks."
         International Journal of Forecasting. 2020.
@@ -199,18 +197,15 @@
         init_kwargs["num_feat_static_real"] = self.num_feat_static_real
         init_kwargs["cardinality"] = self.feat_static_cat_cardinality
         init_kwargs["num_feat_dynamic_real"] = self.num_feat_dynamic_real
         return init_kwargs
 
 
 class SimpleFeedForwardModel(AbstractGluonTSPyTorchModel):
-    """SimpleFeedForward model from GluonTS based on the PyTorch backend.
-
-    The model consists of a multilayer perceptron (MLP) that predicts the distribution of all the target value in the
-    forecast horizon.
+    """Simple feedforward neural network that simultaneously predicts all future values.
 
     Based on `gluonts.torch.model.simple_feedforward.SimpleFeedForwardEstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.simple_feedforward.html>`_.
     See GluonTS documentation for additional hyperparameters.
 
 
     Other Parameters
     ----------------
@@ -234,18 +229,15 @@
         Learning rate used during training
     """
 
     gluonts_estimator_class: Type[GluonTSPyTorchLightningEstimator] = SimpleFeedForwardEstimator
 
 
 class TemporalFusionTransformerModel(AbstractGluonTSPyTorchModel):
-    """TemporalFusionTransformer model from GluonTS.
-
-    The model combines an LSTM encoder, a transformer decoder, and directly predicts
-    the quantiles of future target values. As described in [Lim2021]_.
+    """Combines LSTM with a transformer layer to predict the quantiles of all future target values [Lim2021]_.
 
     Based on `gluonts.torch.model.tft.TemporalFusionTransformerEstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.tft.html>`_.
     See GluonTS documentation for additional hyperparameters.
 
 
     References
     ----------
@@ -303,18 +295,15 @@
             init_kwargs["static_dims"] = [self.num_feat_static_real]
         if len(self.feat_static_cat_cardinality):
             init_kwargs["static_cardinalities"] = self.feat_static_cat_cardinality
         return init_kwargs
 
 
 class DLinearModel(AbstractGluonTSPyTorchModel):
-    """D-Linear model from GluonTS.
-
-    The model combines a moving window detrender with a multilayer perceptron (MLP) that predicts the distribution of
-    all the target value in the forecast horizon.
+    """Simple feedforward neural network that subtracts trend before forecasting [Zeng2023]_.
 
     Based on `gluonts.torch.model.d_linear.DLinearEstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.d_linear.html>`_.
     See GluonTS documentation for additional hyperparameters.
 
     References
     ----------
     .. [Zeng2023] Zeng, Ailing, et al.
@@ -347,17 +336,15 @@
 
     @property
     def default_context_length(self) -> int:
         return 96
 
 
 class PatchTSTModel(AbstractGluonTSPyTorchModel):
-    """PatchTST model from GluonTS.
-
-    The model is based on a transformer that segments each time series into subseries-level patches.
+    """Transformer-based forecaster that segments each time series into patches [Nie2023]_.
 
     Based on `gluonts.torch.model.d_linear.PatchTSTEstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.patch_tst.html>`_.
     See GluonTS documentation for additional hyperparameters.
 
     References
     ----------
     .. [Nie2023] Nie, Yuqi, et al.
```

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,24 +175,24 @@
     def _get_model_type(self):
         from statsforecast.models import AutoETS
 
         return AutoETS
 
 
 class DynamicOptimizedThetaModel(AbstractStatsForecastModel):
-    """Optimized Theta forecasting model from Fiorucci et al. (2016).
+    """Optimized Theta forecasting model [Fiorucci2016]_.
 
     Based on `statsforecast.models.DynamicOptimizedTheta <https://nixtla.github.io/statsforecast/models.html#dynamic-optimized-theta-method>`_.
 
 
     References
     ----------
-    Fiorucci, Jose et al.
-    "Models for optimising the theta method and their relationship to state space models."
-    International journal of forecasting 32.4 (2016): 1151-1161.
+    .. [Fiorucci2016] Fiorucci, Jose et al.
+        "Models for optimising the theta method and their relationship to state space models."
+        International journal of forecasting 32.4 (2016): 1151-1161.
 
 
     Other Parameters
     ----------------
     decomposition_type : {"multiplicative", "additive"}, default = "multiplicative"
         Seasonal decomposition type.
     seasonal_period : int or None, default = None
@@ -219,24 +219,24 @@
     def _get_model_type(self):
         from statsforecast.models import DynamicOptimizedTheta
 
         return DynamicOptimizedTheta
 
 
 class ThetaModel(AbstractStatsForecastModel):
-    """Theta forecasting model from Assimakopoulos and Nikolopoulos (2000).
+    """Theta forecasting model [Assimakopoulos2000]_.
 
     Based on `statsforecast.models.Theta <https://nixtla.github.io/statsforecast/models.html#theta>`_.
 
 
     References
     ----------
-    Assimakopoulos, Vassilis, and Konstantinos Nikolopoulos.
-    "The theta model: a decomposition approach to forecasting."
-    International journal of forecasting 16.4 (2000): 521-530.
+    .. [Assimakopoulos2000] Assimakopoulos, Vassilis, and Konstantinos Nikolopoulos.
+        "The theta model: a decomposition approach to forecasting."
+        International journal of forecasting 16.4 (2000): 521-530.
 
 
     Other Parameters
     ----------------
     decomposition_type : {"multiplicative", "additive"}, default = "multiplicative"
         Seasonal decomposition type.
     seasonal_period : int or None, default = None
```

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230610/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230609
+Version: 0.7.1b20230610
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230610/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

