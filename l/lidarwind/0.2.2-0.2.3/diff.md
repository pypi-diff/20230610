# Comparing `tmp/lidarwind-0.2.2.tar.gz` & `tmp/lidarwind-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidarwind-0.2.2.tar", last modified: Tue Jan 31 21:51:16 2023, max compression
+gzip compressed data, was "lidarwind-0.2.3.tar", last modified: Sat Jun 10 13:33:43 2023, max compression
```

## Comparing `lidarwind-0.2.2.tar` & `lidarwind-0.2.3.tar`

### file list

```diff
@@ -1,110 +1,121 @@
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.783576 lidarwind-0.2.2/
--rw-r--r--   0 jdiasneto (256067988) 1653728465      292 2023-01-04 16:17:26.000000 lidarwind-0.2.2/.editorconfig
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.680258 lidarwind-0.2.2/.github/
--rw-r--r--   0 jdiasneto (256067988) 1653728465      321 2023-01-04 16:17:26.000000 lidarwind-0.2.2/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.682068 lidarwind-0.2.2/.github/workflows/
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2129 2023-01-31 20:26:14.000000 lidarwind-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2522 2023-01-31 20:26:14.000000 lidarwind-0.2.2/.github/workflows/tox.yml
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1810 2023-01-04 16:17:26.000000 lidarwind-0.2.2/.gitignore
--rw-r--r--   0 jdiasneto (256067988) 1653728465      858 2023-01-04 16:17:26.000000 lidarwind-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 jdiasneto (256067988) 1653728465      170 2023-01-04 16:17:26.000000 lidarwind-0.2.2/AUTHORS.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      626 2023-01-04 16:17:26.000000 lidarwind-0.2.2/CITATION.cff
--rw-r--r--   0 jdiasneto (256067988) 1653728465     3529 2023-01-04 16:17:26.000000 lidarwind-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465       89 2023-01-04 16:17:26.000000 lidarwind-0.2.2/HISTORY.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1507 2023-01-04 16:17:26.000000 lidarwind-0.2.2/LICENSE
--rw-r--r--   0 jdiasneto (256067988) 1653728465      262 2023-01-04 16:17:26.000000 lidarwind-0.2.2/MANIFEST.in
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2376 2023-01-04 16:17:26.000000 lidarwind-0.2.2/Makefile
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2718 2023-01-31 21:51:16.783846 lidarwind-0.2.2/PKG-INFO
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2424 2023-01-31 20:26:14.000000 lidarwind-0.2.2/README.rst
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.699724 lidarwind-0.2.2/docs/
--rw-r--r--   0 jdiasneto (256067988) 1653728465      646 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/Makefile
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.711355 lidarwind-0.2.2/docs/_autosummary/
--rw-r--r--   0 jdiasneto (256067988) 1653728465      465 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.data_attributes.LoadAttributes.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      407 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.data_operator.DataOperations.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      432 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.data_operator.DbsOperations.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      498 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.data_operator.GetRestructuredData.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      433 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.data_operator.ReadProcessedData.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      331 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.filters.Filtering.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      519 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.filters.SecondTripEchoFilter.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      490 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.filters.WindCubeCloudRemoval.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      314 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.lidar_code.GetLidarData.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      662 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.lidarwind_config.Configurations.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      666 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.wind_prop_retrieval.GetWindProperties5Beam.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      460 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.wind_prop_retrieval.RetriveWindFFT.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      580 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/_autosummary/lidarwind.wind_prop_retrieval_6_beam.SixBeamMethod.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1150 2023-01-07 23:45:11.000000 lidarwind-0.2.2/docs/api.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465       28 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/authors.rst
--rwxr-xr-x   0 jdiasneto (256067988) 1653728465     5222 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/conf.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465       52 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/contributing.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1129 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/diagram.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      247 2023-01-31 20:26:14.000000 lidarwind-0.2.2/docs/environment.yml
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.729377 lidarwind-0.2.2/docs/examples/
--rw-r--r--   0 jdiasneto (256067988) 1653728465   111726 2023-01-31 20:26:14.000000 lidarwind-0.2.2/docs/examples/dbs_scans_rendered.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465  2706970 2023-01-31 20:26:14.000000 lidarwind-0.2.2/docs/examples/merging_6beam_rendered.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465   761096 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/examples/quicklooks_rendered.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465    63678 2023-01-31 20:26:14.000000 lidarwind-0.2.2/docs/examples/reading_long_dbs_rendered.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465  2486841 2023-01-31 20:26:14.000000 lidarwind-0.2.2/docs/examples/turbulence_6beam_data_rendered.ipynb
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.743851 lidarwind-0.2.2/docs/figures/
--rw-r--r--   0 jdiasneto (256067988) 1653728465   155631 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/figures/dbs.png
--rw-r--r--   0 jdiasneto (256067988) 1653728465   103041 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/figures/diagram.png
--rw-r--r--   0 jdiasneto (256067988) 1653728465   200543 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/figures/six_beam.png
--rw-r--r--   0 jdiasneto (256067988) 1653728465       28 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/history.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      379 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/index.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1122 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/installation.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1913 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/lidarwind.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      771 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/make.bat
--rw-r--r--   0 jdiasneto (256067988) 1653728465       64 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/modules.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      287 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/notebooks.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465     6029 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/overview.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      502 2023-01-04 16:17:26.000000 lidarwind-0.2.2/docs/readme.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465     7410 2023-01-10 18:25:04.000000 lidarwind-0.2.2/docs/usage.rst
--rw-r--r--   0 jdiasneto (256067988) 1653728465      306 2023-01-31 20:26:14.000000 lidarwind-0.2.2/environment.yml
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.747097 lidarwind-0.2.2/joss/
--rw-r--r--   0 jdiasneto (256067988) 1653728465     3439 2023-01-04 16:17:26.000000 lidarwind-0.2.2/joss/paper.bib
--rw-r--r--   0 jdiasneto (256067988) 1653728465     6793 2023-01-04 16:17:26.000000 lidarwind-0.2.2/joss/paper.md
--rw-r--r--   0 jdiasneto (256067988) 1653728465  2610571 2023-01-04 16:17:26.000000 lidarwind-0.2.2/joss/wind_panel.png
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.769782 lidarwind-0.2.2/lidarwind/
--rw-r--r--   0 jdiasneto (256067988) 1653728465      882 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/__init__.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     4691 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/data_attributes.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465    22809 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/data_operator.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465    12202 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/filters.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465      996 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/io.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1093 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/lidar_code.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     4811 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/lidarwind_config.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     6255 2023-01-31 20:26:14.000000 lidarwind-0.2.2/lidarwind/utilities.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465      160 2023-01-31 21:51:16.000000 lidarwind-0.2.2/lidarwind/version.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     7129 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/visualization.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465    18694 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/wind_prop_retrieval.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     5933 2023-01-04 16:17:26.000000 lidarwind-0.2.2/lidarwind/wind_prop_retrieval_6_beam.py
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.773179 lidarwind-0.2.2/lidarwind.egg-info/
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2718 2023-01-31 21:51:16.000000 lidarwind-0.2.2/lidarwind.egg-info/PKG-INFO
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2792 2023-01-31 21:51:16.000000 lidarwind-0.2.2/lidarwind.egg-info/SOURCES.txt
--rw-r--r--   0 jdiasneto (256067988) 1653728465        1 2023-01-31 21:51:16.000000 lidarwind-0.2.2/lidarwind.egg-info/dependency_links.txt
--rw-r--r--   0 jdiasneto (256067988) 1653728465       49 2023-01-31 21:51:16.000000 lidarwind-0.2.2/lidarwind.egg-info/entry_points.txt
--rw-r--r--   0 jdiasneto (256067988) 1653728465        1 2023-01-06 21:00:55.000000 lidarwind-0.2.2/lidarwind.egg-info/not-zip-safe
--rw-r--r--   0 jdiasneto (256067988) 1653728465      316 2023-01-31 21:51:16.000000 lidarwind-0.2.2/lidarwind.egg-info/requires.txt
--rw-r--r--   0 jdiasneto (256067988) 1653728465       10 2023-01-31 21:51:16.000000 lidarwind-0.2.2/lidarwind.egg-info/top_level.txt
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.776354 lidarwind-0.2.2/notebooks/
--rw-r--r--   0 jdiasneto (256067988) 1653728465     6594 2023-01-04 16:17:27.000000 lidarwind-0.2.2/notebooks/dbs_scans.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465     7709 2023-01-31 20:26:14.000000 lidarwind-0.2.2/notebooks/merging_6beam_data.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465     6423 2023-01-04 16:17:27.000000 lidarwind-0.2.2/notebooks/quicklooks.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465     6067 2023-01-04 16:17:27.000000 lidarwind-0.2.2/notebooks/reading_long_dbs.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465     7646 2023-01-31 20:26:14.000000 lidarwind-0.2.2/notebooks/turbulence_6beam_data.ipynb
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1776 2023-01-31 20:26:14.000000 lidarwind-0.2.2/pyproject.toml
--rw-r--r--   0 jdiasneto (256067988) 1653728465       38 2023-01-04 16:17:27.000000 lidarwind-0.2.2/readthedocs.yml
--rw-r--r--   0 jdiasneto (256067988) 1653728465      172 2023-01-04 16:17:27.000000 lidarwind-0.2.2/requirements_dev.txt
--rw-r--r--   0 jdiasneto (256067988) 1653728465      205 2023-01-31 21:51:16.784576 lidarwind-0.2.2/setup.cfg
--rw-r--r--   0 jdiasneto (256067988) 1653728465      220 2023-01-04 16:17:27.000000 lidarwind-0.2.2/setup.py
-drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-01-31 21:51:16.783104 lidarwind-0.2.2/tests/
--rw-r--r--   0 jdiasneto (256067988) 1653728465       39 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/__init__.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2470 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/data.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465      355 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_IO.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2138 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_dataOperator.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     3681 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_fourier_transf_wind_method.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     5140 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_get_restructured_data.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2573 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_get_wind_Properties_5_beam.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     1084 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_lidar_suit.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     3361 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_retrieve_wind_fft.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465      564 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_windPropRetrieval.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465     2740 2023-01-04 16:17:27.000000 lidarwind-0.2.2/tests/test_wind_prop_retrieval_6_beam.py
--rw-r--r--   0 jdiasneto (256067988) 1653728465      620 2023-01-31 20:26:14.000000 lidarwind-0.2.2/tox.ini
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.856103 lidarwind-0.2.3/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      292 2023-06-10 13:30:53.000000 lidarwind-0.2.3/.editorconfig
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.742541 lidarwind-0.2.3/.github/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      321 2023-06-10 13:30:53.000000 lidarwind-0.2.3/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.745021 lidarwind-0.2.3/.github/workflows/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2180 2023-06-10 13:30:53.000000 lidarwind-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2526 2023-06-10 13:30:53.000000 lidarwind-0.2.3/.github/workflows/tox.yml
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1810 2023-06-10 13:30:53.000000 lidarwind-0.2.3/.gitignore
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      871 2023-06-10 13:30:53.000000 lidarwind-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      170 2023-06-10 13:30:53.000000 lidarwind-0.2.3/AUTHORS.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      626 2023-06-10 13:30:53.000000 lidarwind-0.2.3/CITATION.cff
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3529 2023-06-10 13:30:53.000000 lidarwind-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       89 2023-06-10 13:30:53.000000 lidarwind-0.2.3/HISTORY.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1507 2023-06-10 13:30:53.000000 lidarwind-0.2.3/LICENSE
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      262 2023-06-10 13:30:53.000000 lidarwind-0.2.3/MANIFEST.in
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2376 2023-06-10 13:30:53.000000 lidarwind-0.2.3/Makefile
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2718 2023-06-10 13:33:43.856789 lidarwind-0.2.3/PKG-INFO
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3610 2023-06-10 13:30:53.000000 lidarwind-0.2.3/README.rst
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.763145 lidarwind-0.2.3/docs/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      646 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/Makefile
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.775984 lidarwind-0.2.3/docs/_autosummary/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      465 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.data_attributes.LoadAttributes.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      407 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.data_operator.DataOperations.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      432 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.data_operator.DbsOperations.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      498 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.data_operator.GetRestructuredData.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      433 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.data_operator.ReadProcessedData.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      331 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.filters.Filtering.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      519 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.filters.SecondTripEchoFilter.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      490 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.filters.WindCubeCloudRemoval.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      314 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.lidar_code.GetLidarData.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      662 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.lidarwind_config.Configurations.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      666 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.wind_prop_retrieval.GetWindProperties5Beam.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      460 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.wind_prop_retrieval.RetriveWindFFT.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      580 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/_autosummary/lidarwind.wind_prop_retrieval_6_beam.SixBeamMethod.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1150 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/api.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       28 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/authors.rst
+-rwxr-xr-x   0 jdiasneto (256067988) 1653728465     5222 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/conf.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       52 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/contributing.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1129 2023-06-10 13:30:53.000000 lidarwind-0.2.3/docs/diagram.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      247 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/environment.yml
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.789972 lidarwind-0.2.3/docs/examples/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465   111726 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/examples/dbs_scans_rendered.ipynb
+-rw-r--r--   0 jdiasneto (256067988) 1653728465  2706970 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/examples/merging_6beam_rendered.ipynb
+-rw-r--r--   0 jdiasneto (256067988) 1653728465   761096 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/examples/quicklooks_rendered.ipynb
+-rw-r--r--   0 jdiasneto (256067988) 1653728465    63678 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/examples/reading_long_dbs_rendered.ipynb
+-rw-r--r--   0 jdiasneto (256067988) 1653728465  2486841 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/examples/turbulence_6beam_data_rendered.ipynb
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.798515 lidarwind-0.2.3/docs/figures/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465   155631 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/figures/dbs.png
+-rw-r--r--   0 jdiasneto (256067988) 1653728465   103041 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/figures/diagram.png
+-rw-r--r--   0 jdiasneto (256067988) 1653728465   200543 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/figures/six_beam.png
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       28 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/history.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      379 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/index.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1122 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/installation.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1913 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/lidarwind.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      771 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/make.bat
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       64 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/modules.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      287 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/notebooks.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     6029 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/overview.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      502 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/readme.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     7410 2023-06-10 13:30:54.000000 lidarwind-0.2.3/docs/usage.rst
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      307 2023-06-10 13:30:54.000000 lidarwind-0.2.3/environment.yml
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.802320 lidarwind-0.2.3/joss/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3439 2023-06-10 13:30:54.000000 lidarwind-0.2.3/joss/paper.bib
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     6793 2023-06-10 13:30:54.000000 lidarwind-0.2.3/joss/paper.md
+-rw-r--r--   0 jdiasneto (256067988) 1653728465  2610571 2023-06-10 13:30:54.000000 lidarwind-0.2.3/joss/wind_panel.png
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.830417 lidarwind-0.2.3/lidarwind/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      882 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/__init__.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     4691 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/data_attributes.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465    22808 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/data_operator.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465    12202 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/filters.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1014 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/io.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1092 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/lidar_code.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     4811 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/lidarwind_config.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.839649 lidarwind-0.2.3/lidarwind/postprocessing/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       30 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/postprocessing/__init__.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      544 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/postprocessing/post_rpg_radar.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3211 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/postprocessing/post_wind_cube.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.841498 lidarwind-0.2.3/lidarwind/preprocessing/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       24 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/preprocessing/__init__.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     6533 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/preprocessing/rpg_radar.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     6409 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/preprocessing/wind_cube.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     6406 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/utilities.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      160 2023-06-10 13:33:43.000000 lidarwind-0.2.3/lidarwind/version.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     7130 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/visualization.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465    19101 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/wind_prop_retrieval.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     5933 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/wind_prop_retrieval_6_beam.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.842381 lidarwind-0.2.3/lidarwind/wind_retrieval/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/wind_retrieval/__init__.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     5855 2023-06-10 13:30:54.000000 lidarwind-0.2.3/lidarwind/wind_retrieval/fft_wind_retrieval.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.837827 lidarwind-0.2.3/lidarwind.egg-info/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2718 2023-06-10 13:33:43.000000 lidarwind-0.2.3/lidarwind.egg-info/PKG-INFO
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3080 2023-06-10 13:33:43.000000 lidarwind-0.2.3/lidarwind.egg-info/SOURCES.txt
+-rw-r--r--   0 jdiasneto (256067988) 1653728465        1 2023-06-10 13:33:43.000000 lidarwind-0.2.3/lidarwind.egg-info/dependency_links.txt
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       49 2023-06-10 13:33:43.000000 lidarwind-0.2.3/lidarwind.egg-info/entry_points.txt
+-rw-r--r--   0 jdiasneto (256067988) 1653728465        1 2023-06-10 13:33:42.000000 lidarwind-0.2.3/lidarwind.egg-info/not-zip-safe
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      321 2023-06-10 13:33:43.000000 lidarwind-0.2.3/lidarwind.egg-info/requires.txt
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       10 2023-06-10 13:33:43.000000 lidarwind-0.2.3/lidarwind.egg-info/top_level.txt
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2318 2023-06-10 13:30:54.000000 lidarwind-0.2.3/pyproject.toml
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       38 2023-06-10 13:30:54.000000 lidarwind-0.2.3/readthedocs.yml
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      172 2023-06-10 13:30:54.000000 lidarwind-0.2.3/requirements_dev.txt
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      205 2023-06-10 13:33:43.858413 lidarwind-0.2.3/setup.cfg
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      219 2023-06-10 13:30:54.000000 lidarwind-0.2.3/setup.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.850844 lidarwind-0.2.3/tests/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465       39 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/__init__.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2470 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/data.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.852642 lidarwind-0.2.3/tests/postprocessing/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3937 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/postprocessing/test_post_wind_cube.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.854131 lidarwind-0.2.3/tests/preprocessing/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3334 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/preprocessing/test_preprocessing.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      470 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_IO.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2327 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_dataOperator.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     4306 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_fourier_transf_wind_method.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     5140 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_get_restructured_data.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2573 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_get_wind_Properties_5_beam.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     1083 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_lidar_suit.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     3361 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_retrieve_wind_fft.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      564 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_windPropRetrieval.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     2730 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/test_wind_prop_retrieval_6_beam.py
+drwxr-xr-x   0 jdiasneto (256067988) 1653728465        0 2023-06-10 13:33:43.855110 lidarwind-0.2.3/tests/wind_retrieval/
+-rw-r--r--   0 jdiasneto (256067988) 1653728465     5132 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tests/wind_retrieval/test_wind_retrieval.py
+-rw-r--r--   0 jdiasneto (256067988) 1653728465      758 2023-06-10 13:30:54.000000 lidarwind-0.2.3/tox.ini
```

### Comparing `lidarwind-0.2.2/.github/workflows/ci.yml` & `lidarwind-0.2.3/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -64,18 +64,18 @@
         cache-dependency-path: 'pyproject.toml'
 
     - name: Coverage report
       run: |
         python -m pip install --upgrade pip
         pip install -e .[test]
         pytest --cov=./ --cov-report=xml
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/turbulence_6beam_data.ipynb
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/merging_6beam_data.ipynb
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/dbs_scans.ipynb
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/reading_long_dbs.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax docs/examples/turbulence_6beam_data_rendered.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax docs/examples/merging_6beam_rendered.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax docs/examples/dbs_scans_rendered.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax docs/examples/reading_long_dbs_rendered.ipynb
 
 
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         fail_ci_if_error: true
         verbose: true
```

### Comparing `lidarwind-0.2.2/.github/workflows/tox.yml` & `lidarwind-0.2.3/.github/workflows/tox.yml`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         cache-dependency-path: 'pyproject.toml'
 
     - name: Coverage report
       run: |
         python -m pip install --upgrade pip
         pip install -e .[test]
         pytest --cov=./ --cov-report=xml
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/turbulence_6beam_data.ipynb
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/merging_6beam_data.ipynb
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/dbs_scans.ipynb
-        pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/reading_long_dbs.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/turbulence_6beam_data.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/merging_6beam_data.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/dbs_scans.ipynb
+       # pytest --cov=./ --cov-append --cov-report=xml --current-env --nbval-lax notebooks/reading_long_dbs.ipynb
 
 
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         fail_ci_if_error: true
         verbose: true
```

### Comparing `lidarwind-0.2.2/.gitignore` & `lidarwind-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/.pre-commit-config.yaml` & `lidarwind-0.2.3/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     -   id: check-merge-conflict
     -   id: check-yaml
     -   id: check-toml
     -   id: debug-statements
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-added-large-files
--   repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.2
-    hooks:
-    -   id: pyupgrade
-        args: [--py38-plus]
 -   repo: https://github.com/psf/black
     rev: 22.8.0
     hooks:
     -   id: black
         args: [ --safe ]
         exclude: docs/conf.py
 -   repo: https://github.com/PyCQA/flake8
     rev: 5.0.4
     hooks:
     -   id: flake8
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  # Ruff version.
+  rev: 'v0.0.244'
+  hooks:
+    - id: ruff
+      args: [ --fix ]
```

### Comparing `lidarwind-0.2.2/CITATION.cff` & `lidarwind-0.2.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/CONTRIBUTING.rst` & `lidarwind-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/LICENSE` & `lidarwind-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/Makefile` & `lidarwind-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/PKG-INFO` & `lidarwind-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidarwind
-Version: 0.2.2
+Version: 0.2.3
 Summary: LIDAR procedures
 Author: José Dias Neto
 Author-email: jdiasn@gmail.com
 License: 
         
         BSD License
```

### Comparing `lidarwind-0.2.2/docs/Makefile` & `lidarwind-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/_autosummary/lidarwind.filters.SecondTripEchoFilter.rst` & `lidarwind-0.2.3/docs/_autosummary/lidarwind.filters.SecondTripEchoFilter.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/_autosummary/lidarwind.lidarwind_config.Configurations.rst` & `lidarwind-0.2.3/docs/_autosummary/lidarwind.lidarwind_config.Configurations.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/_autosummary/lidarwind.wind_prop_retrieval.GetWindProperties5Beam.rst` & `lidarwind-0.2.3/docs/_autosummary/lidarwind.wind_prop_retrieval.GetWindProperties5Beam.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/_autosummary/lidarwind.wind_prop_retrieval_6_beam.SixBeamMethod.rst` & `lidarwind-0.2.3/docs/_autosummary/lidarwind.wind_prop_retrieval_6_beam.SixBeamMethod.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/api.rst` & `lidarwind-0.2.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/conf.py` & `lidarwind-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/diagram.rst` & `lidarwind-0.2.3/docs/diagram.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/examples/dbs_scans_rendered.ipynb` & `lidarwind-0.2.3/docs/examples/dbs_scans_rendered.ipynb`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/examples/merging_6beam_rendered.ipynb` & `lidarwind-0.2.3/docs/examples/merging_6beam_rendered.ipynb`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/examples/quicklooks_rendered.ipynb` & `lidarwind-0.2.3/docs/examples/quicklooks_rendered.ipynb`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/examples/reading_long_dbs_rendered.ipynb` & `lidarwind-0.2.3/docs/examples/reading_long_dbs_rendered.ipynb`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/examples/turbulence_6beam_data_rendered.ipynb` & `lidarwind-0.2.3/docs/examples/turbulence_6beam_data_rendered.ipynb`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/figures/dbs.png` & `lidarwind-0.2.3/docs/figures/dbs.png`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/figures/diagram.png` & `lidarwind-0.2.3/docs/figures/diagram.png`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/figures/six_beam.png` & `lidarwind-0.2.3/docs/figures/six_beam.png`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/installation.rst` & `lidarwind-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/lidarwind.rst` & `lidarwind-0.2.3/docs/lidarwind.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/make.bat` & `lidarwind-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/overview.rst` & `lidarwind-0.2.3/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/docs/usage.rst` & `lidarwind-0.2.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/joss/paper.bib` & `lidarwind-0.2.3/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/joss/paper.md` & `lidarwind-0.2.3/joss/paper.md`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/joss/wind_panel.png` & `lidarwind-0.2.3/joss/wind_panel.png`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/lidarwind/__init__.py` & `lidarwind-0.2.3/lidarwind/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Top-level package for lidarwind package"""
 
 __author__ = "José Dias Neto"
 __email__ = "jdiasn@gmail.com"
 __affiliation__ = "Delft University of Technology"
 
 
-from pkg_resources import get_distribution, DistributionNotFound
+from pkg_resources import DistributionNotFound, get_distribution
 
 try:
     __version__ = get_distribution(__name__).version
 except DistributionNotFound:
     try:
         from .version import version as __version__
     except ImportError:
         raise ImportError(
             "Failed to find (autogenerated) version.py. "
             "This might be because you are installing from GitHub's tarballs, "
             "use the PyPI ones."
         )
 
 
-from .lidarwind_config import *
+from .data_attributes import *
+from .data_operator import *
+from .filters import *
 from .lidar_code import *
+from .lidarwind_config import *
+from .utilities import *
+from .visualization import *
 from .wind_prop_retrieval import *
 from .wind_prop_retrieval_6_beam import *
-from .visualization import *
-from .utilities import *
-from .data_operator import *
-from .data_attributes import *
-from .filters import *
```

### Comparing `lidarwind-0.2.2/lidarwind/data_attributes.py` & `lidarwind-0.2.3/lidarwind/data_attributes.py`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/lidarwind/data_operator.py` & `lidarwind-0.2.3/lidarwind/data_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Module to manage and prepare the data for other modules
 
 """
 
 
+import datetime as dt
 import logging
 
-import xarray as xr
-import datetime as dt
-import pandas as pd
 import numpy as np
+import pandas as pd
+import xarray as xr
 
 from .filters import Filtering
-
 from .lidar_code import GetLidarData
 
 module_logger = logging.getLogger("lidarwind.data_operator")
 module_logger.debug("loading data_operator")
 
 
 def wc_fixed_preprocessing(ds: xr.Dataset, azimuth_resolution: int = 1):
```

### Comparing `lidarwind-0.2.2/lidarwind/filters.py` & `lidarwind-0.2.3/lidarwind/filters.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for keep all filtering functionalities
 
 """
 import logging
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 import xarray as xr
 
 module_logger = logging.getLogger("lidarwind.filters")
 
 
 def filter_status(ds: xr.Dataset):
     """Filter dataset based on WindCube's software
```

### Comparing `lidarwind-0.2.2/lidarwind/io.py` & `lidarwind-0.2.3/lidarwind/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
     assert (
         "sweep_group_name" in raw_data
     ), "missing sweep group variable in input file"
     sweep_group_name = raw_data["sweep_group_name"].values[0]
     ds = raw_data[f"/{sweep_group_name}"].to_dataset()
 
+    del raw_data
+
     assert "time_reference" in ds, "missing time_reference in input sweep"
     # Guarantee that it is a valid datetime
     reference_time = pd.to_datetime(ds["time_reference"].values).isoformat()
     ds["time"].attrs["units"] = f"seconds since {reference_time}"
 
     ds = xr.decode_cf(ds)
```

### Comparing `lidarwind-0.2.2/lidarwind/lidar_code.py` & `lidarwind-0.2.3/lidarwind/lidar_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Module to open the lidar original output
 
 """
 
 
 import warnings
 
-
 from .io import open_sweep
 
 
 class GetLidarData:
     """Windcube's data reader
```

### Comparing `lidarwind-0.2.2/lidarwind/lidarwind_config.py` & `lidarwind-0.2.3/lidarwind/lidarwind_config.py`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/lidarwind/utilities.py` & `lidarwind-0.2.3/lidarwind/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """Utilities module
 
 """
 
+import glob
 import os
 import shutil
-import glob
 
 import gdown
+import numpy as np
 import pandas as pd
 import pooch
-import numpy as np
 import xarray as xr
 
 
-
 def sample_data(key: str):
     if key == "wc_6beam":
         file_list = pooch.retrieve(
             url="doi:10.5281/zenodo.7312960/wc_6beam.zip",
             known_hash="md5:a7ea3c10a6d2f4a97ff955dc4398f930",
+            path="~/.cache/lidarwind",
             processor=pooch.Unzip(),
         )
     elif key == "wc_long_dbs":
         file_list = pooch.retrieve(
             url="doi:10.5281/zenodo.7312960/wc_long_dbs.zip",
             known_hash="md5:53b4eb6e5dad6dfdaddfbb718dcf8910",
+            path="~/.cache/lidarwind",
             processor=pooch.Unzip(),
         )
     elif key == "wc_short_dbs":
         file_list = pooch.retrieve(
             url="doi:10.5281/zenodo.7312960/wc_short_dbs.zip",
             known_hash="md5:9cbd93f89052d6c6f4407bcce415e277",
+            path="~/.cache/lidarwind",
             processor=pooch.Unzip(),
         )
     else:
         raise ValueError
 
     return file_list
 
@@ -66,15 +68,16 @@
         """Downloading data
 
         It downloads the sample needed for the examples.
 
         """
 
         if file_type == "12-00":
-            url = "https://drive.google.com/uc?export=download&id=1i6iX6KuZOkP_WLuPZHG5uCcvRjlWS-SU"
+            file_id = "1i6iX6KuZOkP_WLuPZHG5uCcvRjlWS-SU"
+            url = f"https://drive.google.com/uc?export=download&id={file_id}"
 
         if file_type == "dbs":
             url = "path"
 
         output = f"{sample_path}{file_type}.zip"
         gdown.download(url, output, quiet=False)
```

### Comparing `lidarwind-0.2.2/lidarwind/visualization.py` & `lidarwind-0.2.3/lidarwind/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
+
+import matplotlib.dates as mdates
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-import matplotlib.dates as mdates
 
 from .filters import Filtering
 
 
 class PlotSettings:
     def __init__(self, mpl, style="dark_background"):
```

### Comparing `lidarwind-0.2.2/lidarwind/wind_prop_retrieval.py` & `lidarwind-0.2.3/lidarwind/wind_prop_retrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 from .data_attributes import LoadAttributes
 from .data_operator import GetRestructuredData
 
 module_logger = logging.getLogger("lidarwind.wind_prop_retrieval")
 module_logger.debug("loading wind_prop_retrieval")
 
 
+def first_harmonic_amplitude(ds: xr.Dataset, dim="azm") -> xr.DataArray:
+    """First harmonic amplitude
+
+    It calculates the complex amplitudes from the first harmonic from the
+    observations along the azm coordinate
+
+    ds doppler_obs
+
+    """
+    module_logger.info("calculating the complex amplitude")
+
+    comp_amp = xrft.fft(ds, dim=[dim], true_amplitude=False)
+
+    return comp_amp.isel(freq_azm=-2)
+
+
 class FourierTransfWindMethod:
     """FFT wind retrieval method
 
     It is a fft wind retrieval method. It was proposed
     by Ishwardat (2017). For more details see
     http://resolver.tudelft.nl/uuid:a659654b-e76a-4513-a656-ecad761bdbc8
 
@@ -31,15 +47,14 @@
         A Dataset containing the horizontal wind speed
         and direction. It also includes the zonal and
         meridional wind components
 
     """
 
     def __init__(self, doppler_obs: xr.DataArray):
-
         self.logger = logging.getLogger(
             "lidarwind.wind_prop_retrieval.FourierTransfWindMethod"
         )
         self.logger.info("creating an instance of FourierTransfWindMethod")
 
         if not isinstance(doppler_obs, xr.DataArray):
             self.logger.error("wrong data type: expecting a xr.DataArray")
@@ -289,15 +304,14 @@
         self,
         data: xr.Dataset,
         status_filter=True,
         cnr=None,
         method="single_dbs",
         tolerance="8s",
     ):
-
         self.logger = logging.getLogger(
             "lidarwind.wind_prop_retrieval.GetWindProperties5Beam"
         )
         self.logger.info("creating an instance of GetWindProperties5Beam")
 
         if not isinstance(data, xr.Dataset):
             self.logger.error("wrong data type: expecting a xr.Dataset")
@@ -543,23 +557,22 @@
         An object containing an dataset of the retrieved wind
         speed, direction, wind components (meridional, zonal
         and vertical) and the relative beta
 
     """
 
     def __init__(self, transfd_data: GetRestructuredData):
-
         self.logger = logging.getLogger(
             "lidarwind.wind_prop_retrieval.FourierTransfWindMethod"
         )
         self.logger.info("creating an instance of FourierTransfWindMethod")
 
         if not isinstance(transfd_data, GetRestructuredData):
             self.logger.error(
-                "wrong data type: expecting a lidarwind.GetRestructuredData instance"
+                "wrong data type: expecting a lidarwind.GetRestructuredData"
             )
             raise TypeError
 
         self.transfd_data = transfd_data
         self.ret_hor_wind_data()
         self.ret_vert_wind_data()
         self.get_beta()
@@ -573,15 +586,15 @@
 
         self.logger.info("retrieving horizontal wind from the 6 beam data")
 
         tmp_wind_prop = FourierTransfWindMethod(
             self.transfd_data.data_transf
         ).wind_prop()
         tmp_wind_prop = tmp_wind_prop.squeeze(dim="elv")
-        tmp_wind_prop = tmp_wind_prop.drop(["elv", "freq_azm"])
+        tmp_wind_prop = tmp_wind_prop.drop_vars(["elv", "freq_azm"])
         self.wind_prop = tmp_wind_prop
 
         return self
 
     def ret_vert_wind_data(self):
         """
         It copies the vertical wind from the observations
```

### Comparing `lidarwind-0.2.2/lidarwind/wind_prop_retrieval_6_beam.py` & `lidarwind-0.2.3/lidarwind/wind_prop_retrieval_6_beam.py`

 * *Files identical despite different names*

### Comparing `lidarwind-0.2.2/lidarwind.egg-info/PKG-INFO` & `lidarwind-0.2.3/lidarwind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidarwind
-Version: 0.2.2
+Version: 0.2.3
 Summary: LIDAR procedures
 Author: José Dias Neto
 Author-email: jdiasn@gmail.com
 License: 
         
         BSD License
```

### Comparing `lidarwind-0.2.2/lidarwind.egg-info/SOURCES.txt` & `lidarwind-0.2.3/lidarwind.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -75,23 +75,29 @@
 lidarwind.egg-info/PKG-INFO
 lidarwind.egg-info/SOURCES.txt
 lidarwind.egg-info/dependency_links.txt
 lidarwind.egg-info/entry_points.txt
 lidarwind.egg-info/not-zip-safe
 lidarwind.egg-info/requires.txt
 lidarwind.egg-info/top_level.txt
-notebooks/dbs_scans.ipynb
-notebooks/merging_6beam_data.ipynb
-notebooks/quicklooks.ipynb
-notebooks/reading_long_dbs.ipynb
-notebooks/turbulence_6beam_data.ipynb
+lidarwind/postprocessing/__init__.py
+lidarwind/postprocessing/post_rpg_radar.py
+lidarwind/postprocessing/post_wind_cube.py
+lidarwind/preprocessing/__init__.py
+lidarwind/preprocessing/rpg_radar.py
+lidarwind/preprocessing/wind_cube.py
+lidarwind/wind_retrieval/__init__.py
+lidarwind/wind_retrieval/fft_wind_retrieval.py
 tests/__init__.py
 tests/data.py
 tests/test_IO.py
 tests/test_dataOperator.py
 tests/test_fourier_transf_wind_method.py
 tests/test_get_restructured_data.py
 tests/test_get_wind_Properties_5_beam.py
 tests/test_lidar_suit.py
 tests/test_retrieve_wind_fft.py
 tests/test_windPropRetrieval.py
-tests/test_wind_prop_retrieval_6_beam.py
+tests/test_wind_prop_retrieval_6_beam.py
+tests/postprocessing/test_post_wind_cube.py
+tests/preprocessing/test_preprocessing.py
+tests/wind_retrieval/test_wind_retrieval.py
```

### Comparing `lidarwind-0.2.2/pyproject.toml` & `lidarwind-0.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [
     "setuptools >= 48",
     "setuptools_scm[toml] >= 4",
     "setuptools_scm_git_archive",
     "milksnake",
-    "wheel >= 0.29.0",
+    "wheel >= 0.38.1",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name="lidarwind"
 dynamic = ['version']
 description="LIDAR procedures"
@@ -28,40 +28,41 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-  "xrft>=0.3.0",
-  "xarray>=0.20",
-  "pandas>=1.3.3",
+  "xrft>=0.3",
+  "xarray>=0.21",
+  "pandas>=1.4",
   "numpy>=1.22",
   "netCDF4 >= 1.5",
   "matplotlib>=3.4.3",
   "click>=8.1.2",
   "gdown~=4.5.1",
-  "xarray-datatree==0.0.9"
+  "xarray-datatree~=0.0.11",
+  "pooch>=1.6",
 ]
 
 [project.optional-dependencies]
 plots = ["matplotlib>=3.4.3"]
 dev = [
   "flake8~=4.0.1",
-  "pyupgrade~=3.2.2",
   "pre-commit~=2.20.0",
+  "ruff~=0.0.220",
   "sphinx_rtd_theme~=0.4.3"
 ]
 test = [
   "gdown~=4.5.1",
   "pytest>=6.2",
   "pytest-cov>=3.0",
   "nbval",
   "pooch>=1.6",
-  "tox~=4.1.1"
+  "tox~=4.3.0"
 ]
 
 [project.urls]
 homepage = "https://github.com/jdiasn/lidarwind"
 repository = "https://github.com/jdiasn/lidarwind"
 documentation = "https://lidarwind.readthedocs.io"
 
@@ -73,7 +74,39 @@
 
 [tool.setuptools_scm]
 write_to = "lidarwind/version.py"
 git_describe_command = "git describe --dirty --tags --long --match 'v*' --first-parent"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
+
+[tool.ruff]
+select = ["A", "I", "UP", "W"]
+ignore = []
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["I"]
+unfixable = ["F401"]
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".eggs",
+    ".git",
+    ".mypy_cache",
+    ".nox",
+    ".ruff_cache",
+    ".tox",
+    "__pypackages__",
+    "_build",
+    "build",
+    "dist",
+    "docs/conf.py",
+    "docs/_autosummary",
+]
+per-file-ignores = {}
+
+line-length = 79
+
+target-version = "py38"
+
+[tool.ruff.pydocstyle]
+convention = "numpy"
```

### Comparing `lidarwind-0.2.2/tests/data.py` & `lidarwind-0.2.3/tests/data.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import glob
 import os
 import shutil
-import glob
 from typing import Optional
 
-import pytest
 import gdown
+import pytest
 
 from lidarwind.io import open_sweep
 
 GDRIVE_ID = "1i6iX6KuZOkP_WLuPZHG5uCcvRjlWS-SU"
 
 
 def lidarwindrc(subdir: Optional[str] = None):
```

### Comparing `lidarwind-0.2.2/tests/test_get_restructured_data.py` & `lidarwind-0.2.3/tests/test_get_restructured_data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pytest
 import numpy as np
+import pytest
 import xarray as xr
 
 import lidarwind as lst
 
 
 @pytest.fixture
 def get_dummy_six_beam_data():
```

### Comparing `lidarwind-0.2.2/tests/test_get_wind_Properties_5_beam.py` & `lidarwind-0.2.3/tests/test_get_wind_Properties_5_beam.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import numpy as np
 import pytest
 import xarray as xr
-import numpy as np
 
 import lidarwind as lst
 
 
 def get_dummy_dbs():
 
     wind = (
```

### Comparing `lidarwind-0.2.2/tests/test_lidar_suit.py` & `lidarwind-0.2.3/tests/test_lidar_suit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 
 """Tests for 'lidarwind' package."""
 
 import pytest
-
 from click.testing import CliRunner
 
 import lidarwind
 
 # from lidarwind import cli
```

### Comparing `lidarwind-0.2.2/tests/test_retrieve_wind_fft.py` & `lidarwind-0.2.3/tests/test_retrieve_wind_fft.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pytest
 import numpy as np
+import pytest
 import xarray as xr
 
 import lidarwind as lst
 
 
 def get_dummy_six_beam_obj():
```

### Comparing `lidarwind-0.2.2/tests/test_windPropRetrieval.py` & `lidarwind-0.2.3/tests/test_windPropRetrieval.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import numpy as np
 import pytest
 import xarray as xr
-import numpy as np
 
 import lidarwind as lst
 
 
 def test_wind_prop_retrieval_ffWindPropRet_doppler_obs():
 
     with pytest.raises(TypeError):
```

### Comparing `lidarwind-0.2.2/tests/test_wind_prop_retrieval_6_beam.py` & `lidarwind-0.2.3/tests/test_wind_prop_retrieval_6_beam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-import pytest
 import numpy as np
+import pytest
 import xarray as xr
 
 import lidarwind as lst
 
 
-def test_six_beam_method_input():
-
-    with pytest.raises(TypeError):
-        lst.SixBeamMethod(data=xr.DataArray(np.array([0, 1])))
-
-
-def test_get_dummy_six_beam_obj():
+def get_dummy_six_beam_obj():
 
     elv = np.array([75, 75, 90, 75, 75, 75])
     data_elv = xr.DataArray(
         elv, dims=("time"), coords={"time": np.arange(len(elv))}
     )
 
     azm = np.array([0, 72, 0, 144, 216, 288])
@@ -51,19 +45,25 @@
             "relative_beta": data,
         }
     )
 
     return lst.GetRestructuredData(test_ds)
 
 
+def test_six_beam_method_input():
+
+    with pytest.raises(TypeError):
+        lst.SixBeamMethod(data=xr.DataArray(np.array([0, 1])))
+
+
 @pytest.fixture
 def test_get_six_beam_obj():
 
     six_beam_obj = lst.SixBeamMethod(
-        test_get_dummy_six_beam_obj(), freq=6, freq90=6
+        get_dummy_six_beam_obj(), freq=6, freq90=6
     )
 
     return six_beam_obj
 
 
 def test_six_beam_method_m_matrix(test_get_six_beam_obj):
```

