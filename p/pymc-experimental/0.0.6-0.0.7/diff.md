# Comparing `tmp/pymc-experimental-0.0.6.tar.gz` & `tmp/pymc-experimental-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-experimental-0.0.6.tar", last modified: Thu Jun  8 10:24:44 2023, max compression
+gzip compressed data, was "pymc-experimental-0.0.7.tar", last modified: Sat Jun 10 09:24:10 2023, max compression
```

## Comparing `pymc-experimental-0.0.6.tar` & `pymc-experimental-0.0.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/histogram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/r2d2m2cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/gp/latent_approx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/inference/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/inference/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_transform/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_transform/conditioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/preprocessing/standard_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_multivariate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_conditioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_histogram_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_prior_from_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/utils/test_model_fgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/model_fgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/pytensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.893581 pymc-experimental-0.0.7/pymc_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/distributions/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/multivariate/r2d2m2cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/gp/latent_approx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/inference/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/inference/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_transform/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_transform/conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/preprocessing/standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_multivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_histogram_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_prior_from_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/utils/test_model_fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/pymc_experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/model_fgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/pytensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/setup.py
```

### Comparing `pymc-experimental-0.0.6/CODE_OF_CONDUCT.md` & `pymc-experimental-0.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/LICENSE` & `pymc-experimental-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/PKG-INFO` & `pymc-experimental-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.6
+Version: 0.0.7
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.6 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.7 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.6/README.md` & `pymc-experimental-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/__init__.py` & `pymc-experimental-0.0.7/pymc_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/distributions/__init__.py` & `pymc-experimental-0.0.7/pymc_experimental/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/distributions/continuous.py` & `pymc-experimental-0.0.7/pymc_experimental/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/distributions/discrete.py` & `pymc-experimental-0.0.7/pymc_experimental/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/distributions/histogram_utils.py` & `pymc-experimental-0.0.7/pymc_experimental/distributions/histogram_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/r2d2m2cp.py` & `pymc-experimental-0.0.7/pymc_experimental/distributions/multivariate/r2d2m2cp.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/distributions/timeseries.py` & `pymc-experimental-0.0.7/pymc_experimental/distributions/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from pymc.distributions.shape_utils import (
     _change_dist_size,
     change_dist_size,
     get_support_shape_1d,
 )
 from pymc.logprob.abstract import _logprob
 from pymc.logprob.basic import logp
-from pymc.logprob.utils import ignore_logprob
 from pymc.pytensorf import intX
 from pymc.util import check_dist_not_registered
 from pytensor.graph.basic import Node
 from pytensor.tensor import TensorVariable
 from pytensor.tensor.random.op import RandomVariable
 
 
@@ -162,17 +161,14 @@
                 "`Categorical.dist(p=pt.full((k_states, ), 1/k_states), shape=...)`. You can specify an init_dist "
                 "manually to suppress this warning.",
                 UserWarning,
             )
             k = P.shape[-1]
             init_dist = pm.Categorical.dist(p=pt.full((k,), 1 / k))
 
-        # We can ignore init_dist, as it will be accounted for in the logp term
-        init_dist = ignore_logprob(init_dist)
-
         return super().dist([P, steps, init_dist], n_lags=n_lags, **kwargs)
 
     @classmethod
     def rv_op(cls, P, steps, init_dist, n_lags, size=None):
         if size is not None:
             batch_size = size
         else:
```

### Comparing `pymc-experimental-0.0.6/pymc_experimental/gp/__init__.py` & `pymc-experimental-0.0.7/pymc_experimental/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/gp/latent_approx.py` & `pymc-experimental-0.0.7/pymc_experimental/gp/latent_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/inference/__init__.py` & `pymc-experimental-0.0.7/pymc_experimental/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/inference/fit.py` & `pymc-experimental-0.0.7/pymc_experimental/inference/fit.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/inference/pathfinder.py` & `pymc-experimental-0.0.7/pymc_experimental/inference/pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/linearmodel.py` & `pymc-experimental-0.0.7/pymc_experimental/linearmodel.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/marginal_model.py` & `pymc-experimental-0.0.7/pymc_experimental/marginal_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Sequence, Tuple, Union
 
 import numpy as np
 import pytensor.tensor as pt
 from pymc import SymbolicRandomVariable
 from pymc.distributions.discrete import Bernoulli, Categorical, DiscreteUniform
 from pymc.distributions.transforms import Chain
-from pymc.logprob.abstract import _get_measurable_outputs, _logprob
-from pymc.logprob.basic import factorized_joint_logprob
+from pymc.logprob.abstract import _logprob
+from pymc.logprob.basic import conditional_logp
 from pymc.logprob.transforms import IntervalTransform
 from pymc.model import Model
 from pymc.pytensorf import constant_fold, inputvars
 from pytensor import Mode
 from pytensor.compile import SharedVariable
 from pytensor.compile.builders import OpFromGraph
 from pytensor.graph import Constant, FunctionGraph, ancestors, clone_replace
@@ -367,20 +367,14 @@
         ndim_supp=0,
     )
     marginalized_rvs = marginalization_op(*replace_inputs.keys())
     fgraph.replace_all(tuple(zip(rvs_to_marginalize, marginalized_rvs)))
     return rvs_to_marginalize, marginalized_rvs
 
 
-@_get_measurable_outputs.register(FiniteDiscreteMarginalRV)
-def _get_measurable_outputs_finite_discrete_marginal_rv(op, node):
-    # Marginalized RVs are not measurable
-    return node.outputs[1:]
-
-
 def get_domain_of_finite_discrete_rv(rv: TensorVariable) -> Tuple[int, ...]:
     op = rv.owner.op
     if isinstance(op, Bernoulli):
         return (0, 1)
     elif isinstance(op, Categorical):
         p_param = rv.owner.inputs[3]
         return tuple(range(pt.get_vector_length(p_param)))
@@ -399,15 +393,15 @@
         op.inner_outputs,
         replace={u: v for u, v in zip(op.inner_inputs, marginalized_rvs_node.inputs)},
     )
     marginalized_rv = inner_rvs[0]
 
     # Obtain the joint_logp graph of the inner RV graph
     inner_rvs_to_values = {rv: rv.clone() for rv in inner_rvs}
-    logps_dict = factorized_joint_logprob(rv_values=inner_rvs_to_values, **kwargs)
+    logps_dict = conditional_logp(rv_values=inner_rvs_to_values, **kwargs)
 
     # Reduce logp dimensions corresponding to broadcasted variables
     joint_logp = logps_dict[inner_rvs_to_values[marginalized_rv]]
     for inner_rv, inner_value in inner_rvs_to_values.items():
         if inner_rv is marginalized_rv:
             continue
         vbcast = inner_value.type.broadcastable
```

### Comparing `pymc-experimental-0.0.6/pymc_experimental/model_builder.py` & `pymc-experimental-0.0.7/pymc_experimental/model_builder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/model_transform/basic.py` & `pymc-experimental-0.0.7/pymc_experimental/model_transform/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/model_transform/conditioning.py` & `pymc-experimental-0.0.7/pymc_experimental/model_transform/conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/preprocessing/standard_scaler.py` & `pymc-experimental-0.0.7/pymc_experimental/preprocessing/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/__init__.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/__init__.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_continuous.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete_markov_chain.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete_markov_chain.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_multivariate.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_basic.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_conditioning.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_histogram_approximation.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_histogram_approximation.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_linearmodel.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_linearmodel.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_marginal_model.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_model_builder.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_model_builder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_pathfinder.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_pivoted_cholesky.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_prior_from_trace.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_prior_from_trace.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/test_splines.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/tests/utils/test_model_fgraph.py` & `pymc-experimental-0.0.7/pymc_experimental/tests/utils/test_model_fgraph.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/utils/__init__.py` & `pymc-experimental-0.0.7/pymc_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/utils/linear_cg.py` & `pymc-experimental-0.0.7/pymc_experimental/utils/linear_cg.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/utils/model_fgraph.py` & `pymc-experimental-0.0.7/pymc_experimental/utils/model_fgraph.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/utils/pivoted_cholesky.py` & `pymc-experimental-0.0.7/pymc_experimental/utils/pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/utils/prior.py` & `pymc-experimental-0.0.7/pymc_experimental/utils/prior.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/utils/pytensorf.py` & `pymc-experimental-0.0.7/pymc_experimental/utils/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental/utils/spline.py` & `pymc-experimental-0.0.7/pymc_experimental/utils/spline.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/pymc_experimental.egg-info/PKG-INFO` & `pymc-experimental-0.0.7/pymc_experimental.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.6
+Version: 0.0.7
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.6 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.7 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.6/pymc_experimental.egg-info/SOURCES.txt` & `pymc-experimental-0.0.7/pymc_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.6/setup.py` & `pymc-experimental-0.0.7/setup.py`

 * *Files identical despite different names*

