# Comparing `tmp/pyhard-2.1.5.tar.gz` & `tmp/pyhard-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhard-2.1.5.tar", last modified: Sat Apr 29 17:11:45 2023, max compression
+gzip compressed data, was "pyhard-2.1.6.tar", last modified: Sat Jun 10 14:23:10 2023, max compression
```

## Comparing `pyhard-2.1.5.tar` & `pyhard-2.1.6.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.456764 pyhard-2.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-29 17:11:33.000000 pyhard-2.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9423 2023-04-29 17:11:45.456764 pyhard-2.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8692 2023-04-29 17:11:33.000000 pyhard-2.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.417760 pyhard-2.1.5/pyhard/
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    37751 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/app.py
--rw-rw-rw-   0 root         (0) root         (0)    19119 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/base.py
--rw-rw-rw-   0 root         (0) root         (0)    12128 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/classification.py
--rw-rw-rw-   0 root         (0) root         (0)    20574 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.419760 pyhard-2.1.5/pyhard/conf/
--rw-rw-rw-   0 root         (0) root         (0)     5199 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/conf/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    12210 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.409759 pyhard-2.1.5/pyhard/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.422761 pyhard-2.1.5/pyhard/data/2normals/
--rw-rw-rw-   0 root         (0) root         (0)    39390 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39209 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   242683 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   168248 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   328455 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.424761 pyhard-2.1.5/pyhard/data/2normalsSd030/
--rw-rw-rw-   0 root         (0) root         (0)    39624 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    38990 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   130100 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)    94130 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   284473 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.426761 pyhard-2.1.5/pyhard/data/2normalsSd045/
--rw-rw-rw-   0 root         (0) root         (0)    39780 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39157 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   178828 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   131886 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   318453 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.429761 pyhard-2.1.5/pyhard/data/circle/
--rw-rw-rw-   0 root         (0) root         (0)    39346 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40231 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   226405 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   145447 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   320526 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.431762 pyhard-2.1.5/pyhard/data/easy/
--rw-rw-rw-   0 root         (0) root         (0)    40190 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40952 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   147238 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)    54473 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/feature_raw_color.csv
--rw-rw-rw-   0 root         (0) root         (0)   282881 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.433762 pyhard-2.1.5/pyhard/data/easy2/
--rw-rw-rw-   0 root         (0) root         (0)    39957 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40817 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   285261 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/projection_matrix.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.434762 pyhard-2.1.5/pyhard/data/iris/
--rw-rw-rw-   0 root         (0) root         (0)     5787 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/iris/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)     3877 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/iris/data.csv
--rw-rw-rw-   0 root         (0) root         (0)    42802 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/iris/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.436762 pyhard-2.1.5/pyhard/data/mix/
--rw-rw-rw-   0 root         (0) root         (0)    39716 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40903 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   193499 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   144369 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   296920 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.438762 pyhard-2.1.5/pyhard/data/overlap/
--rw-rw-rw-   0 root         (0) root         (0)    39233 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/overlap/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39752 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/overlap/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   321095 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/overlap/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.440762 pyhard-2.1.5/pyhard/data/separate/
--rw-rw-rw-   0 root         (0) root         (0)    39995 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    42167 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   177556 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   113525 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   287283 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.453764 pyhard-2.1.5/pyhard/data/wine/
--rw-rw-rw-   0 root         (0) root         (0)    29361 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/algorithm_bin.csv
--rw-rw-rw-   0 root         (0) root         (0)   226327 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/algorithm_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   218520 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/algorithm_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)    10101 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/beta_easy.csv
--rw-rw-rw-   0 root         (0) root         (0)    69563 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)   100951 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   163688 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   163380 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_bagging_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_bagging_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_gradient_boosting_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_gradient_boosting_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_instance_easiness_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_logistic_regression_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1696 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_logistic_regression_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_mlp_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_mlp_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_performance.csv
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_linear_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_linear_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_rbf_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_rbf_good.csv
--rw-rw-rw-   0 root         (0) root         (0)    10103 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/good_algos.csv
--rw-rw-rw-   0 root         (0) root         (0)    37458 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/ih.csv
--rw-rw-rw-   0 root         (0) root         (0)   317680 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)   522841 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/metadata_full.csv
--rw-rw-rw-   0 root         (0) root         (0)    10105 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/portfolio.csv
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/projection_matrix.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.454764 pyhard-2.1.5/pyhard/data/xor/
--rw-rw-rw-   0 root         (0) root         (0)    40143 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40214 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   272866 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/projection_matrix.csv
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/feature_selection.py
--rw-rw-rw-   0 root         (0) root         (0)    10144 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/hpo.py
--rw-rw-rw-   0 root         (0) root         (0)    10847 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/integrator.py
--rw-rw-rw-   0 root         (0) root         (0)    43069 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/measures.py
--rw-rw-rw-   0 root         (0) root         (0)     3787 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.455764 pyhard-2.1.5/pyhard/midia/
--rw-rw-rw-   0 root         (0) root         (0)   157445 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/midia/blobs.svg
--rw-rw-rw-   0 root         (0) root         (0)    11042 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.456764 pyhard-2.1.5/pyhard/thirdparty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10787 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/entropy_estimators.py
--rw-rw-rw-   0 root         (0) root         (0)     4948 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/rank_aggregation.py
--rw-rw-rw-   0 root         (0) root         (0)    21966 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/skfeature.py
--rw-rw-rw-   0 root         (0) root         (0)     5221 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/validator.py
--rw-rw-rw-   0 root         (0) root         (0)    38600 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.419760 pyhard-2.1.5/pyhard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9423 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3654 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      338 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-29 17:11:45.457764 pyhard-2.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-04-29 17:11:33.000000 pyhard-2.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.619742 pyhard-2.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-10 14:23:02.000000 pyhard-2.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9423 2023-06-10 14:23:10.619742 pyhard-2.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8692 2023-06-10 14:23:02.000000 pyhard-2.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.597741 pyhard-2.1.6/pyhard/
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37751 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    19119 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12128 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)    20574 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.598742 pyhard-2.1.6/pyhard/conf/
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/conf/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    12210 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.594741 pyhard-2.1.6/pyhard/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.599742 pyhard-2.1.6/pyhard/data/2normals/
+-rw-rw-rw-   0 root         (0) root         (0)    39390 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    39209 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   242683 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   168248 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   328455 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.601742 pyhard-2.1.6/pyhard/data/2normalsSd030/
+-rw-rw-rw-   0 root         (0) root         (0)    39624 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    38990 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   130100 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)    94130 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   284473 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.602742 pyhard-2.1.6/pyhard/data/2normalsSd045/
+-rw-rw-rw-   0 root         (0) root         (0)    39780 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    39157 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   178828 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   131886 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   318453 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.604742 pyhard-2.1.6/pyhard/data/circle/
+-rw-rw-rw-   0 root         (0) root         (0)    39346 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40231 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   226405 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   145447 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   320526 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.605742 pyhard-2.1.6/pyhard/data/easy/
+-rw-rw-rw-   0 root         (0) root         (0)    40190 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40952 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   147238 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)    54473 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/feature_raw_color.csv
+-rw-rw-rw-   0 root         (0) root         (0)   282881 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.606742 pyhard-2.1.6/pyhard/data/easy2/
+-rw-rw-rw-   0 root         (0) root         (0)    39957 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40817 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   285261 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/metadata.csv
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/projection_matrix.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.607742 pyhard-2.1.6/pyhard/data/iris/
+-rw-rw-rw-   0 root         (0) root         (0)     5787 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/iris/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3877 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/iris/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)    42802 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/iris/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.608742 pyhard-2.1.6/pyhard/data/mix/
+-rw-rw-rw-   0 root         (0) root         (0)    39716 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40903 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   193499 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   144369 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   296920 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.609742 pyhard-2.1.6/pyhard/data/overlap/
+-rw-rw-rw-   0 root         (0) root         (0)    39233 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/overlap/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    39752 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/overlap/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   321095 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/overlap/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.610742 pyhard-2.1.6/pyhard/data/separate/
+-rw-rw-rw-   0 root         (0) root         (0)    39995 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    42167 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   177556 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   113525 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   287283 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.617742 pyhard-2.1.6/pyhard/data/wine/
+-rw-rw-rw-   0 root         (0) root         (0)    29361 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/algorithm_bin.csv
+-rw-rw-rw-   0 root         (0) root         (0)   226327 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/algorithm_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   218520 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/algorithm_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)    10101 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/beta_easy.csv
+-rw-rw-rw-   0 root         (0) root         (0)    69563 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)   100951 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   163688 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   163380 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_bagging_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_bagging_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_gradient_boosting_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_gradient_boosting_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_instance_easiness_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_logistic_regression_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_logistic_regression_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_mlp_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_mlp_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_performance.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_linear_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_linear_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_rbf_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_rbf_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)    10103 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/good_algos.csv
+-rw-rw-rw-   0 root         (0) root         (0)    37458 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/ih.csv
+-rw-rw-rw-   0 root         (0) root         (0)   317680 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/metadata.csv
+-rw-rw-rw-   0 root         (0) root         (0)   522841 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/metadata_full.csv
+-rw-rw-rw-   0 root         (0) root         (0)    10105 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/portfolio.csv
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/projection_matrix.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.618742 pyhard-2.1.6/pyhard/data/xor/
+-rw-rw-rw-   0 root         (0) root         (0)    40143 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40214 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   272866 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/metadata.csv
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/projection_matrix.csv
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/feature_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    10144 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/hpo.py
+-rw-rw-rw-   0 root         (0) root         (0)    10847 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/integrator.py
+-rw-rw-rw-   0 root         (0) root         (0)    43027 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/measures.py
+-rw-rw-rw-   0 root         (0) root         (0)     3787 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.618742 pyhard-2.1.6/pyhard/midia/
+-rw-rw-rw-   0 root         (0) root         (0)   157445 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/midia/blobs.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11042 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.618742 pyhard-2.1.6/pyhard/thirdparty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10787 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/entropy_estimators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4948 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/rank_aggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)    21966 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/skfeature.py
+-rw-rw-rw-   0 root         (0) root         (0)     5221 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2359 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    38600 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.598742 pyhard-2.1.6/pyhard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9423 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-10 14:23:10.619742 pyhard-2.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2023-06-10 14:23:02.000000 pyhard-2.1.6/setup.py
```

### Comparing `pyhard-2.1.5/LICENSE` & `pyhard-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/PKG-INFO` & `pyhard-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyhard
-Version: 2.1.5
+Version: 2.1.6
 Summary: Analyze, explore and visualize instance hardness within datasets
 Home-page: https://gitlab.com/ita-ml/pyhard
-Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.5/pyhard-v2.1.5.tar.gz
+Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.6/pyhard-v2.1.6.tar.gz
 Author: Pedro Paiva
 Author-email: paiva@ita.br
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyhard-2.1.5/README.md` & `pyhard-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/__init__.py` & `pyhard-2.1.6/pyhard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from pathlib import Path
 from typing import Union
 
 
-__version__ = "2.1.5"
+__version__ = "2.1.6"
 
 
 def get_seed() -> Union[int, None]:
     seed = os.environ.get("PYHARD_SEED")
     if seed is None:
         return seed
     else:
```

### Comparing `pyhard-2.1.5/pyhard/app.py` & `pyhard-2.1.6/pyhard/app.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/base.py` & `pyhard-2.1.6/pyhard/base.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/classification.py` & `pyhard-2.1.6/pyhard/classification.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/cli.py` & `pyhard-2.1.6/pyhard/cli.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/conf/config.yaml` & `pyhard-2.1.6/pyhard/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/context.py` & `pyhard-2.1.6/pyhard/context.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normals/coordinates.csv` & `pyhard-2.1.6/pyhard/data/2normals/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normals/data.csv` & `pyhard-2.1.6/pyhard/data/2normals/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normals/feature_process.csv` & `pyhard-2.1.6/pyhard/data/2normals/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normals/feature_raw.csv` & `pyhard-2.1.6/pyhard/data/2normals/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normals/metadata.csv` & `pyhard-2.1.6/pyhard/data/2normals/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd030/coordinates.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd030/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd030/data.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd030/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd030/feature_process.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd030/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd030/feature_raw.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd030/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd030/metadata.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd030/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd045/coordinates.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd045/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd045/data.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd045/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd045/feature_process.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd045/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd045/feature_raw.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd045/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/2normalsSd045/metadata.csv` & `pyhard-2.1.6/pyhard/data/2normalsSd045/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/circle/coordinates.csv` & `pyhard-2.1.6/pyhard/data/circle/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/circle/data.csv` & `pyhard-2.1.6/pyhard/data/circle/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/circle/feature_process.csv` & `pyhard-2.1.6/pyhard/data/circle/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/circle/feature_raw.csv` & `pyhard-2.1.6/pyhard/data/circle/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/circle/metadata.csv` & `pyhard-2.1.6/pyhard/data/circle/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy/coordinates.csv` & `pyhard-2.1.6/pyhard/data/easy/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy/data.csv` & `pyhard-2.1.6/pyhard/data/easy/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy/feature_process.csv` & `pyhard-2.1.6/pyhard/data/easy/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy/feature_raw_color.csv` & `pyhard-2.1.6/pyhard/data/easy/feature_raw_color.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy/metadata.csv` & `pyhard-2.1.6/pyhard/data/easy/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy2/coordinates.csv` & `pyhard-2.1.6/pyhard/data/easy2/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy2/data.csv` & `pyhard-2.1.6/pyhard/data/easy2/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/easy2/metadata.csv` & `pyhard-2.1.6/pyhard/data/easy2/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/iris/coordinates.csv` & `pyhard-2.1.6/pyhard/data/iris/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/iris/data.csv` & `pyhard-2.1.6/pyhard/data/iris/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/iris/metadata.csv` & `pyhard-2.1.6/pyhard/data/iris/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/mix/coordinates.csv` & `pyhard-2.1.6/pyhard/data/mix/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/mix/data.csv` & `pyhard-2.1.6/pyhard/data/mix/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/mix/feature_process.csv` & `pyhard-2.1.6/pyhard/data/mix/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/mix/feature_raw.csv` & `pyhard-2.1.6/pyhard/data/mix/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/mix/metadata.csv` & `pyhard-2.1.6/pyhard/data/mix/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/overlap/coordinates.csv` & `pyhard-2.1.6/pyhard/data/overlap/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/overlap/data.csv` & `pyhard-2.1.6/pyhard/data/overlap/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/overlap/metadata.csv` & `pyhard-2.1.6/pyhard/data/overlap/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/separate/coordinates.csv` & `pyhard-2.1.6/pyhard/data/separate/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/separate/data.csv` & `pyhard-2.1.6/pyhard/data/separate/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/separate/feature_process.csv` & `pyhard-2.1.6/pyhard/data/separate/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/separate/feature_raw.csv` & `pyhard-2.1.6/pyhard/data/separate/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/separate/metadata.csv` & `pyhard-2.1.6/pyhard/data/separate/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/algorithm_bin.csv` & `pyhard-2.1.6/pyhard/data/wine/algorithm_bin.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/algorithm_process.csv` & `pyhard-2.1.6/pyhard/data/wine/algorithm_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/algorithm_raw.csv` & `pyhard-2.1.6/pyhard/data/wine/algorithm_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/beta_easy.csv` & `pyhard-2.1.6/pyhard/data/wine/beta_easy.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/coordinates.csv` & `pyhard-2.1.6/pyhard/data/wine/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/data.csv` & `pyhard-2.1.6/pyhard/data/wine/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/feature_process.csv` & `pyhard-2.1.6/pyhard/data/wine/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/feature_raw.csv` & `pyhard-2.1.6/pyhard/data/wine/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_bagging_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_bagging_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_gradient_boosting_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_gradient_boosting_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_instance_easiness_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_instance_easiness_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_logistic_regression_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_logistic_regression_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_mlp_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_mlp_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_performance.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_performance.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_best.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_best.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_svc_linear_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_svc_linear_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/footprint_svc_rbf_good.csv` & `pyhard-2.1.6/pyhard/data/wine/footprint_svc_rbf_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/good_algos.csv` & `pyhard-2.1.6/pyhard/data/wine/good_algos.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/ih.csv` & `pyhard-2.1.6/pyhard/data/wine/ih.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/metadata.csv` & `pyhard-2.1.6/pyhard/data/wine/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/metadata_full.csv` & `pyhard-2.1.6/pyhard/data/wine/metadata_full.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/wine/portfolio.csv` & `pyhard-2.1.6/pyhard/data/wine/portfolio.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/xor/coordinates.csv` & `pyhard-2.1.6/pyhard/data/xor/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/xor/data.csv` & `pyhard-2.1.6/pyhard/data/xor/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/data/xor/metadata.csv` & `pyhard-2.1.6/pyhard/data/xor/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/feature_selection.py` & `pyhard-2.1.6/pyhard/feature_selection.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/hpo.py` & `pyhard-2.1.6/pyhard/hpo.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/integrator.py` & `pyhard-2.1.6/pyhard/integrator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/measures.py` & `pyhard-2.1.6/pyhard/measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,15 +537,15 @@
             nbrs = NearestNeighbors(n_neighbors=len(self.y), algorithm='auto', metric=distance).fit(self.X)
             distances, indices = nbrs.kneighbors(self.X)
 
         LSC = np.zeros(y.values.shape)
         n_class = y.value_counts()
         for i, label in y.items():
             nn = y.loc[indices[i, :]].values
-            LSC[i] = (np.argmax(nn != label) - 1) / (n_class[label] - 1)
+            LSC[i] = np.argmax(nn != label) / n_class[label]
         return 1 - LSC
 
     def ls_radius(self, distance='gower') -> np.ndarray:
         r"""
         Local Set Radius (LSR) takes the normalized radius of the local set of :math:`\mathbf x_i`:
 
         .. math::
@@ -655,16 +655,16 @@
     def f1(self) -> np.ndarray:
         r"""
         Fraction of features in overlapping areas (F1) takes the percentage of features of the instance
         :math:`\mathbf x_i` whose values lie in an overlapping region of the classes as:
 
         .. math::
 
-            F_1(\mathbf x_i) = \frac{\sum_{j=1}^{m_D}{I(x_{ij} > \textnormal{max_min} (\mathbf f_j)
-            \wedge x_{ij} < \textnormal{min_max} (\mathbf f_j))}}{m_D},
+            F_1(\mathbf x_i) = \frac{\sum_{j=1}^{m_D}{I(x_{ij} \geq \textnormal{max_min} (\mathbf f_j)
+            \wedge x_{ij} \leq \textnormal{min_max} (\mathbf f_j))}}{m_D},
 
         where :math:`I` is the indicator function, which returns 1 if its argument is true and 0 otherwise,
         :math:`\mathbf f_j` is the :math:`j`-th feature vector in :math:`D` and:
 
         .. math::
 
             \textnormal{min_max}(\mathbf f_j) = \min(\max(\mathbf f_j^{c_1}),\max(\mathbf f_j^{c_2}))
@@ -692,19 +692,18 @@
         F1 = pd.Series(0, index=df.index)
         for p in itertools.combinations(classes, 2):
             sub_df = df[(self.y == p[0]) | (self.y == p[1])]
             indicator = pd.Series(0, index=sub_df.index)
             for f in features:
                 m1 = maxmin(sub_df[f].values, sub_df[self.target_col].values)
                 m2 = minmax(sub_df[f].values, sub_df[self.target_col].values)
-                indicator += sub_df[f].between(m1, m2, inclusive='neither') * 1
+                indicator += sub_df[f].between(m1, m2, inclusive='both') * 1
             F1 = F1.add(indicator.divide(n_features), fill_value=0)
 
         F1 = F1.divide(len(classes) - 1)
-        # assert F1.max() <= 1.0
         return F1.values
 
     def do_t(self):
         df = self.data.copy()
         features = self.X.columns.to_list()
         classes = self.y.unique().tolist()
```

### Comparing `pyhard-2.1.5/pyhard/metrics.py` & `pyhard-2.1.6/pyhard/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/midia/blobs.svg` & `pyhard-2.1.6/pyhard/midia/blobs.svg`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/regression.py` & `pyhard-2.1.6/pyhard/regression.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/structures.py` & `pyhard-2.1.6/pyhard/structures.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/thirdparty/entropy_estimators.py` & `pyhard-2.1.6/pyhard/thirdparty/entropy_estimators.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/thirdparty/rank_aggregation.py` & `pyhard-2.1.6/pyhard/thirdparty/rank_aggregation.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/thirdparty/skfeature.py` & `pyhard-2.1.6/pyhard/thirdparty/skfeature.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/utils.py` & `pyhard-2.1.6/pyhard/utils.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/validator.py` & `pyhard-2.1.6/pyhard/validator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard/visualization.py` & `pyhard-2.1.6/pyhard/visualization.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/pyhard.egg-info/PKG-INFO` & `pyhard-2.1.6/pyhard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyhard
-Version: 2.1.5
+Version: 2.1.6
 Summary: Analyze, explore and visualize instance hardness within datasets
 Home-page: https://gitlab.com/ita-ml/pyhard
-Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.5/pyhard-v2.1.5.tar.gz
+Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.6/pyhard-v2.1.6.tar.gz
 Author: Pedro Paiva
 Author-email: paiva@ita.br
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyhard-2.1.5/pyhard.egg-info/SOURCES.txt` & `pyhard-2.1.6/pyhard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.5/setup.py` & `pyhard-2.1.6/setup.py`

 * *Files identical despite different names*

