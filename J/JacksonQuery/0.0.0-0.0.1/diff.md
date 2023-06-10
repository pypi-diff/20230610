# Comparing `tmp/JacksonQuery-0.0.0.tar.gz` & `tmp/JacksonQuery-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JacksonQuery-0.0.0.tar", last modified: Sat Jun 10 18:06:49 2023, max compression
+gzip compressed data, was "JacksonQuery-0.0.1.tar", last modified: Sat Jun 10 21:28:56 2023, max compression
```

## Comparing `JacksonQuery-0.0.0.tar` & `JacksonQuery-0.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 18:06:49.741703 JacksonQuery-0.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-10 18:06:49.648621 JacksonQuery-0.0.0/JacksonQuery.egg-info/
--rw-rw-rw-   0        0        0      549 2023-06-10 18:06:49.000000 JacksonQuery-0.0.0/JacksonQuery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-06-10 18:06:49.000000 JacksonQuery-0.0.0/JacksonQuery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 18:06:49.000000 JacksonQuery-0.0.0/JacksonQuery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      250 2023-06-10 18:06:49.000000 JacksonQuery-0.0.0/JacksonQuery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       36 2023-06-10 18:06:49.000000 JacksonQuery-0.0.0/JacksonQuery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      549 2023-06-10 18:06:49.741703 JacksonQuery-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-10 17:33:54.000000 JacksonQuery-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 18:06:49.732882 JacksonQuery-0.0.0/jacksonquery/
--rw-rw-rw-   0        0        0        0 2023-05-18 00:54:05.000000 JacksonQuery-0.0.0/jacksonquery/__init__.py
--rw-rw-rw-   0        0        0    10827 2023-06-09 00:44:17.000000 JacksonQuery-0.0.0/jacksonquery/classification_schema.py
--rw-rw-rw-   0        0        0     4860 2023-06-09 00:38:44.000000 JacksonQuery-0.0.0/jacksonquery/fee_extractor.py
--rw-rw-rw-   0        0        0     2304 2023-06-09 00:45:07.000000 JacksonQuery-0.0.0/jacksonquery/file_parser.py
--rw-rw-rw-   0        0        0     4781 2023-06-09 00:53:37.000000 JacksonQuery-0.0.0/jacksonquery/returns_extractor.py
--rw-rw-rw-   0        0        0     6833 2023-06-10 17:20:22.000000 JacksonQuery-0.0.0/jacksonquery/source_extractor.py
--rw-rw-rw-   0        0        0     2451 2023-06-09 01:24:57.000000 JacksonQuery-0.0.0/jacksonquery/stats_extractor.py
--rw-rw-rw-   0        0        0     5125 2023-06-09 01:27:31.000000 JacksonQuery-0.0.0/jacksonquery/tenure_extractor.py
--rw-rw-rw-   0        0        0     6983 2023-06-09 04:12:15.000000 JacksonQuery-0.0.0/jacksonquery/turnover_extractor.py
-drwxrwxrwx   0        0        0        0 2023-06-10 18:06:49.740706 JacksonQuery-0.0.0/portfolio_optimization/
--rw-rw-rw-   0        0        0        0 2023-05-18 00:54:05.000000 JacksonQuery-0.0.0/portfolio_optimization/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-06-09 04:17:34.000000 JacksonQuery-0.0.0/portfolio_optimization/benchmark_model.py
--rw-rw-rw-   0        0        0     1496 2023-06-09 04:20:30.000000 JacksonQuery-0.0.0/portfolio_optimization/factor_data.py
--rw-rw-rw-   0        0        0     2534 2023-06-09 04:20:30.000000 JacksonQuery-0.0.0/portfolio_optimization/factor_model.py
--rw-rw-rw-   0        0        0     1573 2023-06-09 14:16:06.000000 JacksonQuery-0.0.0/portfolio_optimization/optimization_config.py
--rw-rw-rw-   0        0        0     7858 2023-06-10 17:54:02.000000 JacksonQuery-0.0.0/portfolio_optimization/optimization_data.py
--rw-rw-rw-   0        0        0     4897 2023-06-09 04:48:14.000000 JacksonQuery-0.0.0/portfolio_optimization/optimization_inputs.py
--rw-rw-rw-   0        0        0    19712 2023-06-09 04:53:50.000000 JacksonQuery-0.0.0/portfolio_optimization/optimization_model.py
--rw-rw-rw-   0        0        0    10897 2023-06-09 04:55:22.000000 JacksonQuery-0.0.0/portfolio_optimization/performance.py
--rw-rw-rw-   0        0        0       42 2023-06-10 18:06:49.741703 JacksonQuery-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1302 2023-06-10 17:25:49.000000 JacksonQuery-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:28:56.235919 JacksonQuery-0.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-10 21:28:56.225901 JacksonQuery-0.0.1/JacksonQuery.egg-info/
+-rw-rw-rw-   0        0        0     3226 2023-06-10 21:28:56.000000 JacksonQuery-0.0.1/JacksonQuery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-06-10 21:28:56.000000 JacksonQuery-0.0.1/JacksonQuery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 21:28:56.000000 JacksonQuery-0.0.1/JacksonQuery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      250 2023-06-10 21:28:56.000000 JacksonQuery-0.0.1/JacksonQuery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       36 2023-06-10 21:28:56.000000 JacksonQuery-0.0.1/JacksonQuery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3226 2023-06-10 21:28:56.235919 JacksonQuery-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2667 2023-06-10 21:11:54.000000 JacksonQuery-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 21:28:56.229938 JacksonQuery-0.0.1/jacksonquery/
+-rw-rw-rw-   0        0        0        0 2023-05-18 00:54:05.000000 JacksonQuery-0.0.1/jacksonquery/__init__.py
+-rw-rw-rw-   0        0        0    10827 2023-06-09 00:44:17.000000 JacksonQuery-0.0.1/jacksonquery/classification_schema.py
+-rw-rw-rw-   0        0        0     4860 2023-06-09 00:38:44.000000 JacksonQuery-0.0.1/jacksonquery/fee_extractor.py
+-rw-rw-rw-   0        0        0     2217 2023-06-10 18:29:49.000000 JacksonQuery-0.0.1/jacksonquery/file_parser.py
+-rw-rw-rw-   0        0        0     4781 2023-06-09 00:53:37.000000 JacksonQuery-0.0.1/jacksonquery/returns_extractor.py
+-rw-rw-rw-   0        0        0     6833 2023-06-10 17:20:22.000000 JacksonQuery-0.0.1/jacksonquery/source_extractor.py
+-rw-rw-rw-   0        0        0     2451 2023-06-09 01:24:57.000000 JacksonQuery-0.0.1/jacksonquery/stats_extractor.py
+-rw-rw-rw-   0        0        0     5125 2023-06-09 01:27:31.000000 JacksonQuery-0.0.1/jacksonquery/tenure_extractor.py
+-rw-rw-rw-   0        0        0     6983 2023-06-09 04:12:15.000000 JacksonQuery-0.0.1/jacksonquery/turnover_extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:28:56.234922 JacksonQuery-0.0.1/portfolio_optimization/
+-rw-rw-rw-   0        0        0        0 2023-05-18 00:54:05.000000 JacksonQuery-0.0.1/portfolio_optimization/__init__.py
+-rw-rw-rw-   0        0        0     3297 2023-06-10 18:29:33.000000 JacksonQuery-0.0.1/portfolio_optimization/benchmark_model.py
+-rw-rw-rw-   0        0        0     1496 2023-06-09 04:20:30.000000 JacksonQuery-0.0.1/portfolio_optimization/factor_data.py
+-rw-rw-rw-   0        0        0     2534 2023-06-09 04:20:30.000000 JacksonQuery-0.0.1/portfolio_optimization/factor_model.py
+-rw-rw-rw-   0        0        0     1573 2023-06-09 14:16:06.000000 JacksonQuery-0.0.1/portfolio_optimization/optimization_config.py
+-rw-rw-rw-   0        0        0     7858 2023-06-10 17:54:02.000000 JacksonQuery-0.0.1/portfolio_optimization/optimization_data.py
+-rw-rw-rw-   0        0        0     4897 2023-06-09 04:48:14.000000 JacksonQuery-0.0.1/portfolio_optimization/optimization_inputs.py
+-rw-rw-rw-   0        0        0    19712 2023-06-09 04:53:50.000000 JacksonQuery-0.0.1/portfolio_optimization/optimization_model.py
+-rw-rw-rw-   0        0        0    10897 2023-06-09 04:55:22.000000 JacksonQuery-0.0.1/portfolio_optimization/performance.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 21:28:56.237022 JacksonQuery-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1308 2023-06-10 20:18:52.000000 JacksonQuery-0.0.1/setup.py
```

### Comparing `JacksonQuery-0.0.0/JacksonQuery.egg-info/SOURCES.txt` & `JacksonQuery-0.0.1/JacksonQuery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/jacksonquery/classification_schema.py` & `JacksonQuery-0.0.1/jacksonquery/classification_schema.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/jacksonquery/fee_extractor.py` & `JacksonQuery-0.0.1/jacksonquery/fee_extractor.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/jacksonquery/file_parser.py` & `JacksonQuery-0.0.1/jacksonquery/file_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     :param filepath: (str) Path to the PDF file.
     :return: (list) List of strings.
     """
     raw = parser.from_file(filepath)
     string_list = raw.get('content').split('\n')
     string_list = list(filter(None, string_list))  # filter Nones
     string_list = [s for s in string_list if s != ' ']  # filter whitespaces
-    # string_list = [s.strip() for s in string_list]  # strip leading/trailing whitespace
+
     return string_list
 
 
 def parse_names(string_list):
     """
     Parses a list of strings into a list of subaccount names.
 
@@ -24,14 +24,15 @@
     :return: (list) List of subaccount names.
     """
     section_name = 'TABLE OF CONTENTS '
     subaccount_names = string_list[string_list.index(section_name) + 5:string_list.index('Additional Information '
                                                                                          'About the Funds 772 ')]
     for s in subaccount_names:
         subaccount_names[subaccount_names.index(s)] = ' '.join(s.split(' ')[:-2])
+
     return subaccount_names
 
 
 def split_into_sublists(string_list, subaccount_names):
     """
     Splits a list of strings into a list of sublists, where each sublist is a subaccount.
```

### Comparing `JacksonQuery-0.0.0/jacksonquery/returns_extractor.py` & `JacksonQuery-0.0.1/jacksonquery/returns_extractor.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/jacksonquery/source_extractor.py` & `JacksonQuery-0.0.1/jacksonquery/source_extractor.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/jacksonquery/stats_extractor.py` & `JacksonQuery-0.0.1/jacksonquery/stats_extractor.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/jacksonquery/tenure_extractor.py` & `JacksonQuery-0.0.1/jacksonquery/tenure_extractor.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/jacksonquery/turnover_extractor.py` & `JacksonQuery-0.0.1/jacksonquery/turnover_extractor.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/benchmark_model.py` & `JacksonQuery-0.0.1/portfolio_optimization/benchmark_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     benchmark_portfolio = pd.DataFrame({
         US_EQUITY_BENCHMARK: [0.6269],
         INTERNATIONAL_EQUITY_BENCHMARK: [0.1240],
         FIXED_INCOME_BENCHMARK: [0.2494]
     }).T
     benchmark_portfolio.columns = ['Weighting%']
     benchmark_portfolio = round(benchmark_portfolio / benchmark_portfolio.sum(), 4)
+
     return benchmark_portfolio
 
 
 def get_market_portfolio_prices_and_returns():
     """
     Returns the market portfolio prices and returns for the JNL Mellon model.
 
@@ -38,14 +39,15 @@
     subaccount_prices = od.get_subaccount_prices()
     market_portfolio_prices = pd.DataFrame(index=subaccount_prices.index)
     market_portfolio_prices['Market_Portfolio_Price'] = subaccount_prices.mul(
         benchmark_portfolio['Weighting%']
     ).sum(axis=1)
     market_portfolio_prices = round((market_portfolio_prices / market_portfolio_prices.iloc[0])*100, 4)
     market_portfolio_returns = round(market_portfolio_prices.pct_change().dropna(), 4)
+
     return market_portfolio_prices, market_portfolio_returns
 
 
 def display_benchmark_portfolio():
     """
     Displays the benchmark portfolio for the JNL Mellon model.
```

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/factor_data.py` & `JacksonQuery-0.0.1/portfolio_optimization/factor_data.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/factor_model.py` & `JacksonQuery-0.0.1/portfolio_optimization/factor_model.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/optimization_config.py` & `JacksonQuery-0.0.1/portfolio_optimization/optimization_config.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/optimization_data.py` & `JacksonQuery-0.0.1/portfolio_optimization/optimization_data.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/optimization_inputs.py` & `JacksonQuery-0.0.1/portfolio_optimization/optimization_inputs.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/optimization_model.py` & `JacksonQuery-0.0.1/portfolio_optimization/optimization_model.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/portfolio_optimization/performance.py` & `JacksonQuery-0.0.1/portfolio_optimization/performance.py`

 * *Files identical despite different names*

### Comparing `JacksonQuery-0.0.0/setup.py` & `JacksonQuery-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='JacksonQuery',
-    version='0.0.0',
+    version='0.0.1',
     description='Automated interaction and data extraction tool for Jackson National Life Insurance website',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Nathan Ramos, CFA®',
     author_email='info@nrcapitalmanagement.com',
-    url='https://github.com/username/JacksonQuery',
+    url='https://github.com/nathanramoscfa/JacksonQuery',
     packages=find_packages(),
     install_requires=[
         'beautifulsoup4>=4.12.2',
         'bt>=0.2.9',
         'ffn>=0.3.6',
         'fuzzywuzzy>=0.18.0',
         'keyring>=23.13.1',
```

