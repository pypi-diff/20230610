# Comparing `tmp/dynamo-release-1.3.0.tar.gz` & `tmp/dynamo-release-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynamo-release-1.3.0.tar", last modified: Tue May 30 20:03:33 2023, max compression
+gzip compressed data, was "dist/dynamo-release-1.3.2.tar", last modified: Fri Jun  9 22:23:32 2023, max compression
```

## Comparing `dynamo-release-1.3.0.tar` & `dynamo-release-1.3.2.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6767 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      748 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32578 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11861 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/data_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34268 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/docrep.py
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/dynamo_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/est.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/estimation/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/estimation/csc/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/csc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26002 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/csc/utils_velocity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    88165 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/csc/velocity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/fit_jacobian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/estimation/tsc/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/tsc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33692 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/tsc/estimation_kinetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/tsc/twostep.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21537 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/tsc/utils_kinetic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8945 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/estimation/tsc/utils_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/external/
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/external/gseapy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/external/hodge.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/external/scifate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/external/scribe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/external/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6440 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/movie/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/movie/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17146 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/movie/fate.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/movie/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/mv.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/pd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/pl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/plot/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3387 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/cell_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/clustering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25248 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/dimension_reduction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   126140 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17396 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/ezplots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6928 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/fate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/fate_utilities_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    68251 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/heatmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/least_action_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23916 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/networks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42698 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/preprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2389 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/pseudotime.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5100 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/scPotential.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    77144 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/scVectorField.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45133 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/scatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/sctransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/space.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15705 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/state_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/streamtube.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/theme.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47637 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/time_series.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    60256 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/topography.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56243 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/utils_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/utils_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    51879 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/plot/vector_calculus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/pp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/prediction/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31622 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/fate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/least_action_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    18467 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/perturbation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19549 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/state_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/trajectory_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/tscRNA_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/prediction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/CnmfPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    36583 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/Preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/QC.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2144 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/cell_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    79367 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/dynast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/preprocessing/external/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/external/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    25574 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/external/pearson_residual_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/external/sctransform.py
--rw-r--r--   0 runner    (1001) docker     (123)    35475 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/gene_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/transform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36269 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/preprocessing/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8736 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/sample_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       71 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/simulation/
--rwxr-xr-x   0 runner    (1001) docker     (123)    21399 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/simulation/Gillespie.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18272 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/simulation/ODE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/simulation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14934 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/simulation/bif_os_inclusive_sim.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/simulation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33644 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/simulation/simulate_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/simulation/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7504 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/DDRTree_py.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34759 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/Markov.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2538 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13110 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/_dynamics_deprecated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46051 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/cell_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)    31842 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/clustering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30327 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6973 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/construct_velocity_tree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12409 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/dimension_reduction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    83861 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/dynamics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/dynamo_bk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4049 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/dynamo_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    30473 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/graph_calculus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/graph_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/growth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36505 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/markers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20934 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/metric_velocity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55606 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/moments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1566 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/multiomics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3642 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/pseudotime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/pseudotime_velocity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7636 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/psl_py.py
--rw-r--r--   0 runner    (1001) docker     (123)    41332 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/sampling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/time_series.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   104052 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/utils_markers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17828 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/utils_moments_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/utils_reduceDimension.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18907 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/tools/velocyto_scvelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo/vectorfield/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5135 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/Ao.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17110 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/Bhattacharya.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/FixedPoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6564 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/Wang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/cell_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20086 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/least_action_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/rank_vf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28474 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/scPotential.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57332 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/scVectorField.py
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/stochastic_process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    52760 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/topography.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/util_vector_calculus.py
--rw-r--r--   0 runner    (1001) docker     (123)    54129 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46453 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/vector_calculus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vectorfield/vfGraph_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/dynamo/vf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo_release.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/dynamo_release.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 20:03:33.000000 dynamo-release-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-05-30 20:03:23.000000 dynamo-release-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6767 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      748 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32578 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11861 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/data_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34268 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/docrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/dynamo_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/est.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/estimation/csc/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/csc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26002 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/csc/utils_velocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    88165 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/csc/velocity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/fit_jacobian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/estimation/tsc/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/tsc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33692 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/tsc/estimation_kinetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/tsc/twostep.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21537 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/tsc/utils_kinetic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8945 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/estimation/tsc/utils_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/external/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/external/gseapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/external/hodge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/external/scifate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/external/scribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/external/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6440 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/movie/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/movie/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17146 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/movie/fate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/movie/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/pd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/pl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/plot/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3387 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/cell_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/clustering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25248 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/dimension_reduction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   126140 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17396 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/ezplots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6928 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/fate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/fate_utilities_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68251 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/least_action_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23916 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/networks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42698 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/preprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2389 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/pseudotime.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5100 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/scPotential.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77144 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/scVectorField.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45133 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/scatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/sctransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15705 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/state_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/streamtube.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/theme.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47637 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/time_series.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60266 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/topography.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56243 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/utils_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/utils_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51879 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/plot/vector_calculus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/pp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/prediction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31622 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/fate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/least_action_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18467 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/perturbation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19549 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/state_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/trajectory_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/tscRNA_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/prediction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/CnmfPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36583 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/Preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/QC.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2144 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/cell_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79367 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/dynast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/preprocessing/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/external/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25574 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/external/pearson_residual_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/external/sctransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35475 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/gene_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36269 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/preprocessing/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8736 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/sample_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       71 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/simulation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21399 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/simulation/Gillespie.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18272 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/simulation/ODE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/simulation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14934 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/simulation/bif_os_inclusive_sim.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/simulation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33644 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/simulation/simulate_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/simulation/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7504 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/DDRTree_py.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34759 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/Markov.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2538 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13110 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/_dynamics_deprecated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46051 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/cell_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31842 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/clustering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30327 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6973 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/construct_velocity_tree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12409 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/dimension_reduction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    83861 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/dynamics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/dynamo_bk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4049 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/dynamo_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30473 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/graph_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/graph_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/growth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36505 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/markers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20934 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/metric_velocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55606 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/moments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1566 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/multiomics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3642 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/pseudotime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/pseudotime_velocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7636 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/psl_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41332 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/sampling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/time_series.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104052 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/utils_markers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17828 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/utils_moments_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/utils_reduceDimension.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18907 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/tools/velocyto_scvelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo/vectorfield/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5135 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/Ao.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17110 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/Bhattacharya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/FixedPoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6564 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/Wang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/cell_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20086 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/least_action_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/rank_vf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28474 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/scPotential.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57332 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/scVectorField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/stochastic_process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52839 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/topography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/util_vector_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54129 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46453 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/vector_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vectorfield/vfGraph_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/dynamo/vf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-09 22:23:31.000000 dynamo-release-1.3.2/dynamo_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/dynamo_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:23:31.000000 dynamo-release-1.3.2/dynamo_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-09 22:23:31.000000 dynamo-release-1.3.2/dynamo_release.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 22:23:31.000000 dynamo-release-1.3.2/dynamo_release.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-09 22:23:32.000000 dynamo-release-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-06-09 22:23:21.000000 dynamo-release-1.3.2/setup.py
```

### Comparing `dynamo-release-1.3.0/PKG-INFO` & `dynamo-release-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamo-release
-Version: 1.3.0
+Version: 1.3.2
 Summary: Mapping Vector Field of Single Cells
 Home-page: https://github.com/aristoteleo/dynamo-release
 Author: Xiaojie Qiu, Yan Zhang, Ke Ni
 Author-email: xqiu.sc@gmail.com
 License: BSD
 Download-URL: https://github.com/aristoteleo/dynamo-release
 Description: <p align="center">
```

### Comparing `dynamo-release-1.3.0/README.md` & `dynamo-release-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/__init__.py` & `dynamo-release-1.3.2/dynamo/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/configuration.py` & `dynamo-release-1.3.2/dynamo/configuration.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/data_io.py` & `dynamo-release-1.3.2/dynamo/data_io.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/docrep.py` & `dynamo-release-1.3.2/dynamo/docrep.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/dynamo_logger.py` & `dynamo-release-1.3.2/dynamo/dynamo_logger.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/csc/utils_velocity.py` & `dynamo-release-1.3.2/dynamo/estimation/csc/utils_velocity.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/csc/velocity.py` & `dynamo-release-1.3.2/dynamo/estimation/csc/velocity.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/fit_jacobian.py` & `dynamo-release-1.3.2/dynamo/estimation/fit_jacobian.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/tsc/__init__.py` & `dynamo-release-1.3.2/dynamo/estimation/tsc/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/tsc/estimation_kinetic.py` & `dynamo-release-1.3.2/dynamo/estimation/tsc/estimation_kinetic.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/tsc/twostep.py` & `dynamo-release-1.3.2/dynamo/estimation/tsc/twostep.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/tsc/utils_kinetic.py` & `dynamo-release-1.3.2/dynamo/estimation/tsc/utils_kinetic.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/estimation/tsc/utils_moments.py` & `dynamo-release-1.3.2/dynamo/estimation/tsc/utils_moments.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/external/gseapy.py` & `dynamo-release-1.3.2/dynamo/external/gseapy.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/external/hodge.py` & `dynamo-release-1.3.2/dynamo/external/hodge.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/external/scifate.py` & `dynamo-release-1.3.2/dynamo/external/scifate.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/external/scribe.py` & `dynamo-release-1.3.2/dynamo/external/scribe.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/external/utils.py` & `dynamo-release-1.3.2/dynamo/external/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/get_version.py` & `dynamo-release-1.3.2/dynamo/get_version.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/movie/fate.py` & `dynamo-release-1.3.2/dynamo/movie/fate.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/__init__.py` & `dynamo-release-1.3.2/dynamo/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/cell_cycle.py` & `dynamo-release-1.3.2/dynamo/plot/cell_cycle.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/clustering.py` & `dynamo-release-1.3.2/dynamo/plot/clustering.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/connectivity.py` & `dynamo-release-1.3.2/dynamo/plot/connectivity.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/dimension_reduction.py` & `dynamo-release-1.3.2/dynamo/plot/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/dynamics.py` & `dynamo-release-1.3.2/dynamo/plot/dynamics.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/ezplots.py` & `dynamo-release-1.3.2/dynamo/plot/ezplots.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/fate.py` & `dynamo-release-1.3.2/dynamo/plot/fate.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/heatmaps.py` & `dynamo-release-1.3.2/dynamo/plot/heatmaps.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/least_action_path.py` & `dynamo-release-1.3.2/dynamo/plot/least_action_path.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/markers.py` & `dynamo-release-1.3.2/dynamo/plot/markers.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/networks.py` & `dynamo-release-1.3.2/dynamo/plot/networks.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/preprocess.py` & `dynamo-release-1.3.2/dynamo/plot/preprocess.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/pseudotime.py` & `dynamo-release-1.3.2/dynamo/plot/pseudotime.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/scPotential.py` & `dynamo-release-1.3.2/dynamo/plot/scPotential.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/scVectorField.py` & `dynamo-release-1.3.2/dynamo/plot/scVectorField.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/scatters.py` & `dynamo-release-1.3.2/dynamo/plot/scatters.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/sctransform.py` & `dynamo-release-1.3.2/dynamo/plot/sctransform.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/space.py` & `dynamo-release-1.3.2/dynamo/plot/space.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/state_graph.py` & `dynamo-release-1.3.2/dynamo/plot/state_graph.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/streamtube.py` & `dynamo-release-1.3.2/dynamo/plot/streamtube.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/theme.py` & `dynamo-release-1.3.2/dynamo/plot/theme.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/time_series.py` & `dynamo-release-1.3.2/dynamo/plot/time_series.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/topography.py` & `dynamo-release-1.3.2/dynamo/plot/topography.py`

 * *Files 0% similar despite different names*

```diff
@@ -1065,15 +1065,15 @@
             warnings.simplefilter("ignore")
 
             if basis == fps_basis:
                 logger.info(
                     f"`basis` and `fps_basis` are all {basis}. Will also map topography ...",
                     indent_level=2,
                 )
-                VectorField(adata, basis, map_topography=True)
+                VectorField(adata, basis, map_topography=True, n=n)
             else:
                 VectorField(adata, basis)
     if fps_uns_key not in adata.uns.keys():
         if "velocity_" + basis not in adata.obsm_keys():
             logger.info(
                 f"velocity_{basis} is computed yet. " f"Projecting the velocity vector to {basis} basis now ...",
                 indent_level=1,
@@ -1121,15 +1121,15 @@
         # if topology is not mapped for this basis, calculate it now.
         logger.info(
             f"Vector field for {fps_basis} is but its topography is not mapped. " f"Mapping topography now ...",
             indent_level=1,
         )
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            _topology(adata, fps_basis, VecFld=None)
+            _topology(adata, fps_basis, VecFld=None, n=n)
     else:
         if fps_vecfld_dict["Xss"].size > 0 and fps_vecfld_dict["Xss"].shape[1] > 2:
             fps_vecfld_dict["X_basis"], fps_vecfld_dict["Xss"] = (
                 vecfld_dict["X"][:, :2],
                 vecfld_dict["X"][fps_vecfld_dict["fp_ind"], :2],
             )
```

### Comparing `dynamo-release-1.3.0/dynamo/plot/utils.py` & `dynamo-release-1.3.2/dynamo/plot/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/utils_dynamics.py` & `dynamo-release-1.3.2/dynamo/plot/utils_dynamics.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/utils_graph.py` & `dynamo-release-1.3.2/dynamo/plot/utils_graph.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/plot/vector_calculus.py` & `dynamo-release-1.3.2/dynamo/plot/vector_calculus.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/__init__.py` & `dynamo-release-1.3.2/dynamo/prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/fate.py` & `dynamo-release-1.3.2/dynamo/prediction/fate.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/least_action_path.py` & `dynamo-release-1.3.2/dynamo/prediction/least_action_path.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/perturbation.py` & `dynamo-release-1.3.2/dynamo/prediction/perturbation.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/state_graph.py` & `dynamo-release-1.3.2/dynamo/prediction/state_graph.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/trajectory.py` & `dynamo-release-1.3.2/dynamo/prediction/trajectory.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/trajectory_analysis.py` & `dynamo-release-1.3.2/dynamo/prediction/trajectory_analysis.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/tscRNA_seq.py` & `dynamo-release-1.3.2/dynamo/prediction/tscRNA_seq.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/prediction/utils.py` & `dynamo-release-1.3.2/dynamo/prediction/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/CnmfPreprocessor.py` & `dynamo-release-1.3.2/dynamo/preprocessing/CnmfPreprocessor.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/Preprocessor.py` & `dynamo-release-1.3.2/dynamo/preprocessing/Preprocessor.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/QC.py` & `dynamo-release-1.3.2/dynamo/preprocessing/QC.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/__init__.py` & `dynamo-release-1.3.2/dynamo/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/cell_cycle.py` & `dynamo-release-1.3.2/dynamo/preprocessing/cell_cycle.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/deprecated.py` & `dynamo-release-1.3.2/dynamo/preprocessing/deprecated.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/dynast.py` & `dynamo-release-1.3.2/dynamo/preprocessing/dynast.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/external/integration.py` & `dynamo-release-1.3.2/dynamo/preprocessing/external/integration.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/external/pearson_residual_recipe.py` & `dynamo-release-1.3.2/dynamo/preprocessing/external/pearson_residual_recipe.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/external/sctransform.py` & `dynamo-release-1.3.2/dynamo/preprocessing/external/sctransform.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import numpy as np
 import pandas as pd
 import scipy
 import scipy as sp
 import statsmodels.discrete.discrete_model
 import statsmodels.nonparametric.kernel_regression
 from anndata import AnnData
-from KDEpy import FFTKDE
 from scipy import stats
 
 from ...configuration import DKM
 from ...dynamo_logger import main_info, main_info_insert_adata_layer, main_warning
 from ..utils import get_gene_selection_filter
 
 _EPS = np.finfo(float).eps
@@ -67,14 +66,18 @@
        y: the array of values to test for outliers.
        x: an array of values corresponding to the locations of `y`.
        th: threshold value for outlier detection.
 
     Returns:
        Boolean array indicating whether each value in `y` is an outlier (`True`) or not (`False`).
     """
+    try:
+        from KDEpy import FFTKDE
+    except ImportError:
+        raise ImportError("Please install KDEpy for sctransform.")
     z = FFTKDE(kernel="gaussian", bw="ISJ").fit(x)
     z.evaluate()
     bin_width = (max(x) - min(x)) * z.bw / 2
     eps = _EPS * 10
 
     breaks1 = np.arange(min(x), max(x) + bin_width, bin_width)
     breaks2 = np.arange(min(x) - eps - bin_width / 2, max(x) + bin_width, bin_width)
@@ -211,14 +214,18 @@
 
     Returns:
         If inplace=True, adata is updated with results in layer `layer`.
         If inplace=False, a new AnnData object with results will be returned.
     """
     import multiprocessing
     import sys
+    try:
+        from KDEpy import FFTKDE
+    except ImportError:
+        raise ImportError("Please install KDEpy for sctransform.")
 
     main_info("sctransform adata on layer: %s" % (layer))
     X = DKM.select_layer_data(adata, layer).copy()
     X = sp.sparse.csr_matrix(X)
     X.eliminate_zeros()
     gene_names = np.array(list(adata.var_names))
     cell_names = np.array(list(adata.obs_names))
```

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/gene_selection.py` & `dynamo-release-1.3.2/dynamo/preprocessing/gene_selection.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/normalization.py` & `dynamo-release-1.3.2/dynamo/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/pca.py` & `dynamo-release-1.3.2/dynamo/preprocessing/pca.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/transform.py` & `dynamo-release-1.3.2/dynamo/preprocessing/transform.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/preprocessing/utils.py` & `dynamo-release-1.3.2/dynamo/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/sample_data.py` & `dynamo-release-1.3.2/dynamo/sample_data.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/simulation/Gillespie.py` & `dynamo-release-1.3.2/dynamo/simulation/Gillespie.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/simulation/ODE.py` & `dynamo-release-1.3.2/dynamo/simulation/ODE.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/simulation/__init__.py` & `dynamo-release-1.3.2/dynamo/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/simulation/bif_os_inclusive_sim.py` & `dynamo-release-1.3.2/dynamo/simulation/bif_os_inclusive_sim.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/simulation/evaluation.py` & `dynamo-release-1.3.2/dynamo/simulation/evaluation.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/simulation/simulate_anndata.py` & `dynamo-release-1.3.2/dynamo/simulation/simulate_anndata.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/simulation/utils.py` & `dynamo-release-1.3.2/dynamo/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/DDRTree_py.py` & `dynamo-release-1.3.2/dynamo/tools/DDRTree_py.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/Markov.py` & `dynamo-release-1.3.2/dynamo/tools/Markov.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/__init__.py` & `dynamo-release-1.3.2/dynamo/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/_dynamics_deprecated.py` & `dynamo-release-1.3.2/dynamo/tools/_dynamics_deprecated.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/cell_velocities.py` & `dynamo-release-1.3.2/dynamo/tools/cell_velocities.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/clustering.py` & `dynamo-release-1.3.2/dynamo/tools/clustering.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/connectivity.py` & `dynamo-release-1.3.2/dynamo/tools/connectivity.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/construct_velocity_tree.py` & `dynamo-release-1.3.2/dynamo/tools/construct_velocity_tree.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/dimension_reduction.py` & `dynamo-release-1.3.2/dynamo/tools/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/dynamics.py` & `dynamo-release-1.3.2/dynamo/tools/dynamics.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/dynamo_bk.py` & `dynamo-release-1.3.2/dynamo/tools/dynamo_bk.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/dynamo_fitting.py` & `dynamo-release-1.3.2/dynamo/tools/dynamo_fitting.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/graph_calculus.py` & `dynamo-release-1.3.2/dynamo/tools/graph_calculus.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/graph_operators.py` & `dynamo-release-1.3.2/dynamo/tools/graph_operators.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/growth.py` & `dynamo-release-1.3.2/dynamo/tools/growth.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/markers.py` & `dynamo-release-1.3.2/dynamo/tools/markers.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/metric_velocity.py` & `dynamo-release-1.3.2/dynamo/tools/metric_velocity.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/moments.py` & `dynamo-release-1.3.2/dynamo/tools/moments.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/multiomics.py` & `dynamo-release-1.3.2/dynamo/tools/multiomics.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/pseudotime.py` & `dynamo-release-1.3.2/dynamo/tools/pseudotime.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/pseudotime_velocity.py` & `dynamo-release-1.3.2/dynamo/tools/pseudotime_velocity.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/psl_py.py` & `dynamo-release-1.3.2/dynamo/tools/psl_py.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/recipes.py` & `dynamo-release-1.3.2/dynamo/tools/recipes.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/sampling.py` & `dynamo-release-1.3.2/dynamo/tools/sampling.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/time_series.py` & `dynamo-release-1.3.2/dynamo/tools/time_series.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/utils.py` & `dynamo-release-1.3.2/dynamo/tools/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/utils_markers.py` & `dynamo-release-1.3.2/dynamo/tools/utils_markers.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/utils_moments_deprecated.py` & `dynamo-release-1.3.2/dynamo/tools/utils_moments_deprecated.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/utils_reduceDimension.py` & `dynamo-release-1.3.2/dynamo/tools/utils_reduceDimension.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/tools/velocyto_scvelo.py` & `dynamo-release-1.3.2/dynamo/tools/velocyto_scvelo.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/utils.py` & `dynamo-release-1.3.2/dynamo/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/Ao.py` & `dynamo-release-1.3.2/dynamo/vectorfield/Ao.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/Bhattacharya.py` & `dynamo-release-1.3.2/dynamo/vectorfield/Bhattacharya.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/FixedPoints.py` & `dynamo-release-1.3.2/dynamo/vectorfield/FixedPoints.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/Wang.py` & `dynamo-release-1.3.2/dynamo/vectorfield/Wang.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/__init__.py` & `dynamo-release-1.3.2/dynamo/vectorfield/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/cell_vectors.py` & `dynamo-release-1.3.2/dynamo/vectorfield/cell_vectors.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/clustering.py` & `dynamo-release-1.3.2/dynamo/vectorfield/clustering.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/least_action_path.py` & `dynamo-release-1.3.2/dynamo/vectorfield/least_action_path.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/networks.py` & `dynamo-release-1.3.2/dynamo/vectorfield/networks.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/rank_vf.py` & `dynamo-release-1.3.2/dynamo/vectorfield/rank_vf.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/scPotential.py` & `dynamo-release-1.3.2/dynamo/vectorfield/scPotential.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/scVectorField.py` & `dynamo-release-1.3.2/dynamo/vectorfield/scVectorField.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/stochastic_process.py` & `dynamo-release-1.3.2/dynamo/vectorfield/stochastic_process.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/topography.py` & `dynamo-release-1.3.2/dynamo/vectorfield/topography.py`

 * *Files 0% similar despite different names*

```diff
@@ -792,14 +792,15 @@
     model_buffer_path: Optional[str] = None,
     return_vf_object: bool = False,
     map_topography: bool = False,
     pot_curl_div: bool = False,
     cores: int = 1,
     result_key: Optional[str] = None,
     copy: bool = False,
+    n: int = 25,
     **kwargs,
 ) -> Union[anndata.AnnData, BaseVectorField]:
     """Learn a function of high dimensional vector field from sparse single cell samples in the entire space robustly.
 
     Args:
         adata: AnnData object that contains embedding and velocity data
         basis: The embedding data to use. The vector field function will be learned on the low  dimensional embedding and can be then projected
@@ -831,14 +832,15 @@
             divergence is by default only applied to 2D basis. However, divergence is applicable for any dimension while curl is generally only defined for 2/3 D systems.
         cores: Number of cores to run the ddhodge function. If cores is set to be > 1, multiprocessing will be used to
             parallel the ddhodge calculation.
         result_key:
             The key that will be used as prefix for the vector field key in .uns
         copy: Whether to return a new deep copy of `adata` instead of updating `adata` object passed in arguments and
             returning `None`.
+        n: Number of samples for calculating the fixed points.
         kwargs: Other additional parameters passed to the vectorfield class.
 
     Returns:
         If `copy` and `return_vf_object` arguments are set to False, `annData` object is updated with the `VecFld`dictionary in the `uns` attribute.
         If `return_vf_object` is set to True, then a vector field class object is returned.
         If `copy` is set to True, a deep copy of the original `adata` object is returned.
     """
@@ -1157,15 +1159,15 @@
         vf_dict["genes"] = genes
         vf_dict["velocity_key"] = velocity_key
 
         logger.info_insert_adata(vf_key, adata_attr="uns")
         adata.uns[vf_key] = vf_dict
 
     if map_topography:
-        tp_kwargs = {"n": 25}
+        tp_kwargs = {"n": n}
         tp_kwargs = update_dict(tp_kwargs, kwargs)
 
         logger.info("Mapping topography...")
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
 
             adata = topography(
```

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/util_vector_calculus.py` & `dynamo-release-1.3.2/dynamo/vectorfield/util_vector_calculus.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/utils.py` & `dynamo-release-1.3.2/dynamo/vectorfield/utils.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/vector_calculus.py` & `dynamo-release-1.3.2/dynamo/vectorfield/vector_calculus.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo/vectorfield/vfGraph_deprecated.py` & `dynamo-release-1.3.2/dynamo/vectorfield/vfGraph_deprecated.py`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo_release.egg-info/PKG-INFO` & `dynamo-release-1.3.2/dynamo_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamo-release
-Version: 1.3.0
+Version: 1.3.2
 Summary: Mapping Vector Field of Single Cells
 Home-page: https://github.com/aristoteleo/dynamo-release
 Author: Xiaojie Qiu, Yan Zhang, Ke Ni
 Author-email: xqiu.sc@gmail.com
 License: BSD
 Download-URL: https://github.com/aristoteleo/dynamo-release
 Description: <p align="center">
```

### Comparing `dynamo-release-1.3.0/dynamo_release.egg-info/SOURCES.txt` & `dynamo-release-1.3.2/dynamo_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamo-release-1.3.0/dynamo_release.egg-info/requires.txt` & `dynamo-release-1.3.2/dynamo_release.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 numpy>=1.20.0
 pandas>=1.3.5
 scipy>=1.4.1
 scikit-learn>=0.19.1
 anndata>=0.8.0
-KDEpy
 loompy>=3.0.5
 matplotlib>=3.5.3
 setuptools
 numdifftools>=0.9.39
 umap-learn>=0.5.1
 PATSY>=0.5.1
 statsmodels>=0.9.0
 numba>=0.54.0
 seaborn>=0.9.0
 colorcet>=2.0.1
 tqdm
 python-igraph>=0.7.1
-cdlib>=0.2.6
 louvain==0.8.0
 pynndescent>=0.5.2
 pre-commit
 networkx>=2.6
-nxviz==0.7.3
 get_version>=3.5.4
 openpyxl
 typing-extensions
 session-info>=1.0.0
 
 [docs]
 sphinx>=4.0.2
```

### Comparing `dynamo-release-1.3.0/setup.py` & `dynamo-release-1.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 if __name__ == "__main__":
     setup(
         name="dynamo-release",
-        version="v1.3.0",
+        version="v1.3.2",
         python_requires=">=3.7",
         install_requires=read_requirements("requirements.txt"),
         extras_require={
             "docs": read_requirements(os.path.join("docs", "requirements.txt")),
         },
         packages=find_packages(exclude=("tests", "docs")),
         classifiers=[
```

