# Comparing `tmp/FLAML-1.2.4.tar.gz` & `tmp/FLAML-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-1.2.4.tar", last modified: Tue May 23 16:02:59 2023, max compression
+gzip compressed data, was "FLAML-2.0.0rc1.tar", last modified: Fri Jun  9 23:38:39 2023, max compression
```

## Comparing `FLAML-1.2.4.tar` & `FLAML-2.0.0rc1.tar`

### file list

```diff
@@ -1,134 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-23 16:01:44.000000 FLAML-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-23 16:01:44.000000 FLAML-1.2.4/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-23 16:02:59.628680 FLAML-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-23 16:01:44.000000 FLAML-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/chat_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/coding_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/code_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45993 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/oai/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/oai/openai_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130309 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)   104984 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/automl/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/generic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgboost/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    37002 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-23 16:01:44.000000 FLAML-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:02:59.628680 FLAML-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-23 16:01:44.000000 FLAML-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/assistant_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/chat_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/code_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45993 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/oai/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/oai/openai_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129988 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22656 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104594 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9829 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44194 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13704 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50288 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40082 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 23:38:39.833034 FLAML-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_version.py
```

### Comparing `FLAML-1.2.4/FLAML.egg-info/PKG-INFO` & `FLAML-2.0.0rc1/FLAML.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.4
+Version: 2.0.0rc1
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: automl
 Provides-Extra: notebook
 Provides-Extra: spark
 Provides-Extra: test
 Provides-Extra: catboost
 Provides-Extra: blendsearch
 Provides-Extra: ray
 Provides-Extra: azureml
@@ -23,14 +24,15 @@
 Provides-Extra: nlp
 Provides-Extra: ts_forecast
 Provides-Extra: forecast
 Provides-Extra: benchmark
 Provides-Extra: openai
 Provides-Extra: autogen
 Provides-Extra: synapse
+Provides-Extra: autozero
 License-File: LICENSE
 License-File: NOTICE.md
 
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
 ![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
@@ -42,26 +44,27 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: v1.2.0 is released with support for ChatGPT and GPT-4.
+:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web)
+:fire: [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) is released with support for ChatGPT and GPT-4, based on [Cost-Effective Hyperparameter Optimization for Large Language Model Generation Inference](https://arxiv.org/abs/2303.04673).
+:fire: FLAML supports AutoML and Hyperparameter Tuning features in [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview) private preview. Sign up for these features at: https://aka.ms/fabric/data-science/sign-up.
 
 
 ## What is FLAML
 FLAML is a lightweight Python library for efficient automation of machine
-learning, including selection of
+learning and AI operations, including selection of
 models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
 
-* For foundation models like the GPT series, it automates the experimentation and optimization of their inference performance to maximize the effectiveness for downstream applications and minimize the inference cost.
-* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources.
-* It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training/inference/evaluation code).
-* It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
+* For foundation models like the GPT models, it automates the experimentation and optimization of their performance to maximize the effectiveness for applications and minimize the inference cost. FLAML enables users to build and use adaptive AI agents with minimal effort.
+* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., search space and metric), or full customization (arbitrary training/inference/evaluation code).
+* It supports fast and economical automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
 and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
@@ -70,50 +73,57 @@
 
 FLAML requires **Python version >= 3.7**. It can be installed from pip:
 
 ```bash
 pip install flaml
 ```
 
-To run the [`notebook examples`](https://github.com/microsoft/FLAML/tree/main/notebook),
-install flaml with the [notebook] option:
-
+Minimal dependencies are installed without extra options. You can install extra options based on the feature you need. For example, use the following to install the dependencies needed by the [`autogen`](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) package.
 ```bash
-pip install flaml[notebook]
+pip install "flaml[autogen]"
 ```
 
+Find more options in [Installation](Installation).
+Each of the [`notebook examples`](https://github.com/microsoft/FLAML/tree/main/notebook) may require a specific option to be installed.
+
 ### .NET
 
 Use the following guides to get started with FLAML in .NET:
 
 - [Install Model Builder](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-model-builder?tabs=visual-studio-2022)
 - [Install ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-ml-net-cli?tabs=windows)
 - [Microsoft.AutoML](https://www.nuget.org/packages/Microsoft.ML.AutoML/0.20.0)
 
 ## Quickstart
 
-* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
-
-```python
-from flaml import oai
-
-config, analysis = oai.Completion.tune(
-    data=tune_data,
-    metric="success",
-    mode="max",
-    eval_func=eval_func,
-    inference_budget=0.05,
-    optimization_budget=3,
-    num_samples=-1,
-)
-```
-
-The automated experimentation and optimization can help you maximize the utility out of these expensive models.
-A suite of utilities such as caching and templating are offered to accelerate the experimentation and application development.
-
+* (New) The [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) package can help you maximize the utility out of the expensive LLMs such as ChatGPT and GPT-4, including:
+    - A drop-in replacement of `openai.Completion` or `openai.ChatCompletion` with powerful functionalites like tuning, caching, templating, filtering. For example, you can optimize generations by LLM with your own tuning data, success metrics and budgets.
+    ```python
+    from flaml import oai
+
+    # perform tuning
+    config, analysis = oai.Completion.tune(
+        data=tune_data,
+        metric="success",
+        mode="max",
+        eval_func=eval_func,
+        inference_budget=0.05,
+        optimization_budget=3,
+        num_samples=-1,
+    )
+
+    # perform inference for a test instance
+    response = oai.Completion.create(context=test_instance, **config)
+    ```
+    - LLM-driven intelligent agents which can perform tasks autonomously or with human feedback, including tasks that require using tools via code.
+    ```python
+    assistant = AssistantAgent("assistant")
+    user = UserProxyAgent("user", human_input_mode="TERMINATE")
+    assistant.receive("Draw a rocket and save to a file named 'rocket.svg'")
+    ```
 * With three lines of code, you can start using this economical and fast
 AutoML engine as a [scikit-learn style estimator](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
 
 ```python
 from flaml import AutoML
 automl = AutoML()
 automl.fit(X_train, y_train, task="classification")
@@ -146,19 +156,19 @@
 
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
-- Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
+- [Research](https://microsoft.github.io/FLAML/docs/Research) and [blogposts](https://microsoft.github.io/FLAML/blog) around FLAML.
 
-- Discord [here](https://discord.gg/Cppx2vSPVP).
+- [Discord](https://discord.gg/Cppx2vSPVP).
 
-- Contributing guide [here](https://microsoft.github.io/FLAML/docs/Contribute).
+- [Contributing guide](https://microsoft.github.io/FLAML/docs/Contribute).
 
 - ML.NET documentation and tutorials for [Model Builder](https://learn.microsoft.com/dotnet/machine-learning/tutorials/predict-prices-with-model-builder), [ML.NET CLI](https://learn.microsoft.com/dotnet/machine-learning/tutorials/sentiment-analysis-cli), and [AutoML API](https://learn.microsoft.com/dotnet/machine-learning/how-to-guides/how-to-use-the-automl-api).
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
```

### Comparing `FLAML-1.2.4/FLAML.egg-info/SOURCES.txt` & `FLAML-2.0.0rc1/FLAML.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 flaml/model.py
 flaml/version.py
 flaml/autogen/__init__.py
 flaml/autogen/code_utils.py
 flaml/autogen/math_utils.py
 flaml/autogen/agent/__init__.py
 flaml/autogen/agent/agent.py
+flaml/autogen/agent/assistant_agent.py
 flaml/autogen/agent/chat_agent.py
-flaml/autogen/agent/coding_agent.py
 flaml/autogen/agent/user_proxy_agent.py
 flaml/autogen/extensions/__init__.py
 flaml/autogen/oai/__init__.py
 flaml/autogen/oai/completion.py
 flaml/autogen/oai/openai_utils.py
 flaml/automl/__init__.py
 flaml/automl/automl.py
 flaml/automl/data.py
 flaml/automl/logger.py
 flaml/automl/ml.py
 flaml/automl/model.py
 flaml/automl/state.py
 flaml/automl/training_log.py
-flaml/automl/utils.py
 flaml/automl/nlp/__init__.py
 flaml/automl/nlp/utils.py
 flaml/automl/nlp/huggingface/__init__.py
 flaml/automl/nlp/huggingface/data_collator.py
 flaml/automl/nlp/huggingface/trainer.py
 flaml/automl/nlp/huggingface/training_args.py
 flaml/automl/nlp/huggingface/utils.py
```

### Comparing `FLAML-1.2.4/FLAML.egg-info/requires.txt` & `FLAML-2.0.0rc1/FLAML.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 NumPy>=1.17.0rc1
+
+[autogen]
+openai==0.27.4
+diskcache
+docker
+
+[automl]
 lightgbm>=2.3.1
 xgboost>=0.90
 scipy>=1.4.1
 pandas>=1.1.4
 scikit-learn>=0.24
 
-[autogen]
-openai==0.27.4
-diskcache
-docker
+[autozero]
+scikit-learn
+pandas
+packaging
 
 [azureml]
 azureml-mlflow
 
 [benchmark]
 catboost>=0.26
 psutil==5.8.0
@@ -46,16 +53,14 @@
 seqeval
 
 [nni]
 nni
 
 [notebook]
 jupyter
-matplotlib
-openml==0.10.2
 
 [openai]
 openai==0.27.4
 diskcache
 
 [ray]
 ray[tune]~=1.13
@@ -66,24 +71,29 @@
 
 [synapse]
 joblibspark>=0.5.0
 optuna==2.8.0
 pyspark>=3.2.0
 
 [test]
+lightgbm>=2.3.1
+xgboost>=0.90
+scipy>=1.4.1
+pandas>=1.1.4
+scikit-learn>=0.24
 thop
 pytest>=6.1.1
 coverage>=5.3
 pre-commit
 torch
 torchvision
 catboost<1.2,>=0.26
 rgf-python
 optuna==2.8.0
-openml==0.10.2
+openml
 statsmodels>=0.12.2
 psutil==5.8.0
 dataclasses
 transformers[torch]==4.26
 datasets
 nltk
 rouge_score
@@ -94,16 +104,18 @@
 pyspark>=3.2.0
 joblibspark>=0.5.0
 nbconvert
 nbformat
 ipykernel
 pytorch-lightning<1.9.1
 requests<2.29.0
+packaging
 
 [ts_forecast]
 holidays<0.14
 prophet>=1.0.1
 statsmodels>=0.12.2
 hcrystalball==0.1.10
 
 [vw]
 vowpalwabbit<9.0.0,>=8.10.0
+scikit-learn
```

### Comparing `FLAML-1.2.4/LICENSE` & `FLAML-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/NOTICE.md` & `FLAML-2.0.0rc1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/PKG-INFO` & `FLAML-2.0.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.4
+Version: 2.0.0rc1
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: automl
 Provides-Extra: notebook
 Provides-Extra: spark
 Provides-Extra: test
 Provides-Extra: catboost
 Provides-Extra: blendsearch
 Provides-Extra: ray
 Provides-Extra: azureml
@@ -23,14 +24,15 @@
 Provides-Extra: nlp
 Provides-Extra: ts_forecast
 Provides-Extra: forecast
 Provides-Extra: benchmark
 Provides-Extra: openai
 Provides-Extra: autogen
 Provides-Extra: synapse
+Provides-Extra: autozero
 License-File: LICENSE
 License-File: NOTICE.md
 
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
 ![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
@@ -42,26 +44,27 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: v1.2.0 is released with support for ChatGPT and GPT-4.
+:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web)
+:fire: [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) is released with support for ChatGPT and GPT-4, based on [Cost-Effective Hyperparameter Optimization for Large Language Model Generation Inference](https://arxiv.org/abs/2303.04673).
+:fire: FLAML supports AutoML and Hyperparameter Tuning features in [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview) private preview. Sign up for these features at: https://aka.ms/fabric/data-science/sign-up.
 
 
 ## What is FLAML
 FLAML is a lightweight Python library for efficient automation of machine
-learning, including selection of
+learning and AI operations, including selection of
 models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
 
-* For foundation models like the GPT series, it automates the experimentation and optimization of their inference performance to maximize the effectiveness for downstream applications and minimize the inference cost.
-* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources.
-* It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training/inference/evaluation code).
-* It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
+* For foundation models like the GPT models, it automates the experimentation and optimization of their performance to maximize the effectiveness for applications and minimize the inference cost. FLAML enables users to build and use adaptive AI agents with minimal effort.
+* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., search space and metric), or full customization (arbitrary training/inference/evaluation code).
+* It supports fast and economical automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
 and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
@@ -70,50 +73,57 @@
 
 FLAML requires **Python version >= 3.7**. It can be installed from pip:
 
 ```bash
 pip install flaml
 ```
 
-To run the [`notebook examples`](https://github.com/microsoft/FLAML/tree/main/notebook),
-install flaml with the [notebook] option:
-
+Minimal dependencies are installed without extra options. You can install extra options based on the feature you need. For example, use the following to install the dependencies needed by the [`autogen`](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) package.
 ```bash
-pip install flaml[notebook]
+pip install "flaml[autogen]"
 ```
 
+Find more options in [Installation](Installation).
+Each of the [`notebook examples`](https://github.com/microsoft/FLAML/tree/main/notebook) may require a specific option to be installed.
+
 ### .NET
 
 Use the following guides to get started with FLAML in .NET:
 
 - [Install Model Builder](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-model-builder?tabs=visual-studio-2022)
 - [Install ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-ml-net-cli?tabs=windows)
 - [Microsoft.AutoML](https://www.nuget.org/packages/Microsoft.ML.AutoML/0.20.0)
 
 ## Quickstart
 
-* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
-
-```python
-from flaml import oai
-
-config, analysis = oai.Completion.tune(
-    data=tune_data,
-    metric="success",
-    mode="max",
-    eval_func=eval_func,
-    inference_budget=0.05,
-    optimization_budget=3,
-    num_samples=-1,
-)
-```
-
-The automated experimentation and optimization can help you maximize the utility out of these expensive models.
-A suite of utilities such as caching and templating are offered to accelerate the experimentation and application development.
-
+* (New) The [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) package can help you maximize the utility out of the expensive LLMs such as ChatGPT and GPT-4, including:
+    - A drop-in replacement of `openai.Completion` or `openai.ChatCompletion` with powerful functionalites like tuning, caching, templating, filtering. For example, you can optimize generations by LLM with your own tuning data, success metrics and budgets.
+    ```python
+    from flaml import oai
+
+    # perform tuning
+    config, analysis = oai.Completion.tune(
+        data=tune_data,
+        metric="success",
+        mode="max",
+        eval_func=eval_func,
+        inference_budget=0.05,
+        optimization_budget=3,
+        num_samples=-1,
+    )
+
+    # perform inference for a test instance
+    response = oai.Completion.create(context=test_instance, **config)
+    ```
+    - LLM-driven intelligent agents which can perform tasks autonomously or with human feedback, including tasks that require using tools via code.
+    ```python
+    assistant = AssistantAgent("assistant")
+    user = UserProxyAgent("user", human_input_mode="TERMINATE")
+    assistant.receive("Draw a rocket and save to a file named 'rocket.svg'")
+    ```
 * With three lines of code, you can start using this economical and fast
 AutoML engine as a [scikit-learn style estimator](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
 
 ```python
 from flaml import AutoML
 automl = AutoML()
 automl.fit(X_train, y_train, task="classification")
@@ -146,19 +156,19 @@
 
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
-- Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
+- [Research](https://microsoft.github.io/FLAML/docs/Research) and [blogposts](https://microsoft.github.io/FLAML/blog) around FLAML.
 
-- Discord [here](https://discord.gg/Cppx2vSPVP).
+- [Discord](https://discord.gg/Cppx2vSPVP).
 
-- Contributing guide [here](https://microsoft.github.io/FLAML/docs/Contribute).
+- [Contributing guide](https://microsoft.github.io/FLAML/docs/Contribute).
 
 - ML.NET documentation and tutorials for [Model Builder](https://learn.microsoft.com/dotnet/machine-learning/tutorials/predict-prices-with-model-builder), [ML.NET CLI](https://learn.microsoft.com/dotnet/machine-learning/tutorials/sentiment-analysis-cli), and [AutoML API](https://learn.microsoft.com/dotnet/machine-learning/how-to-guides/how-to-use-the-automl-api).
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
```

### Comparing `FLAML-1.2.4/README.md` & `FLAML-2.0.0rc1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: v1.2.0 is released with support for ChatGPT and GPT-4.
+:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web)
+:fire: [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) is released with support for ChatGPT and GPT-4, based on [Cost-Effective Hyperparameter Optimization for Large Language Model Generation Inference](https://arxiv.org/abs/2303.04673).
+:fire: FLAML supports AutoML and Hyperparameter Tuning features in [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview) private preview. Sign up for these features at: https://aka.ms/fabric/data-science/sign-up.
 
 
 ## What is FLAML
 FLAML is a lightweight Python library for efficient automation of machine
-learning, including selection of
+learning and AI operations, including selection of
 models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
 
-* For foundation models like the GPT series, it automates the experimentation and optimization of their inference performance to maximize the effectiveness for downstream applications and minimize the inference cost.
-* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources.
-* It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training/inference/evaluation code).
-* It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
+* For foundation models like the GPT models, it automates the experimentation and optimization of their performance to maximize the effectiveness for applications and minimize the inference cost. FLAML enables users to build and use adaptive AI agents with minimal effort.
+* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., search space and metric), or full customization (arbitrary training/inference/evaluation code).
+* It supports fast and economical automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
 and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
@@ -38,50 +39,57 @@
 
 FLAML requires **Python version >= 3.7**. It can be installed from pip:
 
 ```bash
 pip install flaml
 ```
 
-To run the [`notebook examples`](https://github.com/microsoft/FLAML/tree/main/notebook),
-install flaml with the [notebook] option:
-
+Minimal dependencies are installed without extra options. You can install extra options based on the feature you need. For example, use the following to install the dependencies needed by the [`autogen`](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) package.
 ```bash
-pip install flaml[notebook]
+pip install "flaml[autogen]"
 ```
 
+Find more options in [Installation](Installation).
+Each of the [`notebook examples`](https://github.com/microsoft/FLAML/tree/main/notebook) may require a specific option to be installed.
+
 ### .NET
 
 Use the following guides to get started with FLAML in .NET:
 
 - [Install Model Builder](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-model-builder?tabs=visual-studio-2022)
 - [Install ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-ml-net-cli?tabs=windows)
 - [Microsoft.AutoML](https://www.nuget.org/packages/Microsoft.ML.AutoML/0.20.0)
 
 ## Quickstart
 
-* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
-
-```python
-from flaml import oai
-
-config, analysis = oai.Completion.tune(
-    data=tune_data,
-    metric="success",
-    mode="max",
-    eval_func=eval_func,
-    inference_budget=0.05,
-    optimization_budget=3,
-    num_samples=-1,
-)
-```
-
-The automated experimentation and optimization can help you maximize the utility out of these expensive models.
-A suite of utilities such as caching and templating are offered to accelerate the experimentation and application development.
-
+* (New) The [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) package can help you maximize the utility out of the expensive LLMs such as ChatGPT and GPT-4, including:
+    - A drop-in replacement of `openai.Completion` or `openai.ChatCompletion` with powerful functionalites like tuning, caching, templating, filtering. For example, you can optimize generations by LLM with your own tuning data, success metrics and budgets.
+    ```python
+    from flaml import oai
+
+    # perform tuning
+    config, analysis = oai.Completion.tune(
+        data=tune_data,
+        metric="success",
+        mode="max",
+        eval_func=eval_func,
+        inference_budget=0.05,
+        optimization_budget=3,
+        num_samples=-1,
+    )
+
+    # perform inference for a test instance
+    response = oai.Completion.create(context=test_instance, **config)
+    ```
+    - LLM-driven intelligent agents which can perform tasks autonomously or with human feedback, including tasks that require using tools via code.
+    ```python
+    assistant = AssistantAgent("assistant")
+    user = UserProxyAgent("user", human_input_mode="TERMINATE")
+    assistant.receive("Draw a rocket and save to a file named 'rocket.svg'")
+    ```
 * With three lines of code, you can start using this economical and fast
 AutoML engine as a [scikit-learn style estimator](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
 
 ```python
 from flaml import AutoML
 automl = AutoML()
 automl.fit(X_train, y_train, task="classification")
@@ -114,19 +122,19 @@
 
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
-- Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
+- [Research](https://microsoft.github.io/FLAML/docs/Research) and [blogposts](https://microsoft.github.io/FLAML/blog) around FLAML.
 
-- Discord [here](https://discord.gg/Cppx2vSPVP).
+- [Discord](https://discord.gg/Cppx2vSPVP).
 
-- Contributing guide [here](https://microsoft.github.io/FLAML/docs/Contribute).
+- [Contributing guide](https://microsoft.github.io/FLAML/docs/Contribute).
 
 - ML.NET documentation and tutorials for [Model Builder](https://learn.microsoft.com/dotnet/machine-learning/tutorials/predict-prices-with-model-builder), [ML.NET CLI](https://learn.microsoft.com/dotnet/machine-learning/tutorials/sentiment-analysis-cli), and [AutoML API](https://learn.microsoft.com/dotnet/machine-learning/how-to-guides/how-to-use-the-automl-api).
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
```

### Comparing `FLAML-1.2.4/flaml/autogen/agent/agent.py` & `FLAML-2.0.0rc1/flaml/autogen/agent/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,16 +33,17 @@
     def _send(self, message, recipient):
         """Send a message to another agent."""
         self._conversations[recipient.name].append({"content": message, "role": "assistant"})
         recipient.receive(message, self)
 
     def _receive(self, message, sender):
         """Receive a message from another agent."""
-        print("\n****", self.name, "received message from", sender.name, "****\n")
-        print(message)
+        print("\n", "-" * 80, "\n", flush=True)
+        print(sender.name, "(to", f"{self.name}):", flush=True)
+        print(message, flush=True)
         self._conversations[sender.name].append({"content": message, "role": "user"})
 
     def receive(self, message, sender):
         """Receive a message from another agent.
         This method is called by the sender.
         It needs to be overriden by the subclass to perform followup actions.
         """
```

### Comparing `FLAML-1.2.4/flaml/autogen/agent/coding_agent.py` & `FLAML-2.0.0rc1/flaml/autogen/agent/assistant_agent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from .agent import Agent
 from flaml.autogen.code_utils import DEFAULT_MODEL
 from flaml import oai
 
 
-class PythonAgent(Agent):
-    """(Experimental) Suggest code blocks."""
+class AssistantAgent(Agent):
+    """(Experimental) Assistant agent, able to suggest code blocks."""
 
-    DEFAULT_SYSTEM_MESSAGE = """You suggest python code (in a python coding block) for a user to execute for a given task. If you want the user to save the code in a file before executing it, put # filename: <filename> inside the code block as the first line. Finish the task smartly. Don't suggest shell command. Don't include multiple code blocks in one response. Use 'print' function for the output when relevant. Check the execution result returned by the user.
-    If the result indicates there is an error, fix the error and output the code again.
-    Reply "TERMINATE" in the end when the task is done.
+    DEFAULT_SYSTEM_MESSAGE = """You are a helpful AI assistant.
+    In the following cases, suggest python code (in a python coding block) or shell script (in a sh coding block) for the user to execute. You must indicate the script type in the code block.
+    1. When you need to ask the user for some info, use the code to output the info you need, for example, browse or search the web, download/read a file.
+    2. When you need to perform some task with code, use the code to perform the task and output the result. Finish the task smartly. Solve the task step by step if you need to.
+    If you want the user to save the code in a file before executing it, put # filename: <filename> inside the code block as the first line. Don't include multiple code blocks in one response. Do not ask users to copy and paste the result. Instead, use 'print' function for the output when relevant. Check the execution result returned by the user.
+    If the result indicates there is an error, fix the error and output the code again. Suggeset the full code instead of partial code or code changes.
+    Reply "TERMINATE" in the end when everything is done.
     """
 
     DEFAULT_CONFIG = {
         "model": DEFAULT_MODEL,
     }
 
     def __init__(self, name, system_message=DEFAULT_SYSTEM_MESSAGE, **config):
         """
         Args:
-            name (str): agent name
-            system_message (str): system message to be sent to the agent
-            config (dict): other configurations.
+            name (str): agent name.
+            system_message (str): system message to be sent to the agent.
+            **config (dict): other configurations allowed in
+              [oai.Completion.create](../oai/Completion#create).
+              These configurations will be used when invoking LLM.
         """
         super().__init__(name, system_message)
         self._config = self.DEFAULT_CONFIG.copy()
         self._config.update(config)
         self._sender_dict = {}
 
     def receive(self, message, sender):
```

### Comparing `FLAML-1.2.4/flaml/autogen/agent/user_proxy_agent.py` & `FLAML-2.0.0rc1/flaml/autogen/agent/user_proxy_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .agent import Agent
-from flaml.autogen.code_utils import extract_code, execute_code
+from flaml.autogen.code_utils import UNKNOWN, extract_code, execute_code, infer_lang
 from collections import defaultdict
 
 
 class UserProxyAgent(Agent):
     """(Experimental) A proxy agent for the user, that can execute code and provide feedback to the other agents."""
 
     MAX_CONSECUTIVE_AUTO_REPLY = 100  # maximum number of consecutive auto replies (subject to future change)
@@ -20,74 +20,89 @@
         **config,
     ):
         """
         Args:
             name (str): name of the agent
             system_message (str): system message to be sent to the agent
             work_dir (str): working directory for the agent
-            human_input_mode (bool): whether to ask for human inputs every time a message is received.
+            human_input_mode (str): whether to ask for human inputs every time a message is received.
                 Possible values are "ALWAYS", "TERMINATE", "NEVER".
                 (1) When "ALWAYS", the agent prompts for human input every time a message is received.
                     Under this mode, the conversation stops when the human input is "exit",
                     or when is_termination_msg is True and there is no human input.
                 (2) When "TERMINATE", the agent only prompts for human input only when a termination message is received or
                     the number of auto reply reaches the max_consecutive_auto_reply.
                 (3) When "NEVER", the agent will never prompt for human input. Under this mode, the conversation stops
                     when the number of auto reply reaches the max_consecutive_auto_reply or or when is_termination_msg is True.
             max_consecutive_auto_reply (int): the maximum number of consecutive auto replies.
-                default: None (no limit provided, class attribute MAX_CONSECUTIVE_AUTO_REPLY will be used as the limit in this case).
+                default to None (no limit provided, class attribute MAX_CONSECUTIVE_AUTO_REPLY will be used as the limit in this case).
                 The limit only plays a role when human_input_mode is not "ALWAYS".
             is_termination_msg (function): a function that takes a message and returns a boolean value.
                 This function is used to determine if a received message is a termination message.
-            config (dict): other configurations.
-
+            use_docker (bool): whether to use docker to execute the code.
+            **config (dict): other configurations.
         """
         super().__init__(name, system_message)
         self._work_dir = work_dir
         self._human_input_mode = human_input_mode
         self._is_termination_msg = (
             is_termination_msg if is_termination_msg is not None else (lambda x: x == "TERMINATE")
         )
         self._config = config
         self._max_consecutive_auto_reply = (
             max_consecutive_auto_reply if max_consecutive_auto_reply is not None else self.MAX_CONSECUTIVE_AUTO_REPLY
         )
         self._consecutive_auto_reply_counter = defaultdict(int)
         self._use_docker = use_docker
 
-    def _execute_code(self, code, lang):
+    def _execute_code(self, code_blocks):
         """Execute the code and return the result."""
-        if lang in ["bash", "shell"]:
-            if not code.startswith("python "):
-                return 1, f"please do not suggest bash or shell commands like {code}"
-            file_name = code[len("python ") :]
-            exitcode, logs = execute_code(filename=file_name, work_dir=self._work_dir, use_docker=self._use_docker)
-            logs = logs.decode("utf-8")
-        elif lang == "python":
-            if code.startswith("# filename: "):
-                filename = code[11 : code.find("\n")].strip()
+        logs_all = ""
+        for code_block in code_blocks:
+            lang, code = code_block
+            if not lang:
+                lang = infer_lang(code)
+            if lang in ["bash", "shell", "sh"]:
+                # if code.startswith("python "):
+                #     # return 1, f"please do not suggest bash or shell commands like {code}"
+                #     file_name = code[len("python ") :]
+                #     exitcode, logs = execute_code(filename=file_name, work_dir=self._work_dir, use_docker=self._use_docker)
+                # else:
+                exitcode, logs, image = execute_code(
+                    code, work_dir=self._work_dir, use_docker=self._use_docker, lang=lang
+                )
+                logs = logs.decode("utf-8")
+            elif lang == "python":
+                if code.startswith("# filename: "):
+                    filename = code[11 : code.find("\n")].strip()
+                else:
+                    filename = None
+                exitcode, logs, image = execute_code(
+                    code, work_dir=self._work_dir, filename=filename, use_docker=self._use_docker
+                )
+                logs = logs.decode("utf-8")
             else:
-                filename = None
-            exitcode, logs = execute_code(code, work_dir=self._work_dir, filename=filename, use_docker=self._use_docker)
-            logs = logs.decode("utf-8")
-        else:
-            # TODO: could this happen?
-            exitcode, logs = 1, f"unknown language {lang}"
-            # raise NotImplementedError
-        return exitcode, logs
+                # TODO: could this happen?
+                exitcode, logs, image = 1, f"unknown language {lang}"
+                # raise NotImplementedError
+            self._use_docker = image
+            logs_all += "\n" + logs
+            if exitcode != 0:
+                return exitcode, logs_all
+        return exitcode, logs_all
 
     def auto_reply(self, message, sender, default_reply=""):
         """Generate an auto reply."""
-        code, lang = extract_code(message)
-        if lang == "unknown":
-            # no code block is found, lang should be "unknown"
+        code_blocks = extract_code(message)
+        if len(code_blocks) == 1 and code_blocks[0][0] == UNKNOWN:
+            # no code block is found, lang should be `UNKNOWN``
             self._send(default_reply, sender)
         else:
             # try to execute the code
-            exitcode, logs = self._execute_code(code, lang)
+            exitcode, logs = self._execute_code(code_blocks)
             exitcode2str = "execution succeeded" if exitcode == 0 else "execution failed"
             self._send(f"exitcode: {exitcode} ({exitcode2str})\nCode output: {logs}", sender)
 
     def receive(self, message, sender):
         """Receive a message from the sender agent.
         Once a message is received, this function sends a reply to the sender or simply stop.
         The reply can be generated automatically or entered manually by a human.
@@ -107,16 +122,19 @@
                     "Please give feedback to the sender. (Press enter or type 'exit' to stop the conversation): "
                 )
                 reply = reply if reply else "exit"
             else:
                 # this corresponds to the case when self._human_input_mode == "NEVER"
                 reply = "exit"
         if reply == "exit" or (self._is_termination_msg(message) and not reply):
+            # reset the consecutive_auto_reply_counter
+            self._consecutive_auto_reply_counter[sender.name] = 0
             return
-        elif reply:
+        if reply:
             # reset the consecutive_auto_reply_counter
             self._consecutive_auto_reply_counter[sender.name] = 0
             self._send(reply, sender)
             return
 
         self._consecutive_auto_reply_counter[sender.name] += 1
+        print("\n>>>>>>>> NO HUMAN INPUT RECEIVED. USING AUTO REPLY FOR THE USER...", flush=True)
         self.auto_reply(message, sender, default_reply=reply)
```

### Comparing `FLAML-1.2.4/flaml/autogen/code_utils.py` & `FLAML-2.0.0rc1/flaml/autogen/code_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,44 @@
 import time
 from hashlib import md5
 from flaml.autogen import oai, DEFAULT_MODEL, FAST_MODEL
 
 # Regular expression for finding a code block
 CODE_BLOCK_PATTERN = r"```(\w*)\n(.*?)\n```"
 WORKING_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "extensions")
+UNKNOWN = "unknown"
 
 
-def extract_code(text: str, pattern: str = CODE_BLOCK_PATTERN) -> str:
-    # Use a regular expression to find the code block
-    match = re.search(pattern, text, flags=re.DOTALL)
+def infer_lang(code):
+    """infer the language for the code.
+    TODO: make it robust.
+    """
+    if code.startswith("python ") or code.startswith("pip"):
+        return "sh"
+    return "python"
+
+
+def extract_code(text: str, pattern: str = CODE_BLOCK_PATTERN) -> List[Tuple[str, str]]:
+    """Extract code from a text.
+
+    Args:
+        text (str): The text to extract code from.
+        pattern (Optional, str): The regular expression pattern for finding the code block.
+
+    Returns:
+        list: A list of tuples, each containing the language and the code.
+    """
+    # Use a regular expression to find all the code blocks
+    match = re.findall(pattern, text, flags=re.DOTALL)
+    # match = re.search(pattern, text, flags=re.DOTALL)
     # If a match is found, return the code
-    if match:
-        return match.group(2), match.group(1)
+    # if match:
+    #     return match.group(2), match.group(1)
     # If no code block is found, return the whole text
-    return text, "unknown"
+    return match if match else [(UNKNOWN, text)]
 
 
 def generate_code(pattern: str = CODE_BLOCK_PATTERN, **config) -> Tuple[str, float]:
     """Generate code.
 
     Args:
         pattern (Optional, str): The regular expression pattern for finding the code block.
@@ -98,21 +118,30 @@
     return oai.Completion.extract_text(response)[0], response["cost"]
 
 
 def timeout_handler(signum, frame):
     raise TimeoutError("Timed out!")
 
 
+def _cmd(lang):
+    if lang.startswith("python") or lang in ["bash", "sh"]:
+        return lang
+    if lang == "shell":
+        return "sh"
+    raise NotImplementedError(f"{lang} not recognized in code execution")
+
+
 def execute_code(
     code: Optional[str] = None,
     timeout: Optional[int] = 600,
     filename: Optional[str] = None,
     work_dir: Optional[str] = None,
-    use_docker: Optional[bool] = True,
-) -> Tuple[int, bytes]:
+    use_docker: Optional[Union[List[str], str, bool]] = True,
+    lang: Optional[str] = "python",
+) -> Tuple[int, bytes, str]:
     """Execute code in a docker container.
     This function is not tested on MacOS.
 
     Args:
         code (Optional, str): The code to execute.
             If None, the code from the file specified by filename will be executed.
             Either code or filename must be provided.
@@ -121,68 +150,78 @@
             If None, a file with a randomly generated name will be created.
             The randomly generated file will be deleted after execution.
             The file name must be a relative path. Relative paths are relative to the working directory.
         work_dir (Optional, str): The working directory for the code execution.
             If None, a default working directory will be used.
             The default working directory is the "extensions" directory under
             "xxx/flaml/autogen", where "xxx" is the path to the flaml package.
-        use_docker (Optional, bool): Whether to use a docker container for code execution.
-            If True, the code will be executed in a docker container.
-            If False, the code will be executed in the current environment.
-            Default is True. If the code is executed in the current environment,
+        use_docker (Optional, list, str or bool): The docker image to use for code execution.
+            If a list or a str of image name(s) is provided, the code will be executed in a docker container
+              with the first image successfully pulled.
+            If None, False or empty, the code will be executed in the current environment.
+            Default is True, which will be converted into a list.
+            If the code is executed in the current environment,
             the code must be trusted.
+        lang (Optional, str): The language of the code. Default is "python".
 
     Returns:
         int: 0 if the code executes successfully.
         bytes: The error message if the code fails to execute; the stdout otherwise.
+        image: The docker image name after container run when docker is used.
     """
     assert code is not None or filename is not None, "Either code or filename must be provided."
 
     original_filename = filename
     if filename is None:
         code_hash = md5(code.encode()).hexdigest()
         # create a file with a automatically generated name
-        filename = f"tmp_code_{code_hash}.py"
+        filename = f"tmp_code_{code_hash}.{'py' if lang.startswith('python') else lang}"
     if work_dir is None:
         work_dir = WORKING_DIR
     filepath = os.path.join(work_dir, filename)
     file_dir = os.path.dirname(filepath)
     os.makedirs(file_dir, exist_ok=True)
 
     if code is not None:
         with open(filepath, "w") as fout:
             fout.write(code)
     # check if already running in a docker container
     in_docker_container = os.path.exists("/.dockerenv")
     if not use_docker or in_docker_container:
         # already running in a docker container
+        cmd = [sys.executable if lang.startswith("python") else _cmd(lang), filename]
         signal.signal(signal.SIGALRM, timeout_handler)
         try:
             signal.alarm(timeout)
             # run the code in a subprocess in the current docker container in the working directory
             result = subprocess.run(
-                [sys.executable, filename],
+                cmd,
                 cwd=work_dir,
                 capture_output=True,
             )
             signal.alarm(0)
         except TimeoutError:
             if original_filename is None:
                 os.remove(filepath)
-            return 1, "Timeout"
+            return 1, "Timeout", None
         if original_filename is None:
             os.remove(filepath)
-        return result.returncode, result.stderr if result.returncode else result.stdout
+        return result.returncode, result.stderr if result.returncode else result.stdout, None
 
     import docker
-    from requests.exceptions import ReadTimeout, ConnectionError
 
     # create a docker client
     client = docker.from_env()
-    image_list = ["python:3-alpine", "python:3", "python:3-windowsservercore"]
+    image_list = (
+        ["python:3-alpine", "python:3", "python:3-windowsservercore"]
+        if use_docker is True
+        else [use_docker]
+        if isinstance(use_docker, str)
+        else use_docker
+    )
     for image in image_list:
         # check if the image exists
         try:
             client.images.get(image)
             break
         except docker.errors.ImageNotFound:
             # pull the image
@@ -194,47 +233,50 @@
                 print("Failed to pull image", image)
     # get a randomized str based on current time to wrap the exit code
     exit_code_str = f"exitcode{time.time()}"
     abs_path = pathlib.Path(work_dir).absolute()
     # if sys.platform == "win32":
     #     abs_path = str(abs_path).replace("\\", "/")
     #     abs_path = f"/{abs_path[0].lower()}{abs_path[2:]}"
+    cmd = [
+        "sh",
+        "-c",
+        f"{_cmd(lang)} {filename}; exit_code=$?; echo -n {exit_code_str}; echo -n $exit_code; echo {exit_code_str}",
+    ]
     # create a docker container
     container = client.containers.run(
         image,
-        command=[
-            "sh",
-            "-c",
-            f"python {filename}; exit_code=$?; echo -n {exit_code_str}; echo -n $exit_code; echo {exit_code_str}",
-        ],
+        command=cmd,
         working_dir="/workspace",
         detach=True,
         # get absolute path to the working directory
         volumes={abs_path: {"bind": "/workspace", "mode": "rw"}},
     )
     start_time = time.time()
     while container.status != "exited" and time.time() - start_time < timeout:
         # Reload the container object
         container.reload()
     if container.status != "exited":
         container.stop()
         container.remove()
         if original_filename is None:
             os.remove(filepath)
-        return 1, "Timeout"
+        return 1, "Timeout", image
     # try:
     #     container.wait(timeout=timeout)
     # except (ReadTimeout, ConnectionError):
     #     container.stop()
     #     container.remove()
     #     if original_filename is None:
     #         os.remove(filepath)
     #     return 1, "Timeout"
     # get the container logs
     logs = container.logs().decode("utf-8").rstrip()
+    # commit the image
+    container.commit(repository="python", tag=filename.replace("/", ""))
     # remove the container
     container.remove()
     # check if the code executed successfully
     exit_code = container.attrs["State"]["ExitCode"]
     if exit_code == 0:
         # extract the exit code from the logs
         pattern = re.compile(f"{exit_code_str}(\\d+){exit_code_str}")
@@ -242,16 +284,16 @@
         exit_code = int(match.group(1))
         # remove the exit code from the logs
         logs = pattern.sub("", logs)
 
     logs = bytes(logs, "utf-8")
     if original_filename is None:
         os.remove(filepath)
-    # return the exit code and logs
-    return exit_code, logs
+    # return the exit code, logs and image
+    return exit_code, logs, f"python:{filename}"
 
 
 _GENERATE_ASSERTIONS_CONFIG = {
     "prompt": """Given the signature and docstring, write the exactly same number of assertion(s) for the provided example(s) in the docstring, without assertion messages.
 
 func signature:
 {definition}
```

### Comparing `FLAML-1.2.4/flaml/autogen/math_utils.py` & `FLAML-2.0.0rc1/flaml/autogen/math_utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/autogen/oai/completion.py` & `FLAML-2.0.0rc1/flaml/autogen/oai/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                 if isinstance(err, Timeout):
                     if "request_timeout" in config:
                         raise
                     request_timeout <<= 1
                 request_timeout = min(request_timeout, time_left)
                 sleep(cls.retry_time)
             except InvalidRequestError:
-                if "azure" == config.get("api_type", openai.api_type) and "model" in config:
+                if "azure" in config.get("api_type", openai.api_type) and "model" in config:
                     # azure api uses "engine" instead of "model"
                     config["engine"] = config.pop("model").replace("gpt-3.5-turbo", "gpt-35-turbo")
                 else:
                     raise
             else:
                 if use_cache:
                     cls._cache.set(key, response)
```

### Comparing `FLAML-1.2.4/flaml/autogen/oai/openai_utils.py` & `FLAML-2.0.0rc1/flaml/autogen/oai/openai_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,88 +55,134 @@
 
 
 def config_list_openai_aoai(
     key_file_path: Optional[str] = ".",
     openai_api_key_file: Optional[str] = "key_openai.txt",
     aoai_api_key_file: Optional[str] = "key_aoai.txt",
     aoai_api_base_file: Optional[str] = "base_aoai.txt",
+    exclude: Optional[str] = None,
 ) -> List[Dict]:
     """Get a list of configs for openai + azure openai api calls.
 
     Args:
         key_file_path (str, optional): The path to the key files.
         openai_api_key_file (str, optional): The file name of the openai api key.
         aoai_api_key_file (str, optional): The file name of the azure openai api key.
         aoai_api_base_file (str, optional): The file name of the azure openai api base.
+        exclude (str, optional): The api type to exclude, "openai" or "aoai".
 
     Returns:
         list: A list of configs for openai api calls.
     """
-    if "OPENAI_API_KEY" not in os.environ:
+    if "OPENAI_API_KEY" not in os.environ and exclude != "openai":
         try:
-            os.environ["OPENAI_API_KEY"] = open(f"{key_file_path}/{openai_api_key_file}").read().strip()
+            with open(f"{key_file_path}/{openai_api_key_file}") as key_file:
+                os.environ["OPENAI_API_KEY"] = key_file.read().strip()
         except FileNotFoundError:
             logging.info(
                 "To use OpenAI API, please set OPENAI_API_KEY in os.environ "
                 "or create key_openai.txt in the specified path, or specify the api_key in config_list."
             )
-    if "AZURE_OPENAI_API_KEY" not in os.environ:
+    if "AZURE_OPENAI_API_KEY" not in os.environ and exclude != "aoai":
         try:
-            os.environ["AZURE_OPENAI_API_KEY"] = open(f"{key_file_path}/{aoai_api_key_file}").read().strip()
+            with open(f"{key_file_path}/{aoai_api_key_file}") as key_file:
+                os.environ["AZURE_OPENAI_API_KEY"] = key_file.read().strip()
         except FileNotFoundError:
             logging.info(
                 "To use Azure OpenAI API, please set AZURE_OPENAI_API_KEY in os.environ "
                 "or create key_aoai.txt in the specified path, or specify the api_key in config_list."
             )
-    if "AZURE_OPENAI_API_BASE" not in os.environ:
+    if "AZURE_OPENAI_API_BASE" not in os.environ and exclude != "aoai":
         try:
-            os.environ["AZURE_OPENAI_API_BASE"] = open(f"{key_file_path}/{aoai_api_base_file}").read().strip()
+            with open(f"{key_file_path}/{aoai_api_base_file}") as key_file:
+                os.environ["AZURE_OPENAI_API_BASE"] = key_file.read().strip()
         except FileNotFoundError:
             logging.info(
                 "To use Azure OpenAI API, please set AZURE_OPENAI_API_BASE in os.environ "
                 "or create base_aoai.txt in the specified path, or specify the api_base in config_list."
             )
-    aoai_config = get_config_list(
-        # Assuming Azure OpenAI api keys in os.environ["AZURE_OPENAI_API_KEY"], in separated lines
-        api_keys=os.environ.get("AZURE_OPENAI_API_KEY", "").split("\n"),
-        # Assuming Azure OpenAI api bases in os.environ["AZURE_OPENAI_API_BASE"], in separated lines
-        api_bases=os.environ.get("AZURE_OPENAI_API_BASE", "").split("\n"),
-        api_type="azure",
-        api_version="2023-03-15-preview",  # change if necessary
+    aoai_config = (
+        get_config_list(
+            # Assuming Azure OpenAI api keys in os.environ["AZURE_OPENAI_API_KEY"], in separated lines
+            api_keys=os.environ.get("AZURE_OPENAI_API_KEY", "").split("\n"),
+            # Assuming Azure OpenAI api bases in os.environ["AZURE_OPENAI_API_BASE"], in separated lines
+            api_bases=os.environ.get("AZURE_OPENAI_API_BASE", "").split("\n"),
+            api_type="azure",
+            api_version="2023-03-15-preview",  # change if necessary
+        )
+        if exclude != "aoai"
+        else []
     )
-    openai_config = get_config_list(
-        # Assuming OpenAI API_KEY in os.environ["OPENAI_API_KEY"]
-        api_keys=os.environ.get("OPENAI_API_KEY", "").split("\n"),
-        # "api_type": "open_ai",
-        # "api_base": "https://api.openai.com/v1",
+    openai_config = (
+        get_config_list(
+            # Assuming OpenAI API_KEY in os.environ["OPENAI_API_KEY"]
+            api_keys=os.environ.get("OPENAI_API_KEY", "").split("\n"),
+            # "api_type": "open_ai",
+            # "api_base": "https://api.openai.com/v1",
+        )
+        if exclude != "openai"
+        else []
     )
     config_list = openai_config + aoai_config
     return config_list
 
 
+def config_list_from_models(
+    key_file_path: Optional[str] = ".",
+    openai_api_key_file: Optional[str] = "key_openai.txt",
+    aoai_api_key_file: Optional[str] = "key_aoai.txt",
+    aoai_api_base_file: Optional[str] = "base_aoai.txt",
+    exclude: Optional[str] = None,
+    model_list: Optional[list] = None,
+) -> List[Dict]:
+    """Get a list of configs for api calls with models in the model list.
+
+    Args:
+        key_file_path (str, optional): The path to the key files.
+        openai_api_key_file (str, optional): The file name of the openai api key.
+        aoai_api_key_file (str, optional): The file name of the azure openai api key.
+        aoai_api_base_file (str, optional): The file name of the azure openai api base.
+        exclude (str, optional): The api type to exclude, "openai" or "aoai".
+        model_list (list, optional): The model list.
+
+    Returns:
+        list: A list of configs for openai api calls.
+    """
+    config_list = config_list_openai_aoai(
+        key_file_path,
+        openai_api_key_file,
+        aoai_api_key_file,
+        aoai_api_base_file,
+        exclude,
+    )
+    if model_list:
+        config_list = [{**config, "model": model} for config in config_list for model in model_list]
+    return config_list
+
+
 def config_list_gpt4_gpt35(
     key_file_path: Optional[str] = ".",
     openai_api_key_file: Optional[str] = "key_openai.txt",
     aoai_api_key_file: Optional[str] = "key_aoai.txt",
     aoai_api_base_file: Optional[str] = "base_aoai.txt",
+    exclude: Optional[str] = None,
 ) -> List[Dict]:
     """Get a list of configs for gpt-4 followed by gpt-3.5 api calls.
 
     Args:
         key_file_path (str, optional): The path to the key files.
         openai_api_key_file (str, optional): The file name of the openai api key.
         aoai_api_key_file (str, optional): The file name of the azure openai api key.
         aoai_api_base_file (str, optional): The file name of the azure openai api base.
+        exclude (str, optional): The api type to exclude, "openai" or "aoai".
 
     Returns:
         list: A list of configs for openai api calls.
     """
-
-    config_list = config_list_openai_aoai(
+    return config_list_from_models(
         key_file_path,
         openai_api_key_file,
         aoai_api_key_file,
         aoai_api_base_file,
+        exclude,
+        model_list=["gpt-4", "gpt-3.5-turbo"],
     )
-    return [{**config, "model": "gpt-4"} for config in config_list] + [
-        {**config, "model": "gpt-3.5-turbo"} for config in config_list
-    ]
```

### Comparing `FLAML-1.2.4/flaml/automl/automl.py` & `FLAML-2.0.0rc1/flaml/automl/automl.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from __future__ import annotations
 import time
 import os
 import sys
 from typing import Callable, List, Union, Optional
 from functools import partial
 import numpy as np
-from sklearn.base import BaseEstimator
-import pandas as pd
 import logging
 import json
 
 from flaml.automl.state import SearchState, AutoMLState
 from flaml.automl.ml import (
     train_estimator,
     get_estimator_class,
@@ -34,55 +32,36 @@
 from flaml.automl.task.task import CLASSIFICATION, TS_FORECAST, Task
 from flaml.automl.task.factory import task_factory
 from flaml import tune
 from flaml.automl.logger import logger, logger_formatter
 from flaml.automl.training_log import training_log_reader, training_log_writer
 from flaml.default import suggest_learner
 from flaml.version import __version__ as flaml_version
+from flaml.automl.spark import psDataFrame, psSeries, DataFrame, Series
 from flaml.tune.spark.utils import check_spark, get_broadcast_data
 
+ERROR = (
+    DataFrame is None and ImportError("please install flaml[automl] option to use the flaml.automl package.") or None
+)
+
 try:
-    from flaml.automl.spark.utils import (
-        train_test_split_pyspark,
-        unique_pandas_on_spark,
-        len_labels,
-        unique_value_first_index,
-    )
-except ImportError:
-    train_test_split_pyspark = None
-    unique_pandas_on_spark = None
-    from flaml.automl.utils import (
-        len_labels,
-        unique_value_first_index,
-    )
-try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    import pyspark.pandas as ps
-    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
-    from pyspark.pandas.config import set_option, reset_option
+    from sklearn.base import BaseEstimator
 except ImportError:
-    ps = None
-
-    class psDataFrame:
-        pass
-
-    class psSeries:
-        pass
-
+    BaseEstimator = object
+    ERROR = ERROR or ImportError("please install flaml[automl] option to use the flaml.automl package.")
 
 try:
     import mlflow
 except ImportError:
     mlflow = None
 
 try:
     from ray import __version__ as ray_version
 
     assert ray_version >= "1.10.0"
-
     ray_available = True
 except (ImportError, AssertionError):
     ray_available = False
 
 
 def size(learner_classes: dict, config: dict) -> float:
     """Size function.
@@ -342,14 +321,16 @@
         }
         ```
             mlflow_logging: boolean, default=True | Whether to log the training results to mlflow.
                 This requires mlflow to be installed and to have an active mlflow run.
                 FLAML will create nested runs.
 
         """
+        if ERROR:
+            raise ERROR
         self._track_iter = 0
         self._state = AutoMLState()
         self._state.learner_classes = {}
         self._settings = settings
         # no budget by default
         settings["time_budget"] = settings.get("time_budget", -1)
         settings["task"] = settings.get("task", "classification")
@@ -536,30 +517,30 @@
     @property
     def time_to_find_best_model(self) -> float:
         """Time taken to find best model in seconds."""
         return self.__dict__.get("_time_taken_best_iter")
 
     def score(
         self,
-        X: Union[pd.DataFrame, psDataFrame],
-        y: Union[pd.Series, psSeries],
+        X: Union[DataFrame, psDataFrame],
+        y: Union[Series, psSeries],
         **kwargs,
     ):
         estimator = getattr(self, "_trained_estimator", None)
         if estimator is None:
             logger.warning("No estimator is trained. Please run fit with enough budget.")
             return None
         X = self._state.task.preprocess(X, self._transformer)
         if self._label_transformer:
             y = self._label_transformer.transform(y)
         return estimator.score(X, y, **kwargs)
 
     def predict(
         self,
-        X: Union[np.array, pd.DataFrame, List[str], List[List[str]], psDataFrame],
+        X: Union[np.array, DataFrame, List[str], List[List[str]], psDataFrame],
         **pred_kwargs,
     ):
         """Predict label from features.
 
         Args:
             X: A numpy array or pandas dataframe or pyspark.pandas dataframe
             of featurized instances, shape n * m,
@@ -570,15 +551,15 @@
                     arima or sarimax). Other columns in the dataframe
                     are assumed to be exogenous variables (categorical
                     or numeric).
             **pred_kwargs: Other key word arguments to pass to predict() function of
                 the searched learners, such as per_device_eval_batch_size.
 
         ```python
-        multivariate_X_test = pd.DataFrame({
+        multivariate_X_test = DataFrame({
             'timeStamp': pd.date_range(start='1/1/2022', end='1/07/2022'),
             'categorical_col': ['yes', 'yes', 'no', 'no', 'yes', 'no', 'yes'],
             'continuous_col': [105, 107, 120, 118, 110, 112, 115]
         })
         model.predict(multivariate_X_test)
         ```
 
@@ -592,15 +573,15 @@
             return None
         X = self._state.task.preprocess(X, self._transformer)
         y_pred = estimator.predict(X, **pred_kwargs)
 
         if isinstance(y_pred, np.ndarray) and y_pred.ndim > 1 and isinstance(y_pred, np.ndarray):
             y_pred = y_pred.flatten()
         if self._label_transformer:
-            return self._label_transformer.inverse_transform(pd.Series(y_pred.astype(int)))
+            return self._label_transformer.inverse_transform(Series(y_pred.astype(int)))
         else:
             return y_pred
 
     def predict_proba(self, X, **pred_kwargs):
         """Predict the probability of each class from features, only works for
         classification problems.
```

### Comparing `FLAML-1.2.4/flaml/automl/data.py` & `FLAML-2.0.0rc1/flaml/automl/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,22 @@
 # !
 #  * Copyright (c) Microsoft Corporation. All rights reserved.
 #  * Licensed under the MIT License. See LICENSE file in the
 #  * project root for license information.
 import numpy as np
-from scipy.sparse import vstack, issparse
-import pandas as pd
-from pandas import DataFrame, Series
-
-from flaml.automl.training_log import training_log_reader
-
 from datetime import datetime
 from typing import TYPE_CHECKING, Union
-
 import os
+from flaml.automl.training_log import training_log_reader
+from flaml.automl.spark import ps, psDataFrame, psSeries, DataFrame, Series, pd
 
 try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    import pyspark.pandas as ps
-    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
+    from scipy.sparse import vstack, issparse
 except ImportError:
-    ps = None
-
-    class psDataFrame:
-        pass
-
-    class psSeries:
-        pass
-
+    pass
 
 if TYPE_CHECKING:
     from flaml.automl.task import Task
 
 TS_TIMESTAMP_COL = "ds"
 TS_VALUE_COL = "y"
 
@@ -51,15 +37,14 @@
 
     Returns:
         X_train: Training data.
         X_test:  Test data.
         y_train: A series or array of labels for training data.
         y_test:  A series or array of labels for test data.
     """
-    import os
     import openml
     import pickle
     from sklearn.model_selection import train_test_split
 
     filename = "openml_ds" + str(dataset_id) + ".pkl"
     filepath = os.path.join(data_dir, filename)
     if os.path.isfile(filepath):
@@ -104,15 +89,14 @@
 
     Returns:
         X_train: A dataframe of training data.
         X_test:  A dataframe of test data.
         y_train: A series of labels for training data.
         y_test:  A series of labels for test data.
     """
-    import os
     import openml
     import pickle
 
     task = openml.tasks.get_task(task_id)
     filename = "openml_task" + str(task_id) + ".pkl"
     filepath = os.path.join(data_dir, filename)
     if os.path.isfile(filepath):
```

### Comparing `FLAML-1.2.4/flaml/automl/ml.py` & `FLAML-2.0.0rc1/flaml/automl/ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 # !
 #  * Copyright (c) FLAML authors. All rights reserved.
 #  * Licensed under the MIT License. See LICENSE file in the
 #  * project root for license information.
-import os
 import time
 import numpy as np
-import pandas as pd
 from typing import Union, Callable, TypeVar, Optional, Tuple
-
-from sklearn.metrics import (
-    mean_squared_error,
-    r2_score,
-    roc_auc_score,
-    accuracy_score,
-    mean_absolute_error,
-    log_loss,
-    average_precision_score,
-    f1_score,
-    mean_absolute_percentage_error,
-    ndcg_score,
-)
 from flaml.automl.model import (
     XGBoostSklearnEstimator,
     XGBoost_TS,
     XGBoostLimitDepthEstimator,
     XGBoostLimitDepth_TS,
     RandomForestEstimator,
     RF_TS,
@@ -43,35 +28,34 @@
     TemporalFusionTransformerEstimator,
     TransformersEstimatorModelSelection,
     SparkLGBMEstimator,
 )
 from flaml.automl.data import group_counts
 from flaml.automl.task.task import TS_FORECAST, Task
 from flaml.automl.model import BaseEstimator
+from flaml.automl.spark import psDataFrame, psSeries, ERROR as SPARK_ERROR, Series
 
 try:
-    from flaml.automl.spark.utils import len_labels
-except ImportError:
-    from flaml.automl.utils import len_labels
-try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    from pyspark.sql.functions import col
-    import pyspark.pandas as ps
-    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
-    from flaml.automl.spark.utils import to_pandas_on_spark, iloc_pandas_on_spark
-    from flaml.automl.spark.metrics import spark_metric_loss_score
+    from sklearn.metrics import (
+        mean_squared_error,
+        r2_score,
+        roc_auc_score,
+        accuracy_score,
+        mean_absolute_error,
+        log_loss,
+        average_precision_score,
+        f1_score,
+        mean_absolute_percentage_error,
+        ndcg_score,
+    )
 except ImportError:
-    ps = None
-
-    class psDataFrame:
-        pass
-
-    class psSeries:
-        pass
+    pass
 
+if SPARK_ERROR is None:
+    from flaml.automl.spark.metrics import spark_metric_loss_score
 
 EstimatorSubclass = TypeVar("EstimatorSubclass", bound=BaseEstimator)
 
 sklearn_metric_name_set = {
     "r2",
     "rmse",
     "mae",
@@ -205,15 +189,15 @@
             metric = datasets.load_metric(datasets_metric_name)
             metric_mode = huggingface_metric_to_mode[datasets_metric_name]
 
             if metric_name.startswith("seqeval"):
                 y_processed_true = [[labels[tr] for tr in each_list] for each_list in y_processed_true]
             elif metric in ("pearsonr", "spearmanr"):
                 y_processed_true = (
-                    y_processed_true.to_list() if isinstance(y_processed_true, pd.Series) else list(y_processed_true)
+                    y_processed_true.to_list() if isinstance(y_processed_true, Series) else list(y_processed_true)
                 )
             score_dict = metric.compute(predictions=y_processed_predict, references=y_processed_true)
             if "rouge" in metric_name:
                 score = score_dict[metric_name].mid.fmeasure
             elif metric_name.startswith("seqeval"):
                 metric_submetric_names = metric_name.split(":")
                 score = score_dict[metric_submetric_names[1] if len(metric_submetric_names) > 1 else "overall_accuracy"]
@@ -608,15 +592,15 @@
         train_time = estimator.fit(X_train, y_train, budget, free_mem_ratio, **fit_kwargs)
     else:
         estimator = estimator.estimator_class(**estimator.params)
     train_time = time.time() - start_time
     return estimator, train_time
 
 
-def norm_confusion_matrix(y_true: Union[np.array, pd.Series], y_pred: Union[np.array, pd.Series]):
+def norm_confusion_matrix(y_true: Union[np.array, Series], y_pred: Union[np.array, Series]):
     """normalized confusion matrix.
 
     Args:
         estimator: A multi-class classification estimator.
         y_true: A numpy array or a pandas series of true labels.
         y_pred: A numpy array or a pandas series of predicted labels.
 
@@ -627,16 +611,16 @@
 
     conf_mat = confusion_matrix(y_true, y_pred)
     norm_conf_mat = conf_mat.astype("float") / conf_mat.sum(axis=1)[:, np.newaxis]
     return norm_conf_mat
 
 
 def multi_class_curves(
-    y_true: Union[np.array, pd.Series],
-    y_pred_proba: Union[np.array, pd.Series],
+    y_true: Union[np.array, Series],
+    y_pred_proba: Union[np.array, Series],
     curve_func: Callable,
 ):
     """Binarize the data for multi-class tasks and produce ROC or precision-recall curves.
 
     Args:
         y_true: A numpy array or a pandas series of true labels.
         y_pred_proba: A numpy array or a pandas dataframe of predicted probabilites.
```

### Comparing `FLAML-1.2.4/flaml/automl/model.py` & `FLAML-2.0.0rc1/flaml/automl/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,16 @@
 from contextlib import contextmanager
 from functools import partial
 import signal
 import os
 from typing import Callable, List, Union
 import numpy as np
 import time
-from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
-from sklearn.ensemble import ExtraTreesRegressor, ExtraTreesClassifier
-from sklearn.linear_model import LogisticRegression
-from sklearn.dummy import DummyClassifier, DummyRegressor
-from scipy.sparse import issparse
 import logging
 import shutil
-from pandas import DataFrame, Series, to_datetime
 import sys
 import math
 from flaml import tune
 from flaml.automl.data import (
     group_counts,
     add_time_idx_col,
     TS_TIMESTAMP_COL,
@@ -33,44 +27,36 @@
     SEQREGRESSION,
     TOKENCLASSIFICATION,
     SUMMARIZATION,
     NLG_TASKS,
 )
 
 try:
-    from flaml.automl.spark.utils import len_labels, to_pandas_on_spark
+    from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
+    from sklearn.ensemble import ExtraTreesRegressor, ExtraTreesClassifier
+    from sklearn.linear_model import LogisticRegression
+    from sklearn.dummy import DummyClassifier, DummyRegressor
 except ImportError:
-    from flaml.automl.utils import len_labels
+    pass
 
-    to_pandas_on_spark = None
+try:
+    from scipy.sparse import issparse
+except ImportError:
+    pass
+
+from flaml.automl.spark import psDataFrame, sparkDataFrame, psSeries, ERROR as SPARK_ERROR, DataFrame, Series
+from flaml.automl.spark.utils import len_labels, to_pandas_on_spark
 from flaml.automl.spark.configs import (
     ParamList_LightGBM_Classifier,
     ParamList_LightGBM_Regressor,
     ParamList_LightGBM_Ranker,
 )
 
-try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    from pyspark.sql.dataframe import DataFrame as sparkDataFrame
-    from pyspark.sql import SparkSession
-    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
-
-    _have_spark = True
-except ImportError:
-    _have_spark = False
-
-    class psDataFrame:
-        pass
-
-    class psSeries:
-        pass
-
-    class sparkDataFrame:
-        pass
-
+if DataFrame is not None:
+    from pandas import to_datetime
 
 try:
     import psutil
 except ImportError:
     psutil = None
 try:
     import resource
@@ -411,16 +397,16 @@
         return params
 
 
 class SparkEstimator(BaseEstimator):
     """The base class for fine-tuning spark models, using pyspark.ml and SynapseML API."""
 
     def __init__(self, task="binary", **config):
-        if not _have_spark:
-            raise ImportError("pyspark is not installed. Try `pip install flaml[spark]`.")
+        if SPARK_ERROR:
+            raise SPARK_ERROR
         super().__init__(task, **config)
         self.df_train = None
 
     def _preprocess(
         self,
         X_train: Union[psDataFrame, sparkDataFrame],
         y_train: psSeries = None,
```

### Comparing `FLAML-1.2.4/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/trainer.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/training_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 from dataclasses import dataclass, field
-
-from flaml.automl.task.task import NLG_TASKS
 from typing import Optional, List
+from flaml.automl.task.task import NLG_TASKS
 
 try:
     from transformers import TrainingArguments
 except ImportError:
     TrainingArguments = object
```

### Comparing `FLAML-1.2.4/flaml/automl/nlp/huggingface/utils.py` & `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import pandas as pd
 from itertools import chain
 import numpy as np
-
 from flaml.automl.task.task import (
     SUMMARIZATION,
     SEQREGRESSION,
     SEQCLASSIFICATION,
     MULTICHOICECLASSIFICATION,
     TOKENCLASSIFICATION,
     NLG_TASKS,
 )
+from flaml.automl.data import pd
 
 
 def todf(X, Y, column_name):
     """
     todf converts Y from any format (list, pandas.Series, numpy array) to a DataFrame before being returned
     """
     if Y is not None:
```

### Comparing `FLAML-1.2.4/flaml/automl/nlp/utils.py` & `FLAML-2.0.0rc1/flaml/automl/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/automl/spark/configs.py` & `FLAML-2.0.0rc1/flaml/automl/spark/configs.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/automl/spark/metrics.py` & `FLAML-2.0.0rc1/flaml/automl/spark/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,20 @@
-import logging
-import os
 import numpy as np
 from typing import Union
+from flaml.automl.spark import psSeries, F
+from pyspark.ml.evaluation import (
+    BinaryClassificationEvaluator,
+    RegressionEvaluator,
+    MulticlassClassificationEvaluator,
+    MultilabelClassificationEvaluator,
+    RankingEvaluator,
+)
 
-try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    from pyspark.sql import DataFrame
-    import pyspark.pandas as ps
-    from pyspark.ml.evaluation import (
-        BinaryClassificationEvaluator,
-        RegressionEvaluator,
-        MulticlassClassificationEvaluator,
-        MultilabelClassificationEvaluator,
-        RankingEvaluator,
-    )
-    import pyspark.sql.functions as F
-except ImportError:
-    msg = """use_spark=True requires installation of PySpark. Please run pip install flaml[spark]
-    and check [here](https://spark.apache.org/docs/latest/api/python/getting_started/install.html)
-    for more details about installing Spark."""
-    raise ImportError(msg)
 
-
-def ps_group_counts(groups: Union[ps.Series, np.ndarray]) -> np.ndarray:
+def ps_group_counts(groups: Union[psSeries, np.ndarray]) -> np.ndarray:
     if isinstance(groups, np.ndarray):
         _, i, c = np.unique(groups, return_counts=True, return_index=True)
     else:
         i = groups.drop_duplicates().index.values
         c = groups.value_counts().sort_index().to_numpy()
     return c[np.argsort(i)].tolist()
 
@@ -44,32 +32,36 @@
     # Create a new column 'prediction' based on the maximum probability value
     df = df.withColumn(prediction_col, max_index_expr.cast("double"))
     return df
 
 
 def spark_metric_loss_score(
     metric_name: str,
-    y_predict: ps.Series,
-    y_true: ps.Series,
-    sample_weight: ps.Series = None,
-    groups: ps.Series = None,
+    y_predict: psSeries,
+    y_true: psSeries,
+    sample_weight: psSeries = None,
+    groups: psSeries = None,
 ) -> float:
     """
     Compute the loss score of a metric for spark models.
 
     Args:
         metric_name: str | the name of the metric.
-        y_predict: ps.Series | the predicted values.
-        y_true: ps.Series | the true values.
-        sample_weight: ps.Series | the sample weights. Default: None.
-        groups: ps.Series | the group of each row. Default: None.
+        y_predict: psSeries | the predicted values.
+        y_true: psSeries | the true values.
+        sample_weight: psSeries | the sample weights. Default: None.
+        groups: psSeries | the group of each row. Default: None.
 
     Returns:
         float | the loss score. A lower value indicates a better model.
     """
+    import warnings
+
+    warnings.filterwarnings("ignore")
+
     label_col = "label"
     prediction_col = "prediction"
     kwargs = {}
 
     y_predict.name = prediction_col
     y_true.name = label_col
     df = y_predict.to_frame().join(y_true)
```

### Comparing `FLAML-1.2.4/flaml/automl/spark/utils.py` & `FLAML-2.0.0rc1/flaml/automl/spark/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 import logging
-import os
 from typing import Union, List, Optional, Tuple
-import pandas as pd
 import numpy as np
+from flaml.automl.spark import (
+    sparkDataFrame,
+    ps,
+    F,
+    T,
+    psDataFrame,
+    psSeries,
+    _spark_major_minor_version,
+    DataFrame,
+    Series,
+    set_option,
+)
 
 logger = logging.getLogger(__name__)
 logger_formatter = logging.Formatter(
     "[%(name)s: %(asctime)s] {%(lineno)d} %(levelname)s - %(message)s", "%m-%d %H:%M:%S"
 )
 logger.propagate = False
-try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    from pyspark.sql import SparkSession
-    from pyspark.sql import DataFrame
-    import pyspark.pandas as ps
-    from pyspark.util import VersionUtils
-    import pyspark.sql.functions as F
-    import pyspark.sql.types as T
-    import pyspark
-
-    _spark_major_minor_version = VersionUtils.majorMinorVersion(pyspark.__version__)
-except ImportError:
-    msg = """use_spark=True requires installation of PySpark. Please run pip install flaml[spark]
-    and check [here](https://spark.apache.org/docs/latest/api/python/getting_started/install.html)
-    for more details about installing Spark."""
-    raise ImportError(msg)
 
 
 def to_pandas_on_spark(
-    df: Union[pd.DataFrame, DataFrame, pd.Series, ps.DataFrame, ps.Series],
+    df: Union[DataFrame, sparkDataFrame, Series, psDataFrame, psSeries],
     index_col: Optional[str] = None,
     default_index_type: Optional[str] = "distributed-sequence",
-) -> Union[ps.DataFrame, ps.Series]:
+) -> Union[psDataFrame, psSeries]:
     """Convert pandas or pyspark dataframe/series to pandas_on_Spark dataframe/series.
 
     Args:
         df: pandas.DataFrame/series or pyspark dataframe | The input dataframe/series.
         index_col: str, optional | The column name to use as index, default None.
         default_index_type: str, optional | The default index type, default "distributed-sequence".
 
     Returns:
         pyspark.pandas.DataFrame/Series: The converted pandas-on-Spark dataframe/series.
 
     ```python
     import pandas as pd
     from flaml.automl.spark.utils import to_pandas_on_spark
 
-    pdf = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+    pdf = DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
     psdf = to_pandas_on_spark(pdf)
     print(psdf)
 
     from pyspark.sql import SparkSession
 
     spark = SparkSession.builder.getOrCreate()
     sdf = spark.createDataFrame(pdf)
     psdf = to_pandas_on_spark(sdf)
     print(psdf)
 
-    pds = pd.Series([1, 2, 3])
+    pds = Series([1, 2, 3])
     pss = to_pandas_on_spark(pds)
     print(pss)
     ```
     """
-    ps.set_option("compute.default_index_type", default_index_type)
-    if isinstance(df, (pd.DataFrame, pd.Series)):
+    set_option("compute.default_index_type", default_index_type)
+    if isinstance(df, (DataFrame, Series)):
         return ps.from_pandas(df)
-    elif isinstance(df, DataFrame):
+    elif isinstance(df, sparkDataFrame):
         if _spark_major_minor_version[0] == 3 and _spark_major_minor_version[1] < 3:
             return df.to_pandas_on_spark(index_col=index_col)
         else:
             return df.pandas_api(index_col=index_col)
-    elif isinstance(df, (ps.DataFrame, ps.Series)):
+    elif isinstance(df, (psDataFrame, psSeries)):
         return df
     else:
         raise TypeError(f"{type(df)} is not one of pandas.DataFrame, pandas.Series and pyspark.sql.DataFrame")
 
 
 def train_test_split_pyspark(
-    df: Union[DataFrame, ps.DataFrame],
+    df: Union[sparkDataFrame, psDataFrame],
     stratify_column: Optional[str] = None,
     test_fraction: Optional[float] = 0.2,
     seed: Optional[int] = 1234,
     to_pandas_spark: Optional[bool] = True,
     index_col: Optional[str] = "tmp_index_col",
-) -> Tuple[Union[DataFrame, ps.DataFrame], Union[DataFrame, ps.DataFrame]]:
+) -> Tuple[Union[sparkDataFrame, psDataFrame], Union[sparkDataFrame, psDataFrame]]:
     """Split a pyspark dataframe into train and test dataframes.
 
     Args:
         df: pyspark.sql.DataFrame | The input dataframe.
         stratify_column: str | The column name to stratify the split. Default None.
         test_fraction: float | The fraction of the test data. Default 0.2.
         seed: int | The random seed. Default 1234.
         to_pandas_spark: bool | Whether to convert the output to pandas_on_spark. Default True.
         index_col: str | The column name to use as index. Default None.
 
     Returns:
         pyspark.sql.DataFrame/pandas_on_spark DataFrame | The train dataframe.
         pyspark.sql.DataFrame/pandas_on_spark DataFrame | The test dataframe.
     """
-    if isinstance(df, ps.DataFrame):
+    import warnings
+
+    warnings.filterwarnings("ignore")
+
+    if isinstance(df, psDataFrame):
         df = df.to_spark(index_col=index_col)
 
     if stratify_column:
         # Test data
         test_fraction_dict = (
             df.select(stratify_column).distinct().withColumn("fraction", F.lit(test_fraction)).rdd.collectAsMap()
         )
@@ -119,105 +117,113 @@
         df_test.index.name = None
     elif index_col == "tmp_index_col":
         df_train = df_train.drop(index_col)
         df_test = df_test.drop(index_col)
     return [df_train, df_test]
 
 
-def unique_pandas_on_spark(psds: Union[ps.Series, ps.DataFrame]) -> Tuple[np.ndarray, np.ndarray]:
+def unique_pandas_on_spark(psds: Union[psSeries, psDataFrame]) -> Tuple[np.ndarray, np.ndarray]:
     """Get the unique values and counts of a pandas_on_spark series."""
-    if isinstance(psds, ps.DataFrame):
+    if isinstance(psds, psDataFrame):
         psds = psds.iloc[:, 0]
     _tmp = psds.value_counts().to_pandas()
     label_set = _tmp.index.values
     counts = _tmp.values
     return label_set, counts
 
 
-def len_labels(y: Union[ps.Series, np.ndarray], return_labels=False) -> Union[int, Optional[np.ndarray]]:
+def len_labels(y: Union[psSeries, np.ndarray], return_labels=False) -> Union[int, Optional[np.ndarray]]:
     """Get the number of unique labels in y."""
-    if not isinstance(y, (ps.DataFrame, ps.Series)):
+    if not isinstance(y, (psDataFrame, psSeries)):
         labels = np.unique(y)
     else:
-        labels = y.unique() if isinstance(y, ps.Series) else y.iloc[:, 0].unique()
+        labels = y.unique() if isinstance(y, psSeries) else y.iloc[:, 0].unique()
     if return_labels:
         return len(labels), labels
     return len(labels)
 
 
-def unique_value_first_index(y: Union[pd.Series, ps.Series, np.ndarray]) -> Tuple[np.ndarray, np.ndarray]:
+def unique_value_first_index(y: Union[Series, psSeries, np.ndarray]) -> Tuple[np.ndarray, np.ndarray]:
     """Get the unique values and indices of a pandas series,
     pandas_on_spark series or numpy array."""
-    if isinstance(y, ps.Series):
+    if isinstance(y, psSeries):
         y_unique = y.drop_duplicates().sort_index()
         label_set = y_unique.values
         first_index = y_unique.index.values
     else:
         label_set, first_index = np.unique(y, return_index=True)
     return label_set, first_index
 
 
 def iloc_pandas_on_spark(
-    psdf: Union[ps.DataFrame, ps.Series, pd.DataFrame, pd.Series],
+    psdf: Union[psDataFrame, psSeries, DataFrame, Series],
     index: Union[int, slice, list],
     index_col: Optional[str] = "tmp_index_col",
-) -> Union[ps.DataFrame, ps.Series]:
+) -> Union[psDataFrame, psSeries]:
     """Get the rows of a pandas_on_spark dataframe/series by index."""
-    if isinstance(psdf, (pd.DataFrame, pd.Series)):
+    import warnings
+
+    warnings.filterwarnings("ignore")
+
+    if isinstance(psdf, (DataFrame, Series)):
         return psdf.iloc[index]
     if isinstance(index, (int, slice)):
-        if isinstance(psdf, ps.Series):
+        if isinstance(psdf, psSeries):
             return psdf.iloc[index]
         else:
             return psdf.iloc[index, :]
     elif isinstance(index, list):
-        if isinstance(psdf, ps.Series):
+        if isinstance(psdf, psSeries):
             sdf = psdf.to_frame().to_spark(index_col=index_col)
         else:
             if index_col not in psdf.columns:
                 sdf = psdf.to_spark(index_col=index_col)
             else:
                 sdf = psdf.to_spark()
         sdfiloc = sdf.filter(F.col(index_col).isin(index))
         psdfiloc = to_pandas_on_spark(sdfiloc)
-        if isinstance(psdf, ps.Series):
+        if isinstance(psdf, psSeries):
             psdfiloc = psdfiloc[psdfiloc.columns.drop(index_col)[0]]
         elif index_col not in psdf.columns:
             psdfiloc = psdfiloc.drop(columns=[index_col])
         return psdfiloc
     else:
         raise TypeError(f"{type(index)} is not one of int, slice and list for pandas_on_spark iloc")
 
 
 def spark_kFold(
-    dataset: Union[DataFrame, ps.DataFrame],
+    dataset: Union[sparkDataFrame, psDataFrame],
     nFolds: int = 3,
     foldCol: str = "",
     seed: int = 42,
     index_col: Optional[str] = "tmp_index_col",
-) -> List[Tuple[ps.DataFrame, ps.DataFrame]]:
+) -> List[Tuple[psDataFrame, psDataFrame]]:
     """Generate k-fold splits for a Spark DataFrame.
     Adopted from https://spark.apache.org/docs/latest/api/python/_modules/pyspark/ml/tuning.html#CrossValidator
 
     Args:
-        dataset: DataFrame / ps.DataFrame. | The DataFrame to split.
+        dataset: sparkDataFrame / psDataFrame. | The DataFrame to split.
         nFolds: int | The number of folds. Default is 3.
         foldCol: str | The column name to use for fold numbers. If not specified,
             the DataFrame will be randomly split. Default is "".
             The same group will not appear in two different folds (the number of
             distinct groups has to be at least equal to the number of folds).
             The folds are approximately balanced in the sense that the number of
             distinct groups is approximately the same in each fold.
         seed: int | The random seed. Default is 42.
         index_col: str | The name of the index column. Default is "tmp_index_col".
 
     Returns:
         A list of (train, validation) DataFrames.
     """
-    if isinstance(dataset, ps.DataFrame):
+    import warnings
+
+    warnings.filterwarnings("ignore")
+
+    if isinstance(dataset, psDataFrame):
         dataset = dataset.to_spark(index_col=index_col)
 
     datasets = []
     if not foldCol:
         # Do random k-fold split.
         h = 1.0 / nFolds
         randCol = f"rand_col_{seed}"
```

### Comparing `FLAML-1.2.4/flaml/automl/state.py` & `FLAML-2.0.0rc1/flaml/automl/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,16 @@
 import inspect
 import time
-import os
 from typing import Any, Optional
-
 import numpy as np
-import pandas as pd
-
 from flaml import tune
 from flaml.automl.logger import logger
 from flaml.automl.ml import compute_estimator, train_estimator
 from flaml.automl.task.task import TS_FORECAST
-
-try:
-    from flaml.automl.spark.utils import (
-        train_test_split_pyspark,
-        unique_pandas_on_spark,
-        len_labels,
-        unique_value_first_index,
-    )
-except ImportError:
-    train_test_split_pyspark = None
-    unique_pandas_on_spark = None
-    from flaml.automl.utils import (
-        len_labels,
-        unique_value_first_index,
-    )
-try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    import pyspark.pandas as ps
-    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
-    from pyspark.pandas.config import set_option, reset_option
-except ImportError:
-    ps = None
-
-    class psDataFrame:
-        pass
-
-    class psSeries:
-        pass
+from flaml.automl.spark import psDataFrame, psSeries, DataFrame, Series
 
 
 class SearchState:
     @property
     def search_space(self):
         return self._search_space_domain
 
@@ -241,33 +210,33 @@
         return self.time2eval_best * retrain_sample_size / self.best_config_sample_size
 
 
 class AutoMLState:
     def _prepare_sample_train_data(self, sample_size: int):
         sampled_weight = groups = None
         if sample_size <= self.data_size[0]:
-            if isinstance(self.X_train, (pd.DataFrame, psDataFrame)):
+            if isinstance(self.X_train, (DataFrame, psDataFrame)):
                 sampled_X_train = self.X_train.iloc[:sample_size]
             else:
                 sampled_X_train = self.X_train[:sample_size]
-            if isinstance(self.y_train, (pd.Series, psSeries)):
+            if isinstance(self.y_train, (Series, psSeries)):
                 sampled_y_train = self.y_train.iloc[:sample_size]
             else:
                 sampled_y_train = self.y_train[:sample_size]
             weight = self.fit_kwargs.get(
                 "sample_weight"
             )  # NOTE: _prepare_sample_train_data is before kwargs is updated to fit_kwargs_by_estimator
             if weight is not None:
                 sampled_weight = (
-                    weight.iloc[:sample_size] if isinstance(weight, (pd.Series, psSeries)) else weight[:sample_size]
+                    weight.iloc[:sample_size] if isinstance(weight, (Series, psSeries)) else weight[:sample_size]
                 )
             if self.groups is not None:
                 groups = (
                     self.groups.iloc[:sample_size]
-                    if isinstance(self.groups, (pd.Series, psSeries))
+                    if isinstance(self.groups, (Series, psSeries))
                     else self.groups[:sample_size]
                 )
         else:
             sampled_X_train = self.X_train_all
             sampled_y_train = self.y_train_all
             if (
                 "sample_weight" in self.fit_kwargs
```

### Comparing `FLAML-1.2.4/flaml/automl/task/generic_task.py` & `FLAML-2.0.0rc1/flaml/automl/task/generic_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,11 @@
-import os
 import logging
 import time
 from typing import List, Optional
-
-import pandas as pd
 import numpy as np
-from scipy.sparse import issparse
-from sklearn.utils import shuffle
-from sklearn.model_selection import (
-    train_test_split,
-    RepeatedStratifiedKFold,
-    RepeatedKFold,
-    GroupKFold,
-    TimeSeriesSplit,
-    GroupShuffleSplit,
-    StratifiedGroupKFold,
-)
-
 from flaml.automl.data import TS_TIMESTAMP_COL, concat
 from flaml.automl.ml import EstimatorSubclass, default_cv_score_agg_func, get_val_loss
 from flaml.automl.model import (
     XGBoostSklearnEstimator,
     XGBoostLimitDepthEstimator,
     RandomForestEstimator,
     LGBMEstimator,
@@ -36,48 +21,42 @@
 from flaml.automl.task.task import (
     Task,
     get_classification_objective,
     TS_FORECAST,
     TS_FORECASTPANEL,
 )
 from flaml.config import RANDOM_SEED
+from flaml.automl.spark import ps, psDataFrame, psSeries, pd
+from flaml.automl.spark.utils import (
+    iloc_pandas_on_spark,
+    spark_kFold,
+    train_test_split_pyspark,
+    unique_pandas_on_spark,
+    unique_value_first_index,
+    len_labels,
+    set_option,
+)
 
 try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    from pyspark.sql.functions import col
-    import pyspark.pandas as ps
-    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
-    from pyspark.pandas.config import set_option, reset_option
-    from flaml.automl.spark.utils import (
-        to_pandas_on_spark,
-        iloc_pandas_on_spark,
-        spark_kFold,
-        train_test_split_pyspark,
-        unique_pandas_on_spark,
-        unique_value_first_index,
-        len_labels,
-    )
-    from flaml.automl.spark.metrics import spark_metric_loss_score
+    from scipy.sparse import issparse
 except ImportError:
-    train_test_split_pyspark = None
-    unique_pandas_on_spark = None
-    iloc_pandas_on_spark = None
-    from flaml.automl.utils import (
-        len_labels,
-        unique_value_first_index,
+    pass
+try:
+    from sklearn.utils import shuffle
+    from sklearn.model_selection import (
+        train_test_split,
+        RepeatedStratifiedKFold,
+        RepeatedKFold,
+        GroupKFold,
+        TimeSeriesSplit,
+        GroupShuffleSplit,
+        StratifiedGroupKFold,
     )
-
-    ps = None
-
-    class psDataFrame:
-        pass
-
-    class psSeries:
-        pass
-
+except ImportError:
+    pass
 
 logger = logging.getLogger(__name__)
 
 
 class GenericTask(Task):
     estimators = {
         "xgboost": XGBoostSklearnEstimator,
```

### Comparing `FLAML-1.2.4/flaml/automl/task/task.py` & `FLAML-2.0.0rc1/flaml/automl/task/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, List, Optional, Tuple, Union
-
 import numpy as np
-import pandas as pd
+from flaml.automl.data import DataFrame, Series, psDataFrame, psSeries
 
 if TYPE_CHECKING:
     import flaml
 
-try:
-    import ray
-except ImportError:
-    ray = None
-
 # TODO: if your task is not specified in here, define your task as an all-capitalized word
 SEQCLASSIFICATION = "seq-classification"
 MULTICHOICECLASSIFICATION = "multichoice-classification"
 TOKENCLASSIFICATION = "token-classification"
 
 SEQREGRESSION = "seq-regression"
 
@@ -76,16 +70,16 @@
     """
 
     estimators = {}
 
     def __init__(
         self,
         task_name: str,
-        X_train: Optional[Union[np.ndarray, pd.DataFrame]] = None,
-        y_train: Optional[Union[np.ndarray, pd.DataFrame, pd.Series]] = None,
+        X_train: Optional[Union[np.ndarray, DataFrame, psDataFrame]] = None,
+        y_train: Optional[Union[np.ndarray, DataFrame, Series, psSeries]] = None,
     ):
         """Constructor.
 
         Args:
             task_name: String name for this type of task. Used when the Task can be generic and implement a number of
                 types of sub-task.
             X_train: Optional. Some Task types may use the data shape or features to determine details of their usage,
@@ -100,16 +94,16 @@
         return self.name
 
     @abstractmethod
     def evaluate_model_CV(
         self,
         config: dict,
         estimator: "flaml.automl.ml.BaseEstimator",
-        X_train_all: Union[np.ndarray, pd.DataFrame],
-        y_train_all: Union[np.ndarray, pd.DataFrame, pd.Series],
+        X_train_all: Union[np.ndarray, DataFrame, psDataFrame],
+        y_train_all: Union[np.ndarray, DataFrame, Series, psSeries],
         budget: int,
         kf,
         eval_metric: str,
         best_val_loss: float,
         log_training_metric: bool = False,
         fit_kwargs: Optional[dict] = {},
     ) -> Tuple[float, float, float, float]:
@@ -132,20 +126,20 @@
         """
 
     @abstractmethod
     def validate_data(
         self,
         automl: "flaml.automl.automl.AutoML",
         state: "flaml.automl.state.AutoMLState",
-        X_train_all: Union[np.ndarray, pd.DataFrame, None],
-        y_train_all: Union[np.ndarray, pd.DataFrame, pd.Series, None],
-        dataframe: Union[pd.DataFrame, None],
+        X_train_all: Union[np.ndarray, DataFrame, psDataFrame, None],
+        y_train_all: Union[np.ndarray, DataFrame, Series, psSeries, None],
+        dataframe: Union[DataFrame, None],
         label: str,
-        X_val: Optional[Union[np.ndarray, pd.DataFrame]] = None,
-        y_val: Optional[Union[np.ndarray, pd.DataFrame, pd.Series]] = None,
+        X_val: Optional[Union[np.ndarray, DataFrame, psDataFrame]] = None,
+        y_val: Optional[Union[np.ndarray, DataFrame, Series, psSeries]] = None,
         groups_val: Optional[List[str]] = None,
         groups: Optional[List[str]] = None,
     ):
         """Validate that the data is suitable for this task type.
 
         Args:
             automl: The AutoML instance from which this task has been constructed.
@@ -165,16 +159,16 @@
             AssertionError: The data provided is invalid for this task type and configuration.
         """
 
     @abstractmethod
     def prepare_data(
         self,
         state: "flaml.automl.state.AutoMLState",
-        X_train_all: Union[np.ndarray, pd.DataFrame],
-        y_train_all: Union[np.ndarray, pd.DataFrame, pd.Series, None],
+        X_train_all: Union[np.ndarray, DataFrame, psDataFrame],
+        y_train_all: Union[np.ndarray, DataFrame, Series, psSeries, None],
         auto_augment: bool,
         eval_method: str,
         split_type: str,
         split_ratio: float,
         n_splits: int,
         data_is_df: bool,
         sample_weight_full: Optional[List[float]] = None,
@@ -199,26 +193,26 @@
                     ["auto", 'stratified', 'uniform', 'time', 'group']. "auto" -> stratified.
                 For regression tasks, valid choices are ["auto", 'uniform', 'time'].
                     "auto" -> uniform.
                 For time series forecast tasks, must be "auto" or 'time'.
                 For ranking task, must be "auto" or 'group'.
             split_ratio: A float of the valiation data percentage for holdout.
             n_splits: An integer of the number of folds for cross - validation.
-            data_is_df: True if the data was provided as a pd.DataFrame else False.
+            data_is_df: True if the data was provided as a DataFrame else False.
             sample_weight_full: A 1d arraylike of the sample weight.
 
         Raises:
             AssertionError: The configuration provided is invalid for this task type and data.
         """
 
     @abstractmethod
     def decide_split_type(
         self,
         split_type: str,
-        y_train_all: Union[np.ndarray, pd.DataFrame, pd.Series, None],
+        y_train_all: Union[np.ndarray, DataFrame, Series, psSeries, None],
         fit_kwargs: dict,
         groups: Optional[List[str]] = None,
     ) -> str:
         """Choose an appropriate data split type for this data and task.
 
         If split_type is 'auto' then this is determined based on the task type and data.
         If a specific split_type is requested then the choice is validated to be appropriate.
@@ -236,17 +230,17 @@
         Raises:
             AssertionError: The requested split_type is invalid for this task, configuration and data.
         """
 
     @abstractmethod
     def preprocess(
         self,
-        X: Union[np.ndarray, pd.DataFrame],
+        X: Union[np.ndarray, DataFrame, psDataFrame],
         transformer: Optional["flaml.automl.data.DataTransformer"] = None,
-    ) -> Union[np.ndarray, pd.DataFrame]:
+    ) -> Union[np.ndarray, DataFrame]:
         """Preprocess the data ready for fitting or inference with this task type.
 
         Args:
             X: The data set to process.
             transformer: A DataTransformer instance to be used in processing.
 
         Returns:
```

### Comparing `FLAML-1.2.4/flaml/automl/training_log.py` & `FLAML-2.0.0rc1/flaml/automl/training_log.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/all/binary.json` & `FLAML-2.0.0rc1/flaml/default/all/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/all/multiclass.json` & `FLAML-2.0.0rc1/flaml/default/all/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/all/regression.json` & `FLAML-2.0.0rc1/flaml/default/all/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/estimator.py` & `FLAML-2.0.0rc1/flaml/default/estimator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sklearn.ensemble as ensemble
 from functools import wraps
 from flaml.automl.task.task import CLASSIFICATION
 from .suggest import preprocess_and_suggest_hyperparams
 
 DEFAULT_LOCATION = "default_location"
 
 
@@ -139,37 +138,44 @@
                 return y_pred
 
     EstimatorClass.__doc__ += " " + super_class.__doc__
     EstimatorClass.__name__ = super_class.__name__
     return EstimatorClass
 
 
-RandomForestRegressor = flamlize_estimator(ensemble.RandomForestRegressor, "rf", "regression")
-RandomForestClassifier = flamlize_estimator(ensemble.RandomForestClassifier, "rf", "classification")
-ExtraTreesRegressor = flamlize_estimator(ensemble.ExtraTreesRegressor, "extra_tree", "regression")
-ExtraTreesClassifier = flamlize_estimator(ensemble.ExtraTreesClassifier, "extra_tree", "classification")
+try:
+    import sklearn.ensemble as ensemble
+except ImportError:
+    RandomForestClassifier = RandomForestRegressor = ExtraTreesClassifier = ExtraTreesRegressor = ImportError(
+        "Using flaml.default.* requires scikit-learn."
+    )
+else:
+    RandomForestRegressor = flamlize_estimator(ensemble.RandomForestRegressor, "rf", "regression")
+    RandomForestClassifier = flamlize_estimator(ensemble.RandomForestClassifier, "rf", "classification")
+    ExtraTreesRegressor = flamlize_estimator(ensemble.ExtraTreesRegressor, "extra_tree", "regression")
+    ExtraTreesClassifier = flamlize_estimator(ensemble.ExtraTreesClassifier, "extra_tree", "classification")
 
 try:
     import lightgbm
-
+except ImportError:
+    LGBMRegressor = LGBMClassifier = ImportError("Using flaml.default.LGBM* requires lightgbm.")
+else:
     LGBMRegressor = flamlize_estimator(lightgbm.LGBMRegressor, "lgbm", "regression")
     LGBMClassifier = flamlize_estimator(lightgbm.LGBMClassifier, "lgbm", "classification")
-except ImportError:
-    pass
 
 try:
     import xgboost
-
+except ImportError:
+    XGBClassifier = XGBRegressor = ImportError("Using flaml.default.XGB* requires xgboost.")
+else:
     XGBRegressor = flamlize_estimator(
         xgboost.XGBRegressor,
         "xgb_limitdepth",
         "regression",
         [("max_depth", 0, "xgboost")],
     )
     XGBClassifier = flamlize_estimator(
         xgboost.XGBClassifier,
         "xgb_limitdepth",
         "classification",
         [("max_depth", 0, "xgboost")],
     )
-except ImportError:
-    pass
```

### Comparing `FLAML-1.2.4/flaml/default/extra_tree/binary.json` & `FLAML-2.0.0rc1/flaml/default/extra_tree/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/extra_tree/multiclass.json` & `FLAML-2.0.0rc1/flaml/default/extra_tree/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/extra_tree/regression.json` & `FLAML-2.0.0rc1/flaml/default/extra_tree/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/greedy.py` & `FLAML-2.0.0rc1/flaml/default/greedy.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/lgbm/binary.json` & `FLAML-2.0.0rc1/flaml/default/lgbm/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/lgbm/multiclass.json` & `FLAML-2.0.0rc1/flaml/default/lgbm/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/lgbm/regression.json` & `FLAML-2.0.0rc1/flaml/default/lgbm/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/portfolio.py` & `FLAML-2.0.0rc1/flaml/default/portfolio.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/regret.py` & `FLAML-2.0.0rc1/flaml/default/regret.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/rf/binary.json` & `FLAML-2.0.0rc1/flaml/default/rf/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/rf/multiclass.json` & `FLAML-2.0.0rc1/flaml/default/rf/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/rf/regression.json` & `FLAML-2.0.0rc1/flaml/default/rf/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/suggest.py` & `FLAML-2.0.0rc1/flaml/default/suggest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,27 @@
-import os
 import numpy as np
-from sklearn.neighbors import NearestNeighbors
 import logging
 import pathlib
 import json
 from flaml.automl.data import DataTransformer
 from flaml.automl.task.task import CLASSIFICATION, get_classification_objective
+from flaml.automl.task.generic_task import len_labels
 from flaml.automl.ml import get_estimator_class
 from flaml.version import __version__
 
 try:
-    from flaml.automl.spark.utils import len_labels
+    from sklearn.neighbors import NearestNeighbors
 except ImportError:
-    from flaml.automl.utils import len_labels
-try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
-    import pyspark.pandas as ps
-    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
-except ImportError:
-    ps = None
-
-    class psDataFrame:
-        pass
-
-    class psSeries:
-        pass
-
+    pass
 
 LOCATION = pathlib.Path(__file__).parent.resolve()
 logger = logging.getLogger(__name__)
 CONFIG_PREDICTORS = {}
 
 
-def version_parse(version):
-    return tuple(map(int, (version.split("."))))
-
-
 def meta_feature(task, X_train, y_train, meta_feature_names):
     this_feature = []
     n_row = X_train.shape[0]
     n_feat = X_train.shape[1]
 
     is_classification = task in CLASSIFICATION
     for each_feature_name in meta_feature_names:
@@ -90,14 +72,16 @@
     meta_feature_fn=meta_feature,
 ):
     """Suggest a list of configs for the given task and training data.
 
     The returned configs can be used as starting points for AutoML.fit().
     `FLAML_sample_size` is removed from the configs.
     """
+    from packaging.version import parse as version_parse
+
     task = get_classification_objective(len_labels(y)) if task == "classification" and y is not None else task
     predictor = (
         load_config_predictor(estimator_or_predictor, task, location)
         if isinstance(estimator_or_predictor, str)
         else estimator_or_predictor
     )
```

### Comparing `FLAML-1.2.4/flaml/default/xgb_limitdepth/binary.json` & `FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/xgb_limitdepth/regression.json` & `FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/xgboost/binary.json` & `FLAML-2.0.0rc1/flaml/default/xgboost/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/xgboost/multiclass.json` & `FLAML-2.0.0rc1/flaml/default/xgboost/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/default/xgboost/regression.json` & `FLAML-2.0.0rc1/flaml/default/xgboost/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/onlineml/autovw.py` & `FLAML-2.0.0rc1/flaml/onlineml/autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/onlineml/trial.py` & `FLAML-2.0.0rc1/flaml/onlineml/trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import numpy as np
 import logging
 import time
 import math
 import copy
 import collections
 from typing import Optional, Union
-from sklearn.metrics import mean_squared_error, mean_absolute_error
 from flaml.tune import Trial
 
+try:
+    from sklearn.metrics import mean_squared_error, mean_absolute_error
+except ImportError:
+    pass
+
 logger = logging.getLogger(__name__)
 
 
 def get_ns_feature_dim_from_vw_example(vw_example) -> dict:
     """Get a dictionary of feature dimensionality for each namespace singleton."""
     # *************************A NOTE about the input vwexample***********
     # Assumption: assume the vw_example takes one of the following format
```

### Comparing `FLAML-1.2.4/flaml/onlineml/trial_runner.py` & `FLAML-2.0.0rc1/flaml/onlineml/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/__init__.py` & `FLAML-2.0.0rc1/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/analysis.py` & `FLAML-2.0.0rc1/flaml/tune/analysis.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/result.py` & `FLAML-2.0.0rc1/flaml/tune/result.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/sample.py` & `FLAML-2.0.0rc1/flaml/tune/sample.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/scheduler/online_scheduler.py` & `FLAML-2.0.0rc1/flaml/tune/scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-2.0.0rc1/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/searcher/blendsearch.py` & `FLAML-2.0.0rc1/flaml/tune/searcher/blendsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -954,17 +954,15 @@
         qloguniform,
     )
 
 try:
     from nni.tuner import Tuner as NNITuner
     from nni.utils import extract_scalar_reward
 except ImportError:
-
-    class NNITuner:
-        pass
+    NNITuner = object
 
     def extract_scalar_reward(x: Dict):
         return x.get("default")
 
 
 class BlendSearchTuner(BlendSearch, NNITuner):
     """Tuner class for NNI."""
```

### Comparing `FLAML-1.2.4/flaml/tune/searcher/cfo_cat.py` & `FLAML-2.0.0rc1/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/searcher/flow2.py` & `FLAML-2.0.0rc1/flaml/tune/searcher/flow2.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/searcher/online_searcher.py` & `FLAML-2.0.0rc1/flaml/tune/searcher/online_searcher.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/searcher/search_thread.py` & `FLAML-2.0.0rc1/flaml/tune/searcher/search_thread.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/searcher/suggestion.py` & `FLAML-2.0.0rc1/flaml/tune/searcher/suggestion.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/searcher/variant_generator.py` & `FLAML-2.0.0rc1/flaml/tune/searcher/variant_generator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/space.py` & `FLAML-2.0.0rc1/flaml/tune/space.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/spark/utils.py` & `FLAML-2.0.0rc1/flaml/tune/spark/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,55 +7,53 @@
 
 
 logger = logging.getLogger(__name__)
 logger_formatter = logging.Formatter(
     "[%(name)s: %(asctime)s] {%(lineno)d} %(levelname)s - %(message)s", "%m-%d %H:%M:%S"
 )
 logger.propagate = False
+os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
 try:
-    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
     import pyspark
     from pyspark.sql import SparkSession
     from pyspark.util import VersionUtils
     import py4j
-
-    _have_spark = True
-    _spark_major_minor_version = VersionUtils.majorMinorVersion(pyspark.__version__)
-except ImportError as e:
-    logger.debug("Could not import pyspark: %s", e)
+except ImportError:
     _have_spark = False
     py4j = None
     _spark_major_minor_version = (0, 0)
+else:
+    _have_spark = True
+    _spark_major_minor_version = VersionUtils.majorMinorVersion(pyspark.__version__)
 
 
 @lru_cache(maxsize=2)
 def check_spark():
     """Check if Spark is installed and running.
     Result of the function will be cached since test once is enough. As lru_cache will not
     cache exceptions, we don't raise exceptions here but only log a warning message.
 
     Returns:
         Return (True, None) if the check passes, otherwise log the exception message and
         return (False, Exception(msg)). The exception can be raised by the caller.
     """
-    logger.debug("\ncheck Spark installation...This line should appear only once.\n")
+    logger.debug("\nchecking Spark installation...This line should appear only once.\n")
     if not _have_spark:
         msg = """use_spark=True requires installation of PySpark. Please run pip install flaml[spark]
         and check [here](https://spark.apache.org/docs/latest/api/python/getting_started/install.html)
         for more details about installing Spark."""
         return False, ImportError(msg)
 
     if _spark_major_minor_version[0] < 3:
         msg = "Spark version must be >= 3.0 to use flaml[spark]"
         return False, ImportError(msg)
 
     try:
         SparkSession.builder.getOrCreate()
     except RuntimeError as e:
-        # logger.warning(f"\nSparkSession is not available: {e}\n")
         return False, RuntimeError(e)
 
     return True, None
 
 
 def get_n_cpus(node="driver"):
     """Get the number of CPU cores of the given type of node.
```

### Comparing `FLAML-1.2.4/flaml/tune/trial.py` & `FLAML-2.0.0rc1/flaml/tune/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/trial_runner.py` & `FLAML-2.0.0rc1/flaml/tune/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/flaml/tune/tune.py` & `FLAML-2.0.0rc1/flaml/tune/tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 from collections import defaultdict
 
 try:
     from ray import __version__ as ray_version
 
     assert ray_version >= "1.10.0"
     from ray.tune.analysis import ExperimentAnalysis as EA
-
-    ray_available = True
 except (ImportError, AssertionError):
     ray_available = False
     from .analysis import ExperimentAnalysis as EA
+else:
+    ray_available = True
 
 from .trial import Trial
 from .result import DEFAULT_METRIC
 import logging
-from flaml.tune.spark.utils import PySparkOvertimeMonitor
+from flaml.tune.spark.utils import PySparkOvertimeMonitor, check_spark
 
 logger = logging.getLogger(__name__)
 logger.propagate = False
 _use_ray = True
 _runner = None
 _verbose = 0
 _running_trial = None
@@ -227,15 +227,15 @@
     use_incumbent_result_in_evaluation: Optional[bool] = None,
     log_file_name: Optional[str] = None,
     lexico_objectives: Optional[dict] = None,
     force_cancel: Optional[bool] = False,
     n_concurrent_trials: Optional[int] = 0,
     **ray_args,
 ):
-    """The trigger for HPO.
+    """The function-based way of performing HPO.
 
     Example:
 
     ```python
     import time
     from flaml import tune
 
@@ -608,16 +608,14 @@
             _use_ray = old_use_ray
             _verbose = old_verbose
             _running_trial = old_running_trial
             _training_iteration = old_training_iteration
 
     if use_spark:
         # parallel run with spark
-        from flaml.tune.spark.utils import check_spark
-
         spark_available, spark_error_msg = check_spark()
         if not spark_available:
             raise spark_error_msg
         try:
             from pyspark.sql import SparkSession
             from joblib import Parallel, delayed, parallel_backend
             from joblibspark import register_spark
@@ -807,7 +805,88 @@
         _verbose = old_verbose
         _running_trial = old_running_trial
         _training_iteration = old_training_iteration
         if not use_ray:
             _runner = old_runner
             logger.handlers = old_handlers
             logger.setLevel(old_level)
+
+
+class Tuner:
+    """Tuner is the class-based way of launching hyperparameter tuning jobs compatible with Ray Tune 2.
+
+    Args:
+        trainable: A user-defined evaluation function.
+            It takes a configuration as input, outputs a evaluation
+            result (can be a numerical value or a dictionary of string
+            and numerical value pairs) for the input configuration.
+            For machine learning tasks, it usually involves training and
+            scoring a machine learning model, e.g., through validation loss.
+        param_space: Search space of the tuning job.
+            One thing to note is that both preprocessor and dataset can be tuned here.
+        tune_config: Tuning algorithm specific configs.
+            Refer to ray.tune.tune_config.TuneConfig for more info.
+        run_config: Runtime configuration that is specific to individual trials.
+            If passed, this will overwrite the run config passed to the Trainer,
+            if applicable. Refer to ray.air.config.RunConfig for more info.
+
+    Usage pattern:
+
+    .. code-block:: python
+
+        from sklearn.datasets import load_breast_cancer
+
+        from ray import tune
+        from ray.data import from_pandas
+        from ray.air.config import RunConfig, ScalingConfig
+        from ray.train.xgboost import XGBoostTrainer
+        from ray.tune.tuner import Tuner
+
+        def get_dataset():
+            data_raw = load_breast_cancer(as_frame=True)
+            dataset_df = data_raw["data"]
+            dataset_df["target"] = data_raw["target"]
+            dataset = from_pandas(dataset_df)
+            return dataset
+
+        trainer = XGBoostTrainer(
+            label_column="target",
+            params={},
+            datasets={"train": get_dataset()},
+        )
+
+        param_space = {
+            "scaling_config": ScalingConfig(
+                num_workers=tune.grid_search([2, 4]),
+                resources_per_worker={
+                    "CPU": tune.grid_search([1, 2]),
+                },
+            ),
+            # You can even grid search various datasets in Tune.
+            # "datasets": {
+            #     "train": tune.grid_search(
+            #         [ds1, ds2]
+            #     ),
+            # },
+            "params": {
+                "objective": "binary:logistic",
+                "tree_method": "approx",
+                "eval_metric": ["logloss", "error"],
+                "eta": tune.loguniform(1e-4, 1e-1),
+                "subsample": tune.uniform(0.5, 1.0),
+                "max_depth": tune.randint(1, 9),
+            },
+        }
+        tuner = Tuner(trainable=trainer, param_space=param_space,
+            run_config=RunConfig(name="my_tune_run"))
+        analysis = tuner.fit()
+
+    To retry a failed tune run, you can then do
+
+    .. code-block:: python
+
+        tuner = Tuner.restore(experiment_checkpoint_dir)
+        tuner.fit()
+
+    ``experiment_checkpoint_dir`` can be easily located near the end of the
+    console output of your first failed run.
+    """
```

### Comparing `FLAML-1.2.4/flaml/tune/utils.py` & `FLAML-2.0.0rc1/flaml/tune/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/pyproject.toml` & `FLAML-2.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/setup.py` & `FLAML-2.0.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,14 @@
 version = {}
 with open(os.path.join(here, "flaml/version.py")) as fp:
     exec(fp.read(), version)
 __version__ = version["__version__"]
 
 install_requires = [
     "NumPy>=1.17.0rc1",
-    "lightgbm>=2.3.1",
-    "xgboost>=0.90",
-    "scipy>=1.4.1",
-    "pandas>=1.1.4",
-    "scikit-learn>=0.24",
 ]
 
 
 setuptools.setup(
     name="FLAML",
     version=__version__,
     author="Microsoft Corporation",
@@ -35,34 +30,44 @@
     packages=setuptools.find_packages(include=["flaml*"]),
     package_data={
         "flaml.default": ["*/*.json"],
     },
     include_package_data=True,
     install_requires=install_requires,
     extras_require={
+        "automl": [
+            "lightgbm>=2.3.1",
+            "xgboost>=0.90",
+            "scipy>=1.4.1",
+            "pandas>=1.1.4",
+            "scikit-learn>=0.24",
+        ],
         "notebook": [
             "jupyter",
-            "matplotlib",
-            "openml==0.10.2",
         ],
         "spark": [
             "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
         ],
         "test": [
+            "lightgbm>=2.3.1",
+            "xgboost>=0.90",
+            "scipy>=1.4.1",
+            "pandas>=1.1.4",
+            "scikit-learn>=0.24",
             "thop",
             "pytest>=6.1.1",
             "coverage>=5.3",
             "pre-commit",
             "torch",
             "torchvision",
             "catboost>=0.26,<1.2",
             "rgf-python",
             "optuna==2.8.0",
-            "openml==0.10.2",
+            "openml",
             "statsmodels>=0.12.2",
             "psutil==5.8.0",
             "dataclasses",
             "transformers[torch]==4.26",
             "datasets",
             "nltk",
             "rouge_score",
@@ -73,28 +78,30 @@
             "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
             "nbconvert",
             "nbformat",
             "ipykernel",
             "pytorch-lightning<1.9.1",  # test_forecast_panel
             "requests<2.29.0",  # https://github.com/docker/docker-py/issues/3113
+            "packaging",
         ],
         "catboost": ["catboost>=0.26"],
         "blendsearch": ["optuna==2.8.0"],
         "ray": [
             "ray[tune]~=1.13",
         ],
         "azureml": [
             "azureml-mlflow",
         ],
         "nni": [
             "nni",
         ],
         "vw": [
             "vowpalwabbit>=8.10.0, <9.0.0",
+            "scikit-learn",
         ],
         "hf": [
             "transformers[torch]==4.26",
             "datasets",
             "nltk",
             "rouge_score",
             "seqeval",
@@ -118,15 +125,20 @@
             "statsmodels>=0.12.2",
             "hcrystalball==0.1.10",
             "pytorch-forecasting>=0.9.0",
         ],
         "benchmark": ["catboost>=0.26", "psutil==5.8.0", "xgboost==1.3.3"],
         "openai": ["openai==0.27.4", "diskcache"],
         "autogen": ["openai==0.27.4", "diskcache", "docker"],
-        "synapse": ["joblibspark>=0.5.0", "optuna==2.8.0", "pyspark>=3.2.0"],
+        "synapse": [
+            "joblibspark>=0.5.0",
+            "optuna==2.8.0",
+            "pyspark>=3.2.0",
+        ],
+        "autozero": ["scikit-learn", "pandas", "packaging"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

### Comparing `FLAML-1.2.4/test/test_autovw.py` & `FLAML-2.0.0rc1/test/test_autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/test/test_conda_distribution.py` & `FLAML-2.0.0rc1/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/test/test_gpu.py` & `FLAML-2.0.0rc1/test/test_gpu.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.4/test/test_model.py` & `FLAML-2.0.0rc1/test/test_model.py`

 * *Files identical despite different names*

