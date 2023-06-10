# Comparing `tmp/PowerGenome-0.6.1.tar.gz` & `tmp/PowerGenome-0.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowerGenome-0.6.1.tar", last modified: Sat Jun 10 21:20:09 2023, max compression
+gzip compressed data, was "PowerGenome-0.6.1a0.tar", last modified: Thu Jun  8 05:26:42 2023, max compression
```

## Comparing `PowerGenome-0.6.1.tar` & `PowerGenome-0.6.1a0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.484407 PowerGenome-0.6.1/
--rw-r--r--   0 gs5183     (501) staff       (20)     1070 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/LICENSE.md
--rw-r--r--   0 gs5183     (501) staff       (20)    17896 2023-06-10 21:20:09.484207 PowerGenome-0.6.1/PKG-INFO
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.472357 PowerGenome-0.6.1/PowerGenome.egg-info/
--rw-r--r--   0 gs5183     (501) staff       (20)    17896 2023-06-10 21:20:09.000000 PowerGenome-0.6.1/PowerGenome.egg-info/PKG-INFO
--rw-r--r--   0 gs5183     (501) staff       (20)     1308 2023-06-10 21:20:09.000000 PowerGenome-0.6.1/PowerGenome.egg-info/SOURCES.txt
--rw-r--r--   0 gs5183     (501) staff       (20)        1 2023-06-10 21:20:09.000000 PowerGenome-0.6.1/PowerGenome.egg-info/dependency_links.txt
--rw-r--r--   0 gs5183     (501) staff       (20)       99 2023-06-10 21:20:09.000000 PowerGenome-0.6.1/PowerGenome.egg-info/entry_points.txt
--rw-r--r--   0 gs5183     (501) staff       (20)      234 2023-06-10 21:20:09.000000 PowerGenome-0.6.1/PowerGenome.egg-info/requires.txt
--rw-r--r--   0 gs5183     (501) staff       (20)       17 2023-06-10 21:20:09.000000 PowerGenome-0.6.1/PowerGenome.egg-info/top_level.txt
--rw-r--r--   0 gs5183     (501) staff       (20)    17017 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/README.md
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.472552 PowerGenome-0.6.1/data/
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.479163 PowerGenome-0.6.1/data/additional_technologies/
--rw-r--r--   0 gs5183     (501) staff       (20)     1083 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/additional_technologies/AZ_additional_tech.csv
--rw-r--r--   0 gs5183     (501) staff       (20)      823 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/additional_technologies/AZ_additional_tech_2030.csv
--rw-r--r--   0 gs5183     (501) staff       (20)      822 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/additional_technologies/AZ_additional_tech_2045.csv
--rw-r--r--   0 gs5183     (501) staff       (20)      625 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/additional_technologies/sample_additional_tech.csv
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.479402 PowerGenome-0.6.1/data/coal_fgd/
--rw-r--r--   0 gs5183     (501) staff       (20)    15123 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/coal_fgd/fgd_output.csv
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.479804 PowerGenome-0.6.1/data/cost_multipliers/
--rw-r--r--   0 gs5183     (501) staff       (20)     6226 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv
--rw-r--r--   0 gs5183     (501) staff       (20)     1844 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/cost_multipliers/EIA regional cost multipliers.csv
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.480160 PowerGenome-0.6.1/data/cpi_data/
--rw-r--r--   0 gs5183     (501) staff       (20)      694 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/data/cpi_data/cpi_data.csv
--rw-r--r--   0 gs5183     (501) staff       (20)  7754322 2023-06-05 17:55:42.000000 PowerGenome-0.6.1/data/ipm_regions_simple.geojson
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.483713 PowerGenome-0.6.1/powergenome/
--rw-r--r--   0 gs5183     (501) staff       (20)    44811 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/GenX.py
--rw-r--r--   0 gs5183     (501) staff       (20)       22 2023-06-10 21:18:41.000000 PowerGenome-0.6.1/powergenome/__init__.py
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-10 21:20:09.483888 PowerGenome-0.6.1/powergenome/cluster/
--rw-r--r--   0 gs5183     (501) staff       (20)    20651 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/cluster/renewables.py
--rw-r--r--   0 gs5183     (501) staff       (20)     6669 2023-06-07 04:30:00.000000 PowerGenome-0.6.1/powergenome/cluster_method.py
--rw-r--r--   0 gs5183     (501) staff       (20)     7980 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/co2_pipeline_cost.py
--rw-r--r--   0 gs5183     (501) staff       (20)     9047 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/distributed_gen.py
--rw-r--r--   0 gs5183     (501) staff       (20)    19178 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/eia_opendata.py
--rw-r--r--   0 gs5183     (501) staff       (20)    21119 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/external_data.py
--rw-r--r--   0 gs5183     (501) staff       (20)     7656 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/extract_pudl_data.py
--rw-r--r--   0 gs5183     (501) staff       (20)     4856 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/fuels.py
--rw-r--r--   0 gs5183     (501) staff       (20)   135372 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/generators.py
--rw-r--r--   0 gs5183     (501) staff       (20)    11145 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/load_construction.py
--rw-r--r--   0 gs5183     (501) staff       (20)    33579 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/load_profiles.py
--rw-r--r--   0 gs5183     (501) staff       (20)    63909 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/nrelatb.py
--rw-r--r--   0 gs5183     (501) staff       (20)     2381 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/params.py
--rw-r--r--   0 gs5183     (501) staff       (20)     7516 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/price_adjustment.py
--rw-r--r--   0 gs5183     (501) staff       (20)    45619 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/resource_clusters.py
--rw-r--r--   0 gs5183     (501) staff       (20)    17869 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/run_powergenome_multiple_outputs_cli.py
--rw-r--r--   0 gs5183     (501) staff       (20)    14981 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/time_reduction.py
--rw-r--r--   0 gs5183     (501) staff       (20)    11110 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/transmission.py
--rw-r--r--   0 gs5183     (501) staff       (20)    36744 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/util.py
--rw-r--r--   0 gs5183     (501) staff       (20)       23 2023-06-10 21:18:16.000000 PowerGenome-0.6.1/powergenome/version.py
--rw-r--r--   0 gs5183     (501) staff       (20)     1731 2023-06-10 21:18:31.000000 PowerGenome-0.6.1/pyproject.toml
--rw-r--r--   0 gs5183     (501) staff       (20)       38 2023-06-10 21:20:09.484458 PowerGenome-0.6.1/setup.cfg
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.260635 PowerGenome-0.6.1a0/
+-rw-r--r--   0 gs5183     (501) staff       (20)     1070 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/LICENSE.md
+-rw-r--r--   0 gs5183     (501) staff       (20)    16941 2023-06-08 05:26:42.260376 PowerGenome-0.6.1a0/PKG-INFO
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.249740 PowerGenome-0.6.1a0/PowerGenome.egg-info/
+-rw-r--r--   0 gs5183     (501) staff       (20)    16941 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/PKG-INFO
+-rw-r--r--   0 gs5183     (501) staff       (20)     1308 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/SOURCES.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)        1 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/dependency_links.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)       99 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/entry_points.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)      232 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/requires.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)       17 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/top_level.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)    16060 2023-06-08 05:16:33.000000 PowerGenome-0.6.1a0/README.md
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.249896 PowerGenome-0.6.1a0/data/
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255083 PowerGenome-0.6.1a0/data/additional_technologies/
+-rw-r--r--   0 gs5183     (501) staff       (20)     1083 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)      823 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2030.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)      822 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2045.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)      625 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/sample_additional_tech.csv
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255232 PowerGenome-0.6.1a0/data/coal_fgd/
+-rw-r--r--   0 gs5183     (501) staff       (20)    15123 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/coal_fgd/fgd_output.csv
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255548 PowerGenome-0.6.1a0/data/cost_multipliers/
+-rw-r--r--   0 gs5183     (501) staff       (20)     6226 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)     1844 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/cost_multipliers/EIA regional cost multipliers.csv
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255706 PowerGenome-0.6.1a0/data/cpi_data/
+-rw-r--r--   0 gs5183     (501) staff       (20)      694 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/data/cpi_data/cpi_data.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)  7754322 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/ipm_regions_simple.geojson
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.259538 PowerGenome-0.6.1a0/powergenome/
+-rw-r--r--   0 gs5183     (501) staff       (20)    44811 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/GenX.py
+-rw-r--r--   0 gs5183     (501) staff       (20)       23 2023-06-08 02:26:41.000000 PowerGenome-0.6.1a0/powergenome/__init__.py
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.259894 PowerGenome-0.6.1a0/powergenome/cluster/
+-rw-r--r--   0 gs5183     (501) staff       (20)    20651 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/cluster/renewables.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     6669 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/cluster_method.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     7980 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/co2_pipeline_cost.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     9047 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/distributed_gen.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    19178 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/eia_opendata.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    21119 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/external_data.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     7656 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/extract_pudl_data.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     4856 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/fuels.py
+-rw-r--r--   0 gs5183     (501) staff       (20)   135331 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/generators.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    11145 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/load_construction.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    33579 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/load_profiles.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    63909 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/nrelatb.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     2381 2023-06-08 03:45:29.000000 PowerGenome-0.6.1a0/powergenome/params.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     7516 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/price_adjustment.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    45619 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/resource_clusters.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    17869 2023-06-08 03:49:06.000000 PowerGenome-0.6.1a0/powergenome/run_powergenome_multiple_outputs_cli.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    14981 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/time_reduction.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    11110 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/transmission.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    36496 2023-06-08 03:59:24.000000 PowerGenome-0.6.1a0/powergenome/util.py
+-rw-r--r--   0 gs5183     (501) staff       (20)       23 2023-06-08 01:52:09.000000 PowerGenome-0.6.1a0/powergenome/version.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     1730 2023-06-08 03:23:37.000000 PowerGenome-0.6.1a0/pyproject.toml
+-rw-r--r--   0 gs5183     (501) staff       (20)       38 2023-06-08 05:26:42.260707 PowerGenome-0.6.1a0/setup.cfg
```

### Comparing `PowerGenome-0.6.1/LICENSE.md` & `PowerGenome-0.6.1a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/PKG-INFO` & `PowerGenome-0.6.1a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: PowerGenome
-Version: 0.6.1
-Summary: Create power system inputs for capacity expansion models
-Author-email: Greg Schivley <greg.schivley@princeton.edu>
-Maintainer-email: Greg Schivley <greg.schivley@princeton.edu>
-License: MIT
-Project-URL: Source, https://github.com/PowerGenome/PowerGenome
-Keywords: power system data,capacity expansion,two
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
 # PowerGenome
 
 [![The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4426097.svg)](https://doi.org/10.5281/zenodo.4426096)
 [![pytest](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml/badge.svg)](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/PowerGenome/PowerGenome/branch/master/graph/badge.svg?token=7KJYLE3jOW)](https://codecov.io/gh/PowerGenome/PowerGenome)
@@ -41,19 +18,25 @@
 
 Because computational complexity and run times increase as the number of regions and generating unit clusters increases, a user might want only want to disaggregate regions and generating units close to the primary region of interest. For example, a study focused on clean electricity regulations in New Mexico might combine several states in the Pacific Northwest into a single region while also splitting Arizona combined cycle units into multiple clusters.
 
 The goal of PowerGenome is to let a user make all of these choices in a settings file and then run a single script that generates input files for the power system model. PowerGenome currently generates input files for [GenX](https://energy.mit.edu/wp-content/uploads/2017/10/Enhanced-Decision-Support-for-a-Changing-Electricity-Landscape.pdf), and we hope to expand to other models in the near future.
 
 ## Data
 
-PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files. All data files [are available here](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). 
+PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files.
+
+1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below).
+2. A [second sqlite database (pg_misc_efs)](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
+3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios ([efs_files_utc](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=share_link)).
+
+There are also a few data files stored in this repository:
 
-1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below). This file is available at the link above or you can download it from the Zenodo repository.
-2. A second sqlite database (`pg_misc_tables_efs.sqlite`) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
-3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios (`efs_files_utc`).
+- Regional cost multipliers for individual technologies developed by EIA (`data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`).
+- A simplified geojson version of EPA's shapefile for IPM regions (`data/ipm_regions_simple.geojson`).
+- Information on user-defined technologies, which can be included in outputs. This can be used to define a custom cost case (e.g. $500/kW PV) or a new technology such as natural gas with 100% carbon capture. The CSV files are stored in the `extra_inputs` subfolders of each example system. A documentation file in that folder describes what to include in the file.
 
 ## PUDL Dependency
 
 This project pulls data from [PUDL](https://github.com/catalyst-cooperative/pudl). As such, it requires installation of PUDL to access a normalized sqlite database and some of the convienience PUDL functions.
 
 `catalystcoop.pudl` is included in the `environment.yml` file and will be installed automatically in the conda environment (see instructions below). Catalyst Cooperative will be creating versioned data releases of PUDL, which can be [accessed on Zenodo](https://doi.org/10.5281/zenodo.3653158). Download the zip file from Zenodo, unzip it, and find the sqlite database under `pudl_data/sqlite/pudl.sqlite`. Note that the version of `catalystcoop.pudl` software may change based on the database version you use. Look on the right-hand side of the zenodo archive to see what software version was used to compile the data. If the version in your conda environment does not match the version used to compile the data, you can change it in the `environment.yml` file or install a [different version](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-packages) using `mamba install catalystcoop.pudl=<your_version>`.
 
@@ -77,54 +60,41 @@
 
 4. pip-install an editable version of this project
 
 ```sh
 pip install -e .
 ```
 
-5. Download the PUDL database [from Zenodo](https://doi.org/10.5281/zenodo.3653158) or the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
+5. Download [the PUDL database](https://doi.org/10.5281/zenodo.3653158), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
 
-6. Download the additional PowerGenome database from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). It includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
+6. Download [additional PowerGenome data](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) that includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
 
-7. Download the appropriate renewable resource data files from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). There is a single set of generation profiles and resource group folders specific to different regional aggregations. Read through the [included README](https://docs.google.com/document/d/1p_zDk6ng4tvgL1v1ZAXkvY9b34FmaLqdWFlJmUHP1Eo/edit?usp=share_link) for more background. This folder contains:
+7. Download the appropriate [renewable resource data files](https://drive.google.com/drive/folders/1G9IHtY1RMZHUEXAmYQEb-mvzzhqun-Kb?usp=sharing). Read through the README for more background. This folder contains:
 
 - `generation_profiles` can be saved in a single place and used across multiple studies.
-- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the PowerGenome [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
+- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
 
-8. Download data files derived from NREL's EFS from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). These provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps and are used to both build up demand profiles in the future and create flexible demand resources that can shift their load.
+8. Download and unzip [data files derived from NREL's EFS](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=sharing) that provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps.
 
-9. Download distributed generation profiles from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing) compiled from NREL Cambium 2022 scenarios.
+9. Download and unzip [distributed generation profiles](https://drive.google.com/file/d/1kqBQle2CLET_BMZd0Y91o6AjfgunQKf4/view?usp=share_link) compiled from NREL Cambium 2022 scenarios.
 
 9. Create the file `PowerGenome/powergenome/.env`. In this file, add:
 
 - `PUDL_DB=YOUR_PATH_HERE` (your path to the PUDL database downloaded in step 5)
 - `PG_DB=YOUR_PATH_HERE` (your path to the additional PowerGenome data downloaded in step 6)
 - `RESOURCE_GROUP_PROFILES=YOUR_PATH_HERE` (your path to the folder with hourly wind/solar generation parquet files)
 - `EFS_DATA=YOUR_PATH_HERE` (your path to the folder with EFS derived data files)
 - `DISTRIBUTED_GEN_DATA=YOUR_PATH_HERE` (your path to the folder with distributed generation profiles)
 - OPTIONAL: `RESOURCE_GROUPS=YOUR_PATH_HERE` (your path to the resource groups data for a project -- **this can be included in your settings file instead of the .env file**)
 
 Quotation marks are only needed if your values contain spaces. The `.env` file is included in `.gitignore` and will not be synced with the repository.
 
-## Installation with a packaged version (pip/conda-forge)
-
-Installing Powergenome with pip has only been tested within a conda environment but it should work in other environment management systems. Make sure that you have an updated version of pip installed. If you hit dependency errors I suggest trying to install them using mamba or conda. PowerGenome has `catalystcoop.pudl` as a dependency, which has a large number of its own dependencies. I have not (yet) had to install `catalystcoop.pudl` using mamba but doing so may help clear up errors.
-
-Depending on your operating system you might also have issues installing some other packages from pip. The example code below is what works for me on a Mac, where python-snappy fails to build wheels.
-
-```sh
-(base) conda create -n powergenome python=3.10 pip python-snappy
-(base) conda activate powergenome
-(powergenome) pip install powergenome
-```
-
-PowerGenome has been submitted to conda-forge but is not yet available.
-
+## Installation a packaged version (pip/conda-forge)
 
-If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env_params.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
+If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
 
 ## Running code
 
 ### Suggested folder structure
 
 It is best practice to set up project folders outside of the cloned repository so that git doesn't track any new/changed files within the upper-level `PowerGenome` folder. Try copying one of the example systems (settings file and extra inputs) and modifying it. Copy the `notebooks` folder into your project folder, change the path to the settings file as needed, and run code in the notebooks. This can also be a good way to learn how data are created in PowerGenome and debug problem.
```

### Comparing `PowerGenome-0.6.1/PowerGenome.egg-info/PKG-INFO` & `PowerGenome-0.6.1a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowerGenome
-Version: 0.6.1
+Version: 0.6.1a0
 Summary: Create power system inputs for capacity expansion models
 Author-email: Greg Schivley <greg.schivley@princeton.edu>
 Maintainer-email: Greg Schivley <greg.schivley@princeton.edu>
 License: MIT
 Project-URL: Source, https://github.com/PowerGenome/PowerGenome
 Keywords: power system data,capacity expansion,two
 Classifier: Development Status :: 4 - Beta
@@ -41,19 +41,25 @@
 
 Because computational complexity and run times increase as the number of regions and generating unit clusters increases, a user might want only want to disaggregate regions and generating units close to the primary region of interest. For example, a study focused on clean electricity regulations in New Mexico might combine several states in the Pacific Northwest into a single region while also splitting Arizona combined cycle units into multiple clusters.
 
 The goal of PowerGenome is to let a user make all of these choices in a settings file and then run a single script that generates input files for the power system model. PowerGenome currently generates input files for [GenX](https://energy.mit.edu/wp-content/uploads/2017/10/Enhanced-Decision-Support-for-a-Changing-Electricity-Landscape.pdf), and we hope to expand to other models in the near future.
 
 ## Data
 
-PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files. All data files [are available here](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). 
+PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files.
 
-1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below). This file is available at the link above or you can download it from the Zenodo repository.
-2. A second sqlite database (`pg_misc_tables_efs.sqlite`) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
-3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios (`efs_files_utc`).
+1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below).
+2. A [second sqlite database (pg_misc_efs)](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
+3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios ([efs_files_utc](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=share_link)).
+
+There are also a few data files stored in this repository:
+
+- Regional cost multipliers for individual technologies developed by EIA (`data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`).
+- A simplified geojson version of EPA's shapefile for IPM regions (`data/ipm_regions_simple.geojson`).
+- Information on user-defined technologies, which can be included in outputs. This can be used to define a custom cost case (e.g. $500/kW PV) or a new technology such as natural gas with 100% carbon capture. The CSV files are stored in the `extra_inputs` subfolders of each example system. A documentation file in that folder describes what to include in the file.
 
 ## PUDL Dependency
 
 This project pulls data from [PUDL](https://github.com/catalyst-cooperative/pudl). As such, it requires installation of PUDL to access a normalized sqlite database and some of the convienience PUDL functions.
 
 `catalystcoop.pudl` is included in the `environment.yml` file and will be installed automatically in the conda environment (see instructions below). Catalyst Cooperative will be creating versioned data releases of PUDL, which can be [accessed on Zenodo](https://doi.org/10.5281/zenodo.3653158). Download the zip file from Zenodo, unzip it, and find the sqlite database under `pudl_data/sqlite/pudl.sqlite`. Note that the version of `catalystcoop.pudl` software may change based on the database version you use. Look on the right-hand side of the zenodo archive to see what software version was used to compile the data. If the version in your conda environment does not match the version used to compile the data, you can change it in the `environment.yml` file or install a [different version](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-packages) using `mamba install catalystcoop.pudl=<your_version>`.
 
@@ -77,54 +83,41 @@
 
 4. pip-install an editable version of this project
 
 ```sh
 pip install -e .
 ```
 
-5. Download the PUDL database [from Zenodo](https://doi.org/10.5281/zenodo.3653158) or the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
+5. Download [the PUDL database](https://doi.org/10.5281/zenodo.3653158), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
 
-6. Download the additional PowerGenome database from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). It includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
+6. Download [additional PowerGenome data](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) that includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
 
-7. Download the appropriate renewable resource data files from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). There is a single set of generation profiles and resource group folders specific to different regional aggregations. Read through the [included README](https://docs.google.com/document/d/1p_zDk6ng4tvgL1v1ZAXkvY9b34FmaLqdWFlJmUHP1Eo/edit?usp=share_link) for more background. This folder contains:
+7. Download the appropriate [renewable resource data files](https://drive.google.com/drive/folders/1G9IHtY1RMZHUEXAmYQEb-mvzzhqun-Kb?usp=sharing). Read through the README for more background. This folder contains:
 
 - `generation_profiles` can be saved in a single place and used across multiple studies.
-- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the PowerGenome [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
+- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
 
-8. Download data files derived from NREL's EFS from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). These provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps and are used to both build up demand profiles in the future and create flexible demand resources that can shift their load.
+8. Download and unzip [data files derived from NREL's EFS](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=sharing) that provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps.
 
-9. Download distributed generation profiles from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing) compiled from NREL Cambium 2022 scenarios.
+9. Download and unzip [distributed generation profiles](https://drive.google.com/file/d/1kqBQle2CLET_BMZd0Y91o6AjfgunQKf4/view?usp=share_link) compiled from NREL Cambium 2022 scenarios.
 
 9. Create the file `PowerGenome/powergenome/.env`. In this file, add:
 
 - `PUDL_DB=YOUR_PATH_HERE` (your path to the PUDL database downloaded in step 5)
 - `PG_DB=YOUR_PATH_HERE` (your path to the additional PowerGenome data downloaded in step 6)
 - `RESOURCE_GROUP_PROFILES=YOUR_PATH_HERE` (your path to the folder with hourly wind/solar generation parquet files)
 - `EFS_DATA=YOUR_PATH_HERE` (your path to the folder with EFS derived data files)
 - `DISTRIBUTED_GEN_DATA=YOUR_PATH_HERE` (your path to the folder with distributed generation profiles)
 - OPTIONAL: `RESOURCE_GROUPS=YOUR_PATH_HERE` (your path to the resource groups data for a project -- **this can be included in your settings file instead of the .env file**)
 
 Quotation marks are only needed if your values contain spaces. The `.env` file is included in `.gitignore` and will not be synced with the repository.
 
-## Installation with a packaged version (pip/conda-forge)
-
-Installing Powergenome with pip has only been tested within a conda environment but it should work in other environment management systems. Make sure that you have an updated version of pip installed. If you hit dependency errors I suggest trying to install them using mamba or conda. PowerGenome has `catalystcoop.pudl` as a dependency, which has a large number of its own dependencies. I have not (yet) had to install `catalystcoop.pudl` using mamba but doing so may help clear up errors.
-
-Depending on your operating system you might also have issues installing some other packages from pip. The example code below is what works for me on a Mac, where python-snappy fails to build wheels.
-
-```sh
-(base) conda create -n powergenome python=3.10 pip python-snappy
-(base) conda activate powergenome
-(powergenome) pip install powergenome
-```
-
-PowerGenome has been submitted to conda-forge but is not yet available.
-
+## Installation a packaged version (pip/conda-forge)
 
-If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env_params.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
+If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
 
 ## Running code
 
 ### Suggested folder structure
 
 It is best practice to set up project folders outside of the cloned repository so that git doesn't track any new/changed files within the upper-level `PowerGenome` folder. Try copying one of the example systems (settings file and extra inputs) and modifying it. Copy the `notebooks` folder into your project folder, change the path to the settings file as needed, and run code in the notebooks. This can also be a good way to learn how data are created in PowerGenome and debug problem.
```

### Comparing `PowerGenome-0.6.1/PowerGenome.egg-info/SOURCES.txt` & `PowerGenome-0.6.1a0/PowerGenome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/README.md` & `PowerGenome-0.6.1a0/PowerGenome.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: PowerGenome
+Version: 0.6.1a0
+Summary: Create power system inputs for capacity expansion models
+Author-email: Greg Schivley <greg.schivley@princeton.edu>
+Maintainer-email: Greg Schivley <greg.schivley@princeton.edu>
+License: MIT
+Project-URL: Source, https://github.com/PowerGenome/PowerGenome
+Keywords: power system data,capacity expansion,two
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
 # PowerGenome
 
 [![The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4426097.svg)](https://doi.org/10.5281/zenodo.4426096)
 [![pytest](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml/badge.svg)](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/PowerGenome/PowerGenome/branch/master/graph/badge.svg?token=7KJYLE3jOW)](https://codecov.io/gh/PowerGenome/PowerGenome)
@@ -18,19 +41,25 @@
 
 Because computational complexity and run times increase as the number of regions and generating unit clusters increases, a user might want only want to disaggregate regions and generating units close to the primary region of interest. For example, a study focused on clean electricity regulations in New Mexico might combine several states in the Pacific Northwest into a single region while also splitting Arizona combined cycle units into multiple clusters.
 
 The goal of PowerGenome is to let a user make all of these choices in a settings file and then run a single script that generates input files for the power system model. PowerGenome currently generates input files for [GenX](https://energy.mit.edu/wp-content/uploads/2017/10/Enhanced-Decision-Support-for-a-Changing-Electricity-Landscape.pdf), and we hope to expand to other models in the near future.
 
 ## Data
 
-PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files. All data files [are available here](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). 
+PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files.
+
+1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below).
+2. A [second sqlite database (pg_misc_efs)](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
+3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios ([efs_files_utc](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=share_link)).
+
+There are also a few data files stored in this repository:
 
-1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below). This file is available at the link above or you can download it from the Zenodo repository.
-2. A second sqlite database (`pg_misc_tables_efs.sqlite`) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
-3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios (`efs_files_utc`).
+- Regional cost multipliers for individual technologies developed by EIA (`data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`).
+- A simplified geojson version of EPA's shapefile for IPM regions (`data/ipm_regions_simple.geojson`).
+- Information on user-defined technologies, which can be included in outputs. This can be used to define a custom cost case (e.g. $500/kW PV) or a new technology such as natural gas with 100% carbon capture. The CSV files are stored in the `extra_inputs` subfolders of each example system. A documentation file in that folder describes what to include in the file.
 
 ## PUDL Dependency
 
 This project pulls data from [PUDL](https://github.com/catalyst-cooperative/pudl). As such, it requires installation of PUDL to access a normalized sqlite database and some of the convienience PUDL functions.
 
 `catalystcoop.pudl` is included in the `environment.yml` file and will be installed automatically in the conda environment (see instructions below). Catalyst Cooperative will be creating versioned data releases of PUDL, which can be [accessed on Zenodo](https://doi.org/10.5281/zenodo.3653158). Download the zip file from Zenodo, unzip it, and find the sqlite database under `pudl_data/sqlite/pudl.sqlite`. Note that the version of `catalystcoop.pudl` software may change based on the database version you use. Look on the right-hand side of the zenodo archive to see what software version was used to compile the data. If the version in your conda environment does not match the version used to compile the data, you can change it in the `environment.yml` file or install a [different version](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-packages) using `mamba install catalystcoop.pudl=<your_version>`.
 
@@ -54,54 +83,41 @@
 
 4. pip-install an editable version of this project
 
 ```sh
 pip install -e .
 ```
 
-5. Download the PUDL database [from Zenodo](https://doi.org/10.5281/zenodo.3653158) or the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
+5. Download [the PUDL database](https://doi.org/10.5281/zenodo.3653158), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
 
-6. Download the additional PowerGenome database from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). It includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
+6. Download [additional PowerGenome data](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) that includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
 
-7. Download the appropriate renewable resource data files from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). There is a single set of generation profiles and resource group folders specific to different regional aggregations. Read through the [included README](https://docs.google.com/document/d/1p_zDk6ng4tvgL1v1ZAXkvY9b34FmaLqdWFlJmUHP1Eo/edit?usp=share_link) for more background. This folder contains:
+7. Download the appropriate [renewable resource data files](https://drive.google.com/drive/folders/1G9IHtY1RMZHUEXAmYQEb-mvzzhqun-Kb?usp=sharing). Read through the README for more background. This folder contains:
 
 - `generation_profiles` can be saved in a single place and used across multiple studies.
-- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the PowerGenome [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
+- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
 
-8. Download data files derived from NREL's EFS from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). These provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps and are used to both build up demand profiles in the future and create flexible demand resources that can shift their load.
+8. Download and unzip [data files derived from NREL's EFS](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=sharing) that provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps.
 
-9. Download distributed generation profiles from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing) compiled from NREL Cambium 2022 scenarios.
+9. Download and unzip [distributed generation profiles](https://drive.google.com/file/d/1kqBQle2CLET_BMZd0Y91o6AjfgunQKf4/view?usp=share_link) compiled from NREL Cambium 2022 scenarios.
 
 9. Create the file `PowerGenome/powergenome/.env`. In this file, add:
 
 - `PUDL_DB=YOUR_PATH_HERE` (your path to the PUDL database downloaded in step 5)
 - `PG_DB=YOUR_PATH_HERE` (your path to the additional PowerGenome data downloaded in step 6)
 - `RESOURCE_GROUP_PROFILES=YOUR_PATH_HERE` (your path to the folder with hourly wind/solar generation parquet files)
 - `EFS_DATA=YOUR_PATH_HERE` (your path to the folder with EFS derived data files)
 - `DISTRIBUTED_GEN_DATA=YOUR_PATH_HERE` (your path to the folder with distributed generation profiles)
 - OPTIONAL: `RESOURCE_GROUPS=YOUR_PATH_HERE` (your path to the resource groups data for a project -- **this can be included in your settings file instead of the .env file**)
 
 Quotation marks are only needed if your values contain spaces. The `.env` file is included in `.gitignore` and will not be synced with the repository.
 
-## Installation with a packaged version (pip/conda-forge)
-
-Installing Powergenome with pip has only been tested within a conda environment but it should work in other environment management systems. Make sure that you have an updated version of pip installed. If you hit dependency errors I suggest trying to install them using mamba or conda. PowerGenome has `catalystcoop.pudl` as a dependency, which has a large number of its own dependencies. I have not (yet) had to install `catalystcoop.pudl` using mamba but doing so may help clear up errors.
-
-Depending on your operating system you might also have issues installing some other packages from pip. The example code below is what works for me on a Mac, where python-snappy fails to build wheels.
-
-```sh
-(base) conda create -n powergenome python=3.10 pip python-snappy
-(base) conda activate powergenome
-(powergenome) pip install powergenome
-```
-
-PowerGenome has been submitted to conda-forge but is not yet available.
-
+## Installation a packaged version (pip/conda-forge)
 
-If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env_params.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
+If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
 
 ## Running code
 
 ### Suggested folder structure
 
 It is best practice to set up project folders outside of the cloned repository so that git doesn't track any new/changed files within the upper-level `PowerGenome` folder. Try copying one of the example systems (settings file and extra inputs) and modifying it. Copy the `notebooks` folder into your project folder, change the path to the settings file as needed, and run code in the notebooks. This can also be a good way to learn how data are created in PowerGenome and debug problem.
```

### Comparing `PowerGenome-0.6.1/data/additional_technologies/AZ_additional_tech.csv` & `PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/additional_technologies/AZ_additional_tech_2030.csv` & `PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2030.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/additional_technologies/AZ_additional_tech_2045.csv` & `PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2045.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/additional_technologies/sample_additional_tech.csv` & `PowerGenome-0.6.1a0/data/additional_technologies/sample_additional_tech.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/coal_fgd/fgd_output.csv` & `PowerGenome-0.6.1a0/data/coal_fgd/fgd_output.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv` & `PowerGenome-0.6.1a0/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/cost_multipliers/EIA regional cost multipliers.csv` & `PowerGenome-0.6.1a0/data/cost_multipliers/EIA regional cost multipliers.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/cpi_data/cpi_data.csv` & `PowerGenome-0.6.1a0/data/cpi_data/cpi_data.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/data/ipm_regions_simple.geojson` & `PowerGenome-0.6.1a0/data/ipm_regions_simple.geojson`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/GenX.py` & `PowerGenome-0.6.1a0/powergenome/GenX.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/cluster/renewables.py` & `PowerGenome-0.6.1a0/powergenome/cluster/renewables.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/cluster_method.py` & `PowerGenome-0.6.1a0/powergenome/cluster_method.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/co2_pipeline_cost.py` & `PowerGenome-0.6.1a0/powergenome/co2_pipeline_cost.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/distributed_gen.py` & `PowerGenome-0.6.1a0/powergenome/distributed_gen.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/eia_opendata.py` & `PowerGenome-0.6.1a0/powergenome/eia_opendata.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/external_data.py` & `PowerGenome-0.6.1a0/powergenome/external_data.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/extract_pudl_data.py` & `PowerGenome-0.6.1a0/powergenome/extract_pudl_data.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/fuels.py` & `PowerGenome-0.6.1a0/powergenome/fuels.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/generators.py` & `PowerGenome-0.6.1a0/powergenome/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import collections
 import logging
-import os
 import re
 from numbers import Number
 from pathlib import Path
 from typing import Dict, List, Union
 from zipfile import BadZipFile
 
-os.environ["USE_PYGEOS"] = "0"
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pudl
 import requests
 import sqlalchemy
 from bs4 import BeautifulSoup
```

### Comparing `PowerGenome-0.6.1/powergenome/load_construction.py` & `PowerGenome-0.6.1a0/powergenome/load_construction.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/load_profiles.py` & `PowerGenome-0.6.1a0/powergenome/load_profiles.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/nrelatb.py` & `PowerGenome-0.6.1a0/powergenome/nrelatb.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/params.py` & `PowerGenome-0.6.1a0/powergenome/params.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/price_adjustment.py` & `PowerGenome-0.6.1a0/powergenome/price_adjustment.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/resource_clusters.py` & `PowerGenome-0.6.1a0/powergenome/resource_clusters.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/run_powergenome_multiple_outputs_cli.py` & `PowerGenome-0.6.1a0/powergenome/run_powergenome_multiple_outputs_cli.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/time_reduction.py` & `PowerGenome-0.6.1a0/powergenome/time_reduction.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/transmission.py` & `PowerGenome-0.6.1a0/powergenome/transmission.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1/powergenome/util.py` & `PowerGenome-0.6.1a0/powergenome/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import re
 import subprocess
 from collections.abc import Iterable
 from copy import deepcopy
 from pathlib import Path
 from typing import Dict, List, Tuple, Union
 
-os.environ["USE_PYGEOS"] = "0"
 import geopandas as gpd
 import pandas as pd
 import pudl
 import requests
 import sqlalchemy as sa
 import yaml
 from flatten_dict import flatten
@@ -60,23 +59,14 @@
     settings = apply_all_tag_to_regions(settings)
 
     for key in ["PUDL_DB", "PG_DB"]:
         # Add correct connection string prefix if it isn't there
         if settings.get(key):
             settings[key] = sqlalchemy_prefix(settings[key])
 
-    for key in [
-        "EFS_DATA",
-        "RESOURCE_GROUPS",
-        "DISTRIBUTED_GEN_DATA",
-        "RESOURCE_GROUP_PROFILES",
-    ]:
-        if settings.get(key):
-            settings[key] = Path(settings[key])
-
     return fix_param_names(settings)
 
 
 def sqlalchemy_prefix(db_path: str) -> str:
     """Check the database path and add sqlite prefix if needed
 
     Parameters
```

### Comparing `PowerGenome-0.6.1/pyproject.toml` & `PowerGenome-0.6.1a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66,<68", "wheel"] # , "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PowerGenome"
-version = "0.6.1"
+version = "0.6.1a"
 authors = [{ name = "Greg Schivley", email = "greg.schivley@princeton.edu" }]
 maintainers = [
     { name = "Greg Schivley", email = "greg.schivley@princeton.edu" },
 ]
 description = "Create power system inputs for capacity expansion models"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -24,22 +24,22 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "catalystcoop.pudl>=0.6.0, <=2022.11.30",
     "beautifulsoup4 >= 4.8.13",
-    "statsmodels>=0.12.2",
+    "statsmodels>=0.13",
     "python-dotenv",
     "flatten-dict",
     "ruamel.yaml",
     "pyyaml",
     "frozendict",
     "openpyxl>=3.0",
-    "geopandas>=0.11",
+    "geopandas>=0.12",
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["powergenome*", "data*"]
```

