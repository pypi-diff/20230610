# Comparing `tmp/NEMED-0.3.2.tar.gz` & `tmp/nemed-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMED-0.3.2.tar", max compression
+gzip compressed data, was "nemed-0.3.3.tar", max compression
```

## Comparing `NEMED-0.3.2.tar` & `nemed-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0     1518 2022-11-08 06:39:49.540019 NEMED-0.3.2/LICENSE
--rw-r--r--   0        0        0     2124 2023-01-15 08:37:58.282506 NEMED-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4737 2023-01-15 08:21:48.094722 NEMED-0.3.2/README.md
--rw-r--r--   0        0        0      331 2023-01-07 22:23:33.997114 NEMED-0.3.2/src/nemed/__init__.py
--rw-r--r--   0        0        0        0 2022-11-08 08:43:35.689633 NEMED-0.3.2/src/nemed/data/__init__.py
--rw-r--r--   0        0        0    31287 2023-01-01 10:48:29.604157 NEMED-0.3.2/src/nemed/data/duid_mapping.csv
--rw-r--r--   0        0        0    31508 2022-11-08 06:39:52.734494 NEMED-0.3.2/src/nemed/data/existing_gen_data_summary.csv
--rw-r--r--   0        0        0    24611 2023-01-01 10:06:21.374475 NEMED-0.3.2/src/nemed/data/plant_auxiliary/_plant_auxload_assumptions.csv
--rw-r--r--   0        0        0   132206 2023-01-01 09:36:05.866006 NEMED-0.3.2/src/nemed/data/plant_auxiliary/comparison.xlsx
--rw-r--r--   0        0        0      733 2023-01-10 01:57:38.564594 NEMED-0.3.2/src/nemed/data/plant_auxiliary/readme.txt
--rw-r--r--   0        0        0    64022 2023-01-11 23:29:08.377040 NEMED-0.3.2/src/nemed/data/plant_technology/_plant_techname_assumptions.csv
--rw-r--r--   0        0        0      733 2023-01-10 01:57:38.564594 NEMED-0.3.2/src/nemed/data/plant_technology/readme.txt
--rw-r--r--   0        0        0     4137 2023-01-15 05:54:45.003329 NEMED-0.3.2/src/nemed/defaults.py
--rw-r--r--   0        0        0    37203 2023-01-15 08:26:32.182650 NEMED-0.3.2/src/nemed/downloader.py
--rw-r--r--   0        0        0        0 2022-11-08 08:43:29.091576 NEMED-0.3.2/src/nemed/helper_functions/__init__.py
--rw-r--r--   0        0        0     1577 2023-01-01 07:13:27.624820 NEMED-0.3.2/src/nemed/helper_functions/helpers.py
--rw-r--r--   0        0        0     5346 2023-01-13 23:04:33.491308 NEMED-0.3.2/src/nemed/helper_functions/mod_nemosis.py
--rw-r--r--   0        0        0     6202 2023-01-15 08:34:58.330243 NEMED-0.3.2/src/nemed/helper_functions/mod_xml_cache.py
--rw-r--r--   0        0        0     6343 2023-01-15 08:33:33.512238 NEMED-0.3.2/src/nemed/nemed.py
--rw-r--r--   0        0        0    25468 2023-01-15 08:25:49.164972 NEMED-0.3.2/src/nemed/process.py
--rw-r--r--   0        0        0     5657 1970-01-01 00:00:00.000000 NEMED-0.3.2/setup.py
--rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 NEMED-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-06-10 00:39:54.604054 nemed-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2124 2023-06-10 01:12:40.837175 nemed-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4737 2023-06-10 00:39:54.630060 nemed-0.3.3/README.md
+-rw-r--r--   0        0        0      331 2023-06-10 00:39:56.933106 nemed-0.3.3/src/nemed/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 00:39:57.014972 nemed-0.3.3/src/nemed/data/__init__.py
+-rw-r--r--   0        0        0    31287 2023-06-10 00:38:54.650216 nemed-0.3.3/src/nemed/data/duid_mapping.csv
+-rw-r--r--   0        0        0    31508 2023-06-10 00:38:54.650216 nemed-0.3.3/src/nemed/data/existing_gen_data_summary.csv
+-rw-r--r--   0        0        0    24611 2023-06-10 00:39:57.015973 nemed-0.3.3/src/nemed/data/plant_auxiliary/_plant_auxload_assumptions.csv
+-rw-r--r--   0        0        0   132206 2023-06-10 00:39:57.018973 nemed-0.3.3/src/nemed/data/plant_auxiliary/comparison.xlsx
+-rw-r--r--   0        0        0      733 2023-06-10 00:39:57.019974 nemed-0.3.3/src/nemed/data/plant_auxiliary/readme.txt
+-rw-r--r--   0        0        0     4137 2023-06-10 00:39:57.032976 nemed-0.3.3/src/nemed/defaults.py
+-rw-r--r--   0        0        0    37203 2023-06-10 00:52:55.927467 nemed-0.3.3/src/nemed/downloader.py
+-rw-r--r--   0        0        0        0 2023-06-10 00:39:57.037977 nemed-0.3.3/src/nemed/helper_functions/__init__.py
+-rw-r--r--   0        0        0     1577 2023-06-10 00:39:57.038977 nemed-0.3.3/src/nemed/helper_functions/helpers.py
+-rw-r--r--   0        0        0     5346 2023-06-10 00:39:57.040978 nemed-0.3.3/src/nemed/helper_functions/mod_nemosis.py
+-rw-r--r--   0        0        0     6392 2023-06-10 01:02:56.010191 nemed-0.3.3/src/nemed/helper_functions/mod_xml_cache.py
+-rw-r--r--   0        0        0     6343 2023-06-10 00:39:57.053513 nemed-0.3.3/src/nemed/nemed.py
+-rw-r--r--   0        0        0    25468 2023-06-10 00:52:55.929856 nemed-0.3.3/src/nemed/process.py
+-rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 nemed-0.3.3/setup.py
+-rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 nemed-0.3.3/PKG-INFO
```

### Comparing `NEMED-0.3.2/LICENSE` & `nemed-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/pyproject.toml` & `nemed-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NEMED"
-version = "0.3.2"
+version = "0.3.3"
 description = "NEM Emissions Data tool"
 authors = ["Declan Heim","Shayan Naderi"]
 license = "Licence"
 readme = "README.md"
 
 # Main dependencies for the package via poetry. Package users will need these dependencies.
 [tool.poetry.dependencies]
```

### Comparing `NEMED-0.3.2/README.md` & `nemed-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/data/duid_mapping.csv` & `nemed-0.3.3/src/nemed/data/duid_mapping.csv`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/data/existing_gen_data_summary.csv` & `nemed-0.3.3/src/nemed/data/existing_gen_data_summary.csv`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/data/plant_auxiliary/_plant_auxload_assumptions.csv` & `nemed-0.3.3/src/nemed/data/plant_auxiliary/_plant_auxload_assumptions.csv`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/data/plant_auxiliary/comparison.xlsx` & `nemed-0.3.3/src/nemed/data/plant_auxiliary/comparison.xlsx`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/data/plant_auxiliary/readme.txt` & `nemed-0.3.3/src/nemed/data/plant_auxiliary/readme.txt`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/defaults.py` & `nemed-0.3.3/src/nemed/defaults.py`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/downloader.py` & `nemed-0.3.3/src/nemed/downloader.py`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/helper_functions/helpers.py` & `nemed-0.3.3/src/nemed/helper_functions/helpers.py`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/helper_functions/mod_nemosis.py` & `nemed-0.3.3/src/nemed/helper_functions/mod_nemosis.py`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/helper_functions/mod_xml_cache.py` & `nemed-0.3.3/src/nemed/helper_functions/mod_xml_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,22 @@
     base_name = "NEMPriceSetter_{year}{month}{day}{interval_number}00.xml"
     name = base_name.format(
         year=year, month=month, day=day, interval_number=interval_number
     )
     path_name = Path(self.cache_folder) / name
     name_OCD = name.replace(".xml", "_OCD.xml")
     path_name_OCD = Path(self.cache_folder) / name_OCD
+    name_zero = name.replace(".xml", "00.xml")
+    path_name_zero = Path(self.cache_folder) / name_zero
     if os.path.exists(path_name):
         return name
-    elif path_name_OCD:
+    elif os.path.exists(path_name_OCD):
         return name_OCD
+    elif os.path.exists(path_name_zero):
+        return name_zero
     else:
         return name
 
 
 def modpricesetter_download_xml_from_nemweb(self):
     """Modified function from nempy.historical_inputs.xml_cache
     """
```

### Comparing `NEMED-0.3.2/src/nemed/nemed.py` & `nemed-0.3.3/src/nemed/nemed.py`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/src/nemed/process.py` & `nemed-0.3.3/src/nemed/process.py`

 * *Files identical despite different names*

### Comparing `NEMED-0.3.2/setup.py` & `nemed-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['nemed', 'nemed.data', 'nemed.helper_functions']
 
 package_data = \
-{'': ['*'], 'nemed.data': ['plant_auxiliary/*', 'plant_technology/*']}
+{'': ['*'], 'nemed.data': ['plant_auxiliary/*']}
 
 install_requires = \
 ['datetime',
  'joblib>=1.2.0,<2.0.0',
  'nemosis',
  'nempy',
  'pandas>=1.2,<2.0',
@@ -20,15 +20,15 @@
  'plotly',
  'requests',
  'tqdm',
  'xmltodict']
 
 setup_kwargs = {
     'name': 'nemed',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'NEM Emissions Data tool',
     'long_description': '# NEMED\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Documentation Status](https://readthedocs.org/projects/nemed/badge/?version=latest)](https://nemed.readthedocs.io/en/latest/?badge=latest)\n\nNEMED[^1], or NEM Emissions Data, is a python package to retrieve and process historical emissions data of the National Electricity Market (NEM), reproduced by datasets published by the Australian Energy Market Operator (AEMO).\n\n[^1]: Not to be confused with *"Nemed", "Nimeth"* of the [Irish legend](https://en.wikipedia.org/wiki/Nemed), who was the leader of the third group of people to settle in Ireland.\n\n## Installation\n```bash\npip install nemed\n```\n\n## Introduction\n\nThis tool is designed to allow users to retrieve historical NEM regional emissions data, either total or marginal emissions, for any 5-minute dispatch interval or aggregations thereof. Total emissions data produced by NEMED is given as both absolute total emissions (tCO2-e) and as an emissions intensity index (tCO2-e/MWh). Marginal emissions data reflects the price setter of a particular region, yielding an emissions intensity index (tCO2-e/MWh) corresponding to a particular plant.\nAlthough data is published by AEMO via the [Carbon Dioxide Equivalent Intensity Index (CDEII) Procedure](https://www.aemo.com.au/energy-systems/electricity/national-electricity-market-nem/market-operations/settlements-and-payments/settlements/carbon-dioxide-equivalent-intensity-index) this only reflects a daily summary for each region by total and (average) emissions intensity.\n\n### How does NEMED calculate emissions?\nTotal Emissions are computed by considering 5-minute generation dispatch data for each generator in the NEM for each respective region, along with their CO2-equivalent emissions factors per unit (generator) level. A detailed method of the process to produce results for total emissions(tCO2-e) and the corresponding emisssions intensities can be found [here](https://nemed.readthedocs.io/en/latest/method.html). The tool is able to provide these metrics on a dispatch interval basis, or aggregated to hourly, daily, monthly or yearly measures. For more advanced users, the emissions associated with each generator and hence that generator\'s contribution to total regional emissions can be extracted.\n\nMarginal Emissions are computed by identifying the marginally dispatched generators from AEMO\'s Price Setter files, mapping emissions intensity metrics mentioned above and computing marginal emissions intensity (tCO2-e/MWh).\n\n### How accurate is NEMED?\nA series of [benchmark results](https://nemed.readthedocs.io/en/latest/examples/cdeii_benchmark.html) for total emissions shows a comparison between AEMO\'s daily CDEII reported emissions figures and NEMED\'s emissions figures which have been aggregated from a 5-minute dispatch-interval resolution to a daily basis.   \n\nThe [example](https://nemed.readthedocs.io/en/latest/examples/cdeii_benchmark.html) includes a region by region comparison for each metric, while an overview of the historical NEM Emissions Intensity produced using NEMED is shown here.\n![NEM Emissions Intensity](./docs/source/examples/charts_benchmark/intensity_NEM.png)\n\n## Usage\n\n### Examples\nExamples can be found in [NEMED\'s documentation](https://nemed.readthedocs.io/en/latest/examples/total_emissions.html).\n\n### Possible Use Cases\nSome example use cases of data produced from this tool include:\n- Analysis of historical emissions between NEM regions, generation technologies contributions to them and assessing the difference between total and marginal emissions.\n- Using emissions intensities traces (total and marginal) from NEMED in counter-factual optimisation models; studying the influence of shadow-pricing carbon or imposing carbon constraints.\n- Considering the emissions assosciated with grid-energy consumption for residential/C&I consumers, or in counterfactual studies of hypothetical EV usage or H2 electrolyser operation. \n\n## Contributing\nInterested in contributing? Check out the [contributing guidelines](CONTRIBUTING.md), which also includes steps to install `NEMED` for development.\n\nPlease note that this project is released with a [Code of Conduct](CONDUCT.md). By contributing to this project, you agree to abide by its terms.\n\n## License\n`NEMED` was created by Declan Heim and Shayan Naderi. It is licensed under the terms of the `BSD 3-Clause license`.\n\n## Credits\nThis package was created using the [`UNSW CEEM template`](https://github.com/UNSW-CEEM/ceem-python-template). It also adopts functionality from sister tools including [`NEMOSIS`](https://github.com/UNSW-CEEM/NEMOSIS) and [`NEMPY`](https://github.com/UNSW-CEEM/nempy).',
     'author': 'Declan Heim',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `NEMED-0.3.2/PKG-INFO` & `nemed-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: nemed
-Version: 0.3.2
+Version: 0.3.3
 Summary: NEM Emissions Data tool
 License: Licence
 Author: Declan Heim
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datetime
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: nemosis
 Requires-Dist: nempy
 Requires-Dist: pandas (>=1.2,<2.0)
 Requires-Dist: pathlib
 Requires-Dist: plotly
```

