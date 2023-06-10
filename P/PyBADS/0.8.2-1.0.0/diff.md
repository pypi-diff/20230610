# Comparing `tmp/PyBADS-0.8.2.tar.gz` & `tmp/PyBADS-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBADS-0.8.2.tar", last modified: Tue Feb 28 07:44:48 2023, max compression
+gzip compressed data, was "PyBADS-1.0.0.tar", last modified: Sat Jun 10 18:48:09 2023, max compression
```

## Comparing `PyBADS-0.8.2.tar` & `PyBADS-1.0.0.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.680105 PyBADS-0.8.2/
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.667105 PyBADS-0.8.2/.github/
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.670105 PyBADS-0.8.2/.github/workflows/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      504 2023-02-06 14:04:16.000000 PyBADS-0.8.2/.github/workflows/build.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1297 2023-02-06 14:04:16.000000 PyBADS-0.8.2/.github/workflows/docs.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2223 2023-02-06 14:04:16.000000 PyBADS-0.8.2/.github/workflows/merge-tests.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1054 2023-02-24 14:46:37.000000 PyBADS-0.8.2/.github/workflows/tests.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2239 2023-01-06 15:11:47.000000 PyBADS-0.8.2/.gitignore
--rw-r--r--   0 jeet      (1000) jeet      (1000)      619 2022-12-31 10:58:21.000000 PyBADS-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1517 2022-12-31 10:58:21.000000 PyBADS-0.8.2/LICENSE
--rw-r--r--   0 jeet      (1000) jeet      (1000)       12 2023-02-19 09:10:54.000000 PyBADS-0.8.2/MANIFEST.in
--rw-r--r--   0 jeet      (1000) jeet      (1000)    12184 2023-02-28 07:44:48.680105 PyBADS-0.8.2/PKG-INFO
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.671105 PyBADS-0.8.2/PyBADS.egg-info/
--rw-r--r--   0 jeet      (1000) jeet      (1000)    12184 2023-02-28 07:44:48.000000 PyBADS-0.8.2/PyBADS.egg-info/PKG-INFO
--rw-r--r--   0 jeet      (1000) jeet      (1000)     3391 2023-02-28 07:44:48.000000 PyBADS-0.8.2/PyBADS.egg-info/SOURCES.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)        1 2023-02-28 07:44:48.000000 PyBADS-0.8.2/PyBADS.egg-info/dependency_links.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)      313 2023-02-28 07:44:48.000000 PyBADS-0.8.2/PyBADS.egg-info/requires.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)        7 2023-02-28 07:44:48.000000 PyBADS-0.8.2/PyBADS.egg-info/top_level.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10217 2023-02-28 07:37:36.000000 PyBADS-0.8.2/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)      137 2022-12-31 10:58:21.000000 PyBADS-0.8.2/environment.yml
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.671105 PyBADS-0.8.2/examples/
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10334 2023-02-18 15:28:04.000000 PyBADS-0.8.2/examples/pybads_example_1_basic_usage.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9069 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/pybads_example_2_nonbox_constraints.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    12745 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/pybads_example_3_noisy_objective.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10153 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/pybads_example_4_user_provided_noise.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9264 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/pybads_example_5_extended_usage.ipynb
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.672105 PyBADS-0.8.2/examples/scripts/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      949 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/scripts/pybads_example_1_basic_usage.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1133 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/scripts/pybads_example_2_nonbox_constraints.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1274 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/scripts/pybads_example_3_noisy_objective.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1599 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/scripts/pybads_example_4_user_provided_noise.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1579 2022-12-31 10:58:21.000000 PyBADS-0.8.2/examples/scripts/pybads_example_5_extended_usage.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.672105 PyBADS-0.8.2/pybads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      556 2023-02-20 16:40:10.000000 PyBADS-0.8.2/pybads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      635 2023-02-06 14:04:16.000000 PyBADS-0.8.2/pybads/__main__.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.673105 PyBADS-0.8.2/pybads/acquisition_functions/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       37 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/acquisition_functions/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1418 2023-01-06 15:11:47.000000 PyBADS-0.8.2/pybads/acquisition_functions/acq_fcn_lcb.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.673105 PyBADS-0.8.2/pybads/bads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      255 2023-02-18 13:47:05.000000 PyBADS-0.8.2/pybads/bads/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)      388 2023-02-20 11:32:39.000000 PyBADS-0.8.2/pybads/bads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)   100587 2023-02-20 07:59:38.000000 PyBADS-0.8.2/pybads/bads/bads.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2249 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/bads/bads_dump.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    38283 2023-02-28 07:37:36.000000 PyBADS-0.8.2/pybads/bads/gaussian_process_train.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5756 2023-02-18 13:47:05.000000 PyBADS-0.8.2/pybads/bads/optimize_result.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.674105 PyBADS-0.8.2/pybads/bads/option_configs/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       53 2023-02-20 16:40:10.000000 PyBADS-0.8.2/pybads/bads/option_configs/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    15671 2023-01-06 15:11:47.000000 PyBADS-0.8.2/pybads/bads/option_configs/advanced_bads_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)      725 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/bads/option_configs/basic_bads_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-02-20 16:40:10.000000 PyBADS-0.8.2/pybads/bads/option_configs/options_confs.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/bads/option_configs/test_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)      108 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/bads/option_configs/test_options2.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)     7371 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/bads/options.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.674105 PyBADS-0.8.2/pybads/decorators/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      573 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/decorators/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)       51 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/decorators/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2175 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/decorators/handle_0D_1D_input.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1779 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/function_examples.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.675105 PyBADS-0.8.2/pybads/function_logger/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      106 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/function_logger/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1730 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/function_logger/constraints_check.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    16376 2023-02-18 13:47:05.000000 PyBADS-0.8.2/pybads/function_logger/function_logger.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.675105 PyBADS-0.8.2/pybads/init_functions/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       35 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/init_functions/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1256 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/init_functions/init_sobol.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.675105 PyBADS-0.8.2/pybads/poll/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/poll/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1403 2023-01-06 15:11:47.000000 PyBADS-0.8.2/pybads/poll/poll_mads_2n.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.675105 PyBADS-0.8.2/pybads/search/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      177 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/search/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10551 2023-02-06 14:04:16.000000 PyBADS-0.8.2/pybads/search/es_search.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1659 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/search/grid_functions.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5377 2023-01-06 15:11:47.000000 PyBADS-0.8.2/pybads/search/search_hedge.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.676105 PyBADS-0.8.2/pybads/stats/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      110 2023-01-06 15:11:47.000000 PyBADS-0.8.2/pybads/stats/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)       87 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/stats/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1197 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/stats/get_hpd.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     8723 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/stats/kde1d.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1435 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/stats/kldiv_mvn.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.676105 PyBADS-0.8.2/pybads/testing/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/__init__.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.677105 PyBADS-0.8.2/pybads/testing/bads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      349 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/X.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      202 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/dF.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)      211 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/dF_gplogjoint.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1286 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/hyp.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)       89 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/mu.dat
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.677105 PyBADS-0.8.2/pybads/testing/bads/poll/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/poll/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      551 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/poll/test_poll_mads.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.678105 PyBADS-0.8.2/pybads/testing/bads/scripts/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      747 2023-02-26 09:26:05.000000 PyBADS-0.8.2/pybads/testing/bads/scripts/ackley_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2629 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1874 2023-02-26 09:26:05.000000 PyBADS-0.8.2/pybads/testing/bads/scripts/bads_rosenbrock_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      908 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/scripts/non_bound_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      780 2023-02-26 09:26:05.000000 PyBADS-0.8.2/pybads/testing/bads/scripts/rastrigin_example.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.678105 PyBADS-0.8.2/pybads/testing/bads/search/
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5573 2023-02-20 16:40:10.000000 PyBADS-0.8.2/pybads/testing/bads/search/test_search.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     6693 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/test_gaussian_process_train.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)       97 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/test_init_conf.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4933 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/test_iteration_history.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      192 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/bads/y.dat
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.678105 PyBADS-0.8.2/pybads/testing/decorators/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/decorators/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4746 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.678105 PyBADS-0.8.2/pybads/testing/function_logger/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/function_logger/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9336 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/function_logger/test_function_logger.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      240 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/run_tests.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.678105 PyBADS-0.8.2/pybads/testing/variable_transformer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/variable_transformer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5524 2023-02-19 09:10:54.000000 PyBADS-0.8.2/pybads/testing/variable_transformer/test_variable_transformer.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.679105 PyBADS-0.8.2/pybads/utils/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      119 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/utils/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4359 2023-01-06 15:11:47.000000 PyBADS-0.8.2/pybads/utils/iteration_history.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      117 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/utils/period_check.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.679105 PyBADS-0.8.2/pybads/utils/timer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/utils/timer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1544 2023-01-06 15:11:47.000000 PyBADS-0.8.2/pybads/utils/timer/timer.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-02-28 07:44:48.679105 PyBADS-0.8.2/pybads/variable_transformer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       55 2022-12-31 10:58:21.000000 PyBADS-0.8.2/pybads/variable_transformer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9919 2023-02-06 14:04:16.000000 PyBADS-0.8.2/pybads/variable_transformer/variables_transformer.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1446 2023-02-17 14:08:47.000000 PyBADS-0.8.2/pyproject.toml
--rw-r--r--   0 jeet      (1000) jeet      (1000)       38 2023-02-28 07:44:48.680105 PyBADS-0.8.2/setup.cfg
--rw-r--r--   0 jeet      (1000) jeet      (1000)      169 2023-02-21 13:00:26.000000 PyBADS-0.8.2/setup.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.968071 PyBADS-1.0.0/
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.951071 PyBADS-1.0.0/.github/
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.955071 PyBADS-1.0.0/.github/workflows/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      504 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/build.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1297 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2223 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/merge-tests.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1054 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2258 2023-06-10 16:10:47.000000 PyBADS-1.0.0/.gitignore
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      619 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1517 2022-12-31 10:58:21.000000 PyBADS-1.0.0/LICENSE
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       12 2023-06-10 16:10:47.000000 PyBADS-1.0.0/MANIFEST.in
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    11820 2023-06-10 18:48:09.968071 PyBADS-1.0.0/PKG-INFO
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.956071 PyBADS-1.0.0/PyBADS.egg-info/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    11820 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/PKG-INFO
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     3456 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/SOURCES.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        1 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/dependency_links.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      313 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/requires.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        7 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/top_level.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     9853 2023-06-10 18:40:03.000000 PyBADS-1.0.0/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      137 2022-12-31 10:58:21.000000 PyBADS-1.0.0/environment.yml
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.956071 PyBADS-1.0.0/examples/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10064 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_1_basic_usage.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     9582 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_2_nonbox_constraints.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    14148 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_3_noisy_objective.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    17944 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_4_user_provided_noise.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10359 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_5_extended_usage.ipynb
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.957071 PyBADS-1.0.0/examples/scripts/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      981 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_1_basic_usage.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1179 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_2_nonbox_constraints.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1307 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_3_noisy_objective.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1637 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_4_user_provided_noise.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1629 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_5_extended_usage.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.957071 PyBADS-1.0.0/pybads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      556 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      635 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/__main__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      160 2023-06-10 18:48:09.000000 PyBADS-1.0.0/pybads/_version.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.957071 PyBADS-1.0.0/pybads/acquisition_functions/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       37 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/acquisition_functions/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1418 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/acquisition_functions/acq_fcn_lcb.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.958071 PyBADS-1.0.0/pybads/bads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      255 2023-06-10 07:26:33.000000 PyBADS-1.0.0/pybads/bads/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      388 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)   103341 2023-06-10 18:40:03.000000 PyBADS-1.0.0/pybads/bads/bads.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2249 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/bads_dump.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    38330 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/gaussian_process_train.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5870 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/optimize_result.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.959071 PyBADS-1.0.0/pybads/bads/option_configs/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       53 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    15922 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/advanced_bads_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      805 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/basic_bads_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/options_confs.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/option_configs/test_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      108 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/option_configs/test_options2.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     7371 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/bads/options.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.959071 PyBADS-1.0.0/pybads/decorators/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      573 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/decorators/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       51 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/decorators/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2175 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/decorators/handle_0D_1D_input.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1779 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/function_examples.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.960071 PyBADS-1.0.0/pybads/function_logger/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      106 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/function_logger/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1731 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/function_logger/constraints_check.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    16376 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/function_logger/function_logger.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.960071 PyBADS-1.0.0/pybads/init_functions/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       35 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/init_functions/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1256 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/init_functions/init_sobol.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.960071 PyBADS-1.0.0/pybads/poll/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/poll/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1403 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/poll/poll_mads_2n.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.961071 PyBADS-1.0.0/pybads/search/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      177 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/search/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10559 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/search/es_search.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1659 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/search/grid_functions.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5383 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/search/search_hedge.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.962071 PyBADS-1.0.0/pybads/stats/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      110 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/stats/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       87 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/stats/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1197 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/stats/get_hpd.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     8723 2023-06-10 07:27:45.000000 PyBADS-1.0.0/pybads/stats/kde1d.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1435 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/stats/kldiv_mvn.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.962071 PyBADS-1.0.0/pybads/testing/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/__init__.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.964071 PyBADS-1.0.0/pybads/testing/bads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      349 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/X.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      202 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/dF.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      211 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/dF_gplogjoint.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1286 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/hyp.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       89 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/mu.dat
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.964071 PyBADS-1.0.0/pybads/testing/bads/poll/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/poll/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      551 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/poll/test_poll_mads.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.965071 PyBADS-1.0.0/pybads/testing/bads/scripts/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      747 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/ackley_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2629 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1874 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/bads_rosenbrock_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      908 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/non_bound_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      780 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/rastrigin_example.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.965071 PyBADS-1.0.0/pybads/testing/bads/search/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5578 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/search/test_search.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     3482 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_bads_optimization.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     6697 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_gaussian_process_train.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      132 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_init_conf.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4933 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_iteration_history.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      192 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/y.dat
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.966071 PyBADS-1.0.0/pybads/testing/decorators/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/decorators/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4746 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.966071 PyBADS-1.0.0/pybads/testing/function_logger/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/function_logger/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     9336 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/function_logger/test_function_logger.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      240 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/run_tests.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.967071 PyBADS-1.0.0/pybads/testing/variable_transformer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/variable_transformer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5524 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/variable_transformer/test_variable_transformer.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.967071 PyBADS-1.0.0/pybads/utils/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      119 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4359 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/iteration_history.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      117 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/period_check.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.967071 PyBADS-1.0.0/pybads/utils/timer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/utils/timer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1544 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/timer/timer.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.968071 PyBADS-1.0.0/pybads/variable_transformer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       55 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/variable_transformer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10171 2023-06-10 18:40:03.000000 PyBADS-1.0.0/pybads/variable_transformer/variables_transformer.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1477 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pyproject.toml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       38 2023-06-10 18:48:09.968071 PyBADS-1.0.0/setup.cfg
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      169 2023-04-23 21:57:13.000000 PyBADS-1.0.0/setup.py
```

### Comparing `PyBADS-0.8.2/.github/workflows/docs.yml` & `PyBADS-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/.github/workflows/merge-tests.yml` & `PyBADS-1.0.0/.github/workflows/merge-tests.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/.github/workflows/tests.yml` & `PyBADS-1.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/.gitignore` & `PyBADS-1.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
+pybads/_version.py
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
```

### Comparing `PyBADS-0.8.2/.pre-commit-config.yaml` & `PyBADS-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/LICENSE` & `PyBADS-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/PKG-INFO` & `PyBADS-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBADS
-Version: 0.8.2
+Version: 1.0.0
 Summary: Bayesian Adaptive Direct Search in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2022, acerbilab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -38,17 +38,17 @@
 License-File: LICENSE
 
 
 # PyBADS: Bayesian Adaptive Direct Search in Python
 
 ## What is it?
 
-PyBads is a Python implementation of the Bayesian Adaptive Direct Search (BADS) algorithm for solving difficult and mildly expensive optimization problems, originally implemented [in MATLAB](https://github.com/lacerbi/bads). BADS has been intensively tested for fitting a variety of computational models, and is currently being used in many computational labs around the world (see [Google Scholar](https://scholar.google.co.uk/scholar?cites=7209174494000095753&as_sdt=2005&sciodt=0,5&hl=en) for many example applications).
+PyBADS is a Python implementation of the Bayesian Adaptive Direct Search (BADS) algorithm for solving difficult and mildly expensive optimization problems, originally implemented [in MATLAB](https://github.com/lacerbi/bads). BADS has been intensively tested for fitting a variety of computational models, and is currently being used in many computational labs around the world (see [Google Scholar](https://scholar.google.co.uk/scholar?cites=7209174494000095753&as_sdt=2005&sciodt=0,5&hl=en) for many example applications).
 
-In a benchmark with real model-fitting problems, BADS performed on par or better than many other common and state-of-the-art optimizers, as shown in the original paper presented at NeurIPS in 2017 [[1](#references-and-citation)].
+In a benchmark with real model-fitting problems from computational and cognitive neuroscience, BADS performed on par or better than many other common and state-of-the-art optimizers, as shown in the original *NeurIPS* paper [[1](#references-and-citation)].
 
 PyBADS requires no specific tuning and runs off-the-shelf like other Python optimizers (e.g., `scipy.optimize.minimize`).
 
 *Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out Variational Bayesian Monte Carlo for Python ([PyVBMC](https://github.com/acerbilab/pyvbmc)), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.
 
 ## Documentation
 
@@ -72,95 +72,89 @@
     python -m pip install pybads
     ```
     or:
     ```console
     conda install --channel=conda-forge pybads
     ```
     PyBADS requires Python version 3.9 or newer.
-2. (Optional): Install Jupyter to view the example Notebooks. You can skip this step if you're working from a Conda environment which already has Jupyter, but be aware that if the wrong `jupyter` executable is found on your path then import errors may arise.
+2. (Optional): Install Jupyter to view the example Notebooks. You can skip this step if you are working from a Conda environment which already has Jupyter, but be aware that if the wrong `jupyter` executable is found on your path then import errors may arise.
    ```console
    conda install jupyter
    ```
    If you are running Python 3.11 and get an `UnsatisfiableError` you may need to install Jupyter from `conda-forge`:
    ```console
    conda install --channel=conda-forge jupyter
    ```
    The example notebooks can then be accessed by running
    ```console
    python -m pybads
    ```
 
 If you wish to install directly from latest source code, please see the [instructions for developers and contributors](/docs/development.html#installation-instructions-for-developers).
 
-### Quick start
+## Quick start
 
 The typical workflow of PyBADS follows four steps:
 
 1. Define the target (or objective) function;
 2. Setup the problem configuration (optimization bounds, starting point, possible constraint violation function);
 3. Initialize and run the optimization;
 4. Examine and visualize the results.
    
 Running the optimizer in step 3 only involves a couple of lines of code:
 
 ```
 from pybads import BADS
 # ...
-bads = BADS(target, x0, lb, ub, plb, pub)
+bads = BADS(target, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds)
 optimize_result = bads.optimize()
 ```
 
 with input arguments:
 
 - ``target``: the target function, it takes as input a vector and returns its function evaluation;
 - ``x0``: the starting point of the optimization problem. If it is not given, the starting point is randomly drawn from the problems bounds;
-- ``lb`` and ``ub``: hard lower and upper bounds for the optimization region (can be ``-inf`` and ``inf``, or bounded);
-- ``plb`` and ``pub``: *plausible* lower and upper bounds, that represent our best guess at bounding the region where the solution might lie;
-- ``non_box_cons`` (optional): a callable non-bound constraints function.
+- ``lower_bounds`` and ``upper_bounds``: hard lower and upper bounds for the optimization region (can be ``-inf`` and ``inf``, or bounded);
+- ``plausible_lower_bounds`` and ``plausible_upper_bounds``: *plausible* lower and upper bounds, that represent our best guess at bounding the region where the solution might lie;
+- ``non_box_cons`` (optional): a callable function that denotes non-box constraint violations.
 
 The outputs are:
 
 - ``optimize_result``: a ``OptimizeResult`` which presents relevant information about the solution and the optimization problem. In particular:
   - ``"x"``: the minimum point found by the optimizer;
   - ``"fval"``: the value of the function at the given solution.
 
 For a full list and description of the entries of the ``optimize_result`` object, see the [OptimizeResult](https://acerbilab.github.io/pybads/api/classes/optimize_result.html) class documentation.
 
-Examples of usages of PyBADS are present in the directory `examples` of the repository, which provides a tutorial going from simpler to more complex problems, such as noisy targets (see [this example notebook](examples/pybads_example_3_noisy_objective.ipynb)).
-
-In addition, checkout the [BADS FAQ](https://github.com/acerbilab/bads/wiki#bads-frequently-asked-questions) page for practical recommendations, such as how to set the bounds `LB` and `UB`, and other practical insights. Even though the FAQ refers to the MATLAB version of BADS, most of the concepts still apply to PyBADS.
-
 ## Next steps
 
-Once installed, example Jupyter notebooks can be found in the `pybads/examples` directory. They can also be [viewed statically](https://acerbilab.github.io/pybads/index.html#examples) on the [main documentation pages](https://acerbilab.github.io/pybads/index.html). These examples will walk you through the basic usage of PyBADS as well as some if its more advanced features.
+Once installed, example Jupyter notebooks can be found in the `pybads/examples` directory. They can also be [viewed statically](https://acerbilab.github.io/pybads/index.html#examples) on the [main documentation pages](https://acerbilab.github.io/pybads/index.html). These examples represent a full tutorial that will walk you through the basic usage of PyBADS as well as some if its more advanced features, such as [noisy targets](examples/pybads_example_3_noisy_objective.ipynb).
 
-For practical recommendations, such as how to set `lb` and `ub` and the plausible bounds, check out the FAQ on the [BADS wiki](https://github.com/acerbilab/bads/wiki). The wiki was written with the MATLAB toolbox in mind, but the general advice applies to the Python version as well.
+For practical recommendations, such as how to set `lower_bounds`, `upper_bounds` and the plausible bounds, check out the FAQ on the [BADS wiki](https://github.com/acerbilab/bads/wiki). Even though the FAQ refers to the MATLAB version of BADS, most of the concepts apply equally to PyBADS.
 
 ## How does it work?
 
 PyBADS/BADS follows a [mesh adaptive direct search](http://epubs.siam.org/doi/abs/10.1137/040603371) (MADS) procedure for function minimization that alternates **poll** steps and **search** steps (see **Fig 1**). 
 
 - In the **poll** stage, points are evaluated on a mesh by taking steps in one direction at a time, until an improvement is found or all directions have been tried. The step size is doubled in case of success, halved otherwise. 
-- In the **search** stage, a [Gaussian process](https://en.wikipedia.org/wiki/Gaussian_process) (GP) is fit to a (local) subset of the points evaluated so far. Then, we iteratively choose points to evaluate according to a *lower confidence bound* strategy that trades off between exploration of uncertain regions (high GP uncertainty) and exploitation of promising solutions (low GP mean).
+- In the **search** stage, a [Gaussian process](https://distill.pub/2019/visual-exploration-gaussian-processes/) (GP) is fit to a (local) subset of the points evaluated so far. Then, we iteratively choose points to evaluate according to a *lower confidence bound* strategy that trades off between exploration of uncertain regions (high GP uncertainty) and exploitation of promising solutions (low GP mean).
 
-**Fig 1: BADS procedure** ![BADS procedure](https://raw.githubusercontent.com/acerbilab/bads/master/docs/bads-cartoon.png)
+**Fig 1: BADS procedure** ![BADS procedure](https://raw.githubusercontent.com/acerbilab/pybads/main/docsrc/source/_static/bads-cartoon.png)
 
 See [here](https://github.com/lacerbi/optimviz) for a visualization of several optimizers at work, including BADS.
 
-See our paper for more details ([Acerbi and Ma, 2017](#references-and-citation)).
+See the original BADS paper for more details ([Acerbi and Ma, 2017](#references-and-citation)).
 
 ## Troubleshooting and contact
 
-PyBADS is under active development. The original BADS algorithm has been extensively tested in several benchmarks and published papers, and the some benchmarks have been replicated using PyBADS. But as with any optimization method, you should double-check your results.
+PyBADS is under active development. The original BADS algorithm has been extensively tested in several benchmarks and published papers, and the some benchmarks have been replicated with PyBADS. However, as with any optimization method, you should double-check your results.
 
 If you have trouble doing something with PyBADS, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyBADS, your problems & applications;
-- [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub;
-- Contact the project lead at <luigi.acerbi@helsinki.fi>, putting 'PyBADS' in the subject of the email.
-
+- [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub.
 
 ## References and citation
 
 1. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
 
 You can cite PyBADS in your work with something along the lines of
```

### Comparing `PyBADS-0.8.2/PyBADS.egg-info/PKG-INFO` & `PyBADS-1.0.0/PyBADS.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBADS
-Version: 0.8.2
+Version: 1.0.0
 Summary: Bayesian Adaptive Direct Search in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2022, acerbilab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -38,17 +38,17 @@
 License-File: LICENSE
 
 
 # PyBADS: Bayesian Adaptive Direct Search in Python
 
 ## What is it?
 
-PyBads is a Python implementation of the Bayesian Adaptive Direct Search (BADS) algorithm for solving difficult and mildly expensive optimization problems, originally implemented [in MATLAB](https://github.com/lacerbi/bads). BADS has been intensively tested for fitting a variety of computational models, and is currently being used in many computational labs around the world (see [Google Scholar](https://scholar.google.co.uk/scholar?cites=7209174494000095753&as_sdt=2005&sciodt=0,5&hl=en) for many example applications).
+PyBADS is a Python implementation of the Bayesian Adaptive Direct Search (BADS) algorithm for solving difficult and mildly expensive optimization problems, originally implemented [in MATLAB](https://github.com/lacerbi/bads). BADS has been intensively tested for fitting a variety of computational models, and is currently being used in many computational labs around the world (see [Google Scholar](https://scholar.google.co.uk/scholar?cites=7209174494000095753&as_sdt=2005&sciodt=0,5&hl=en) for many example applications).
 
-In a benchmark with real model-fitting problems, BADS performed on par or better than many other common and state-of-the-art optimizers, as shown in the original paper presented at NeurIPS in 2017 [[1](#references-and-citation)].
+In a benchmark with real model-fitting problems from computational and cognitive neuroscience, BADS performed on par or better than many other common and state-of-the-art optimizers, as shown in the original *NeurIPS* paper [[1](#references-and-citation)].
 
 PyBADS requires no specific tuning and runs off-the-shelf like other Python optimizers (e.g., `scipy.optimize.minimize`).
 
 *Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out Variational Bayesian Monte Carlo for Python ([PyVBMC](https://github.com/acerbilab/pyvbmc)), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.
 
 ## Documentation
 
@@ -72,95 +72,89 @@
     python -m pip install pybads
     ```
     or:
     ```console
     conda install --channel=conda-forge pybads
     ```
     PyBADS requires Python version 3.9 or newer.
-2. (Optional): Install Jupyter to view the example Notebooks. You can skip this step if you're working from a Conda environment which already has Jupyter, but be aware that if the wrong `jupyter` executable is found on your path then import errors may arise.
+2. (Optional): Install Jupyter to view the example Notebooks. You can skip this step if you are working from a Conda environment which already has Jupyter, but be aware that if the wrong `jupyter` executable is found on your path then import errors may arise.
    ```console
    conda install jupyter
    ```
    If you are running Python 3.11 and get an `UnsatisfiableError` you may need to install Jupyter from `conda-forge`:
    ```console
    conda install --channel=conda-forge jupyter
    ```
    The example notebooks can then be accessed by running
    ```console
    python -m pybads
    ```
 
 If you wish to install directly from latest source code, please see the [instructions for developers and contributors](/docs/development.html#installation-instructions-for-developers).
 
-### Quick start
+## Quick start
 
 The typical workflow of PyBADS follows four steps:
 
 1. Define the target (or objective) function;
 2. Setup the problem configuration (optimization bounds, starting point, possible constraint violation function);
 3. Initialize and run the optimization;
 4. Examine and visualize the results.
    
 Running the optimizer in step 3 only involves a couple of lines of code:
 
 ```
 from pybads import BADS
 # ...
-bads = BADS(target, x0, lb, ub, plb, pub)
+bads = BADS(target, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds)
 optimize_result = bads.optimize()
 ```
 
 with input arguments:
 
 - ``target``: the target function, it takes as input a vector and returns its function evaluation;
 - ``x0``: the starting point of the optimization problem. If it is not given, the starting point is randomly drawn from the problems bounds;
-- ``lb`` and ``ub``: hard lower and upper bounds for the optimization region (can be ``-inf`` and ``inf``, or bounded);
-- ``plb`` and ``pub``: *plausible* lower and upper bounds, that represent our best guess at bounding the region where the solution might lie;
-- ``non_box_cons`` (optional): a callable non-bound constraints function.
+- ``lower_bounds`` and ``upper_bounds``: hard lower and upper bounds for the optimization region (can be ``-inf`` and ``inf``, or bounded);
+- ``plausible_lower_bounds`` and ``plausible_upper_bounds``: *plausible* lower and upper bounds, that represent our best guess at bounding the region where the solution might lie;
+- ``non_box_cons`` (optional): a callable function that denotes non-box constraint violations.
 
 The outputs are:
 
 - ``optimize_result``: a ``OptimizeResult`` which presents relevant information about the solution and the optimization problem. In particular:
   - ``"x"``: the minimum point found by the optimizer;
   - ``"fval"``: the value of the function at the given solution.
 
 For a full list and description of the entries of the ``optimize_result`` object, see the [OptimizeResult](https://acerbilab.github.io/pybads/api/classes/optimize_result.html) class documentation.
 
-Examples of usages of PyBADS are present in the directory `examples` of the repository, which provides a tutorial going from simpler to more complex problems, such as noisy targets (see [this example notebook](examples/pybads_example_3_noisy_objective.ipynb)).
-
-In addition, checkout the [BADS FAQ](https://github.com/acerbilab/bads/wiki#bads-frequently-asked-questions) page for practical recommendations, such as how to set the bounds `LB` and `UB`, and other practical insights. Even though the FAQ refers to the MATLAB version of BADS, most of the concepts still apply to PyBADS.
-
 ## Next steps
 
-Once installed, example Jupyter notebooks can be found in the `pybads/examples` directory. They can also be [viewed statically](https://acerbilab.github.io/pybads/index.html#examples) on the [main documentation pages](https://acerbilab.github.io/pybads/index.html). These examples will walk you through the basic usage of PyBADS as well as some if its more advanced features.
+Once installed, example Jupyter notebooks can be found in the `pybads/examples` directory. They can also be [viewed statically](https://acerbilab.github.io/pybads/index.html#examples) on the [main documentation pages](https://acerbilab.github.io/pybads/index.html). These examples represent a full tutorial that will walk you through the basic usage of PyBADS as well as some if its more advanced features, such as [noisy targets](examples/pybads_example_3_noisy_objective.ipynb).
 
-For practical recommendations, such as how to set `lb` and `ub` and the plausible bounds, check out the FAQ on the [BADS wiki](https://github.com/acerbilab/bads/wiki). The wiki was written with the MATLAB toolbox in mind, but the general advice applies to the Python version as well.
+For practical recommendations, such as how to set `lower_bounds`, `upper_bounds` and the plausible bounds, check out the FAQ on the [BADS wiki](https://github.com/acerbilab/bads/wiki). Even though the FAQ refers to the MATLAB version of BADS, most of the concepts apply equally to PyBADS.
 
 ## How does it work?
 
 PyBADS/BADS follows a [mesh adaptive direct search](http://epubs.siam.org/doi/abs/10.1137/040603371) (MADS) procedure for function minimization that alternates **poll** steps and **search** steps (see **Fig 1**). 
 
 - In the **poll** stage, points are evaluated on a mesh by taking steps in one direction at a time, until an improvement is found or all directions have been tried. The step size is doubled in case of success, halved otherwise. 
-- In the **search** stage, a [Gaussian process](https://en.wikipedia.org/wiki/Gaussian_process) (GP) is fit to a (local) subset of the points evaluated so far. Then, we iteratively choose points to evaluate according to a *lower confidence bound* strategy that trades off between exploration of uncertain regions (high GP uncertainty) and exploitation of promising solutions (low GP mean).
+- In the **search** stage, a [Gaussian process](https://distill.pub/2019/visual-exploration-gaussian-processes/) (GP) is fit to a (local) subset of the points evaluated so far. Then, we iteratively choose points to evaluate according to a *lower confidence bound* strategy that trades off between exploration of uncertain regions (high GP uncertainty) and exploitation of promising solutions (low GP mean).
 
-**Fig 1: BADS procedure** ![BADS procedure](https://raw.githubusercontent.com/acerbilab/bads/master/docs/bads-cartoon.png)
+**Fig 1: BADS procedure** ![BADS procedure](https://raw.githubusercontent.com/acerbilab/pybads/main/docsrc/source/_static/bads-cartoon.png)
 
 See [here](https://github.com/lacerbi/optimviz) for a visualization of several optimizers at work, including BADS.
 
-See our paper for more details ([Acerbi and Ma, 2017](#references-and-citation)).
+See the original BADS paper for more details ([Acerbi and Ma, 2017](#references-and-citation)).
 
 ## Troubleshooting and contact
 
-PyBADS is under active development. The original BADS algorithm has been extensively tested in several benchmarks and published papers, and the some benchmarks have been replicated using PyBADS. But as with any optimization method, you should double-check your results.
+PyBADS is under active development. The original BADS algorithm has been extensively tested in several benchmarks and published papers, and the some benchmarks have been replicated with PyBADS. However, as with any optimization method, you should double-check your results.
 
 If you have trouble doing something with PyBADS, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyBADS, your problems & applications;
-- [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub;
-- Contact the project lead at <luigi.acerbi@helsinki.fi>, putting 'PyBADS' in the subject of the email.
-
+- [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub.
 
 ## References and citation
 
 1. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
 
 You can cite PyBADS in your work with something along the lines of
```

### Comparing `PyBADS-0.8.2/PyBADS.egg-info/SOURCES.txt` & `PyBADS-1.0.0/PyBADS.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 examples/scripts/pybads_example_1_basic_usage.py
 examples/scripts/pybads_example_2_nonbox_constraints.py
 examples/scripts/pybads_example_3_noisy_objective.py
 examples/scripts/pybads_example_4_user_provided_noise.py
 examples/scripts/pybads_example_5_extended_usage.py
 pybads/__init__.py
 pybads/__main__.py
+pybads/_version.py
 pybads/function_examples.py
 pybads/acquisition_functions/__init__.py
 pybads/acquisition_functions/acq_fcn_lcb.py
 pybads/bads/README.md
 pybads/bads/__init__.py
 pybads/bads/bads.py
 pybads/bads/bads_dump.py
@@ -66,14 +67,15 @@
 pybads/testing/run_tests.py
 pybads/testing/bads/X.dat
 pybads/testing/bads/__init__.py
 pybads/testing/bads/dF.dat
 pybads/testing/bads/dF_gplogjoint.dat
 pybads/testing/bads/hyp.dat
 pybads/testing/bads/mu.dat
+pybads/testing/bads/test_bads_optimization.py
 pybads/testing/bads/test_gaussian_process_train.py
 pybads/testing/bads/test_init_conf.py
 pybads/testing/bads/test_iteration_history.py
 pybads/testing/bads/y.dat
 pybads/testing/bads/poll/__init__.py
 pybads/testing/bads/poll/test_poll_mads.py
 pybads/testing/bads/scripts/ackley_example.py
```

### Comparing `PyBADS-0.8.2/README.md` & `PyBADS-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # PyBADS: Bayesian Adaptive Direct Search in Python
 
 ## What is it?
 
-PyBads is a Python implementation of the Bayesian Adaptive Direct Search (BADS) algorithm for solving difficult and mildly expensive optimization problems, originally implemented [in MATLAB](https://github.com/lacerbi/bads). BADS has been intensively tested for fitting a variety of computational models, and is currently being used in many computational labs around the world (see [Google Scholar](https://scholar.google.co.uk/scholar?cites=7209174494000095753&as_sdt=2005&sciodt=0,5&hl=en) for many example applications).
+PyBADS is a Python implementation of the Bayesian Adaptive Direct Search (BADS) algorithm for solving difficult and mildly expensive optimization problems, originally implemented [in MATLAB](https://github.com/lacerbi/bads). BADS has been intensively tested for fitting a variety of computational models, and is currently being used in many computational labs around the world (see [Google Scholar](https://scholar.google.co.uk/scholar?cites=7209174494000095753&as_sdt=2005&sciodt=0,5&hl=en) for many example applications).
 
-In a benchmark with real model-fitting problems, BADS performed on par or better than many other common and state-of-the-art optimizers, as shown in the original paper presented at NeurIPS in 2017 [[1](#references-and-citation)].
+In a benchmark with real model-fitting problems from computational and cognitive neuroscience, BADS performed on par or better than many other common and state-of-the-art optimizers, as shown in the original *NeurIPS* paper [[1](#references-and-citation)].
 
 PyBADS requires no specific tuning and runs off-the-shelf like other Python optimizers (e.g., `scipy.optimize.minimize`).
 
 *Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out Variational Bayesian Monte Carlo for Python ([PyVBMC](https://github.com/acerbilab/pyvbmc)), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.
 
 ## Documentation
 
@@ -33,95 +33,89 @@
     python -m pip install pybads
     ```
     or:
     ```console
     conda install --channel=conda-forge pybads
     ```
     PyBADS requires Python version 3.9 or newer.
-2. (Optional): Install Jupyter to view the example Notebooks. You can skip this step if you're working from a Conda environment which already has Jupyter, but be aware that if the wrong `jupyter` executable is found on your path then import errors may arise.
+2. (Optional): Install Jupyter to view the example Notebooks. You can skip this step if you are working from a Conda environment which already has Jupyter, but be aware that if the wrong `jupyter` executable is found on your path then import errors may arise.
    ```console
    conda install jupyter
    ```
    If you are running Python 3.11 and get an `UnsatisfiableError` you may need to install Jupyter from `conda-forge`:
    ```console
    conda install --channel=conda-forge jupyter
    ```
    The example notebooks can then be accessed by running
    ```console
    python -m pybads
    ```
 
 If you wish to install directly from latest source code, please see the [instructions for developers and contributors](/docs/development.html#installation-instructions-for-developers).
 
-### Quick start
+## Quick start
 
 The typical workflow of PyBADS follows four steps:
 
 1. Define the target (or objective) function;
 2. Setup the problem configuration (optimization bounds, starting point, possible constraint violation function);
 3. Initialize and run the optimization;
 4. Examine and visualize the results.
    
 Running the optimizer in step 3 only involves a couple of lines of code:
 
 ```
 from pybads import BADS
 # ...
-bads = BADS(target, x0, lb, ub, plb, pub)
+bads = BADS(target, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds)
 optimize_result = bads.optimize()
 ```
 
 with input arguments:
 
 - ``target``: the target function, it takes as input a vector and returns its function evaluation;
 - ``x0``: the starting point of the optimization problem. If it is not given, the starting point is randomly drawn from the problems bounds;
-- ``lb`` and ``ub``: hard lower and upper bounds for the optimization region (can be ``-inf`` and ``inf``, or bounded);
-- ``plb`` and ``pub``: *plausible* lower and upper bounds, that represent our best guess at bounding the region where the solution might lie;
-- ``non_box_cons`` (optional): a callable non-bound constraints function.
+- ``lower_bounds`` and ``upper_bounds``: hard lower and upper bounds for the optimization region (can be ``-inf`` and ``inf``, or bounded);
+- ``plausible_lower_bounds`` and ``plausible_upper_bounds``: *plausible* lower and upper bounds, that represent our best guess at bounding the region where the solution might lie;
+- ``non_box_cons`` (optional): a callable function that denotes non-box constraint violations.
 
 The outputs are:
 
 - ``optimize_result``: a ``OptimizeResult`` which presents relevant information about the solution and the optimization problem. In particular:
   - ``"x"``: the minimum point found by the optimizer;
   - ``"fval"``: the value of the function at the given solution.
 
 For a full list and description of the entries of the ``optimize_result`` object, see the [OptimizeResult](https://acerbilab.github.io/pybads/api/classes/optimize_result.html) class documentation.
 
-Examples of usages of PyBADS are present in the directory `examples` of the repository, which provides a tutorial going from simpler to more complex problems, such as noisy targets (see [this example notebook](examples/pybads_example_3_noisy_objective.ipynb)).
-
-In addition, checkout the [BADS FAQ](https://github.com/acerbilab/bads/wiki#bads-frequently-asked-questions) page for practical recommendations, such as how to set the bounds `LB` and `UB`, and other practical insights. Even though the FAQ refers to the MATLAB version of BADS, most of the concepts still apply to PyBADS.
-
 ## Next steps
 
-Once installed, example Jupyter notebooks can be found in the `pybads/examples` directory. They can also be [viewed statically](https://acerbilab.github.io/pybads/index.html#examples) on the [main documentation pages](https://acerbilab.github.io/pybads/index.html). These examples will walk you through the basic usage of PyBADS as well as some if its more advanced features.
+Once installed, example Jupyter notebooks can be found in the `pybads/examples` directory. They can also be [viewed statically](https://acerbilab.github.io/pybads/index.html#examples) on the [main documentation pages](https://acerbilab.github.io/pybads/index.html). These examples represent a full tutorial that will walk you through the basic usage of PyBADS as well as some if its more advanced features, such as [noisy targets](examples/pybads_example_3_noisy_objective.ipynb).
 
-For practical recommendations, such as how to set `lb` and `ub` and the plausible bounds, check out the FAQ on the [BADS wiki](https://github.com/acerbilab/bads/wiki). The wiki was written with the MATLAB toolbox in mind, but the general advice applies to the Python version as well.
+For practical recommendations, such as how to set `lower_bounds`, `upper_bounds` and the plausible bounds, check out the FAQ on the [BADS wiki](https://github.com/acerbilab/bads/wiki). Even though the FAQ refers to the MATLAB version of BADS, most of the concepts apply equally to PyBADS.
 
 ## How does it work?
 
 PyBADS/BADS follows a [mesh adaptive direct search](http://epubs.siam.org/doi/abs/10.1137/040603371) (MADS) procedure for function minimization that alternates **poll** steps and **search** steps (see **Fig 1**). 
 
 - In the **poll** stage, points are evaluated on a mesh by taking steps in one direction at a time, until an improvement is found or all directions have been tried. The step size is doubled in case of success, halved otherwise. 
-- In the **search** stage, a [Gaussian process](https://en.wikipedia.org/wiki/Gaussian_process) (GP) is fit to a (local) subset of the points evaluated so far. Then, we iteratively choose points to evaluate according to a *lower confidence bound* strategy that trades off between exploration of uncertain regions (high GP uncertainty) and exploitation of promising solutions (low GP mean).
+- In the **search** stage, a [Gaussian process](https://distill.pub/2019/visual-exploration-gaussian-processes/) (GP) is fit to a (local) subset of the points evaluated so far. Then, we iteratively choose points to evaluate according to a *lower confidence bound* strategy that trades off between exploration of uncertain regions (high GP uncertainty) and exploitation of promising solutions (low GP mean).
 
-**Fig 1: BADS procedure** ![BADS procedure](https://raw.githubusercontent.com/acerbilab/bads/master/docs/bads-cartoon.png)
+**Fig 1: BADS procedure** ![BADS procedure](https://raw.githubusercontent.com/acerbilab/pybads/main/docsrc/source/_static/bads-cartoon.png)
 
 See [here](https://github.com/lacerbi/optimviz) for a visualization of several optimizers at work, including BADS.
 
-See our paper for more details ([Acerbi and Ma, 2017](#references-and-citation)).
+See the original BADS paper for more details ([Acerbi and Ma, 2017](#references-and-citation)).
 
 ## Troubleshooting and contact
 
-PyBADS is under active development. The original BADS algorithm has been extensively tested in several benchmarks and published papers, and the some benchmarks have been replicated using PyBADS. But as with any optimization method, you should double-check your results.
+PyBADS is under active development. The original BADS algorithm has been extensively tested in several benchmarks and published papers, and the some benchmarks have been replicated with PyBADS. However, as with any optimization method, you should double-check your results.
 
 If you have trouble doing something with PyBADS, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyBADS, your problems & applications;
-- [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub;
-- Contact the project lead at <luigi.acerbi@helsinki.fi>, putting 'PyBADS' in the subject of the email.
-
+- [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub.
 
 ## References and citation
 
 1. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
 
 You can cite PyBADS in your work with something along the lines of
```

### Comparing `PyBADS-0.8.2/examples/pybads_example_1_basic_usage.ipynb` & `PyBADS-1.0.0/examples/pybads_example_1_basic_usage.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9837905969416386%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'This notebook is Part 1 of a series of notebooks in "*

 * *            "which we present various example usages for BADS with the PyBADS package.\\n'), (3, "*

 * *            "'The code used in this example is available as a script "*

 * *            "[here](./scripts/pybads_example_1_basic_usage.py).')], delete: [2]}}, 3: {'source': "*

 * *            "{insert: [(12, 'BADS requires no specific tuning and runs off-the-shelf like other "*

 * *            "built-in Python optimizers (e.g., f […]*

```diff
@@ -11,15 +11,16 @@
         {
             "cell_type": "markdown",
             "id": "7f191949",
             "metadata": {},
             "source": [
                 "In this introductory example, we will show a simple usage of Bayesian Adaptive Direct Search (BADS) to perform optimization of a synthetic target function.\n",
                 "\n",
-                "This notebook is Part 1 of a series of notebooks in which we present various example usages for BADS with the PyBADS package."
+                "This notebook is Part 1 of a series of notebooks in which we present various example usages for BADS with the PyBADS package.\n",
+                "The code used in this example is available as a script [here](./scripts/pybads_example_1_basic_usage.py)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "eef2e4d6",
             "metadata": {},
@@ -42,39 +43,39 @@
                 "\n",
                 "BADS is particularly recommended when:\n",
                 "- the objective function landscape is rough (nonsmooth), typically due to numerical approximations or noise;\n",
                 "- the objective function is moderately expensive to compute (e.g., more than 0.1 second per function evaluation);\n",
                 "- the gradient is unavailable;\n",
                 "- the number of input parameters is up to about `D = 20` or so.\n",
                 "\n",
-                "BADS requires no specific tuning and runs off-the-shelf like other built-in optimizers (e.g., from `scipy.optimize.minimize`).\n",
+                "BADS requires no specific tuning and runs off-the-shelf like other built-in Python optimizers (e.g., from `scipy.optimize.minimize`).\n",
                 "\n",
-                "*Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out Variational Bayesian Monte Carlo for Python (PyVBMC), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.\n",
+                "*Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out [Variational Bayesian Monte Carlo for Python (PyVBMC)](https://github.com/acerbilab/pyvbmc), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.\n",
                 "\n",
                 "### Optimization problem\n",
                 "\n",
                 "Formally, the goal of BADS is to *minimize* a target (or objective) function $f(\\mathbf{x}): \\mathbb{R}^D \\rightarrow \\mathbb{R}$, for $\\mathbf{x} \\in \\mathbb{R}^D$,\n",
                 "$$\n",
-                "\\mathbf{x}^\\star = \\arg\\min_\\mathbf{x} f(\\mathbf{x}) \\qquad \\text{with} \\; \\text{lb}_d \\le x_d \\le \\text{ub}_d \\; \\text{ for } 1\\le d \\le D,\n",
+                "\\mathbf{x}^\\star = \\arg\\min_\\mathbf{x} f(\\mathbf{x}) \\qquad \\text{with} \\; \\text{lower_bounds}_d \\le x_d \\le \\text{upper_bounds}_d \\; \\text{ for } 1\\le d \\le D,\n",
                 "$$\n",
-                "where $D$ is the dimensionality of the problem and `lb`, `ub` are arrays representing lower/upper bound constraints, which can be set to infinite for unbounded parameters."
+                "where $D$ is the dimensionality of the problem and `lower_bounds`, `upper_bounds` are arrays representing lower/upper bound constraints, which can be set to infinite for unbounded parameters."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2456c17e",
             "metadata": {},
             "source": [
                 "## 1. Problem setup\n",
                 "\n",
                 "Here we show PyBADS at work on [Rosenbrock's banana function](https://en.wikipedia.org/wiki/Rosenbrock_function) in 2D as target function.  \n",
                 "\n",
                 "We specify wide hard bounds and tighter plausible bounds that (hopefully) contain the solution. \n",
-                "- Hard lower/upper bounds `lb`, `ub` are the actual optimization bounds; PyBADS will not evaluate the target function outside these bounds, but might evaluate the target on the bounds. You can use `-np.inf` and `np.inf` for unbounded parameters.\n",
-                "- Plausible lower/upper bounds `plb`, `pub` represent our best guess at bounding the region where the solution might lie. The plausible bounds do not change the optimization problem, but help define the initial exploration and hyperparameters of PyBADS.\n",
+                "- Hard lower/upper bounds `lower_bounds`, `upper_bounds` are the actual optimization bounds; PyBADS will not evaluate the target function outside these bounds, but might evaluate the target on the bounds. You can use `-np.inf` and `np.inf` for unbounded parameters.\n",
+                "- Plausible lower/upper bounds `plausible_lower_bounds`, `plausible_upper_bounds` represent our best guess at bounding the region where the solution might lie. The plausible bounds do not change the optimization problem, but help define the initial exploration and hyperparameters of PyBADS.\n",
                 "\n",
                 "We set as starting point for the optimization $\\mathbf{x}_0 = (0, 0)$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
@@ -85,18 +86,18 @@
                 "def rosenbrocks_fcn(x):\n",
                 "    \"\"\"Rosenbrock's 'banana' function in any dimension.\"\"\"\n",
                 "    x_2d = np.atleast_2d(x)\n",
                 "    return np.sum(100 * (x_2d[:, 0:-1]**2 - x_2d[:, 1:])**2 + (x_2d[:, 0:-1]-1)**2, axis=1)\n",
                 "\n",
                 "target = rosenbrocks_fcn;\n",
                 "\n",
-                "lb = np.array([-20, -20])     # Lower bounds\n",
-                "ub = np.array([20, 20])       # Upper bounds\n",
-                "plb = np.array([-5, -5])      # Plausible lower bounds\n",
-                "pub = np.array([5, 5])        # Plausible upper bounds\n",
+                "lower_bounds = np.array([-20, -20])\n",
+                "upper_bounds = np.array([20, 20])\n",
+                "plausible_lower_bounds = np.array([-5, -5])\n",
+                "plausible_upper_bounds = np.array([5, 5])\n",
                 "x0 = np.array([0, 0]);        # Starting point"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d6fb12aa",
             "metadata": {},
@@ -120,60 +121,57 @@
                         "Beginning optimization of a DETERMINISTIC objective function\n",
                         "\n",
                         " Iteration    f-count         f(x)           MeshScale          Method             Actions\n",
                         "     0           2               1               1                                 Uncertainty test\n",
                         "     0           6               1               1         Initial mesh            Initial points\n",
                         "     0          10               1             0.5         Refine grid             Train\n",
                         "     1          18               1            0.25         Refine grid             Train\n",
-                        "     2          19       0.0600236            0.25     Successful search (ES-wcm)        \n",
-                        "     2          24      0.00320034            0.25     Incremental search (ES-ell)        \n",
-                        "     2          30      0.00320034           0.125         Refine grid             Train\n",
-                        "     3          34     0.000634688           0.125     Incremental search (ES-wcm)        \n",
-                        "     3          38     0.000634688          0.0625         Refine grid             \n",
-                        "     4          46     0.000634688         0.03125         Refine grid             \n",
-                        "     5          48     0.000629039         0.03125     Incremental search (ES-ell)        \n",
-                        "     5          54     0.000629039        0.015625         Refine grid             Train\n",
-                        "     6          58     0.000456147        0.015625     Incremental search (ES-ell)        \n",
-                        "     6          62     0.000456147      0.00390625         Refine grid             Train\n",
-                        "     7          63     0.000342996      0.00390625     Incremental search (ES-ell)        \n",
-                        "     7          70     0.000342996     0.000976562         Refine grid             \n",
-                        "     8          71     0.000320662     0.000976562     Incremental search (ES-wcm)        \n",
-                        "Optimization terminated: change in the function value less than options.TolFun.\n",
-                        "Function value at minimum: 0.0003206622739026016\n",
+                        "     2          22        0.250428            0.25     Successful search (ES-wcm)        \n",
+                        "     2          24       0.0851394            0.25     Successful search (ES-ell)        \n",
+                        "     2          26      0.00997961            0.25     Incremental search (ES-ell)        \n",
+                        "     2          27     0.000224117            0.25     Incremental search (ES-ell)        \n",
+                        "     2          34     0.000224117           0.125         Refine grid             \n",
+                        "     3          42     0.000224117          0.0625         Refine grid             Train\n",
+                        "     4          44     7.97867e-05          0.0625     Incremental search (ES-wcm)        \n",
+                        "     4          50     7.97867e-05         0.03125         Refine grid             \n",
+                        "     5          58     7.97867e-05       0.0078125         Refine grid             \n",
+                        "     6          66     7.97867e-05      0.00195312         Refine grid             Train\n",
+                        "Optimization terminated: change in the function value less than options['tol_fun'].\n",
+                        "Function value at minimum: 7.97867122044391e-05\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "bads = BADS(target, x0, lb, ub, plb, pub)\n",
+                "bads = BADS(target, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds)\n",
                 "optimize_result = bads.optimize()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2cc75241",
             "metadata": {},
             "source": [
                 "## 3. Results and conclusions\n",
                 "\n",
-                "We examine now the result of the optimization stored in `optimize_result`. The most important keys are the minimum, `optimize_result['x']`, and the value of the function at the solution, `optimize_result['fval']`."
+                "We examine now the result of the optimization stored in `optimize_result`. The most important keys are the location of the minimum, `optimize_result['x']`, and the value of the function at the minimum, `optimize_result['fval']`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "9b95d46d",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "BADS minimum at: x_min = [1.01732125 1.0353968 ], fval = 0.0003207\n",
-                        "total f-count: 71, time: 4.07 s\n"
+                        "BADS minimum at: x_min = [1.00744247 1.01543427], fval = 7.979e-05\n",
+                        "total f-count: 67, time: 1.34 s\n"
                     ]
                 }
             ],
             "source": [
                 "x_min = optimize_result['x']\n",
                 "fval = optimize_result['fval']\n",
                 "\n",
@@ -182,29 +180,19 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d7d79d83",
             "metadata": {},
             "source": [
-                "The true minimum of the Rosenbrock function is at $\\textbf{x}^\\star = [1, 1]$, where $f^\\star = 0$.  \n",
+                "For reference, the true minimum of the Rosenbrock function is at $\\textbf{x}^\\star = [1, 1]$, where $f^\\star = 0$.  \n",
                 "\n",
                 "In conclusion, PyBADS found the solution with a fairly small number of function evaluations (`f-count`), which is particularly important if the target function is mildly-to-very expensive to compute as in many computational models.\n",
                 "\n",
-                "*Note*: PyBADS by default does not aim for extreme numerical precision of the target (e.g., beyond the 2nd or 3rd decimal place), since in most realistic model-fitting problems a higher resolution is typically pointless, e.g. due to noise or variability in the data."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "e6b8571e",
-            "metadata": {},
-            "source": [
-                "## Example 1: Full code\n",
-                "\n",
-                "See [here](./scripts/pybads_example_1_basic_usage.py) for a Python file with the code used in this example, with no extra fluff."
+                "*Note*: PyBADS by default does not aim for extreme numerical precision of the target (e.g., beyond the 2nd or 3rd decimal place), since in most realistic model-fitting problems a higher resolution is not particularly useful, e.g. due to noise or variability in the data."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -216,15 +204,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "5f12204c93c4274de084c6b76e73171147c8e51a8507bf20dfb1db4f14f6829f"
             }
         }
     },
```

### Comparing `PyBADS-0.8.2/examples/pybads_example_2_nonbox_constraints.ipynb` & `PyBADS-1.0.0/examples/pybads_example_2_nonbox_constraints.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9817747549518383%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'This notebook is Part 2 of a series of notebooks in "*

 * *            "which we present various example usages for BADS with the PyBADS package.\\n'), (3, "*

 * *            "'The code used in this example is available as a script "*

 * *            "[here](./scripts/pybads_example_2_nonbox_constraints.py).')], delete: [2]}}, 4: "*

 * *            "{'source': {insert: [(4, 'Since we know the optimization region, we set tight box "*

 * *            'bounds `lb` and `ub` around the circle.  […]*

```diff
@@ -11,15 +11,16 @@
         {
             "cell_type": "markdown",
             "id": "810b5d8b",
             "metadata": {},
             "source": [
                 "In this example, we will show how to set more complex constraints in PyBADS, besides a simple bounded box.\n",
                 "\n",
-                "This notebook is Part 2 of a series of notebooks in which we present various example usages for BADS with the PyBADS package."
+                "This notebook is Part 2 of a series of notebooks in which we present various example usages for BADS with the PyBADS package.\n",
+                "The code used in this example is available as a script [here](./scripts/pybads_example_2_nonbox_constraints.py)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "d0c7306b",
             "metadata": {},
@@ -51,19 +52,21 @@
             "id": "fccd1931",
             "metadata": {},
             "source": [
                 "## 1. Problem setup\n",
                 "\n",
                 "We optimize [Rosenbrock's banana function](https://en.wikipedia.org/wiki/Rosenbrock_function) in 2D as in the [previous example](./pybads_example_1_basic_usage.ipynb), but here we force the input to stay within a circle with unit radius.\n",
                 "\n",
-                "Since we know the optimization region, we set tight box bounds `lb` and `ub` around the circle. This step is not necessary, but it will further help the search.\n",
+                "Since we know the optimization region, we set tight box bounds `lb` and `ub` around the circle. This step is not necessary, but it is recommended as it further helps the search.\n",
                 "\n",
                 "The function passed to `non_box_cons`: \n",
                 "- takes as input an array $\\mathbf{x}_1, \\ldots, \\mathbf{x}_M$ with shape `(M, D)`, where each $\\mathbf{x}_m \\in \\mathbb{R}^D$;\n",
-                "- outputs a `bool` array with shape `(M, 1)`, where the $m$-th value is `True` if $\\mathbf{x}_m$ *violates* the constraint, `False` otherwise ($M$ is an arbitrary number of inputs)."
+                "- outputs a `bool` array with shape `(M, 1)`, where the $m$-th value is `True` if $\\mathbf{x}_m$ *violates* the constraint, `False` otherwise;\n",
+                "\n",
+                "where $M$ is an arbitrary number of inputs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "192fbe30",
             "metadata": {},
@@ -71,16 +74,16 @@
             "source": [
                 "def rosenbrocks_fcn(x):\n",
                 "    \"\"\"Rosenbrock's 'banana' function in any dimension.\"\"\"\n",
                 "    x_2d = np.atleast_2d(x)\n",
                 "    return np.sum(100 * (x_2d[:, 0:-1]**2 - x_2d[:, 1:])**2 + (x_2d[:, 0:-1]-1)**2, axis=1)\n",
                 "\n",
                 "x0 = np.array([0, 0]);      # Starting point\n",
-                "lb = np.array([-1, -1])     # Lower bounds\n",
-                "ub = np.array([1, 1])       # Upper bounds\n",
+                "lower_bounds = np.array([-1, -1])\n",
+                "upper_bounds = np.array([1, 1])\n",
                 "\n",
                 "def circle_constr(x):\n",
                 "    \"\"\"Return constraints violation outside the unit circle.\"\"\"\n",
                 "    x_2d = np.atleast_2d(x)\n",
                 "    # Note that nonboxcons assumes the function takes a 2D input \n",
                 "    return np.sum(x_2d**2, axis=1) > 1."
             ]
@@ -88,15 +91,15 @@
         {
             "cell_type": "markdown",
             "id": "363e280e",
             "metadata": {},
             "source": [
                 "## 2. Run the optimization\n",
                 "\n",
-                "We initialize `bads` with the non-box constraints defined by `non_box_cons`. Note that we also still specify standard box constraints `lb` and `ub`, as this will help the search.\n",
+                "We initialize `bads` with the non-box constraints defined by `non_box_cons`. Note that we also still specify standard box constraints `lower_bounds` and `upper_bounds`, as this will help the search.\n",
                 "\n",
                 "Here BADS will complain because we did not specify the plausible bounds explicitly. In the absence of plausible bounds, BADS will create them based on the lower/upper bounds instead. As a general rule, it is strongly recommended to specify the plausible bounds."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
@@ -110,37 +113,43 @@
                         "bads:TooCloseBounds: For each variable, hard and plausible bounds should not be too close. Moving plausible bounds.\n",
                         "Beginning optimization of a DETERMINISTIC objective function\n",
                         "\n",
                         " Iteration    f-count         f(x)           MeshScale          Method             Actions\n",
                         "     0           2               1               1                                 Uncertainty test\n",
                         "     0           5               1               1         Initial mesh            Initial points\n",
                         "     0           9               1             0.5         Refine grid             Train\n",
-                        "     1          13        0.767214             0.5     Incremental search (ES-wcm)        \n",
-                        "     1          17        0.767214            0.25         Refine grid             Train\n",
-                        "     2          19        0.580625            0.25     Successful search (ES-ell)        \n",
-                        "     2          20        0.401071            0.25     Successful search (ES-ell)        \n",
-                        "     2          23        0.231718            0.25     Successful search (ES-wcm)        \n",
-                        "     2          24        0.136006            0.25     Incremental search (ES-wcm)        \n",
-                        "     2          25       0.0459402            0.25     Incremental search (ES-ell)        \n",
-                        "     2          31       0.0459402           0.125         Refine grid             \n",
-                        "     3          35       0.0457466           0.125     Incremental search (ES-wcm)        \n",
-                        "     3          37       0.0457466          0.0625         Refine grid             \n",
-                        "     4          43       0.0457466         0.03125         Refine grid             \n",
-                        "     5          44       0.0457105         0.03125     Incremental search (ES-ell)        \n",
-                        "     5          49       0.0457105       0.0078125         Refine grid             \n",
-                        "     6          50       0.0456749       0.0078125     Incremental search (ES-wcm)        \n",
-                        "     6          55       0.0456749      0.00195312         Refine grid             \n",
-                        "Optimization terminated: change in the function value less than options.TolFun.\n",
-                        "Function value at minimum: 0.04567486581177021\n",
+                        "     1          13         0.71573             0.5     Incremental search (ES-wcm)        \n",
+                        "     1          17         0.71573            0.25         Refine grid             Train\n",
+                        "     2          18        0.213085            0.25     Successful search (ES-wcm)        \n",
+                        "     2          20       0.0866235            0.25     Successful search (ES-wcm)        \n",
+                        "     2          22       0.0750055            0.25     Incremental search (ES-wcm)        \n",
+                        "     2          23       0.0555838            0.25     Incremental search (ES-ell)        \n",
+                        "     2          24       0.0503648            0.25     Incremental search (ES-ell)        \n",
+                        "     2          27       0.0503648           0.125         Refine grid             \n",
+                        "     3          28       0.0473246           0.125     Incremental search (ES-wcm)        \n",
+                        "     3          29       0.0460316           0.125     Incremental search (ES-wcm)        \n",
+                        "     3          30       0.0460089           0.125     Incremental search (ES-ell)        \n",
+                        "     3          33       0.0460089          0.0625         Refine grid             \n",
+                        "     4          36       0.0459778          0.0625     Incremental search (ES-wcm)        \n",
+                        "     4          39       0.0459778         0.03125         Refine grid             Train\n",
+                        "     5          40       0.0457596         0.03125     Incremental search (ES-ell)        \n",
+                        "     5          43       0.0456915         0.03125     Incremental search (ES-ell)        \n",
+                        "     5          45       0.0456915        0.015625         Refine grid             \n",
+                        "     6          48       0.0456879        0.015625     Incremental search (ES-ell)        \n",
+                        "     6          51       0.0456879      0.00390625         Refine grid             Train\n",
+                        "     7          55       0.0456831      0.00390625     Incremental search (ES-ell)        \n",
+                        "     7          57       0.0456831     0.000976562         Refine grid             \n",
+                        "Optimization terminated: change in the function value less than options['tol_fun'].\n",
+                        "Function value at minimum: 0.04568314807326722\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "bads = BADS(rosenbrocks_fcn, x0, lb, ub, non_box_cons=circle_constr)\n",
+                "bads = BADS(rosenbrocks_fcn, x0, lower_bounds, upper_bounds, non_box_cons=circle_constr)\n",
                 "optimize_result = bads.optimize()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4a7af7d8",
             "metadata": {},
@@ -154,16 +163,16 @@
             "id": "6507b31a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "BADS minimum at: x_min = [0.78642143 0.61769016], fval = 0.04567\n",
-                        "total f-count: 56, time: 2.91 s\n",
+                        "BADS minimum at: x_min = [0.78639246 0.6176717 ], fval = 0.04568\n",
+                        "total f-count: 58, time: 1.03 s\n",
                         "Problem type: non-box constraints\n"
                     ]
                 }
             ],
             "source": [
                 "x_min = optimize_result['x']\n",
                 "fval = optimize_result['fval']\n",
@@ -181,43 +190,33 @@
                 "The true global minimum of the Rosenbrock function under these constraints is at $\\textbf{x}^\\star = [0.786,0.618]$, where $f^\\star = 0.0457$.\n",
                 "\n",
                 "### Remarks\n",
                 "\n",
                 "- While in theory `non_box_cons` can receive any arbitrary constraints, in practice PyBADS will likely work well only within relatively simple domains (e.g., simple convex regions), as the current version of (Py)BADS uses a simple heuristic to reject samples outside the admissible region.\n",
                 "- In particular, PyBADS does *not* support equality constraints (e.g., of the form $x_1 + x_2 + x_3 = 1$)."
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "83320a21",
-            "metadata": {},
-            "source": [
-                "## Example 2: Full code\n",
-                "\n",
-                "See [here](./scripts/pybads_example_2_nonbox_constraints.py) for a Python file with the code used in this example, with no extra fluff."
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.10.4 ('pybads-dev')",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "5f12204c93c4274de084c6b76e73171147c8e51a8507bf20dfb1db4f14f6829f"
             }
         }
     },
```

### Comparing `PyBADS-0.8.2/examples/pybads_example_3_noisy_objective.ipynb` & `PyBADS-1.0.0/examples/pybads_example_3_noisy_objective.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9845372198497199%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'This notebook is Part 3 of a series of notebooks in "*

 * *            "which we present various example usages for BADS with the PyBADS package.\\n'), (3, "*

 * *            "'The code used in this example is available as a script "*

 * *            "[here](./scripts/pybads_example_3_noisy_objective.py).')], delete: [2]}}, 3: "*

 * *            "{'source': {insert: [(2, 'PyBADS is also able to optimize *noisy* objective "*

 * *            'functions. A noisy (or stochastic) objective func […]*

```diff
@@ -11,15 +11,16 @@
         {
             "cell_type": "markdown",
             "id": "810b5d8b",
             "metadata": {},
             "source": [
                 "In this example, we will show how to run PyBADS on a noisy target.\n",
                 "\n",
-                "This notebook is Part 3 of a series of notebooks in which we present various example usages for BADS with the PyBADS package."
+                "This notebook is Part 3 of a series of notebooks in which we present various example usages for BADS with the PyBADS package.\n",
+                "The code used in this example is available as a script [here](./scripts/pybads_example_3_noisy_objective.py)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "d0c7306b",
             "metadata": {},
@@ -32,17 +33,17 @@
         {
             "cell_type": "markdown",
             "id": "18652cfa",
             "metadata": {},
             "source": [
                 "## 0. Noisy optimization\n",
                 "\n",
-                "PyBADS is able to optimize also *noisy* objective functions. A noisy (or stochastic) objective function is an objective that will return different results if evaluated twice at the same point $\\mathbf{x}$. Conversely, a non-noisy objective function is known as noiseless or deterministic. For example, noisy objectives are common in model fitting when the model is evaluated through simulation (e.g., via sampling aka Monte Carlo methods).\n",
+                "PyBADS is also able to optimize *noisy* objective functions. A noisy (or stochastic) objective function is an objective that will return different results if evaluated twice at the same point $\\mathbf{x}$. Conversely, a non-noisy objective function is known as noiseless or deterministic. For example, noisy objectives are common in model fitting when the model is evaluated through simulation (e.g., via sampling aka Monte Carlo methods).\n",
                 "\n",
-                "For a noisy objective, PyBADS attempts to minimize the *expected value* of $f(\\mathbf{x})$,\n",
+                "For a noisy objective, PyBADS aims to minimize the *expected value* of $f(\\mathbf{x})$:\n",
                 "$$\n",
                 "\\mathbf{x}^\\star = \\arg\\min_{\\mathbf{x} \\in \\mathcal{X} \\subseteq \\mathbb{R}^D} \\mathbb{E}\\left[f(\\mathbf{x})\\right].\n",
                 "$$"
             ]
         },
         {
             "cell_type": "markdown",
@@ -71,18 +72,18 @@
                 "    \"\"\"Simple quadratic function with added noise.\"\"\"\n",
                 "    x_2d = np.atleast_2d(x)\n",
                 "    f = np.sum(x_2d**2, axis=1)\n",
                 "    noise = sigma*np.random.normal(size=x_2d.shape[0])\n",
                 "    return f + noise\n",
                 "\n",
                 "x0 = np.array([-3, -3]);      # Starting point\n",
-                "lb = np.array([-5, -5])       # Lower bounds\n",
-                "ub = np.array([5, 5])         # Upper bounds\n",
-                "plb = np.array([-2, -2])      # Plausible lower bounds\n",
-                "pub = np.array([2, 2])        # Plausible upper bounds\n",
+                "lower_bounds = np.array([-5, -5])\n",
+                "upper_bounds = np.array([5, 5])\n",
+                "plausible_lower_bounds = np.array([-2, -2])\n",
+                "plausible_upper_bounds = np.array([2, 2])\n",
                 "\n",
                 "options = {\n",
                 "    \"uncertainty_handling\": True,\n",
                 "    \"max_fun_evals\": 300,\n",
                 "    \"noise_final_samples\": 100\n",
                 "}"
             ]
@@ -106,48 +107,63 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Beginning optimization of a STOCHASTIC objective function\n",
                         "\n",
                         " Iteration    f-count      E[f(x)]        SD[f(x)]           MeshScale          Method              Actions\n",
-                        "     0           1         20.5617             nan               1                                  \n",
-                        "     0          33        -1.22191             nan               1          Initial mesh            Initial points\n",
-                        "     0          37        -1.22191               1             0.5          Refine grid             Train\n",
-                        "     1          45        -1.22191               1            0.25          Refine grid             Train\n",
-                        "     2          53       -0.435447        0.279863           0.125          Refine grid             Train\n",
-                        "     3          54      -0.0421095        0.212522           0.125      Incremental search (ES-ell)        \n",
-                        "     3          55      -0.0520148        0.205262           0.125      Incremental search (ES-ell)        \n",
-                        "     3          61      -0.0520148        0.205262          0.0625          Refine grid             \n",
-                        "     4          69      -0.0190601        0.172788         0.03125          Refine grid             Train\n",
-                        "     5          70       0.0155653        0.153169         0.03125      Successful search (ES-ell)        \n",
-                        "     5          72     -0.00509212        0.148866         0.03125      Successful search (ES-ell)        \n",
-                        "     5          75     -0.00994359        0.143169         0.03125      Incremental search (ES-ell)        \n",
-                        "     5          81     -0.00994359        0.143169        0.015625          Refine grid             Train\n",
-                        "     6          89       0.0461287        0.133138      0.00390625          Refine grid             Train\n",
-                        "     7          97       0.0685939        0.115893       0.0078125        Successful poll           Train\n",
-                        "     8          98       0.0606537        0.113455       0.0078125      Successful search (ES-wcm)        \n",
-                        "     8         100       0.0543558        0.109812       0.0078125      Successful search (ES-wcm)        \n",
-                        "     8         102       0.0495223        0.108131       0.0078125      Successful search (ES-ell)        \n",
-                        "     8         112       0.0476534        0.105235        0.015625        Successful poll           Train\n",
-                        "     9         113       0.0415597        0.101935        0.015625      Successful search (ES-wcm)        \n",
-                        "     9         115       0.0360151        0.100619        0.015625      Successful search (ES-ell)        \n",
-                        "     9         117       0.0286623       0.0994139        0.015625      Successful search (ES-ell)        \n",
-                        "     9         128       0.0107932       0.0955954         0.03125        Successful poll           \n",
-                        "    10         129       0.0302242        0.100893         0.03125      Successful search (ES-ell)        \n",
-                        "    10         140       0.0241649       0.0943882          0.0625        Successful poll           \n",
-                        "    11         148        0.022237       0.0879658        0.015625          Refine grid             Train\n",
-                        "    12         155       0.0341453       0.0842745         0.03125        Successful poll           Train\n",
-                        "Optimization terminated: change in the function value less than options.TolFun.\n",
-                        "Estimated function value at minimum: 0.13138157013731047 \u00b1 0.10476143847907263 (mean \u00b1 SEM from 100 samples)\n"
+                        "     0           1         17.0467             nan               1                                  \n",
+                        "     0          33       -0.573104             nan               1          Initial mesh            Initial points\n",
+                        "     0          37       -0.573104               1             0.5          Refine grid             Train\n",
+                        "     1          45       -0.573104               1            0.25          Refine grid             Train\n",
+                        "     2          46      -0.0875221        0.236985            0.25      Successful search (ES-wcm)        \n",
+                        "     2          47       -0.133904        0.229856            0.25      Incremental search (ES-wcm)        \n",
+                        "     2          51        -0.14124        0.205711            0.25      Incremental search (ES-ell)        \n",
+                        "     2          53       -0.184658        0.196127            0.25      Incremental search (ES-ell)        \n",
+                        "     2          57       -0.184658        0.196127           0.125          Refine grid             Train\n",
+                        "     3          58       -0.113416        0.181841           0.125      Incremental search (ES-wcm)        \n",
+                        "     3          59       -0.143424         0.17853           0.125      Incremental search (ES-wcm)        \n",
+                        "     3          60       -0.153414        0.175473           0.125      Incremental search (ES-wcm)        \n",
+                        "     3          65       -0.153414        0.175473          0.0625          Refine grid             \n",
+                        "     4          73       -0.202447        0.162169         0.03125          Refine grid             \n",
+                        "     5          77      -0.0930382        0.136617         0.03125      Successful search (ES-ell)        \n",
+                        "     5          78      -0.0993084        0.139908         0.03125      Successful search (ES-ell)        \n",
+                        "     5          79       -0.108523        0.138428         0.03125      Successful search (ES-ell)        \n",
+                        "     5          80       -0.110481        0.137001         0.03125      Incremental search (ES-ell)        \n",
+                        "     5          81       -0.116493        0.135622         0.03125      Successful search (ES-ell)        \n",
+                        "     5          82       -0.119346        0.134247         0.03125      Incremental search (ES-wcm)        \n",
+                        "     5          83       -0.126705        0.132937         0.03125      Successful search (ES-wcm)        \n",
+                        "     5          93       -0.126705        0.132937        0.015625          Refine grid             Train\n",
+                        "     6          94       -0.112421        0.115326        0.015625      Successful search (ES-ell)        \n",
+                        "     6          95       -0.138253        0.114425        0.015625      Successful search (ES-wcm)        \n",
+                        "     6         105       -0.138253        0.114425       0.0078125          Refine grid             \n",
+                        "     7         106       -0.108284        0.103892       0.0078125      Incremental search (ES-wcm)        \n",
+                        "     7         111       -0.110376        0.101127        0.015625        Successful poll           Train\n",
+                        "     8         119      -0.0915521       0.0990537      0.00390625          Refine grid             Train\n",
+                        "     9         127      -0.0813753       0.0944134     0.000976562          Refine grid             Train\n",
+                        "    10         131       -0.037847       0.0890104     0.000976562      Successful search (ES-ell)        \n",
+                        "    10         134      -0.0528433        0.089216     0.000976562      Successful search (ES-ell)        \n",
+                        "    10         135      -0.0639539       0.0887966     0.000976562      Successful search (ES-ell)        \n",
+                        "    10         143      -0.0639539       0.0887966     0.000488281          Refine grid             \n",
+                        "    11         145      -0.0383948        0.084316     0.000488281      Successful search (ES-ell)        \n",
+                        "    11         146      -0.0420733       0.0839543     0.000488281      Successful search (ES-ell)        \n",
+                        "    11         147      -0.0479433       0.0835921     0.000488281      Successful search (ES-ell)        \n",
+                        "    11         150      -0.0501619       0.0825213     0.000488281      Successful search (ES-wcm)        \n",
+                        "    11         152      -0.0640664       0.0818386     0.000488281      Successful search (ES-wcm)        \n",
+                        "    11         153      -0.0722405       0.0815143     0.000488281      Successful search (ES-wcm)        \n",
+                        "    11         163      -0.0722405       0.0815143     0.000244141          Refine grid             \n",
+                        "Optimization terminated: change in the function value less than options['tol_fun'].\n",
+                        "Estimated function value at minimum: -0.04111370566211175 \u00b1 0.09385579705318894 (mean \u00b1 SEM from 100 samples)\n"
                     ]
                 }
             ],
             "source": [
-                "bads = BADS(noisy_sphere, x0, lb, ub, plb, pub, options=options)\n",
+                "bads = BADS(\n",
+                "    noisy_sphere, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds, options=options\n",
+                ")\n",
                 "optimize_result = bads.optimize()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4a7af7d8",
             "metadata": {},
@@ -165,16 +181,16 @@
             "id": "6507b31a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "BADS minimum at: x_min = [-0.03988647  0.17327881], fval (estimated) = 0.1314 +/- 0.1\n",
-                        "total f-count: 256, time: 23.14 s\n",
+                        "BADS minimum at: x_min = [-0.0268445   0.00389814], fval (estimated) = -0.04111 +/- 0.094\n",
+                        "total f-count: 264, time: 5.38 s\n",
                         "final evaluations (shape): (100,)\n"
                     ]
                 }
             ],
             "source": [
                 "x_min = optimize_result['x']\n",
                 "fval = optimize_result['fval']\n",
@@ -199,15 +215,15 @@
             "id": "17089c5d",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "The true, noiseless value of f(x_min) is 0.0316.\n"
+                        "The true, noiseless value of f(x_min) is 0.000736.\n"
                     ]
                 }
             ],
             "source": [
                 "print(f\"The true, noiseless value of f(x_min) is {noisy_sphere(x_min,sigma=0)[0]:.3g}.\")"
             ]
         },
@@ -232,43 +248,33 @@
                 "\n",
                 "- If the noise around the solution is too large, PyBADS will perform poorly. In that case, we recommend to increase the precision of your computation of the objective (e.g., by drawing more Monte Carlo samples) such that $\\sigma \\approx 1$ or even lower, as needed by your problem. Note that the noise farther away from the solution can be larger, and this is usually okay.\n",
                 "\n",
                 "- In this example, we assumed the amount of noise in each target evaluation is unknown. If instead you *can* estimate the magnitude of the noise for each evaluation, see the [next example notebook](./pybads_example_4_user_provided_noise.ipynb).\n",
                 "\n",
                 "- For more information on optimizing noisy objective functions, see the BADS wiki: https://github.com/acerbilab/bads/wiki#noisy-objective-function (this link points to the MATLAB wiki, but many of the questions and answers apply to PyBADS as well).\n"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "83320a21",
-            "metadata": {},
-            "source": [
-                "## Example 3: Full code\n",
-                "\n",
-                "See [here](./scripts/pybads_example_3_noisy_objective.py) for a Python file with the code used in this example, with no extra fluff."
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.10.4 ('pybads-dev')",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "5f12204c93c4274de084c6b76e73171147c8e51a8507bf20dfb1db4f14f6829f"
             }
         }
     },
```

### Comparing `PyBADS-0.8.2/examples/pybads_example_5_extended_usage.ipynb` & `PyBADS-1.0.0/examples/pybads_example_5_extended_usage.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9892355879360636%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'In this example, we will show PyBADS at work on a "*

 * *            'target with multiple local minima (also referred to as "multimodal" in statistics), '*

 * *            "and showcase some additional useful features of the package.\\n'), (2, 'This notebook "*

 * *            'is Part 5 of a series of notebooks in which we present various example usages for '*

 * *            "BADS with the PyBADS package.\\n'), (3, 'The code used in this example is available "*

 * *            "as a scr […]*

```diff
@@ -9,17 +9,18 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "810b5d8b",
             "metadata": {},
             "source": [
-                "In this example, we will show PyBADS at work on a multimodal target and showcase some additional features.\n",
+                "In this example, we will show PyBADS at work on a target with multiple local minima (also referred to as \"multimodal\" in statistics), and showcase some additional useful features of the package.\n",
                 "\n",
-                "This notebook is Part 5 of a series of notebooks in which we present various example usages for BADS with the PyBADS package."
+                "This notebook is Part 5 of a series of notebooks in which we present various example usages for BADS with the PyBADS package.\n",
+                "The code used in this example is available as a script [here](./scripts/pybads_example_5_extended_usage.py)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "d0c7306b",
             "metadata": {},
@@ -34,15 +35,15 @@
             "id": "fccd1931",
             "metadata": {},
             "source": [
                 "## 1. Problem setup\n",
                 "\n",
                 "In this example, we are going to optimize the *six-hump camelback function*, which has six local minima, two of which are global minima.\n",
                 "\n",
-                "Note that, in most realistic scenarios, you would not know whether your problem has only a single local minimum (which is also the global minimum). In practice, many optimization problems exhibit *multiple* local minima."
+                "Note that, in most realistic scenarios, you would not know whether your problem has only a single local minimum (which is also the global minimum). In practice, many optimization problems exhibit *multiple* local minima and you should assume so, in the absence of additional knowledge."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "192fbe30",
             "metadata": {},
@@ -52,99 +53,90 @@
                 "    \"\"\"Six-hump camelback function.\"\"\"\n",
                 "    x_2d = np.atleast_2d(x)\n",
                 "    x1 = x_2d[:,0]\n",
                 "    x2 = x_2d[:,1]\n",
                 "    f = (4 - 2.1*(x1*x1) + (x1*x1*x1*x1)/3.0)*(x1*x1) + x1*x2 + (-4 + 4*(x2*x2))*(x2*x2)\n",
                 "    return f\n",
                 "\n",
-                "lb = np.array([-3, -2])       # Lower bounds\n",
-                "ub = np.array([3, 2])         # Upper bounds\n",
-                "plb = np.array([-2.9, -1.9])  # Plausible lower bounds\n",
-                "pub = np.array([2.9, 1.9])    # Plausible upper bounds\n",
+                "lower_bounds = np.array([-3, -2])\n",
+                "upper_bounds = np.array([3, 2])\n",
+                "plausible_lower_bounds = np.array([-2.9, -1.9])\n",
+                "plausible_upper_bounds = np.array([2.9, 1.9])\n",
                 "\n",
                 "options = {\n",
                 "    \"display\" : 'off',             # We switch off the printing\n",
                 "    \"uncertainty_handling\": False, # Good to specify that this is a deterministic function\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "363e280e",
             "metadata": {},
             "source": [
                 "## 2. Run the optimization\n",
                 "\n",
-                "PyBADS is not a global optimization algorithm in that there is no guarantee that a single run would return the global optimum (in fact, this is true of almost all algorithms). The gold rule of optimization, regardless of optimization algorithm, is to always rerun the optimization multiple times from different starting points (a multi-start strategy), to explore the landscape of the target and gain some confidence about the results.\n",
+                "PyBADS is **not** a global optimization algorithm in that there is no guarantee that a single run would return the global optimum (in practice, this is true of all algorithms, under a finite budget of evaluations). The gold rule of optimization, regardless of optimization algorithm, is to always rerun the optimization multiple times from different starting points (a *multi-start* strategy), to explore the landscape of the target and gain some confidence about the results.\n",
                 "\n",
-                "Below, we rerun PyBADS `num_opts` times from different starting points and store the results of each run, which we will examine later. Note that we switched off PyBADS default printing.\n",
+                "Below, we rerun PyBADS `num_opts` times from different starting points and store the results of each run, which we will examine later. A few observations:\n",
                 "\n",
-                "Also note that each optimization uses a different `BADS` object (the general rule is: one BADS instance per optimization)."
+                "- Each optimization uses a different `BADS` object (the general rule is: one BADS instance per optimization).\n",
+                "- We specified `x0 = None`. This choice will randomly draw a starting point `x0` uniformly inside the provided plausible box, delimited by `plausible_lower_bounds` and `plausible_upper_bounds`.\n",
+                "- For each run, we set a different, predetermined random seed via `options['random_seed']`, which can be helpful for reproducibility of the results.\n",
+                "- We switched off PyBADS default printing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "853bf3c9",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Running optimization 0...\n",
                         "Running optimization 1...\n",
-                        "Running optimization 2...\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/jeet/miniconda3/envs/pybads-dev/lib/python3.10/site-packages/scipy/stats/_morestats.py:1789: RuntimeWarning: invalid value encountered in subtract\n",
-                        "  x = x - np.median(x)\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
+                        "Running optimization 2...\n",
                         "Running optimization 3...\n",
                         "Running optimization 4...\n",
                         "Running optimization 5...\n",
                         "Running optimization 6...\n",
                         "Running optimization 7...\n",
                         "Running optimization 8...\n",
                         "Running optimization 9...\n"
                     ]
                 }
             ],
             "source": [
                 "num_opts = 10\n",
                 "optimize_results = []\n",
-                "x_vec = np.zeros((num_opts,lb.shape[0]))\n",
+                "x_vec = np.zeros((num_opts,lower_bounds.shape[0]))\n",
                 "fval_vec = np.zeros(num_opts)\n",
                 "\n",
                 "for opt_count in range(num_opts):\n",
                 "    print('Running optimization ' + str(opt_count) + '...')\n",
-                "    x0 = np.random.uniform(low=plb, high=pub)\n",
-                "    bads = BADS(camelback6, x0, lb, ub, plb, pub, options=options)\n",
+                "    options['random_seed'] = opt_count\n",
+                "    bads = BADS(\n",
+                "        camelback6, None, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds, options=options\n",
+                "    )\n",
                 "    optimize_results.append(bads.optimize())\n",
                 "    x_vec[opt_count] = optimize_results[opt_count].x\n",
                 "    fval_vec[opt_count] = optimize_results[opt_count].fval"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4a7af7d8",
             "metadata": {},
             "source": [
                 "## 3. Results and conclusions\n",
                 "\n",
-                "First, we inspect the results. In this example, the target function has two equally-good solutions, \n",
+                "First, we inspect the results. In this example, the target function (six-hump camelback function) has two equally-good solutions:\n",
                 "$$\n",
                 "x^\\star = \\left\\{ (0.0898, -0.7126), (-0.0898, 0.7126) \\right\\}, \\qquad f(x^\\star) = -1.0316\n",
                 "$$\n",
                 "which should be represented in the set of results. \n",
                 "\n",
                 "Importantly, we should find below that (almost) all solutions are very close in function value, suggesting that we found the minimizers of the target."
             ]
@@ -156,27 +148,27 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Found solutions:\n",
-                        "[[-0.088363    0.71202897]\n",
-                        " [-0.08937492  0.71252174]\n",
-                        " [ 0.09027936 -0.71363788]\n",
-                        " [ 0.08980637 -0.71252174]\n",
-                        " [-0.0888812   0.71267469]\n",
-                        " [-0.0895537   0.71308493]\n",
-                        " [-0.08965201  0.71412195]\n",
-                        " [-0.08988068  0.71264689]\n",
-                        " [ 0.0897425  -0.71266455]\n",
-                        " [-0.09000549  0.71264496]]\n",
+                        "[[ 0.08939411 -0.712172  ]\n",
+                        " [-0.09008138  0.71347182]\n",
+                        " [ 0.09082897 -0.71192109]\n",
+                        " [-0.09414637  0.71077771]\n",
+                        " [-0.09105368  0.71271563]\n",
+                        " [ 0.08997784 -0.71272106]\n",
+                        " [-0.08990161  0.71246268]\n",
+                        " [ 0.09031594 -0.71231801]\n",
+                        " [ 0.0895162  -0.71246247]\n",
+                        " [-0.09016521  0.71251721]]\n",
                         "Function values at solutions:\n",
-                        "[-1.03161763 -1.03162752 -1.03162024 -1.0316283  -1.03162483 -1.0316265\n",
-                        " -1.03161041 -1.03162845 -1.03162841 -1.03162835]\n"
+                        "[-1.03162597 -1.03162297 -1.03161951 -1.03151937 -1.03162277 -1.03162836\n",
+                        " -1.03162812 -1.03162648 -1.03162779 -1.03162784]\n"
                     ]
                 }
             ],
             "source": [
                 "print('Found solutions:')\n",
                 "print(x_vec)\n",
                 "\n",
@@ -198,16 +190,16 @@
             "id": "6507b31a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "BADS minimum at x_min = [-0.08988068  0.71264689]\n",
-                        "Function value at minimum fval = -1.0316284465531482\n"
+                        "BADS minimum at x_min = [ 0.08997784 -0.71272106]\n",
+                        "Function value at minimum fval = -1.0316283561123913\n"
                     ]
                 }
             ],
             "source": [
                 "idx_best = np.argmin(fval_vec)\n",
                 "result_best = optimize_results[idx_best]\n",
                 "\n",
@@ -237,69 +229,72 @@
                 {
                     "data": {
                         "text/plain": [
                             "{'fun': <function __main__.camelback6(x)>,\n",
                             " 'non_box_cons': None,\n",
                             " 'target_type': 'deterministic',\n",
                             " 'problem_type': 'bound constraints',\n",
-                            " 'iterations': 10,\n",
-                            " 'func_count': 93,\n",
-                            " 'mesh_size': 0.000244140625,\n",
-                            " 'overhead': 1071.5030670489548,\n",
+                            " 'iterations': 8,\n",
+                            " 'func_count': 77,\n",
+                            " 'mesh_size': 0.0009765625,\n",
+                            " 'overhead': 1307.5565116015111,\n",
                             " 'algorithm': 'Bayesian adaptive direct search',\n",
                             " 'yval_vec': None,\n",
                             " 'ysd_vec': None,\n",
-                            " 'x0': array([[2.84035495, 0.37700157]]),\n",
-                            " 'x': array([-0.08988068,  0.71264689]),\n",
-                            " 'fval': -1.0316284465531482,\n",
+                            " 'x0': array([[-1.61243961,  1.40878276]]),\n",
+                            " 'x': array([ 0.08997784, -0.71272106]),\n",
+                            " 'fval': -1.0316283561123913,\n",
                             " 'fsd': 0,\n",
-                            " 'total_time': 4.9732985506521,\n",
+                            " 'total_time': 1.3023214350209962,\n",
+                            " 'random_seed': 5,\n",
+                            " 'version': '0.8.3.dev21+g2aaa7af',\n",
                             " 'success': True,\n",
-                            " 'random_seed': None,\n",
-                            " 'version': '0.0.1',\n",
-                            " 'message': 'Optimization terminated: change in the function value less than options.TolFun.'}"
+                            " 'message': \"Optimization terminated: change in the function value less than options['tol_fun'].\"}"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "result_best"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "83320a21",
+            "id": "772490b5",
             "metadata": {},
             "source": [
-                "## Example 5: Full code\n",
+                "In particular:\n",
                 "\n",
-                "See [here](./scripts/pybads_example_5_extended_usage.py) for a Python file with the code used in this example, with no extra fluff."
+                "- `total_time` is the total runtime (in seconds), including both the time spent evaluating the target and the algorithmic cost of BADS.\n",
+                "- `overhead` represents the *fractional overhead* of BADS compared to the time spent evaluating the target. In this example, `overhead` is astronomical because the target function we are using is analytical and extremely fast, which is not what BADS is designed for. In a realistic scenario, the objective function will be moderately costly (e.g., more than 0.1 s per function evaluation), and the fractional overhead should be less than 1.\n",
+                "- `random_seed` is the random seed used for this run (`None` if not specified).\n",
+                "- `version` is the version of PyBADS used (e.g., `0.8.1`); developer versions have an additional `dev` suffix with more versioning information."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.10.4 ('pybads-dev')",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "5f12204c93c4274de084c6b76e73171147c8e51a8507bf20dfb1db4f14f6829f"
             }
         }
     },
```

### Comparing `PyBADS-0.8.2/examples/scripts/pybads_example_1_basic_usage.py` & `PyBADS-1.0.0/examples/scripts/pybads_example_2_nonbox_constraints.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# PyBADS Example 1: Basic usage
+# PyBADS Example 2: Non-box constraints
 # (code only - see Jupyter notebook for the tutorial)
 
 import numpy as np
 
 from pybads import BADS
 
 
@@ -12,26 +12,32 @@
     return np.sum(
         100 * (x_2d[:, 0:-1] ** 2 - x_2d[:, 1:]) ** 2
         + (x_2d[:, 0:-1] - 1) ** 2,
         axis=1,
     )
 
 
-target = rosenbrocks_fcn
+x0 = np.array([0, 0])  # Starting point
+lower_bounds = np.array([-1, -1])
+upper_bounds = np.array([1, 1])
 
-lb = np.array([-20, -20])  # Lower bounds
-ub = np.array([20, 20])  # Upper bounds
-plb = np.array([-5, -5])  # Plausible lower bounds
-pub = np.array([5, 5])  # Plausible upper bounds
-x0 = np.array([0, 0])
-# Starting point
 
-bads = BADS(target, x0, lb, ub, plb, pub)
+def circle_constr(x):
+    """Return constraints violation outside the unit circle."""
+    x_2d = np.atleast_2d(x)
+    # Note that nonboxcons assumes the function takes a 2D input
+    return np.sum(x_2d**2, axis=1) > 1
+
+
+options = {}
+options["rng_seed"] = 3
+bads = BADS(rosenbrocks_fcn, x0, lower_bounds, upper_bounds, non_box_cons=circle_constr)
 optimize_result = bads.optimize()
 
 x_min = optimize_result["x"]
 fval = optimize_result["fval"]
 
 print(f"BADS minimum at: x_min = {x_min.flatten()}, fval = {fval:.4g}")
 print(
     f"total f-count: {optimize_result['func_count']}, time: {round(optimize_result['total_time'], 2)} s"
 )
+print(f"Problem type: {optimize_result['problem_type']}")
```

### Comparing `PyBADS-0.8.2/examples/scripts/pybads_example_3_noisy_objective.py` & `PyBADS-1.0.0/examples/scripts/pybads_example_4_user_provided_noise.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,55 @@
-# PyBADS Example 3: Noisy objective function
+# PyBADS Example 4: Noisy objective with user-provided noise estimates
 # (code only - see Jupyter notebook for a tutorial)
 
 import numpy as np
 
 from pybads import BADS
 
 
-def noisy_sphere(x, sigma=1.0):
-    """Simple quadratic function with added noise."""
+def noisy_sphere_estimated_noise(x, scale=1.0):
+    """Quadratic function with heteroskedastic noise; also return noise estimate."""
     x_2d = np.atleast_2d(x)
     f = np.sum(x_2d**2, axis=1)
-    noise = sigma * np.random.normal(size=x_2d.shape[0])
-    return f + noise
+    sigma = scale * (1.0 + np.sqrt(f))
+    y = f + sigma * np.random.normal(size=x_2d.shape[0])
+    return y, sigma
 
 
-x0 = np.array([-3, -3])
-# Starting point
-lb = np.array([-5, -5])  # Lower bounds
-ub = np.array([5, 5])  # Upper bounds
-plb = np.array([-2, -2])  # Plausible lower bounds
-pub = np.array([2, 2])  # Plausible upper bounds
+x0 = np.array([-3, -3])  # Starting point
+lower_bounds = np.array([-5, -5])
+upper_bounds = np.array([5, 5])
+plausible_lower_bounds = np.array([-2, -2])
+plausible_upper_bounds = np.array([2, 2])
 
 options = {
     "uncertainty_handling": True,
-    "max_fun_evals": 300,
+    "specify_target_noise": True,
     "noise_final_samples": 100,
 }
 
-bads = BADS(noisy_sphere, x0, lb, ub, plb, pub, options=options)
+bads = BADS(
+    noisy_sphere_estimated_noise, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds, 
+    options=options
+)
 optimize_result = bads.optimize()
 
 x_min = optimize_result["x"]
 fval = optimize_result["fval"]
 fsd = optimize_result["fsd"]
 
+x_min = optimize_result["x"]
+fval = optimize_result["fval"]
+fsd = optimize_result["fsd"]
+
 print(
     f"BADS minimum at: x_min = {x_min.flatten()}, fval (estimated) = {fval:.4g} +/- {fsd:.2g}"
 )
 print(
     f"total f-count: {optimize_result['func_count']}, time: {round(optimize_result['total_time'], 2)} s"
 )
 print(f"final evaluations (shape): {optimize_result['yval_vec'].shape}")
+print(f"final evaluations SD (shape): {optimize_result['ysd_vec'].shape}")
 
 print(
-    f"The true, noiseless value of f(x_min) is {noisy_sphere(x_min,sigma=0)[0]:.3g}."
+    f"The true, noiseless value of f(x_min) is {noisy_sphere_estimated_noise(x_min,scale=0)[0][0]:.3g}."
 )
```

### Comparing `PyBADS-0.8.2/examples/scripts/pybads_example_4_user_provided_noise.py` & `PyBADS-1.0.0/examples/scripts/pybads_example_3_noisy_objective.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,46 @@
-# PyBADS Example 4: Noisy objective with user-provided noise estimates
+# PyBADS Example 3: Noisy objective function
 # (code only - see Jupyter notebook for a tutorial)
 
 import numpy as np
 
 from pybads import BADS
 
 
-def noisy_sphere_estimated_noise(x, scale=1.0):
-    """Quadratic function with heteroskedastic noise; also return noise estimate."""
+def noisy_sphere(x, sigma=1.0):
+    """Simple quadratic function with added noise."""
     x_2d = np.atleast_2d(x)
     f = np.sum(x_2d**2, axis=1)
-    sigma = scale * (1.0 + np.sqrt(f))
-    y = f + sigma * np.random.normal(size=x_2d.shape[0])
-    return y, sigma
+    noise = sigma * np.random.normal(size=x_2d.shape[0])
+    return f + noise
 
 
-x0 = np.array([-3, -3])
-# Starting point
-lb = np.array([-5, -5])  # Lower bounds
-ub = np.array([5, 5])  # Upper bounds
-plb = np.array([-2, -2])  # Plausible lower bounds
-pub = np.array([2, 2])  # Plausible upper bounds
+x0 = np.array([-3, -3])  # Starting point
+lower_bounds = np.array([-5, -5])
+upper_bounds = np.array([5, 5])
+plausible_lower_bounds = np.array([-2, -2])
+plausible_upper_bounds = np.array([2, 2])
 
 options = {
     "uncertainty_handling": True,
-    "specify_target_noise": True,
+    "max_fun_evals": 300,
     "noise_final_samples": 100,
 }
 
-bads = BADS(
-    noisy_sphere_estimated_noise, x0, lb, ub, plb, pub, options=options
-)
+bads = BADS(noisy_sphere, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds, options=options)
 optimize_result = bads.optimize()
 
 x_min = optimize_result["x"]
 fval = optimize_result["fval"]
 fsd = optimize_result["fsd"]
 
-x_min = optimize_result["x"]
-fval = optimize_result["fval"]
-fsd = optimize_result["fsd"]
-
 print(
     f"BADS minimum at: x_min = {x_min.flatten()}, fval (estimated) = {fval:.4g} +/- {fsd:.2g}"
 )
 print(
     f"total f-count: {optimize_result['func_count']}, time: {round(optimize_result['total_time'], 2)} s"
 )
 print(f"final evaluations (shape): {optimize_result['yval_vec'].shape}")
-print(f"final evaluations SD (shape): {optimize_result['ysd_vec'].shape}")
 
 print(
-    f"The true, noiseless value of f(x_min) is {noisy_sphere_estimated_noise(x_min,scale=0)[0][0]:.3g}."
+    f"The true, noiseless value of f(x_min) is {noisy_sphere(x_min,sigma=0)[0]:.3g}."
 )
```

### Comparing `PyBADS-0.8.2/examples/scripts/pybads_example_5_extended_usage.py` & `PyBADS-1.0.0/examples/scripts/pybads_example_5_extended_usage.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,35 @@
         (4 - 2.1 * (x1 * x1) + (x1 * x1 * x1 * x1) / 3.0) * (x1 * x1)
         + x1 * x2
         + (-4 + 4 * (x2 * x2)) * (x2 * x2)
     )
     return f
 
 
-lb = np.array([-3, -2])  # Lower bounds
-ub = np.array([3, 2])  # Upper bounds
-plb = np.array([-2.9, -1.9])  # Plausible lower bounds
-pub = np.array([2.9, 1.9])  # Plausible upper bounds
+lower_bounds = np.array([-3, -2])
+upper_bounds = np.array([3, 2])
+plausible_lower_bounds = np.array([-2.9, -1.9])
+plausible_upper_bounds = np.array([2.9, 1.9])
 
 options = {
     "display": "off",  # We switch off the printing
     "uncertainty_handling": False,  # Good to specify that this is a deterministic function
 }
 
 num_opts = 10
 optimize_results = []
-x_vec = np.zeros((num_opts, lb.shape[0]))
+x_vec = np.zeros((num_opts,lower_bounds.shape[0]))
 fval_vec = np.zeros(num_opts)
 
 for opt_count in range(num_opts):
-    print("Running optimization " + str(opt_count) + "...")
-    x0 = np.random.uniform(low=plb, high=pub)
-    bads = BADS(camelback6, x0, lb, ub, plb, pub, options=options)
+    print('Running optimization ' + str(opt_count) + '...')
+    options['random_seed'] = opt_count
+    bads = BADS(
+        camelback6, None, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds, options=options
+    )
     optimize_results.append(bads.optimize())
     x_vec[opt_count] = optimize_results[opt_count].x
     fval_vec[opt_count] = optimize_results[opt_count].fval
 
 print("Found solutions:")
 print(x_vec)
```

### Comparing `PyBADS-0.8.2/pybads/__init__.py` & `PyBADS-1.0.0/pybads/__init__.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/__main__.py` & `PyBADS-1.0.0/pybads/__main__.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/acquisition_functions/acq_fcn_lcb.py` & `PyBADS-1.0.0/pybads/acquisition_functions/acq_fcn_lcb.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/bads/bads.py` & `PyBADS-1.0.0/pybads/bads/bads.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,87 +28,103 @@
 )
 from .optimize_result import OptimizeResult
 from .options import Options
 
 
 class BADS:
     """
-    BADS Constrained optimization using Bayesian Adaptive Direct Search (v0.0.1).
+    BADS Constrained optimization using Bayesian Adaptive Direct Search.
     
     BADS attempts to solve problems of the form:
-       :math:`\mathtt{argmin}_X  f(X)`  subject to:  lb :math:`<= X <=` ub, and optionally :math:`C(X) <= 0`
+       :math:`\mathtt{argmin}_x  f(x)`  subject to:  lower_bounds :math:`<= x <=` upper_bounds, and optionally :math:`C(x) <= 0`
                                
 
     Initialize a ``PyBADS`` object to set up the optimization problem, then run
     ``optimize()``. See the examples for more details under the `examples` directory.
 
     Parameters
     ----------
     fun : callable
-        A given target `fun`. `fun` accepts input `x` and returns a scalar function
-        value of the target evaluated at 'x' and the noise if provided.
+        A given target ``fun``. ``fun`` accepts input ``x`` and returns a scalar 
+        function value of the target evaluated at ``x`` and the noise if provided.
+        In case the target function ``fun`` requires additional data/parameters, 
+        they can be handled using an anonymous function.
+        For example: ``fun_for_pybads = lambda x: fun(x, data, extra_params)``, 
+        where ``fun`` is the function to optimize, and ``data`` and ``extra_params`` 
+        are given in the outer scope.
     x0 : np.ndarray, optional
-        Starting point.
+        Starting point for the optimization. If not specified or ``None``, the 
+        starting point ``x0`` is uniformly randomly drawn inside the plausible 
+        box between ``plausible_lower_bounds`` and ``plausible_upper_bounds`` (see 
+        below).
     lower_bounds, upper_bounds : np.ndarray, optional
-        `lower_bounds` (`lb`) and `upper_bounds` (`ub`) define a set
-        of strict lower and upper bounds for the coordinate vector, `x`, so
-        that the unknown function has support on `lb` < `x` < `ub`.
+        ``lower_bounds`` (``lb``) and ``upper_bounds`` (``ub``) define a set
+        of strict lower and upper bounds for the coordinate vector, ``x``, so
+        that the unknown function has support on ``lb`` <= ``x`` <= ``ub``.
         If scalars, the bound is replicated in each dimension. Use
-        ``None`` for `lb` and `ub` if no bounds exist. Set `lb` [`i`] = -``inf``
-        and `ub` [`i`] = ``inf`` if the `i`-th coordinate is unbounded (while
-        other coordinates may be bounded). Note that if `lb` and `ub` contain
-        unbounded variables, the respective values of `plb` and `pub` need to
-        be specified (see below), by default ``None``.
+        ``None`` for ``lb`` and ``ub`` if no bounds exist. Set ``lb[i] = -inf``
+        and ``ub [i] = inf`` if the `i`-th coordinate is unbounded (while
+        other coordinates may be bounded). Note that if ``lb`` and ``ub`` contain
+        unbounded variables, the respective values of ``plb`` and ``pub`` need to
+        be specified (see below). By default ``None``.
     plausible_lower_bounds, plausible_upper_bounds : np.ndarray, optional
-        Specifies a set of `plausible_lower_bounds` (`plb`) and
-        `plausible_upper_bounds` (`pub`) such that `lb` < `plb` < `pub` < `ub`.
-        Both `plb` and `pub` need to be finite. `plb` and `pub` represent a
-        "plausible" range, which should denote a region of the global minimum.
-        As a rule of thumb, set plausible_lower_bounds and plausible_upper_bounds such that
-        there is > 90% probability that the minimum is found within the box
-        (where in doubt, just set `plb`=`lb` and `pub`=`ub`).
+        Specifies a set of ``plausible_lower_bounds`` (``plb``) and
+        ``plausible_upper_bounds`` (``pub``) such that ``lb`` <= ``plb`` < ``pub`` <= ``ub``.
+        Both ``plb`` and ``pub`` need to be finite. ``plb`` and ``pub`` represent a
+        `plausible` range, which should denote a region where the global minimum
+        is expected to be found. As a rule of thumb, set ``plausible_lower_bounds`` 
+        and ``plausible_upper_bounds`` such that there is > 90% probability that 
+        the minimum is found within the box (where in doubt, just set 
+        ``plb = lb`` and ``pub = ub``).
 
     non_box_cons: callable, optional
-        A given non-bound constraints function. e.g : ``lambda x: np.sum(x.^2,1)>1``
+        A given non-box constraints function that specifies constraint 
+        `violations`, e.g : ``lambda x: np.sum(x.^2,1)>1``
 
     options : dict, optional
         Additional options can be passed as a dict. Please refer to the
         BADS options page for the default options. If no `options` are
         passed, the default options are used.
-        To run BADS on a noisy (stochastic) objective function, set:
-            * ``options.uncertainty_handling`` = ``True``
-            * ``options.noise_size`` = SIGMA
-                *  SIGMA is an estimate of the SD of the noise in your problem in
-                    a good region of the parameter space. (If not specified, default
-                    SIGMA = 1). To help BADS work better, it is recommended that you
-                    provide to BADS an estimate of the noise at each location.
-        If ``options.uncertainty_handling`` is not specified, BADS will determine at
-        runtime if the objective function is noisy.
+        To run BADS on a noisy (stochastic) objective function, set 
+        ``options['uncertainty_handling']`` = ``True``. You can help BADS by 
+        providing an estimate of the noise. ``options['noise_size'] = sigma`` provides a global estimate of the 
+        SD of the noise in your problem in a good region of the parameter 
+        space. (If not specified, default ``sigma = 1.0``). 
+        Alternatively, you can specify the target noise `at each location` 
+        with ``options['specify_target_noise']`` = ``True``. In this case, 
+        ``fun`` is expected to return `two` values, the estimate of the
+        target at ``x`` and an estimate of the SD of the noise at ``x`` 
+        (see the examples). 
+        If ``options['uncertainty_handling']`` is not specified, BADS will 
+        determine at runtime if the objective function is noisy.
+        To obtain reproducible results of the optimization, set ``options['random_seed']`` 
+        to a fixed integer value.
 
     Raises
     ------
     ValueError
         When neither ``x0`` or (``plausible_lower_bounds`` and
         ``plausible_upper_bounds``) are specified.
     ValueError
-        When various checks for the bounds (lb, ub, plb, pub) of BADS fail.
+        When various checks for the bounds (``lower_bounds``, ``upper_bounds``, 
+        ``plausible_lower_bounds``, ``plausible_upper_bounds``) of BADS fail.
 
 
     References
     ----------
     .. [1]  Acerbi, L. & Ma, W. J. (2017). "Practical Bayesian
             Optimization for Model Fitting with Bayesian Adaptive Direct Search".
-            In Advances in Neural Information Processing Systems 30, pages 1834-1844.
+            In `Advances in Neural Information Processing Systems` 30, pages 1834-1844.
             (arXiv preprint: https://arxiv.org/abs/1705.04405).
             
     Examples
     --------
     For `BADS` usage examples, please look up the Jupyter notebook tutorials
     in the PyBADS documentation:
-    https://acerbilab.github.io/pybads/_examples/pybads_example_1.html
+    https://acerbilab.github.io/pybads/examples.html
     """
 
     def __init__(
         self,
         fun: callable,
         x0: np.ndarray = None,
         lower_bounds: np.ndarray = None,
@@ -136,15 +152,15 @@
         if x0 is None:
             if (
                 plausible_lower_bounds is None
                 or plausible_upper_bounds is None
             ):
                 raise ValueError(
                     """bads:UnknownDims If no starting point is
-                 provided, plb and pub need to be specified."""
+                 provided, plausible_lower_bounds and plausible_upper_bounds need to be specified."""
                 )
             else:
                 x0 = np.full((plausible_lower_bounds.shape), np.NaN)
 
         x0 = np.atleast_2d(x0)
         self.D = x0.shape[1]
 
@@ -164,14 +180,17 @@
             evaluation_parameters={"D": self.D},
         )
         self.options.validate_option_names([basic_path, advanced_path])
 
         if self.options["stobads"] is None or self.options["stobads"] == False:
             self.options["stobads"] = False
 
+        # set up random seed
+        self._init_random_seed_()
+
         # set up BADS logger
         self.logger = logging.getLogger("BADS")
         self.logger.setLevel(logging.INFO)
         if self.options.get("display") == "off":
             self.logger.setLevel(logging.WARN)
         elif self.options.get("display") == "iter":
             self.logger.setLevel(logging.INFO)
@@ -229,15 +248,15 @@
         self.function_logger = FunctionLogger(
             fun=fun,
             D=self.D,
             noise_flag=self.optim_state.get("uncertainty_handling_level") > 0,
             uncertainty_handling_level=self.optim_state.get(
                 "uncertainty_handling_level"
             ),
-            cache_size=self.options.get("cachesize"),
+            cache_size=self.options.get("cache_size"),
             variable_transformer=self.var_transf,
         )
 
         self.iteration_history = IterationHistory(
             [
                 "iter",
                 "func_count",
@@ -277,15 +296,15 @@
 
         N0, D = x0.shape
 
         # Estimation of the plb and pub if any of them is not specified
         if plausible_lower_bounds is None or plausible_upper_bounds is None:
             if N0 > 1:
                 self.logger.warning(
-                    "plb and/or pub not specified. Estimating"
+                    "plausible_lower_bounds and/or plausible_upper_bounds not specified. Estimating"
                     + "plausible bounds from starting set X0..."
                 )
                 width = x0.max(0) - x0.min(0)
                 if plausible_lower_bounds is None:
                     plausible_lower_bounds = x0.min(0) - width / N0
                     plausible_lower_bounds = np.maximum(
                         plausible_lower_bounds, lower_bounds
@@ -303,16 +322,16 @@
                     self.logger.warning(
                         "bads:pbInitFailed: Some plausible bounds could not be "
                         + "determined from starting set. Using hard upper/lower"
                         + " bounds for those instead."
                     )
             else:
                 self.logger.warning(
-                    "bads:pbUnspecified: Plausible lower/upper bounds plb and"
-                    "/or pub not specified and X0 is not a valid starting set. "
+                    "bads:pbUnspecified: Plausible lower/upper bounds"
+                    " not specified and X0 is not a valid starting set. "
                     + "Using hard upper/lower bounds instead."
                 )
                 if plausible_lower_bounds is None:
                     plausible_lower_bounds = np.copy(lower_bounds)
                 if plausible_upper_bounds is None:
                     plausible_upper_bounds = np.copy(upper_bounds)
 
@@ -339,15 +358,15 @@
             )
 
         # check that plausible bounds are finite
         if np.any(np.invert(np.isfinite(plausible_lower_bounds))) or np.any(
             np.invert(np.isfinite(plausible_upper_bounds))
         ):
             raise ValueError(
-                "Plausible interval bounds plb and pub need to be finite."
+                "Plausible interval bounds plausible_lower_bounds and plausible_upper_bounds need to be finite."
             )
 
         # Test that all vectors are real-valued
         if (
             np.any(np.invert(np.isreal(x0)))
             or np.any(np.invert(np.isreal(lower_bounds)))
             or np.any(np.invert(np.isreal(upper_bounds)))
@@ -379,15 +398,15 @@
             plausible lower and upper bounds need to be distinct."""
             )
 
         # Check that all X0 are inside the bounds
         if np.any(x0 < lower_bounds) or np.any(x0 > upper_bounds):
             raise ValueError(
                 """bads:InitialPointsNotInsideBounds: The starting
-                points X0 are not inside the provided hard bounds lb and ub."""
+                points X0 are not inside the provided hard bounds lower_bounds and upper_bounds."""
             )
 
         # # Compute "effective" bounds (slightly inside provided hard bounds)
         bounds_range = upper_bounds - lower_bounds
         bounds_range[np.isinf(bounds_range)] = 1e3
         scale_factor = 1e-3
         realmin = sys.float_info.min
@@ -401,37 +420,37 @@
         )
         # Infinities stay the same
         LB_eff[np.isinf(lower_bounds)] = lower_bounds[np.isinf(lower_bounds)]
         UB_eff[np.isinf(upper_bounds)] = upper_bounds[np.isinf(upper_bounds)]
 
         if np.any(LB_eff >= UB_eff):
             raise ValueError(
-                """bads:StrictBoundsTooClose: Hard bounds lb and ub
+                """bads:StrictBoundsTooClose: Hard bounds lower_bounds and upper_bounds
                 are numerically too close. Make them more separate."""
             )
 
         # Fix when provided X0 are almost on the bounds -- move them inside
         if np.any(x0 < LB_eff) or np.any(x0 > UB_eff):
             self.logger.warning(
                 "bads:InitialPointsTooClosePB: The starting points X0 are on "
-                + "or numerically too close to the hard bounds lb and ub. "
+                + "or numerically too close to the hard bounds lower_bounds and upper_bounds. "
                 + "Moving the initial points more inside..."
             )
             x0 = np.maximum((np.minimum(x0, UB_eff)), LB_eff)
 
         # Test order of bounds (permissive)
         ordidx = (
             (lower_bounds <= plausible_lower_bounds)
             & (plausible_lower_bounds < plausible_upper_bounds)
             & (plausible_upper_bounds <= upper_bounds)
         )
         if np.any(np.invert(ordidx)):
             raise ValueError(
                 """bads:StrictBounds: For each variable, hard and
-            plausible bounds should respect the ordering lb < plb < pub < ub."""
+            plausible bounds should respect the ordering lower_bounds < plausible_lower_bounds < plausible_upper_bounds < upper_bounds."""
             )
 
         # Test that plausible bounds are reasonably separated from hard bounds
         if np.any(LB_eff > plausible_lower_bounds) or np.any(
             plausible_upper_bounds > UB_eff
         ):
             self.logger.warning(
@@ -443,16 +462,16 @@
             plausible_upper_bounds = np.minimum(plausible_upper_bounds, UB_eff)
 
         # Check that all X0 are inside the plausible bounds,
         # move bounds otherwise
         if np.any(x0 <= LB_eff) or np.any(x0 >= UB_eff):
             self.logger.warning(
                 "bads:InitialPointsOutsidePB. The starting points X0"
-                + " are not inside the provided plausible bounds plb and "
-                + "pub. Expanding the plausible bounds..."
+                + " are not inside the provided plausible bounds (plausible_lower_bounds and plausible_upper_bounds)."
+                + " Expanding the plausible bounds..."
             )
             plausible_lower_bounds = np.minimum(
                 plausible_lower_bounds, x0.min(0)
             )
             plausible_upper_bounds = np.maximum(
                 plausible_upper_bounds, x0.max(0)
             )
@@ -462,15 +481,15 @@
             (lower_bounds <= plausible_lower_bounds)
             & (plausible_lower_bounds < plausible_upper_bounds)
             & (plausible_upper_bounds <= upper_bounds)
         )
         if np.any(np.invert(ordidx)):
             raise ValueError(
                 """bads:StrictBounds: For each variable, hard and
-            plausible bounds should respect the ordering lb <= plb < pub <= ub."""
+            plausible bounds should respect the ordering lower_bounds <= plausible_lower_bounds < plausible_upper_bounds <= upper_bounds."""
             )
 
         # Check that variables are either bounded or unbounded
         # (not half-bounded)
         if (
             np.any(np.isfinite(lower_bounds))
             and np.any(np.invert(np.isfinite(upper_bounds)))
@@ -513,28 +532,29 @@
         )
 
     def _init_optim_state_(self):
         """
         A private function to initialize the optim_state dict that contains information about BADS variables.
         """
         # Record starting points (original coordinates)
-        if self.options["fvals"] is not None:
-            y_orig = np.array(self.options.get("fvals")).flatten()
+        if self.options["f_vals"] is not None:
+            y_orig = np.array(self.options.get("f_vals")).flatten()
             if len(y_orig) == 0:
                 y_orig = np.full([self.x0.shape[0]], np.nan)
             if len(self.x0) != len(y_orig):
                 raise ValueError(
                     """bads:MismatchedStartingInputs The number of
                 points in X0 and of their function values as specified in
-                self.options.fvals are not the same."""
+                self.options.['f_vals'] are not the same."""
                 )
         else:
             y_orig = np.full([self.x0.shape[0]], np.nan)
 
         optim_state = dict()
+        optim_state["random_seed"] = self._random_seed
         optim_state["cache"] = dict()
         optim_state["cache"]["x_orig"] = self.x0
         optim_state["cache"]["y_orig"] = y_orig
         optim_state["last_re_eval"] = -np.inf
 
         # Does the starting cache contain function values?
         optim_state["cache_active"] = np.any(
@@ -543,24 +563,24 @@
 
         # Grid parameters
         self.mesh_size_integer = self.options[
             "init_mesh_size_integer"
         ]  # Mesh size in log base units
         optim_state["search_size_integer"] = np.minimum(
             0,
-            self.mesh_size_integer * self.options.get("searchgridmultiplier")
-            - self.options.get("searchgridnumber"),
+            self.mesh_size_integer * self.options.get("search_grid_multiplier")
+            - self.options.get("search_grid_number"),
         )
         optim_state["mesh_size"] = (
-            float(self.options.get("pollmeshmultiplier"))
+            float(self.options.get("poll_mesh_multiplier"))
             ** self.mesh_size_integer
         )
         self.mesh_size = optim_state["mesh_size"]
         optim_state["search_mesh_size"] = (
-            float(self.options.get("pollmeshmultiplier"))
+            float(self.options.get("poll_mesh_multiplier"))
             ** optim_state["search_size_integer"]
         )
         self.search_mesh_size = optim_state["search_mesh_size"]
         optim_state["scale"] = 1.0
 
         # Check if periodic_vars is not None and raise error, since it is not yet supported
         if self.options["periodic_vars"] is not None:
@@ -637,32 +657,32 @@
         )
         optim_state["u"] = u0
         self.u = u0.flatten().copy()
 
         # Test starting point u0 is within bounds
         if np.any(u0 > self.upper_bounds) or np.any(u0 < self.lower_bounds):
             self.logger.error(
-                "Initial starting point u0 is not within the hard bounds lb and ub"
+                "Initial starting point u0 is not within the hard bounds lower_bounds and upper_bounds"
             )
             raise ValueError(
-                """bads:Initpoint: Initial starting point u0 is not within the hard bounds lb and ub"""
+                """bads:Initpoint: Initial starting point u0 is not within the hard bounds lower_bounds and upper_bounds"""
             )
 
         # Report variable transformation
         if np.any(self.var_transf.apply_log_t):
             self.logger.info(
                 f"Variables (index) internally transformed to log coordinates: {np.argwhere(self.var_transf.apply_log_t)}"
             )
 
-        # Put TOLMESH on space
+        # Put tol_mesh on space
         optim_state["tol_mesh"] = self.options[
-            "pollmeshmultiplier"
+            "poll_mesh_multiplier"
         ] ** np.ceil(
-            np.log(self.options["tolmesh"])
-            / np.log(self.options["pollmeshmultiplier"])
+            np.log(self.options["tol_mesh"])
+            / np.log(self.options["poll_mesh_multiplier"])
         )
 
         # Periodic variables
         idx_periodic_vars = self.options["periodic_vars"]
         periodic_vars = np.zeros((1, self.D)).astype(bool)
         if idx_periodic_vars is not None:
             periodic_vars[:, idx_periodic_vars] = True
@@ -677,27 +697,27 @@
                 f"Variables (index) defined with periodic boundaries: {idx_periodic_vars}"
             )
         optim_state["periodic_vars"] = periodic_vars
 
         # Setup covariance information (unused)
 
         # Import prior function evaluations
-        fun_values = self.options["funvalues"]
+        fun_values = self.options["fun_values"]
         if fun_values is not None and len(fun_values) != 0:
             if "X" not in fun_values or "Y" not in fun_values:
                 raise ValueError(
-                    """bads:funvalues: The 'FunValue' field in OPTIONS need to have X and Y fields (respectively, inputs and their function values)"""
+                    """bads:fun_values: The 'fun_values' field in options need to have X and Y fields (respectively, inputs and their function values)"""
                 )
 
             X = fun_values["X"]
             Y = fun_values["Y"]
 
             if len(X) != len(Y):
                 raise ValueError(
-                    "X and Y arrays in the OPTIONS.FunValues need to have the same number of rows (each row is a tested point)."
+                    "X and Y arrays in the options['fun_values'] need to have the same number of rows (each row is a tested point)."
                 )
             if (
                 (not np.all(np.isfinite(X)))
                 or (not np.all(np.isfinite(Y)))
                 or (not np.isreal(X))
                 or (not np.isreal(Y))
             ):
@@ -715,15 +735,15 @@
                 )
 
             S = None
             if "S" in fun_values:
                 S = fun_values["S"]
                 if len(S) != len(Y):
                     raise ValueError(
-                        "X, Y, and S arrays in the OPTIONS.FunValues need to have the same number of rows (each row is a tested point)."
+                        "X, Y, and S arrays in the options['fun_values'] need to have the same number of rows (each row is a tested point)."
                     )
                 S = np.atleast_2d(S).T
                 if len(S) != 0 and S.shape[1] != 1:
                     raise ValueError(
                         "S should be a vertical nd-array (, 1) of estimated function SD values (one SD per row)."
                     )
 
@@ -731,17 +751,17 @@
                 if S is None:
                     self.function_logger.add(X[i], Y[i])
                 else:
                     self.function_logger.add(X[i], Y[i], S[i])
 
         # Other variables initializations
         optim_state["search_factor"] = 1
-        optim_state["sd_level"] = self.options["incumbentsigmamultiplier"]
+        optim_state["sd_level"] = self.options["incumbent_sigma_multiplier"]
         optim_state["search_count"] = self.options[
-            "searchntry"
+            "search_n_try"
         ]  # Skip search at first iteration
         optim_state["lastreeval"] = -np.inf
         # Last time function values were re-evaluated
         optim_state["lastfitgp"] = -np.inf
         # Last fcn evaluation for which the gp was trained
         self.mesh_overflows = 0
         # Number of attempted mesh expansions when already at maximum size
@@ -778,25 +798,25 @@
 
         if (
             self.options["specify_target_noise"]
             and self.options["uncertainty_handling"] is not None
             and self.options["uncertainty_handling"] == False
         ):
             raise ValueError(
-                "If options.specify_target_noise is ON, options.uncertainty_handling should be ON as well. \
-                                Leave options.uncertainty_handling empty or set it to ON to avoid this error."
+                "If options['specify_target_noise'] is True, options['uncertainty_handling'] should be True as well. \
+                                Leave options['uncertainty_handling'] empty or set it to True to avoid this error."
             )
         if (
             self.options["specify_target_noise"]
             and self.options["noise_size"] is not None
             and np.array(self.options["noise_size"] > 0)[0]
         ):
             self.logger.warn(
-                "If options.specify_target_noise is ON, options.noise_size is ignored. \
-                Leave options.noise_size empty or set it to 0 to silence this warning."
+                "If options['specify_target_noise'] is True, options['noise_size'] is ignored. \
+                Leave options['noise_size'] empty or set it to 0 to silence this warning."
             )
 
         # Set uncertainty handling level
         # (0: none; 1: unknown noise level; 2: user-provided noise)
         if self.options.get("specify_target_noise"):
             optim_state["uncertainty_handling_level"] = 2
         elif (
@@ -804,70 +824,82 @@
             and self.options["uncertainty_handling"]
         ):
             optim_state["uncertainty_handling_level"] = 1
         else:
             optim_state["uncertainty_handling_level"] = 0
 
         # Empty hedge struct for acquisition functions
-        if self.options.get("acqhedge"):
+        if self.options.get("acq_hedge"):
             optim_state["acq_hedge"] = dict()
 
         # List of points at the end of each iteration
         optim_state["iterlist"] = dict()
         optim_state["iterlist"]["u"] = []
         optim_state["iterlist"]["fval"] = []
         optim_state["iterlist"]["fsd"] = []
         optim_state["iterlist"]["fhyp"] = []
 
         # Initialize Gaussian process settings
         # Squared exponential kernel with separate length scales
-        optim_state["gp_covfun"] = 1
+        optim_state["gp_cov_fun"] = 1
 
         if optim_state.get("uncertainty_handling_level") == 0:
             # Observation noise for stability
             optim_state["gp_noisefun"] = [1, 0, 0]
         elif optim_state.get("uncertainty_handling_level") == 1:
             # Infer noise
             optim_state["gp_noisefun"] = [1, 2, 0]
         elif optim_state.get("uncertainty_handling_level") == 2:
             # Provided heteroskedastic noise
             optim_state["gp_noisefun"] = [1, 1, 0]
 
         if (
-            self.options.get("noiseshaping")
+            self.options.get("noise_shaping")
             and optim_state["gp_noisefun"][1] == 0
         ):
             optim_state["gp_noisefun"][1] = 1
 
-        optim_state["gp_meanfun"] = self.options.get("gp_meanfun")
-        valid_gp_meanfuns = [
+        optim_state["gp_mean_fun"] = self.options.get("gp_mean_fun")
+        valid_gp_mean_funs = [
             "zero",
             "const",
             "negquad",
             "se",
             "negquadse",
             "negquadfixiso",
             "negquadfix",
             "negquadsefix",
             "negquadonly",
             "negquadfixonly",
             "negquadlinonly",
             "negquadmix",
         ]
 
-        if not optim_state["gp_meanfun"] in valid_gp_meanfuns:
+        if not optim_state["gp_mean_fun"] in valid_gp_mean_funs:
             raise ValueError(
                 """bads:UnknownGPmean:Unknown/unsupported GP mean
             function. Supported mean functions are zero, const,
             egquad, and se"""
             )
         optim_state["int_meanfun"] = self.options.get("gpintmeanfun")
 
         return optim_state
 
+    def _init_random_seed_(self):
+        # set random seed if provided
+        if "random_seed" in self.options and \
+            self.options["random_seed"] is not None:
+            # set random seed to numpy and consequently to scipy (scipy uses the same number generator)
+            random_seed = int(self.options["random_seed"])
+            np.random.seed(random_seed)
+        else:
+            random_seed = None
+        self._random_seed = random_seed
+        return random_seed
+
     def _init_mesh_(self):
         """
         A private function to initialize the mesh frame and the optimization problem.
         It evaluates the initial points, which includes the starting point and the generated point retrieved from a sobol sequence generating method.
         The init_mesh also assess if the target function is stochastic and set the parameter of BADS for handling stochastic targets.
         """
         # Evaluate starting point and initial mesh, determine if function is noisy
@@ -888,15 +920,15 @@
 
         if self.optim_state["uncertainty_handling_level"] < 1:
             # test if the function is noisy
             self.logging_action.append("Uncertainty test")
             yval_bis, _, _ = self.function_logger(
                 self.u, record_duplicate_data=False
             )
-            if np.abs(self.yval - yval_bis) > self.options["tolnoise"]:
+            if np.abs(self.yval - yval_bis) > self.options["tol_noise"]:
                 self.optim_state["uncertainty_handling_level"] = 1
                 self.logging_action.append("Uncertainty test")
         else:
             self.logging_action.append("")
 
         if self.optim_state["uncertainty_handling_level"] > 0:
             if self.options["specify_target_noise"]:
@@ -926,20 +958,20 @@
 
         # set up strings for logging of the iteration
         self.display_format = self._setup_logging_display_format()
         self._log_column_headers()
         self._display_function_log_(0, "")
 
         if self.options["fun_eval_start"] > 0:
-            # Evaluate initial points but not more than options.max_fun_evals
+            # Evaluate initial points but not more than options['max_fun_evals']
             fun_eval_start = np.minimum(
                 self.options["fun_eval_start"],
                 self.options["max_fun_evals"] - 1,
             )
-            if self.options["initfcn"] == "init_sobol":
+            if self.options["init_fun"] == "init_sobol":
 
                 u1, _ = init_sobol(
                     self.u,
                     self.lower_bounds,
                     self.upper_bounds,
                     self.plausible_lower_bounds,
                     self.plausible_upper_bounds,
@@ -976,15 +1008,15 @@
                 self.u = self.function_logger.X[idx_yval].copy()
                 self.yval = self.function_logger.Y[idx_yval].item()
                 self.fval = self.yval
                 self.logging_action.append("Initial points")
                 self._display_function_log_(0, "Initial mesh")
             else:
                 raise ValueError(
-                    "bads:initfcn:Initialization function not implemented yet"
+                    "bads:init_fun:Initialization function not implemented yet"
                 )
 
         if not np.isfinite(self.yval):
             raise ValueError("init mesh: Cannot find valid starting point.")
 
         self.optim_state["fval"] = self.fval
         self.optim_state["yval"] = self.yval
@@ -999,28 +1031,30 @@
         """
         A private function initialize the optimization problem.
         It calls the init_mesh, sets the option configurations required by BADS, and initializes the Guassian Process (GP)
         """
         gp = None
         self.reset_gp = False
         hyp_dict = {}
-
+        # set random seed if provided
+        self.optim_state["random_seed"] = self._init_random_seed_()
+        
         # Evaluate starting point and initial mesh,
         self._init_mesh_()
 
         # Change options for uncertainty handling
         if self.optim_state["uncertainty_handling_level"] > 0:
-            self.options["tolstalliters"] = 2 * self.options["tolstalliters"]
-            self.options["ntrain_max"] = max(200, self.options["ntrain_max"])
-            self.options["ntrain_min"] = 2 * self.options["ntrain_min"]
-            self.options["meshoverflowswarning"] = (
-                2 * self.options["meshoverflowswarning"]
+            self.options["tol_stall_iters"] = 2 * self.options["tol_stall_iters"]
+            self.options["n_train_max"] = max(200, self.options["n_train_max"])
+            self.options["n_train_min"] = 2 * self.options["n_train_min"]
+            self.options["mesh_overflow_warning"] = (
+                2 * self.options["mesh_overflow_warning"]
             )
-            self.options["minfailedpollsteps"] = np.inf
-            self.options["meshnoisemultiplier"] = 0
+            self.options["min_failed_poll_steps"] = np.inf
+            self.options["mesh_noise_multiplier"] = 0
             if self.options["noise_size"] is None:
                 self.options["noise_size"] = 1.0
             if isinstance(
                 self.options["noise_size"], np.ndarray
             ):  # ensure the noise_size is a scalar
                 self.options["noise_size"] = self.options["noise_size"].item()
 
@@ -1044,15 +1078,15 @@
                 self.fsd = self.function_logger.S[idx_min_y]
                 self.fsd = self.fsd.item()
             else:
                 self.fsd = self.options["noise_size"]
 
         else:
             if self.options["noise_size"] is None:
-                self.options["noise_size"] = np.sqrt(self.options["tolfun"])
+                self.options["noise_size"] = np.sqrt(self.options["tol_fun"])
             self.fsd = 0.0
             # Since the function is fully-deterministic no need of stobads
             if self.options["stobads"]:
                 self.options["stobads"] = False
 
         self.optim_state["fsd"] = self.fsd
         self.u_best = self.u.copy()
@@ -1120,18 +1154,19 @@
         self.last_skipped = -1
         # Last skipped iteration
         self.search_spree = 0
         self.restarts = self.options["restarts"]
 
         # Initialize gp
         gp, Ns_gp, sn2hpd, hyp_dict = self._init_optimization_()
+        
         self.search_es_hedge = None  # init search hedge to None
 
-        if self.options["outputfcn"] is not None:
-            output_fcn = self.options["outputfcn"]
+        if self.options["output_fcn"] is not None:
+            output_fcn = self.options["output_fcn"]
             is_finished = output_fcn(
                 self.var_transf.inverse_transf(self.u), "init"
             )
 
         poll_iteration += 1
         loop_iter = 0
         while not is_finished:
@@ -1139,54 +1174,54 @@
             self.gp_refitted_flag = False
             self.gp_exit_flag = np.inf
             action_txt = (
                 ""  # Action performed this iteration (for printing purposes)
             )
 
             # Compute mesh size and search mesh size
-            self.mesh_size = self.options["pollmeshmultiplier"] ** (
+            self.mesh_size = self.options["poll_mesh_multiplier"] ** (
                 self.mesh_size_integer
             )
             self.optim_state["mesh_size"] = self.mesh_size
 
-            if self.options["searchsizelocked"]:
+            if self.options["search_size_locked"]:
                 self.optim_state["search_size_integer"] = np.minimum(
                     0,
                     self.mesh_size_integer
-                    * self.options["searchgridmultiplier"]
-                    - self.options["searchgridnumber"],
+                    * self.options["search_grid_multiplier"]
+                    - self.options["search_grid_number"],
                 )
 
             self.optim_state["search_mesh_size"] = (
-                self.options["pollmeshmultiplier"]
+                self.options["poll_mesh_multiplier"]
                 ** self.optim_state["search_size_integer"]
             )
             self.search_mesh_size = self.optim_state["search_mesh_size"]
 
             # Update bounds to grid search mesh
             (
                 self.optim_state["lb_search"],
                 self.optim_state["ub_search"],
             ) = self._update_search_bounds_()
 
             # Minimum improvement for a poll/search to be considered successful
-            self.sufficient_improvement = self.options["tolimprovement"] * (
-                self.mesh_size ** (self.options["forcingexponent"])
+            self.sufficient_improvement = self.options["tol_improvement"] * (
+                self.mesh_size ** (self.options["forcing_exponent"])
             )
-            if self.options["sloppyimprovement"]:
+            if self.options["sloppy_improvement"]:
                 self.sufficient_improvement = np.maximum(
-                    self.sufficient_improvement, self.options["tolfun"]
+                    self.sufficient_improvement, self.options["tol_fun"]
                 )
 
             self.optim_state[
                 "search_sufficient_improvement"
             ] = self.sufficient_improvement.copy()
 
             do_search_step_flag = (
-                self.optim_state["search_count"] < self.options["searchntry"]
+                self.optim_state["search_count"] < self.options["search_n_try"]
                 and len(self.function_logger.Y[self.function_logger.X_flag])
                 > self.D
             )
 
             if do_search_step_flag:
                 # Search stage
                 (
@@ -1198,39 +1233,39 @@
                 ) = self._search_step_(gp)
             # End Search step
 
             # Check whether to perform the poll stage, it can be run consecutively after the search.
             if (
                 self.optim_state["search_count"] == 0
                 or self.optim_state["search_count"]
-                == self.options["searchntry"]
+                == self.options["search_n_try"]
             ):
 
                 self.optim_state["search_count"] = 0
                 if (
                     self.search_success > 0
-                    and self.options["skippollaftersearch"]
+                    and self.options["skip_poll_after_search"]
                 ):
                     do_poll_step = False
                     self.search_spree += 1
                     if (
-                        self.options["searchmeshexpand"] > 0
+                        self.options["search_mesh_expand"] > 0
                         and np.mod(
-                            self.search_spree, self.options["searchmeshexpand"]
+                            self.search_spree, self.options["search_mesh_expand"]
                         )
                         == 0
-                        and self.options["searchmeshincrement"] > 0
+                        and self.options["search_mesh_increment"] > 0
                     ):
                         # Check if mesh size is already maximal
                         self._check_mesh_overflow_()
 
                         self.mesh_size_integer = np.minimum(
                             self.mesh_size_integer
-                            + self.options["searchmeshincrement"],
-                            self.options["maxpollgridnumber"],
+                            + self.options["search_mesh_increment"],
+                            self.options["max_poll_grid_number"],
                         )
                 else:
                     do_poll_step = True
                     self.search_spree = 0
 
                 self.search_success = 0
             else:  # In-between searches, no poll
@@ -1255,43 +1290,43 @@
             # Check termination conditions
             if (
                 self.function_logger.func_count
                 >= self.options["max_fun_evals"]
             ):
                 is_finished = True
                 # exit_flag = 0
-                msg = "Optimization terminated: reached maximum number of function evaluations options.max_fun_evals."
+                msg = "Optimization terminated: reached maximum number of function evaluations options['max_fun_evals']."
 
             if poll_iteration >= self.options["max_iter"] - 1:
                 is_finished = True
                 # exit_flag = 0
-                msg = "Optimization terminated: reached maximum number of iterations options.max_iter."
+                msg = "Optimization terminated: reached maximum number of iterations options['max_iter']."
 
             if self.optim_state["mesh_size"] < self.optim_state["tol_mesh"]:
                 is_finished = True
                 # exit_flag = 1
-                msg = "Optimization terminated: mesh size less than options.tolmesh."
+                msg = "Optimization terminated: change in the function value less than options['tol_mesh']"
 
             # Historic improvement
-            if poll_iteration > self.options["tolstalliters"] - 1:
-                idx = poll_iteration - self.options["tolstalliters"]
+            if poll_iteration > self.options["tol_stall_iters"] - 1:
+                idx = poll_iteration - self.options["tol_stall_iters"]
                 f_base = self.iteration_history.get("fval")[idx]
                 f_sd_base = self.iteration_history.get("fsd")[idx]
                 self.f_q_historic_improvement = self._eval_improvement_(
                     f_base,
                     self.fval,
                     f_sd_base,
                     self.fsd,
-                    self.options["improvementquantile"],
+                    self.options["improvement_quantile"],
                 )
 
-                if self.f_q_historic_improvement < self.options["tolfun"]:
+                if self.f_q_historic_improvement < self.options["tol_fun"]:
                     is_finished = True
                     exit_flag = 2
-                    msg = "Optimization terminated: change in the function value less than options.TolFun."
+                    msg = "Optimization terminated: change in the function value less than options['tol_fun']."
 
             self.optim_state["termination_msg"] = msg
 
             # Store best points at the end of each iteration, or upon termination
             if do_poll_step or is_finished:
                 self.iteration_history.record(
                     "u", self.u.flatten(), poll_iteration
@@ -1340,23 +1375,23 @@
                 gp = self.iteration_history.get("gp")[poll_iteration]
 
                 f_q_re_impr = self._eval_improvement_(
                     self.fval,
                     self.iteration_history.get("fval").astype("float"),
                     self.fsd,
                     self.iteration_history.get("fsd").astype("float"),
-                    self.options["improvementquantile"],
+                    self.options["improvement_quantile"],
                 )
                 f_q_re_impr = f_q_re_impr[1:]  # Skip the first iteration
                 idx_impr = np.argmax(f_q_re_impr)
                 improvement = f_q_re_impr[idx_impr]
                 idx_impr = idx_impr + 1  # offset original index without skip
 
                 # Check if any point got better
-                if improvement > self.options["tolfun"]:
+                if improvement > self.options["tol_fun"]:
                     self.yval = self.iteration_history.get("yval")[idx_impr]
                     self.fval = self.iteration_history.get("fval")[idx_impr]
                     self.fsd = self.iteration_history.get("fsd")[idx_impr]
                     self.u = self.iteration_history.get("u")[idx_impr]
                     self.best_u = self.u.copy()
                     self.best_gp_hyp = self.iteration_history.get(
                         "gp_hyp_full"
@@ -1387,15 +1422,15 @@
             and poll_iteration > 0
         ):
             self._re_evaluate_history_(gp)
 
             # Order by lowest probabilistic upper bound and choose
             # the point with the lowest quantile values of the history of the optimization run: inf{x: F(x)>p}.
             sigma_multiplier = np.sqrt(2) * erfcinv(
-                2 * self.options["finalquantile"]
+                2 * self.options["final_quantile"]
             )  # Using inverted convention
             q_beta = self.iteration_history.get(
                 "fval"
             ) + sigma_multiplier * self.iteration_history.get("fsd")
             min_q_beta_idx = np.argmin(q_beta[1:])  # Skip first iteration
             min_q_beta_idx += 1  # offset original index with no skip
             self.yval = self.iteration_history.get("yval")[min_q_beta_idx]
@@ -1497,15 +1532,15 @@
             Estimated mean function at the candidate search point.
         f_sd_search : float
             Estimated noise at the candidate search point.
         gp : gpyreg.gaussian_process.GP
         """
         # Check whether it is time to refit the GP
         refit_flag, do_gp_calibration = self._is_gp_refit_time_(
-            self.options["normalphalevel"]
+            self.options["normalpha_level"]
         )
 
         if (
             refit_flag
             or self.optim_state["search_count"] == 0
             or self.reset_gp
         ):
@@ -1536,15 +1571,15 @@
         self.optim_state["f_target"] = f_target.item()
 
         # Generate search set (normalized coordinate)
         self.optim_state["search_count"] += 1
 
         if self.search_es_hedge is None:
             self.search_es_hedge = ESSearchHedge(
-                self.options["searchmethod"], self.options, self.non_box_cons
+                self.options["search_method"], self.options, self.non_box_cons
             )
         u_search_set, z = self.search_es_hedge(
             self.u,
             self.lower_bounds,
             self.upper_bounds,
             self.function_logger,
             gp,
@@ -1594,28 +1629,28 @@
                 self.logger.warn("bads:optimize: Acquisition function failed")
                 index_acq = np.random.randint(0, len(u_search_set) + 1)
 
             # u_search at the candidate acquisition point
             u_search = u_search_set[index_acq]
 
             # TODO: Local optimization of the acquisition function (generally it does not improve results)
-            if self.options["searchoptimize"]:
+            if self.options["search_optimize"]:
                 pass
 
             y_search, f_sd_search, idx = self.function_logger(u_search)
 
             if z.size > 0:
                 # Save statistics of gp prediction,
                 self._save_gp_stats_(y_search, f_mu[index_acq], fs[index_acq])
 
             # Add search point to training setMeshSize
             if (
                 u_search.size
                 > 0 & self.search_es_hedge.count
-                < self.options["searchntry"]
+                < self.options["search_n_try"]
             ):
                 # TODO: Handle fitness_shaping and rotate gp axes (latter one is unsupported)
                 gp = add_and_update_gp(
                     self.function_logger,
                     gp,
                     u_search,
                     y_search,
@@ -1666,39 +1701,39 @@
             y_search = self.yval
             f_mu_search = self.fval
             f_sd_search = 0
             search_dist = 0
 
         # TODO: CMA-ES like estimation of local covariance structure (unused)
         if (
-            self.options["hessianupdate"]
-            and self.options["hessianmethod"] == "cmaes"
+            self.options["hessian_update"]
+            and self.options["hessian_method"] == "cmaes"
         ):
             pass
 
         fval_old = self.fval
 
         # Evaluate search
         if not self.options["stobads"]:
             search_improvement = self._eval_improvement_(
                 self.fval,
                 f_mu_search,
                 self.fsd,
                 f_sd_search,
-                self.options["improvementquantile"],
+                self.options["improvement_quantile"],
             )
 
             # Declare if search was success or not
             is_search_success = (
                 search_improvement
                 > self.optim_state["search_sufficient_improvement"]
             )
             is_search_improved = (
                 search_improvement > 0
-                and self.options["sloppyimprovement"]
+                and self.options["sloppy_improvement"]
                 or is_search_success
             )
 
         else:
             # For StoBads an improvement corresponds to a success
             sto_success = self._sto_success_improvement_(
                 self.fval,
@@ -1713,15 +1748,15 @@
                 is_search_success = sto_success == 1
             else:
                 is_search_improved = sto_success == 1
                 is_search_success = is_search_improved
 
         # A search improvement implies an update of the incumbent
         if is_search_improved:
-            if self.options["acqhedge"]:
+            if self.options["acq_hedge"]:
                 # Acquisition hedge (acquisition portfolio) not supported yet
                 pass
             else:
                 method = self.search_es_hedge.chosen_search_fun[0]
 
             # StoBads or sufficient improvement
             if is_search_success:
@@ -1901,15 +1936,15 @@
                 period_check(
                     u_poll_new,
                     self.lower_bounds,
                     self.upper_bounds,
                     self.optim_state["periodic_vars"],
                 )
 
-                if self.options["forcepollmesh"]:
+                if self.options["force_poll_mesh"]:
                     u_poll_new = force_to_grid(
                         u_poll_new, self.optim_state["search_mesh_size"]
                     )
 
                 u_poll_new = contraints_check(
                     u_poll_new,
                     self.lower_bounds,
@@ -1933,19 +1968,19 @@
 
             # Cannot refill poll vector set, stop polling
             if u_poll is None or u_poll.size == 0:
                 break
 
             # Check whether it is time to refit the GP
             refit_flag, do_gp_calibration = self._is_gp_refit_time_(
-                self.options["normalphalevel"]
+                self.options["normalpha_level"]
             )
 
             if (
-                not self.options["polltraining"]
+                not self.options["poll_training"]
                 and self.optim_state["iter"] > 0
             ):
                 refit_flag = False
 
             # Local GP approximation around polled points
             if refit_flag or poll_count == 0 or self.reset_gp:
                 gp, gp_exit_flag = local_gp_fitting(
@@ -2007,27 +2042,27 @@
 
             # Consider whether to stop polling
             if not self.options["complete_poll"]:
                 # Stop polling if last poll was good
                 if certain_good_poll:
                     if do_gp_calibration:
                         break  # GP is unreliable, just stop polling
-                    elif p_less > 1 - self.options["tolpoi"]:
+                    elif p_less > 1 - self.options["tol_poi"]:
                         break  # Use GP prediction whether to stop polling
                 else:
                     # No good polling so far -- if GP is reliable, stop polling
                     # If probability of improvement at any location is to low
                     if (
                         not do_gp_calibration
                         and (
-                            self.options["consecutiveskipping"]
+                            self.options["consecutive_skipping"]
                             or self.last_skipped < self.optim_state["iter"] - 1
                         )
-                        and poll_count >= self.options["minfailedpollsteps"]
-                        and p_less > (1 - self.options["tolpoi"])
+                        and poll_count >= self.options["min_failed_poll_steps"]
+                        and p_less > (1 - self.options["tol_poi"])
                     ):
 
                         self.last_skipped = self.optim_state["iter"]
                         break
 
             # Evaluate function and store the value
             u_new = u_poll[index_acq]
@@ -2057,15 +2092,15 @@
                 f_sd_poll = 0
 
             poll_improvement = self._eval_improvement_(
                 self.fval,
                 f_poll,
                 self.fsd,
                 f_sd_poll,
-                self.options["improvementquantile"],
+                self.options["improvement_quantile"],
             )
 
             # Check if current point improves over best polled point so far
             if poll_improvement > poll_best_improvement:
                 u_poll_best = u_new.copy()
                 y_poll_best = y_poll
                 f_poll_best = f_poll
@@ -2093,15 +2128,15 @@
             # Increase poll counter
             poll_count += 1
         # End poll loop
 
         # Evaluate poll
         if not self.options["stobads"]:
             if (
-                poll_best_improvement > 0 and self.options["sloppyimprovement"]
+                poll_best_improvement > 0 and self.options["sloppy_improvement"]
             ) or poll_best_improvement > self.sufficient_improvement:
 
                 # Update incumbent point (self.yval, self.fval, self.fsd) and optim_state
                 self._update_incumbent_(
                     u_poll_best, y_poll_best, f_poll_best, f_sd_poll_best
                 )
                 is_poll_moved = True
@@ -2126,15 +2161,15 @@
         if certain_good_poll:
             is_sucess_poll_flag = True
 
             # Check if mesh size is already maximal
             self._check_mesh_overflow_()
             # Successful poll, increase mesh size
             self.mesh_size_integer = np.minimum(
-                self.mesh_size_integer + 1, self.options["maxpollgridnumber"]
+                self.mesh_size_integer + 1, self.options["max_poll_grid_number"]
             )
 
             self.optim_state["u_success"].append(self.u_best.copy)
             self.optim_state["y_success"].append(self.yval)
             self.optim_state["f_success"].append(self.fval)
         else:
             is_sucess_poll_flag = False
@@ -2162,38 +2197,38 @@
                     iter - self.options["accelerate_mesh_steps"]
                 ]
                 self.f_q_historic_improvement = self._eval_improvement_(
                     f_base,
                     self.fval,
                     f_sd_base,
                     self.fsd,
-                    self.options["improvementquantile"],
+                    self.options["improvement_quantile"],
                 )
                 if (
-                    self.f_q_historic_improvement < self.options["tolfun"]
+                    self.f_q_historic_improvement < self.options["tol_fun"]
                 ):  # or np.all(u_base.flatten() == self.u.flatten()):
 
                     self.mesh_size_integer -= 1
                     logger.debug(
                         "bads: The optimization is stalling, further decrease of the mesh size"
                     )
 
             self.optim_state["search_size_integer"] = np.minimum(
                 self.optim_state["search_size_integer"],
-                self.mesh_size_integer * self.options["searchgridmultiplier"]
-                - self.options["searchgridnumber"],
+                self.mesh_size_integer * self.options["search_grid_multiplier"]
+                - self.options["search_grid_number"],
             )
 
             # TODO: Profile plot iteration
 
         # End POLL evaluation
 
         # Update mesh size
         self.mesh_size = (
-            self.options["pollmeshmultiplier"] ** self.mesh_size_integer
+            self.options["poll_mesh_multiplier"] ** self.mesh_size_integer
         )
         self.optim_state["mesh_size"] = self.mesh_size
 
         # Print iteration
         if is_sucess_poll_flag:
             poll_string = "Successful poll"
         else:
@@ -2254,30 +2289,34 @@
         else:
             gp_iter_idx = gp_iter_idx[
                 -1
             ]  # retrieve last recorded gp stat iteration
 
         # if stats data is available check z_score
         if not do_gp_calibration:
-            fvals = (
+            f_vals = (
                 self.gp_stats.get("fval")[: gp_iter_idx + 1]
                 .flatten()
                 .astype("float")
             )
             yvals = (
                 self.gp_stats.get("ymu")[: gp_iter_idx + 1]
                 .flatten()
                 .astype("float")
             )
-            zscore = fvals - yvals
+            zscore = f_vals - yvals
             gp_ys = (
                 self.gp_stats.get("ys")[: gp_iter_idx + 1]
                 .flatten()
                 .astype("float")
             )
+            # Avoid division by zero, sometimes the GP variance is zero (e.g at end of the optimization of a deterministic)
+            idx_zero_gp_ys = np.where(np.isclose(0., gp_ys))[0]
+            gp_ys[idx_zero_gp_ys] = 1e-6
+            
             zscore = zscore / gp_ys
 
             if np.any(np.isnan(zscore)):
                 do_gp_calibration = True
             else:
                 n = np.size(zscore)
                 if n < 3:
@@ -2298,15 +2337,15 @@
                     shapiro_test = shapiro(zscore)
                     do_gp_calibration = shapiro_test.pvalue < alpha
 
         func_count = self.function_logger.func_count
 
         refit_flag = (
             self.optim_state["lastfitgp"]
-            < (func_count - self.options["minrefittime"])
+            < (func_count - self.options["min_refit_time"])
             and (gp_iter_idx >= refit_period or do_gp_calibration)
             and func_count > self.D
         )
 
         if refit_flag:
 
             self.optim_state["lastfitgp"] = self.function_logger.func_count
@@ -2344,15 +2383,15 @@
                 GP variance/noise at point u.
             f_target : optimization target, it is slighly below the GP prediction when the target function is stochastic.
 
         """
         # Corresponds to Matlab: updateTarget
         if (
             self.optim_state["uncertainty_handling_level"] > 0
-            or self.options["uncertainincumbent"]
+            or self.options["uncertain_incumbent"]
         ):
             tmp_gp = copy.deepcopy(gp)
             tmp_gp.set_hyperparameters(hyp_best)
             f_target_mu, fs2 = tmp_gp.predict(np.atleast_2d(u))
 
             f_target_s = np.sqrt(np.max(fs2, axis=0))
             if (
@@ -2360,27 +2399,27 @@
                 | ~np.isreal(f_target_s)
                 | ~np.isfinite(f_target_s)
             ):
                 f_target_mu = self.optim_state["fval"]
                 f_target_s = self.optim_state["fsd"]
 
             # f_target: Set optimization target slightly below the current incumbent
-            if self.options["alternativeincumbent"]:
+            if self.options["alternative_incumbent"]:
                 f_target = (
                     f_target_mu
                     - np.sqrt(self.D)
                     / np.sqrt(self.function_logger.func_count)
                     * f_target_s
                 )
             else:
                 f_target = f_target_mu - self.optim_state[
                     "sd_level"
-                ] * np.sqrt(fs2 + self.options["tolfun"] ** 2)
+                ] * np.sqrt(fs2 + self.options["tol_fun"] ** 2)
         else:
-            f_target = self.optim_state["fval"] - self.options["tolfun"]
+            f_target = self.optim_state["fval"] - self.options["tol_fun"]
             f_target_mu = self.optim_state["fval"]
             f_target_s = 0
 
         return f_target_mu, f_target_s, f_target
 
     def _update_search_bounds_(self):
         lb = self.optim_state["lb"]
@@ -2430,44 +2469,44 @@
         )
         search_stats["udist"].append(search_dist)
 
         if search_status == "success":
             search_stats["success"].append(1.0)
             self.optim_state["search_factor"] = (
                 self.optim_state["search_factor"]
-                * self.options["searchscalesuccess"]
+                * self.options["search_scale_success"]
             )
-            if self.options["adaptiveincumbentshift"]:
+            if self.options["adaptive_incumbent_shift"]:
                 self.optim_state["sd_level"] = self.optim_state["sd_level"] * 2
 
         elif search_status == "incremental":
             search_stats["success"].append(0.5)
             self.optim_state["search_factor"] = (
                 self.optim_state["search_factor"]
-                * self.options["searchscaleincremental"]
+                * self.options["search_scale_incremental"]
             )
-            if self.options["adaptiveincumbentshift"]:
+            if self.options["adaptive_incumbent_shift"]:
                 self.optim_state["sd_level"] = (
                     self.optim_state["sd_level"] * 2**2
                 )
 
         elif search_status == "failure":
             search_stats["success"].append(0.0)
             self.optim_state["search_factor"] = (
                 self.optim_state["search_factor"]
-                * self.options["searchscalefailure"]
+                * self.options["search_scale_failure"]
             )
-            if self.options["adaptiveincumbentshift"]:
+            if self.options["adaptive_incumbent_shift"]:
                 self.optim_state["sd_level"] = np.maximum(
-                    self.options["incumbentsigmamultiplier"],
+                    self.options["incumbent_sigma_multiplier"],
                     self.optim_state["sd_level"] / 2,
                 )
 
         # Reset search factor at the end of each search
-        if self.optim_state["search_count"] == self.options["searchntry"]:
+        if self.optim_state["search_count"] == self.options["search_n_try"]:
             self.optim_state["search_factor"] = 1
 
         return search_stats
 
     def _re_evaluate_history_(self, gp: GP):
         """A private method used in the case of a stochastic target function.
         It updates the predicted values and the variance for each stored GP at each iteration, by computing the posterior on the current training set without refitting the parameters.
@@ -2494,21 +2533,21 @@
 
                 self.iteration_history.record("fval", fval, i)
                 self.iteration_history.record("fsd", fsd, i)
 
             self.optim_state["last_re_eval"] = self.function_logger.func_count
 
     def _check_mesh_overflow_(self):
-        if self.mesh_size_integer == self.options["maxpollgridnumber"]:
+        if self.mesh_size_integer == self.options["max_poll_grid_number"]:
             self.mesh_overflows += 1
             if self.mesh_overflows == np.ceil(
-                self.options["meshoverflowswarning"]
+                self.options["mesh_overflow_warning"]
             ):
                 self.logger.warn(
-                    "bads:meshOverflow \t The mesh attempted to expand above maximum size too many times. Try widening plb and pub."
+                    "bads:meshOverflow \t The mesh attempted to expand above maximum size too many times. Try widening plausible_lower_bounds and plausible_upper_bounds."
                 )
 
     def _log_column_headers(self):
         """
         Private method to log the column headers for the iteration log.
         """
         if self.optim_state["cache_active"]:
```

### Comparing `PyBADS-0.8.2/pybads/bads/bads_dump.py` & `PyBADS-1.0.0/pybads/bads/bads_dump.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/bads/gaussian_process_train.py` & `PyBADS-1.0.0/pybads/bads/gaussian_process_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,19 +74,19 @@
         hyp_dict["run_cov"] = None
 
     # Get training dataset.
     x_train, y_train, s2_train, t_train = _get_fevals_data(function_logger)
     D = x_train.shape[1]
 
     # Pick the mean function
-    mean_f = _meanfun_name_to_mean_function(optim_state["gp_meanfun"])
+    mean_f = _meanfun_name_to_mean_function(optim_state["gp_mean_fun"])
 
     # Pick the covariance function.
     covariance_f = _cov_identifier_to_covariance_function(
-        optim_state["gp_covfun"]
+        optim_state["gp_cov_fun"]
     )
 
     # Pick the noise function.
     const_add = optim_state["gp_noisefun"][0] == 1
     user_add = optim_state["gp_noisefun"][1] == 1
     user_scale = optim_state["gp_noisefun"][1] == 2
     rlod_add = optim_state["gp_noisefun"][2] == 1
@@ -186,18 +186,18 @@
                 f"bads:gp: Cholesky decomposition has failed. The initial fit on the GP has failed due to the hyp. init."
             )
     # end gp hyp. init
 
     # Update running average of GP hyperparameter covariance (coarse)
     if hyp_dict["full"] is not None and hyp_dict["full"].shape[1] > 1:
         hyp_cov = np.cov(hyp_dict["full"].T)
-        if hyp_dict["run_cov"] is None or options["hyprunweight"] == 0:
+        if hyp_dict["run_cov"] is None or options["hyp_run_weight"] == 0:
             hyp_dict["run_cov"] = hyp_cov
         else:
-            w = options["hyprunweight"] ** options["fun_evals_per_iter"]
+            w = options["hyp_run_weight"] ** options["fun_evals_per_iter"]
             hyp_dict["run_cov"] = (1 - w) * hyp_cov + w * hyp_dict["run_cov"]
     else:
         hyp_dict["run_cov"] = None
 
     # Missing port: sample for GP for debug (not used)
 
     # Estimate of GP noise around the top high posterior density region
@@ -244,24 +244,24 @@
 
     # TODO: Rotate dataset (unsupported)
 
     # Update GP
 
     ## Update priors hyperparameters using empirical Bayes method.
     if options.get("specify_target_noise"):
-        noise_size = options["tolfun"]  # Additional jitter to specified noise
+        noise_size = options["tol_fun"]  # Additional jitter to specified noise
     else:
         noise_size = options["noise_size"]
 
     # Update GP Noise
     old_priors = gp.get_priors()
     gp_priors = gp.get_priors()
     prior_noise = gp_priors["noise_log_scale"]
     mu_noise_prior = np.log(noise_size) + options[
-        "meshnoisemultiplier"
+        "mesh_noise_multiplier"
     ] * np.log(optim_state["mesh_size"])
     prior_noise = (prior_noise[0], (mu_noise_prior, prior_noise[1][1]))
 
     # TODO: warped likelihood (unsupported)
 
     # Update GP Mean
     y_mean = np.percentile(gp.y, options["gp_mean_percentile"])
@@ -275,15 +275,15 @@
     if prior_mean is not None and ~options["gp_fixed_mean"]:
         prior_mean = (prior_mean[0], (prior_mean[1][0], y_range ** (1 / 4)))
     elif options["gp_fixed_mean"]:
         # TODO: update hyp mean by assigning ymean
         pass
 
     # Update GP Covariance length scale
-    if options["gpcovprior"] == "iso":
+    if options["gp_cov_prior"] == "iso":
         dist = udist(
             gp.X,
             gp.X,
             1,
             optim_state["lb"],
             optim_state["ub"],
             optim_state["scale"],
@@ -302,15 +302,15 @@
                 "gaussian",
                 (cov_mu, cov_sigma),
             )
 
     # TODO Adjust prior length scales for periodic variables (mapped to unit circle)
 
     # Empirical prior on covariance signal variance ((output scale)
-    if options["warpfunc"] == 0:
+    if options["warp_func"] == 0:
         sd_y = np.log(np.std(gp.y))
     else:
         # TODO warp function (Matlab  gpdefbads line-code 302)
         pass
 
     # Re-fit gaussian Process (optimize or sample -- only optimization supported)
     gp_priors["covariance_log_outputscale"] = ("gaussian", (sd_y, 2.0))
@@ -346,15 +346,15 @@
             )
 
         is_low_mean = False  # Check for mean stuck below minimum
         if isinstance(gp.mean, gpr.mean_functions.ConstantMean):
             is_low_mean = last_dic_hyp_gp["mean_const"] < np.min(gp.y)
 
         # Conditions for performing a second fit
-        second_fit = options["doublerefit"] | is_high_noise | is_low_mean
+        second_fit = options["double_refit"] | is_high_noise | is_low_mean
         optim_state["second_fit"] = second_fit
         dic_hyp_gp[-1] = last_dic_hyp_gp
 
         if second_fit:
             # Sample the hyper-params from priors
             prev_hyp_gp = gp.get_hyperparameters(as_array=True)
             if options["use_slice_sampler"]:
@@ -417,15 +417,15 @@
         else:
             gp.temporary_data["len_scale"] = 1.0
 
         # GP-based geometric length scale
         ll = np.zeros((hyp_n_samples, D))
         for i in range(hyp_n_samples):
             ll[i, :] = (
-                options["gprescalepoll"]
+                options["gp_rescale_poll"]
                 * dic_hyp_gp[i]["covariance_log_lengthscale"]
             )
         # ll = exp(sum(bsxfun(@times, gpstruct.hypweight, ll - mean(ll(:))),2))';
         ll = ll - np.mean(ll)
         ll = np.exp(np.sum(ll, axis=0))
 
         # Take bounded limits
@@ -658,15 +658,15 @@
     return gp.hyperparameters_from_dict(hyp)
 
 
 def _get_samples_from_slice_sampler_(gp: gpr.GP, hyp_gp, optim_state, options):
     """
     A private method that retrieves a new set of parameters using the slice sampler method.
     """
-    hyp_sampler_name = options.get("gphypsampler", "slicesample")
+    hyp_sampler_name = options.get("gp_hyp_sampler", "slicesample")
     if hyp_sampler_name != "slicesample":
         raise ValueError("Wrong sampler")
 
     sample_f = lambda hyp_: gp._GP__gp_obj_fun(hyp_, False, True)
     width = gp.upper_bounds - gp.lower_bounds
 
     # If there are multiple parameter samples
@@ -800,56 +800,56 @@
         cov_x0[-1] = 0.0  # shape hyp.
 
     mean_x0 = mean_bounds_info["x0"]
 
     noise_x0 = noise_bounds_info["x0"]
 
     # Hyperparams over observation noise
-    if options["fitlik"]:
+    if options["fit_lik"]:
         # Unknown noise level (even for deterministic function, it helps for regularization)
         if options.get("specify_target_noise"):
             noise_size = options[
-                "tolfun"
+                "tol_fun"
             ]  # Additional jitter to specified noise
         else:
             noise_size = options["noise_size"]
 
         if np.isscalar(noise_size) or np.size(noise_size) == 1:
             noise_std = 1
             noise_mu = np.log(noise_size)
         else:
             noise_mu = np.log(noise_size[0])
             noise_std = noise_size[1]
 
     else:
-        noise_size = options["tolfun"]
+        noise_size = options["tol_fun"]
         noise_mu = np.log(noise_size)
 
     noise_x0[0] = noise_mu
     hyp0 = np.concatenate([cov_x0, noise_x0, mean_x0])
 
     # Missing port: output warping hyperparameters not implemented
 
     ## Change default bounds and set priors over hyperparameters.
 
     bounds = gp.get_bounds()
-    if options["uppergplengthfactor"] > 0:
+    if options["upper_gp_length_factor"] > 0:
         # Max GP input length scale
         bounds["covariance_log_lengthscale"] = (
             -np.inf,
-            np.log(options["uppergplengthfactor"] * (pub - plb)),
+            np.log(options["upper_gp_length_factor"] * (pub - plb)),
         )
     # Increase minimum noise.
-    bounds["noise_log_scale"] = (np.log(options["tolfun"]) - 1, 5)
+    bounds["noise_log_scale"] = (np.log(options["tol_fun"]) - 1, 5)
 
     # Set priors over hyperparameters
     priors = gp.get_priors()
 
     tol_mesh = optim_state["tol_mesh"]
-    tol_fun = options["tolfun"]
+    tol_fun = options["tol_fun"]
 
     D = X.shape[1]
     cov_range = (optim_state["ub"] - optim_state["lb"]) / optim_state["scale"]
     cov_range = (np.minimum(100, 10 * cov_range)).flatten()
     # Bads prior on covariance length scale(s)
     priors["covariance_log_lengthscale"] = ("gaussian", (-1, 2.0))
     # BADS bounds on covariance length scale
@@ -884,25 +884,25 @@
     elif isinstance(gp.mean, gpr.mean_functions.ConstantMean):
         # Lower maximum constant mean
         sd = np.std(hpd_y) if len(hpd_y) > 1 else 1.0
         priors["mean_const"] = ("gaussian", (mean_x0, sd))
         bounds["mean_const"] = (mean_bounds_info["LB"], mean_bounds_info["UB"])
 
     elif isinstance(gp.mean, gpr.mean_functions.NegativeQuadratic):
-        if options["gpquadraticmeanbound"]:
+        if options["gp_quadratic_mean_bound"]:
             delta_y = max(
-                options["tolsd"],
+                options["tol_sd"],
                 min(D, np.max(hpd_y) - np.min(hpd_y)),
             )
             bounds["mean_const"] = (-np.inf, np.max(hpd_y) + delta_y)
     else:
         raise TypeError("The mean function is not supported by gpyreg.")
 
     # Prior over observation noise
-    if options["fitlik"]:
+    if options["fit_lik"]:
         priors["noise_log_scale"] = ("gaussian", (noise_mu, noise_std))
     else:
         # Known noise level
         priors["noise_log_scale"] = ("delta", (noise_mu))
 
     gp.temporary_data["len_scale"] = 1
     gp.temporary_data["poll_scale"] = np.ones(D)
@@ -959,29 +959,29 @@
 
     """
     iteration = optim_state["iter"]
 
     n_eff = np.sum(function_logger.n_evals[function_logger.X_flag])
 
     gp_train = {}
-    gp_train["init_method"] = options["gptraininitmethod"]
-    gp_train["tol_opt"] = options["gptolopt"]
+    gp_train["init_method"] = options["gp_train_init_method"]
+    gp_train["tol_opt"] = options["gp_tol_opt"]
     gp_train["widths"] = None
 
     # Set GP training options
     gp_train["sampler"] = "slicesample"
 
     # N-dependent initial training points.
     a = -(options["gp_train_n_init"] - options["gp_train_n_init_final"])
     b = -3 * a
     c = 3 * a
     d = options["gp_train_n_init"]
     eff_starting_points = optim_state["eff_starting_points"]
     x = (n_eff - eff_starting_points) / (
-        min(options["max_fun_evals"], options["ntrain_max"])
+        min(options["max_fun_evals"], options["n_train_max"])
         - eff_starting_points
     )
     f = lambda x_: a * x_**3 + b * x**2 + c * x + d
     init_N = max(round(f(x)), options["gp_train_n_init_final"])
     if (
         iteration >= 0
     ):  # the first time is called when the gp is initialized, and iteration is -1
@@ -1030,28 +1030,28 @@
         optim_state["periodic_vars"],
     )
     if dist.ndim > 1:
         dist = np.min(dist, axis=1)
     sort_idx = np.argsort(dist)  # Ascending sort
 
     # Keep only points within a certain (rescale) radius from target
-    radius = options["gpradius"] * gp.temporary_data["effective_radius"]
-    ntrain = np.minimum(options["ntrain_max"], np.sum(dist <= radius**2))
+    radius = options["gp_radius"] * gp.temporary_data["effective_radius"]
+    ntrain = np.minimum(options["n_train_max"], np.sum(dist <= radius**2))
 
     # Minimum number of point to keep
     ntrain = np.max(
         [
-            options["ntrain_min"],
-            options["ntrain_max"] - options["buffer_ntrain"],
+            options["n_train_min"],
+            options["n_train_max"] - options["buffer_ntrain"],
             ntrain,
         ]
     )
 
     # Up to the maximum number of available points
-    ntrain = np.minimum(ntrain, function_logger.X_max_idx)
+    ntrain = np.minimum(ntrain, function_logger.X_max_idx +1)
     optim_state["ntrain"] = ntrain
     # Take points closest to reference points
     res_S = None
     if function_logger.noise_flag:
         res_S = function_logger.S[sort_idx[0:ntrain]]
     return (U[sort_idx[0:ntrain]], Y[sort_idx[0:ntrain]], res_S)
 
@@ -1081,15 +1081,15 @@
     x = function_logger.X[function_logger.X_flag, :]
     y = function_logger.Y[function_logger.X_flag]
     if function_logger.noise_flag:
         s2 = function_logger.S[function_logger.X_flag] ** 2
     else:
         s2 = None
 
-    # Missing port: noiseshaping
+    # Missing port: noise_shaping
 
     evals_time = function_logger.fun_eval_time[function_logger.X_flag]
 
     return x, y, s2, evals_time
 
 
 def _estimate_noise_(gp: gpr.GP):
```

### Comparing `PyBADS-0.8.2/pybads/bads/optimize_result.py` & `PyBADS-1.0.0/pybads/bads/optimize_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import copy
 
+from importlib.metadata import version, PackageNotFoundError
+import logging
+
 import numpy as np
 
 class OptimizeResult(dict):
     """
     It represents the optimization result.
     
     Attributes:
     
         - fun: callable
             - The objective function to be minimized.
         - non_box_cons: callable
-            - Non-bound constraints function (if any).
+            - Non-box constraints function (if any).
         - x0: np.ndarray
             - Initial starting point.
         - x: np.ndarray
             - The solution of the optimization.
         - fval: float
             - Value of objective function at solution.
         - fsd: float
-            - Standard deviation of objective function at solution.
+            - Standard deviation of objective function at solution (0 if noiseless).
         - yval_vec: np.ndarray
             - Final sampled observations at the solution.
         - ysd_vec: np.ndarray
             - Standard deviations of the final sampled observations (``"yval_vec"``).
         - mesh_size: float
             - Final mesh size.
         - func_count: int
@@ -33,17 +36,17 @@
         - message: str
             - Termination message.
         - problem_type: str
             - Type of problem (unconstrained, bound constraints, non-box constraints).
         - total_time: float
             - Total time taken by the optimizer.
         - overhead: float
-            - Overhead time taken by the optimizer.
+            - Fractional overhead taken by the optimizer, compared to function time.
         - random_seed: int
-            - Random seed used by the optimizer.
+            - Random seed used by the optimizer (``None`` if not set).
         - version: str
             - Version of the optimizer.
     
     Parameters:
         bads: pybads.BADS
             - An Instance of the BADS class. It is used to set the attributes of the optimization result.
     """
@@ -127,27 +130,30 @@
             self["ysd_vec"] = None
 
         self["x0"] = bads.x0.copy()
         self["x"] = bads.x.copy()
         self["fval"] = bads.fval
         self["fsd"] = bads.fsd
         self["total_time"] = bads.optim_state["total_time"]
+        
+        self["random_seed"] = bads.optim_state["random_seed"]
 
-        # self['version'] = bads.version   # part of setuptools version = pkg_resources.require("MyProject")[0].version
-        #'status',
+        try:
+            __version__ = version("pybads")
+        except PackageNotFoundError:
+            # package is not installed
+            __version__ = None
+            logger = logging.getLogger("BADS")
+            logger.warning("Cannot read version number from package metadata.")
+            
+        self["version"] = __version__
+        
         self[
             "success"
         ] = True  # TODO: In our case when an error occurs, the application just stops.
-        self[
-            "random_seed"
-        ] = None  # TODO: PyBADS does not receive seed as input right now
-        self[
-            "version"
-        ] = "0.8.0"  # TODO: Retrieve the version from setup.py, or define it somewhere in BADS class.
-        # version = pkg_resources.require("pybads")[0].version
         self["message"] = bads.optim_state["termination_msg"]
 
     def __getattr__(self, name):
         try:
             return self[name]
         except KeyError as e:
             raise AttributeError(name) from e
```

### Comparing `PyBADS-0.8.2/pybads/bads/option_configs/advanced_bads_options.ini` & `PyBADS-1.0.0/pybads/bads/option_configs/advanced_bads_options.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,353 +1,353 @@
 [AdvancedOptions]
 # Show optimization plots ("profile", "scatter", or "False")
 plot = False
 
 # Tolerance and termination conditions
 # Tolerance on mesh size
-tolmesh = 1e-6
+tol_mesh = 1e-6
 # Min significant change of objective fcn
-tolfun = 1e-3
+tol_fun = 1e-3
 # Max iterations with no significant change (doubled under uncertainty)
-tolstalliters = int(4 + np.floor(D/2))
+tol_stall_iters = int(4 + np.floor(D/2))
 # Min variabitility for a fcn to be considered noisy
-tolnoise = np.spacing(1.0) * self.get("tolfun")
+tol_noise = np.spacing(1.0) * self.get("tol_fun")
 
 #Initialization
 # Initialization function
-initfcn = "init_sobol"
+init_fun = "init_sobol"
 # Number of restarts attempts
 restarts = 0
 # Size of cache for storing fcn evaluations
-cachesize = 500
+cache_size = 500
 # Number of initial objective fcn evaluations
 fun_eval_start = D
 # Pregress fcn evaluation with Y and X fields
-funvalues = {}
+fun_values = {}
 # Array with indices of periodic variables, like periodic_vars = [1, 2]
 periodic_vars = None
 
 # Poll Options
 # Poll function
-pollmethod                              = 'poll_mads_2n'        
+poll_method                              = 'poll_mads_2n'        
 
-nbasis                                  = 200 * D
+n_basis                                  = 200 * D
 # Mesh multiplicative factor between iterations
-pollmeshmultiplier                      = 2.0                   
+poll_mesh_multiplier                      = 2.0                   
 # Force poll vectors to be on mesh
-forcepollmesh                           = False                 
+force_poll_mesh                           = False                 
 # Maximum poll integer
-maxpollgridnumber                       = 0                     
+max_poll_grid_number                       = 0                     
 # Use alternative incumbent offset'
-alternativeincumbent                    = False                 
+alternative_incumbent                    = False                 
 # Adaptive multiplier to incumbent uncertainty'
-adaptiveincumbentshift                  = False                 
+adaptive_incumbent_shift                  = False                 
 # GP-based geometric scaling factor of poll vectors'
-gprescalepoll                           = 1.0                   
+gp_rescale_poll                           = 1.0                   
 # Threshold probability of improvement (PoI); set to 0 to always complete polling'
-tolpoi                                  = 1e-6/D                
+tol_poi                                  = 1e-6/D                
 # Skip polling if PoI below threshold, even with no success'
-skippoll                                = True                  
+skip_poll                                = True                  
 # Allow consecutive incomplete polls'
-consecutiveskipping                     = True                  
+consecutive_skipping                     = True                  
 # Skip polling after successful search'
-skippollaftersearch                     = True                  
+skip_poll_after_search                     = True                  
 # Number of failed fcn evaluations before skipping is allowed'
-minfailedpollsteps                      = np.Inf                
+min_failed_poll_steps                      = np.Inf                
 # Accelerate mesh after this number of stalled iterations'
 accelerate_mesh_steps                     = 3                  
 # Move incumbent even after insufficient improvement
-sloppyimprovement                       = True                  
+sloppy_improvement                       = True                  
 # Move incumbent even for the uncertain unsuccess when Sto-BADS is configured
 opp_stobads                             = True                  
 # Power value of the Sto-BADS incumbent decision rule:  \gamma *  \epsilon * frame_size**(power_value)
 stobads_frame_size_scaling_power        = 2                     
 # Threshold # mesh overflows for warning';
-meshoverflowswarning                    = 2 + D/2               
+mesh_overflow_warning                    = 2 + D/2               
 # Initial mesh size (power value)
 init_mesh_size_integer                  = 0                     
 
 # StoBADS option, if True switch to stochastic optimization and uncertain incumbent
 stobads = False
 
 # Improvement parameters
 # Minimum significant improvement at unit mesh size'
-tolimprovement          = 1                    
+tol_improvement          = 1                    
 # Exponent of forcing function'
-forcingexponent         = 3/2                  
+forcing_exponent         = 3/2                  
 # Multiplier to incumbent uncertainty for acquisition functions'
-incumbentsigmamultiplier = 0.1                 
+incumbent_sigma_multiplier = 0.1                 
 # Quantile when computing improvement (<0.5 for conservative improvement)'
-improvementquantile     = 0.5                  
+improvement_quantile     = 0.5                  
 # Top quantile when choosing final iteration'
-finalquantile           = 1e-3                 
+final_quantile           = 1e-3                 
 
 # Search properties
 # Number of candidate search points'
-nsearch                 = 2**12                
+n_search                 = 2**12                
 # Number of optimization iterations for search'
-nsearchiter             = 2                    
+n_search_iter             = 2                    
 # Multiplier in ES'
-esbeta                  = 1                    
+es_beta                  = 1                    
 # Starting scale value in ES'
-esstart                 = 0.25                 
+es_start                 = 0.25                 
 # Fraction of candidate search points with (slower) improved estimate'
-searchimprovefrac       = 0                    
+search_improve_frac       = 0                    
 # Search radius expansion factor for successful search'
-searchscalesuccess      = np.sqrt(2)           
+search_scale_success      = np.sqrt(2)           
 # Search radius expansion factor for incremental search'
-searchscaleincremental  = 2                    
+search_scale_incremental  = 2                    
 # Search radius contraction factor for failed search'
-searchscalefailure      = np.sqrt(0.5)         
-searchfactormin         = 0.5
+search_scale_failure      = np.sqrt(0.5)         
+search_factor_min         = 0.5
 # Search function(s) (list of tuples with function name and sumrule flag)'
-searchmethod            = [('ES-wcm',1), ('ES-ell',1)]  
+search_method            = [('ES-wcm',1), ('ES-ell',1)]  
 # Iteration scale factor between poll and search'
-searchgridnumber        = 10                   
+search_grid_number        = 10                   
 # Multiplier integer scale factor between poll and search'
-searchgridmultiplier    = 2                    
+search_grid_multiplier    = 2                    
 # Relative search scale factor locked to poll scale factor'
-searchsizelocked       = True                  
+search_size_locked       = True                  
 # Number of searches per iteration'
-searchntry              = np.maximum(D, np.floor(3 + D/2)) 
+search_n_try              = np.maximum(D, np.floor(3 + D/2)) 
 # Search-triggered mesh expansion after this number of successful search rounds'
-searchmeshexpand        = 0                    
+search_mesh_expand        = 0                    
 # Mesh size increment after search-triggered mesh expansion'
-searchmeshincrement     = 1                    
+search_mesh_increment     = 1                    
 # Further optimize acquisition function'
-searchoptimize          = False                
+search_optimize          = False                
 
 # Noise parameters
 # Treat incumbent as if uncertain regardless of uncertainty handling'
-uncertainincumbent      = True                  
+uncertain_incumbent      = True                  
 # Contribution to log noise magnitude from log mesh size (0 for noisy functions)'
-meshnoisemultiplier      = 0.5                  
+mesh_noise_multiplier      = 0.5                  
 
 # Gaussian process properties
 # Number of training data (minimum 200 under uncertainty)
-ntrain_max                = 50 + 10*D           
+n_train_max                = 50 + 10*D           
 # Minimum number of training data (doubled under uncertainty)
-ntrain_min                = 50                  
+n_train_min                = 50                  
 # Max number of training data removed if too far from current point
 buffer_ntrain             = 100                 
 # Hyperparameters samples (0 = optimize)
-gpsamples                 = 0                     
+gp_samples                 = 0                     
 # MCMC sampler for GP hyperparameters
-gphypsampler = "slicesample"                    
+gp_hyp_sampler = "slicesample"                    
 # High Posterior Density region (fraction of training inputs)
 hpd_frac = 0.8                                  
 # Switch to covariance sampling below this threshold of stability index
-covsamplethresh = 10                            
+cov_sample_thresh = 10                            
 # Multiplier to widths from previous posterior for GP sampling (Inf = do not use previous widths)
-gpsamplewidths = 0                              
+gp_sample_widths = 0                              
 # Use weighted hyperparameter posterior covariance
-weightedhypcov=True                             
+weighted_hyp_cov=True                             
 # Minimum weight for weighted hyperparameter posterior covariance
-tolcovweight = 0                                
+tol_cov_weight = 0                                
 # Weight of previous trials (per trial) for running avg of GP hyperparameter covariance
-hyprunweight = 1                                
+hyp_run_weight = 1                                
 # Minimum fcn evals before refitting the GP
-minrefittime            = 2*D                   
+min_refit_time            = 2*D                   
 # Train GP also during poll stage
-polltraining            = True                  
+poll_training            = True                  
 # Always try a second GP fit
-doublerefit             = False  
+double_refit             = False  
 # GP mean function               
-gp_meanfun              = 'const'
-gp_covfun               = 1
+gp_mean_fun              = 'const'
+gp_cov_fun               = 1
 # Percentile of empirical GP mean
 gp_mean_percentile        = 90                    
 # Empirical range of hyperprior over the mean
 gp_mean_range_fun          = lambda ym,y: (ym - np.median(y))/5*2   
 # GP definition fcn'
-gpdeffcn                = ('gp_def_bads','rq',[1,1])  
+gp_def_fcn                = ('gp_def_bads','rq',[1,1])  
 # GP training set selection method'
-gpmethod                = 'nearest'             
+gp_method                = 'nearest'             
 # Cluster additional points during training
-gpcluster               = False                 
+gp_cluster               = False                 
 # Rotate GP basis
-rotategp                = False                 
+rotate_gp                = False                 
 # Radius of training set
-gpradius                = 3                     
+gp_radius                = 3                     
 use_effective_radius      = True                
 # GP hyper-prior over covariance'
-gpcovprior              = 'iso'                  
+gp_cov_prior              = 'iso'                  
 gp_fixed_mean             = False
 # Fit the likelihood term
-fitlik                  = True                  
+fit_lik                  = True                  
 # Acquisition fcn for poll stage
-pollacqfcn              = ('acq_LCB', None)         
+poll_acq_fcn              = ('acq_LCB', None)         
 # Acquisition fcn for search stage
-searchacqfcn            = ('acq_LCB', None)         
+search_acq_fcn            = ('acq_LCB', None)         
 # Hedge acquisition function
-acqhedge                = False                  
+acq_hedge                = False                  
 # Attempts at performing the Cholesky decomposition
-cholattempts            = 0                    
+chol_attempts            = 0                    
 # Increase nudge to noise in case of Cholesky failure
 noise_nudge             = np.array([1, 0])                
 # Start removing training points after this number of failures
 remove_points_after_tries  = 1                    
 # SVGD iterations for GP training
-gpsvditers              = 200                  
+gp_svd_iters              = 200                  
 # Issue warning if GP hyperparameters fit fails
 gp_warnings             = False          
 # Alpha level for normality test of gp predictions
-normalphalevel          = 1e-6                 
+normalpha_level          = 1e-6                 
 # Number of target fcn evals per iteration
 fun_evals_per_iter = 1                      
 # Thinning for GP hyperparameter sampling
-gpsamplethin = 5                            
+gp_sample_thin = 5                            
 # Force stable GP hyperparameter sampling (reduce samples or start optimizing)
-stablegpsampling = 200 + 10 * D             
+stable_gp_sampling = 200 + 10 * D             
 # Initial design points for GP hyperparameter training
 gp_train_n_init = 128                         
 # Final design points for GP hyperparameter training
 gp_train_n_init_final = 8                      
 # Initial design method for GP hyperparameter training
-gptraininitmethod = "rand"                  
+gp_train_init_method = "rand"                  
 # Tolerance for optimization of GP hyperparameters
-gptolopt = 1e-5                             
+gp_tol_opt = 1e-5                             
 # Tolerance for optimization of GP hyperparameters preliminary to MCMC
-gptoloptmcmc = 1e-2                         
+gp_tol_optmcmc = 1e-2                         
 # Max GP hyperparameter samples (decreases with training points)
-nsgpmax = 0                                 
+nsgp_max = 0                                 
 # Max GP hyperparameter samples during warmup
-nsgpmaxwarmup = 8                           
+nsgp_maxwarmup = 8                           
 # Max GP hyperparameter samples during main algorithm
-nsgpmaxmain = np.Inf                        
+nsgp_maxmain = np.Inf                        
 # Number of GP samples when GP is stable (0 = optimize)
-stablegpsamples = 0                         
+stable_gp_samples = 0                         
 # Tolerance for optimization of GP hyperparameters during active sampling
-gptoloptactive = 1e-4                       
+gp_tol_optactive = 1e-4                       
 # Tolerance for optimization of GP hyperparameters preliminary to MCMC during active sampling
-gptoloptmcmcactive = 1e-2                   
+gp_tol_optmcmcactive = 1e-2                   
 # Threshold True GP variance used by regulatized acquisition fcns
-tolgpvar = 1e-4                             
+tol_gp_var = 1e-4                             
 # Threshold True GP variance used to stabilize sampling
-tolgpvarmcmc = 1e-4                        
+tol_gp_varmcmc = 1e-4                        
 # Perform GP training after each active sample
-activesamplegpupdate = False                
+active_sample_gp_update = False                
 # Extra variational components sampled from GP profile
-sampleextravpmeans = 0                      
+sample_extra_vp_means = 0                      
 # Try integrating GP mean function
-integrategpmean = False                     
+integrate_gp_mean = False                     
 # Tolerance True ELBO uncertainty for stopping (if variational posterior is stable)
-tolsd = 0.1                                 
+tol_sd = 0.1                                 
 # Stopping threshold True change of variational posterior per training point
-tolskl = 0.01 * np.sqrt(D)                  
+tol_skl = 0.01 * np.sqrt(D)                  
 # Number of stable fcn evals for stopping warmup
-tolstablewarmup = 15                        
+tol_stable_warmup = 15                        
 # MCMC sampler for variational posteriors
-variationalsampler = "malasample"           
+variational_sampler = "malasample"           
 # Use Gaussian approximation for symmetrized KL-divergence b\w iters
-klgauss = True                              
+kl_gauss = True                              
 # Variational components during warmup
-kwarmup = 2                                 
+k_warmup = 2                                 
 # Force stable GP hyperparameter sampling after reaching this number of components
-stablegpvpk = np.Inf                        
+stable_gp_vpk = np.Inf                        
 # GP warping function type
-warpfunc = 0                                
+warp_func = 0                                
 # Slice sampler option for prior hyper-parameter sampling method
 use_slice_sampler = False                   
 
 # Adaptive basis (unsupported)
-hessianupdate           = False                 # Update Hessian as you go
-hessianmethod           = 'bfgs'               # Hessian update method
-hessianalternate        = False                 # Alternate Hessian iterations
+hessian_update           = False                 # Update Hessian as you go
+hessian_method           = 'bfgs'               # Hessian update method
+hessian_alternate        = False                 # Alternate Hessian iterations
 
 # Hedge heuristic parameters (currently used during the search stage)
-hedgegamma              = 0.125
-hedgebeta               = 1e-3/self.get('tolfun')
-hedgedecay              = 0.1**(1/(2*D))
+hedge_gamma              = 0.125
+hedge_beta               = 1e-3/self.get('tol_fun')
+hedge_decay              = 0.1**(1/(2*D))
 
 # Max number of consecutive repeated measurements for noisy inputs
-maxrepeatedobservations = 0
+max_repeated_observations = 0
 # Multiplicative discount True acquisition fcn to repeat measurement at the same location
-repeatedacqdiscount = 1
+repeated_acq_discount = 1
 # Base step size for stochastic gradient descent
-sgdstepsize = 0.005
+sgd_step_size = 0.005
 # Use ranking criterion to pick best non-converged solution
-rankcriterion = True
+rank_criterion = True
 # Run in diagnostics mode get additional info
 diagnostics = False
 # Output function
-outputfcn = None
+output_fcn = None
 
-# Evaluated fcn values at X0
-fvals = None
+# Evaluated function values at X0
+f_vals = None
 # Samples for fast acquisition fcn eval per new point
-nssearch = 2 ** 13
+ns_search = 2 ** 13
 # Set stochastic optimization stepsize via GP hyperparameters
-gpstochasticstepsize = False
+gp_stochastic_step_size = False
 # Min number of fcn evals
-minfunevals = 5 * D
+min_fun_evals = 5 * D
 # Min number of iterations
-miniter = D
+min_iter = D
 # Fraction of search points from heavy-tailed variational posterior
-heavytailsearchfrac = 0.25
+heavy_tail_search_frac = 0.25
 # Fraction of search points from multivariate normal
-mvnsearchfrac = 0.25
+mvn_search_frac = 0.25
 # Fraction of search points from multivariate normal fitted to HPD points
-hpdsearchfrac = 0
+hpd_search_frac = 0
 # Fraction of search points from uniform random box based True training inputs
-boxsearchfrac = 0.25
+box_search_frac = 0.25
 # Fraction of search points from previous iterations
-searchcachefrac = 0
+search_cache_frac = 0
 # Empirical Bayes prior over some GP hyperparameters
-empiricalgpprior = False
+empirical_gp_prior = False
 # Minimum GP observation noise
-tolgpnoise = np.sqrt(1e-5)
+tol_gp_noise = np.sqrt(1e-5)
 # Prior mean over GP input length scale (in plausible units)
-gplengthpriormean = np.sqrt(D / 6)
+gp_length_prior_mean = np.sqrt(D / 6)
 # Prior std over GP input length scale (in plausible units)
-gplengthpriorstd = 0.5 * np.log(1e3)
+gp_length_prior_std = 0.5 * np.log(1e3)
 # Upper bound True GP input lengths based True plausible box (0 = ignore)
-uppergplengthfactor = 0
+upper_gp_length_factor = 0
 # Initial samples (plausible is uniform in the plausible box)
-initdesign = "plausible"
+init_design = "plausible"
 # Stricter upper bound True GP negative quadratic mean function
-gpquadraticmeanbound = True
-# Bandwidth parameter for GP smoothing (in units of plausible box)
+gp_quadratic_mean_bound = True
+# bandwidth parameter for GP smoothing (in units of plausible box)
 bandwidth = 0
 # Heuristic output warping (fitness shaping)
 fitness_shaping = False
 # Output warping starting threshold
-outwarpthreshbase = 10 * D
+out_warp_thresh_base = 10 * D
 # Output warping threshold multiplier when failed sub-threshold check
-outwarpthreshmult = 1.25
+out_warp_thresh_mult = 1.25
 # Output warping base threshold tolerance (fraction of current threshold)
-outwarpthreshtol = 0.8
+out_warp_thresh_tol = 0.8
 # Temperature for posterior tempering (allowed values T = 1234)
 temperature = 1
 # Use separate GP with constant mean for active search
-separatesearchgp = False
+separate_search_gp = False
 # Discount observations from extremely low-density regions
-noiseshaping = False
+noise_shaping = False
 # Threshold from max observed value to start discounting
-noiseshapingthreshold = 10 * D
+noise_shaping_threshold = 10 * D
 # Proportionality factor of added noise wrt distance from threshold
-noiseshapingfactor = 0.05
+noise_shaping_factor = 0.05
 # Past iterations window to judge acquisition fcn improvement
-acqhedgeiterwindow = 4
+acq_hedge_iter_window = 4
 # Portfolio value decay per function evaluation
-acqhedgedecay = 0.9
+acqhedge_decay = 0.9
 
 # Active search bound multiplier
-activesearchbound = 2
+active_search_bound = 2
 # Tolerance True closeness to bound constraints (fraction of total range)
-tolboundx = 1e-5
+tol_bound_x = 1e-5
 # Recompute LCB max for each iteration based True current GP estimate
-recomputelcbmax = True
+recompute_lcb_max = True
 # Use double GP
-doublegp = False
+double_gp = False
 # Warp every this number of iterations
-warpeveryiters = 5
+warp_every_iters = 5
 # Increase delay between warpings
-incrementalwarpdelay = True
+incremental_warp_delay = True
 # Threshold True reliability index to perform warp
-warptolreliability = 3
+warp_tol_reliability = 3
 # Rotate and scale input
-warprotoscaling = True
+warp_proto_scaling = True
 # Regularization weight towards diagonal covariance matrix for N training inputs
-warpcovreg = 0
+warp_cov_reg = 0
 # Threshold True correlation matrix for roto-scaling
-warprotocorrthresh = 0.05
+warp_proto_corr_thresh = 0.05
```

### Comparing `PyBADS-0.8.2/pybads/bads/option_configs/basic_bads_options.ini` & `PyBADS-1.0.0/pybads/bads/option_configs/basic_bads_options.ini`

 * *Files 14% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 uncertainty_handling = None
 # Base observation noise magnitude (SD), e.g noise_size = 1.0
 noise_size = None
 # Target function returns noise estimate (SD) as second output
 specify_target_noise = False
 # Samples to estimate FVAL at the end (for noisy objectives)
 noise_final_samples = 10
+# Random seed used by the optimizer. If None, no seed is set.
+random_seed = None
```

### Comparing `PyBADS-0.8.2/pybads/bads/options.py` & `PyBADS-1.0.0/pybads/bads/options.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/decorators/README.md` & `PyBADS-1.0.0/pybads/decorators/README.md`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/decorators/handle_0D_1D_input.py` & `PyBADS-1.0.0/pybads/decorators/handle_0D_1D_input.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/function_examples.py` & `PyBADS-1.0.0/pybads/function_examples.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/function_logger/constraints_check.py` & `PyBADS-1.0.0/pybads/function_logger/constraints_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         idx = np.any(U > ub, axis=1) | np.any(U < lb, axis=1)
         U_new = U[~idx].copy()
 
     # Remove duplicate vectors and preserve the initial order
     _, idx_sort = np.unique(U_new, axis=0, return_index=True)
     U_new = U_new[np.sort(idx_sort), :]
 
-    # Remove previously evaluated vectors (within TolMesh)
+    # Remove previously evaluated vectors (within tol_mesh)
     if U_new.size > 0:
         tol = tol_mesh / 2.0
         u1 = np.round(U_new / tol)
         X_max_idx = function_logger.X_max_idx
         u2 = np.round(function_logger.X[: X_max_idx + 1] / tol)
         tmp_u = np.vstack((u1, u2))
         _, idx_sort = np.unique(tmp_u, axis=0, return_index=True)
```

### Comparing `PyBADS-0.8.2/pybads/function_logger/function_logger.py` & `PyBADS-1.0.0/pybads/function_logger/function_logger.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/init_functions/init_sobol.py` & `PyBADS-1.0.0/pybads/init_functions/init_sobol.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/poll/poll_mads_2n.py` & `PyBADS-1.0.0/pybads/poll/poll_mads_2n.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/search/es_search.py` & `PyBADS-1.0.0/pybads/search/es_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,30 @@
     """An Abstract class describing an Evolutionary Strategy Search."""
 
     def __init__(self, mu, lamb, options_dict):
         self.mu = mu
         self.lamb = lamb
         self.vec = np.array([-1, 0])
         self.w = (
-            options_dict["pollmeshmultiplier"] ** self.vec
+            options_dict["poll_mesh_multiplier"] ** self.vec
         )  # helps with the stability
         self.ns = np.diff(
             np.round(np.linspace(0, self.mu, np.size(self.w) + 1)).astype(int)
         )
 
         self.vec = np.empty((0, 1), dtype="float")
         for i in range(0, len(self.w)):
             self.vec = np.append(
                 self.vec, self.w[i] * np.ones((self.ns[i], 1)), axis=0
             )
 
-        self.scale = options_dict["esstart"]
-        self.n_search_iter = options_dict["nsearchiter"]
-        self.search_acq_fcn = options_dict["searchacqfcn"]
-        self.es_beta = options_dict["esbeta"]
+        self.scale = options_dict["es_start"]
+        self.n_search_iter = options_dict["n_search_iter"]
+        self.search_acq_fcn = options_dict["search_acq_fcn"]
+        self.es_beta = options_dict["es_beta"]
         self.logger = logging.getLogger("BADS")
         logging.basicConfig(stream=sys.stdout, format="%(message)s")
 
     def _get_selection_idx_mask_(self, mu, lamb):
         """
         Corresponds to esupdate of the  BADS Matlab version
         """
```

### Comparing `PyBADS-0.8.2/pybads/search/grid_functions.py` & `PyBADS-1.0.0/pybads/search/grid_functions.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/search/search_hedge.py` & `PyBADS-1.0.0/pybads/search/search_hedge.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,21 @@
         self.n_funs = len(search_fcns)
         self.g = np.zeros(self.n_funs)
         self.g[0] = 10
         self.count = -1
         self.options_dict = options_dict
         self.non_box_cons = non_box_cons
 
-        self.gamma = options_dict["hedgegamma"]
-        self.beta = options_dict["hedgebeta"]
-        self.decay = options_dict["hedgedecay"]
+        self.gamma = options_dict["hedge_gamma"]
+        self.beta = options_dict["hedge_beta"]
+        self.decay = options_dict["hedge_decay"]
 
         # Create vector of ES weights (for ESSearch)
-        es_iter = self.options_dict["nsearchiter"]
-        self.mu = int(self.options_dict["nsearch"] / es_iter)
+        es_iter = self.options_dict["n_search_iter"]
+        self.mu = int(self.options_dict["n_search"] / es_iter)
         self.lamb = self.mu
 
     def __call__(self, u, lb, ub, func_logger, gp: GP, optim_state):
         self.count += 1
         # gamma = np.minimum(1/n_funs, np.sqrt(np.log(n_funs)/(n_funs*count)));
 
         self.prob = np.exp(self.beta * (self.g - np.max(self.g)))
```

### Comparing `PyBADS-0.8.2/pybads/stats/get_hpd.py` & `PyBADS-1.0.0/pybads/stats/get_hpd.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/stats/kde1d.py` & `PyBADS-1.0.0/pybads/stats/kde1d.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/stats/kldiv_mvn.py` & `PyBADS-1.0.0/pybads/stats/kldiv_mvn.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/hyp.dat` & `PyBADS-1.0.0/pybads/testing/bads/hyp.dat`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/poll/test_poll_mads.py` & `PyBADS-1.0.0/pybads/testing/bads/poll/test_poll_mads.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/scripts/ackley_example.py` & `PyBADS-1.0.0/pybads/testing/bads/scripts/ackley_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py` & `PyBADS-1.0.0/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/scripts/bads_rosenbrock_example.py` & `PyBADS-1.0.0/pybads/testing/bads/scripts/bads_rosenbrock_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/scripts/non_bound_example.py` & `PyBADS-1.0.0/pybads/testing/bads/scripts/non_bound_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/scripts/rastrigin_example.py` & `PyBADS-1.0.0/pybads/testing/bads/scripts/rastrigin_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/bads/search/test_search.py` & `PyBADS-1.0.0/pybads/testing/bads/search/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     plb = np.array([[-5, -5, -5]])  # Plausible lower bounds
     pub = np.array([[5, 5, 5]])  # Plausible upper bounds
     D = 3
     bads = BADS(rosenbrocks_fcn, x0, lb, ub, plb, pub)
     bads.options["fun_eval_start"] = 0
     gp, Ns_gp, sn2hpd, hyp_dict = bads._init_optimization_()
 
-    es_iter = bads.options["nsearchiter"]
-    mu = int(bads.options["nsearch"] / es_iter)
+    es_iter = bads.options["n_search_iter"]
+    mu = int(bads.options["n_search"] / es_iter)
     lamb = mu
     search_es = ESSearchWM(mu, lamb, bads.options)
     us, z = search_es(
         bads.u, lb, ub, bads.function_logger, gp, bads.optim_state, True, None
     )
 
     assert us.size == 3 and (np.isscalar(z) or z.size == 1)
@@ -111,15 +111,15 @@
     pub = np.array([[5, 5, 5]])  # Plausible upper bounds
     D = 3
 
     bads = BADS(rosenbrocks_fcn, x0, lb, ub, plb, pub)
     bads.options["fun_eval_start"] = 0
     gp, Ns_gp, sn2hpd, hyp_dict = bads._init_optimization_()
 
-    search_hedge = ESSearchHedge(bads.options["searchmethod"], bads.options)
+    search_hedge = ESSearchHedge(bads.options["search_method"], bads.options)
 
     us, z = search_hedge(
         bads.u, lb, ub, bads.function_logger, gp, bads.optim_state
     )
     print(search_hedge.chosen_search_fun)
     assert us.size == 3 and (np.isscalar(z) or z.size == 1)
     assert np.all(gp.y >= z)
@@ -161,15 +161,15 @@
     gp.y = np.array([1, 405.1637, 5.082e3])
     f.Y = gp.y.copy()
 
     f.X_max_idx = 3
 
     gp.temporary_data["len_scale"] = 1.0
     bads.optim_state["scale"] = 1.0
-    bads.options["gpradius"] = 3
+    bads.options["gp_radius"] = 3
 
     result = get_grid_search_neighbors(
         f, np.array([[0, 0]]), gp, bads.options, bads.optim_state
     )[0]
     assert (
         result[0, 0] == 0.0
         and np.isclose(result[1, 0], -0.1055, 1e-3)
```

### Comparing `PyBADS-0.8.2/pybads/testing/bads/test_gaussian_process_train.py` & `PyBADS-1.0.0/pybads/testing/bads/test_gaussian_process_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     
 
     hyp_dict = {"run_cov": np.eye(3)}
     hyp_dict_none = {"run_cov": None}
     bads.optim_state['eff_starting_points'] = 10
     bads.optim_state["ntrain"] = 10
     bads.optim_state["iter"] = 1
-    bads.options["weightedhypcov"] = False
+    bads.options["weighted_hyp_cov"] = False
 
     res1 = _get_gp_training_options(
         bads.optim_state, bads.iteration_history, bads.options, hyp_dict, 8, bads.function_logger
     )
     assert res1["sampler"] == "slicesample"
 
 
@@ -186,15 +186,15 @@
     pub = np.ones((1, D)) * 4
     f = lambda x: np.sum(x + 2)
     bads = BADS(f, x0, lb, ub, plb, pub)
 
     bads.optim_state['eff_starting_points'] = 10
     bads.optim_state["ntrain"] = 10
     bads.optim_state["iter"] = 2
-    bads.options["weightedhypcov"] = False
+    bads.options["weighted_hyp_cov"] = False
     hyp_dict = {"run_cov": np.eye(3)}
     hyp_dict_none = {"run_cov": None}
     bads.options["gpretrainthreshold"] = 10
 
     res1 = _get_gp_training_options(
     bads.optim_state, bads.iteration_history, bads.options, hyp_dict, 0, bads.function_logger
     )
```

### Comparing `PyBADS-0.8.2/pybads/testing/bads/test_iteration_history.py` & `PyBADS-1.0.0/pybads/testing/bads/test_iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py` & `PyBADS-1.0.0/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/function_logger/test_function_logger.py` & `PyBADS-1.0.0/pybads/testing/function_logger/test_function_logger.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/testing/variable_transformer/test_variable_transformer.py` & `PyBADS-1.0.0/pybads/testing/variable_transformer/test_variable_transformer.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/utils/iteration_history.py` & `PyBADS-1.0.0/pybads/utils/iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/utils/timer/timer.py` & `PyBADS-1.0.0/pybads/utils/timer/timer.py`

 * *Files identical despite different names*

### Comparing `PyBADS-0.8.2/pybads/variable_transformer/variables_transformer.py` & `PyBADS-1.0.0/pybads/variable_transformer/variables_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 from pybads.decorators import handle_0D_1D_input
 
 
 class VariableTransformer:
     """
-    A class enabling linear or non-linear transformation of the bounds (plb and pub) and map them to an hypercube [-1, 1]^D
+    A class enabling linear or non-linear transformation of the bounds (plausible_lower_bounds and plausible_upper_bounds) and map them to an hypercube [-1, 1]^D
     
     Parameters
     ----------
     D : int
         The dimension of the space.
     lower_bounds : np.ndarray, optional
         The lower bounds of the space. ``lower_bounds`` and ``upper_bounds`` define a set
@@ -115,17 +115,17 @@
             self.z,
             self.zlog,
         ) = self.__create_hypercube_trans__()
 
     def __create_hypercube_trans__(self):
         """
         Standardize variables via linear or nonlinear transformation.
-        The standardized transform maps plb and pub to the hypercube [-1,1]^D.
-        If plb and/or pub are empty, lb and/or ub are used instead. Note that
-        at least one among lb, plb and one among ub, pub needs to be nonempty.
+        The standardized transform maps ``plausible_lower_bounds`` (``plb``) and plausible_upper_bounds (``pub``) to the hypercube [-1,1]^D.
+        If plb and/or pub are empty, ``lower_bound``(``lb``) and/or ``upper_bound``(``ub``) are used instead. Note that
+        at least one among ``lb``, ``plb`` and one among ``ub``, ``pub`` needs to be nonempty.
 
         Parameters
         ----------
 
         D : scalar
             dimension
         lower_bound: np.ndarray
@@ -133,21 +133,21 @@
         plausible_lower_bounds: np.ndarray
         plausible_upper_bounds: np.ndarray
 
 
         """
         # Check finiteness of plausible range
         if not (np.all(np.isfinite(np.concatenate([self.plb, self.pub])))):
-            raise ValueError("Plausible interval ranges plb and pub need to be finite.")
+            raise ValueError("Plausible interval ranges plausible_lower_bounds and plausible_upper_bounds need to be finite.")
 
         # Check that the order of bounds is respected
         if  not (np.all(self.lb <= self.plb) \
             and np.all(self.plb < self.pub)\
             and np.all(self.pub <= self.ub)):
-                raise ValueError("Interval bounds needs to respect the order lb <= plb < pub <= ub for all coordinates.")
+                raise ValueError("Interval bounds needs to respect the order lower_bound <= plausible_lower_bounds < plausible_upper_bounds <= upper_bound for all coordinates.")
          
 
         # A variable is converted to log scale if all bounds are positive and
         # the plausible range spans at least one order of magnitude
         for i in np.argwhere(np.isnan(self.apply_log_t.squeeze())):
             self.apply_log_t[:, i] = (
                 np.all(
```

### Comparing `PyBADS-0.8.2/pyproject.toml` & `PyBADS-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -62,7 +62,8 @@
 use_parentheses = true
 profile = "black"
 
 [tool.pycln]
 all = true
 
 [tool.setuptools_scm]
+write_to = "pybads/_version.py"
```

