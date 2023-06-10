# Comparing `tmp/spark_llm-0.1.2.tar.gz` & `tmp/spark_llm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_llm-0.1.2.tar", max compression
+gzip compressed data, was "spark_llm-0.1.3.tar", max compression
```

## Comparing `spark_llm-0.1.2.tar` & `spark_llm-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-07 23:43:47.653712 spark_llm-0.1.2/LICENSE
--rw-r--r--   0        0        0     1925 2023-06-08 22:10:10.249098 spark_llm-0.1.2/README.md
--rw-r--r--   0        0        0      903 2023-06-09 04:34:28.145833 spark_llm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-08 22:37:32.156425 spark_llm-0.1.2/spark_llm/__init__.py
--rw-r--r--   0        0        0     5272 2023-06-08 22:37:32.162648 spark_llm-0.1.2/spark_llm/prompt.py
--rw-r--r--   0        0        0     8829 2023-06-08 22:37:32.194595 spark_llm-0.1.2/spark_llm/spark_llm_assistant.py
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 spark_llm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1847 2023-06-10 06:58:48.977364 spark_llm-0.1.3/README.md
+-rw-r--r--   0        0        0      903 2023-06-10 07:02:10.271109 spark_llm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.3/spark_llm/__init__.py
+-rw-r--r--   0        0        0     5272 2023-06-09 17:49:03.119511 spark_llm-0.1.3/spark_llm/prompt.py
+-rw-r--r--   0        0        0     9146 2023-06-10 06:14:57.409593 spark_llm-0.1.3/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     2993 1970-01-01 00:00:00.000000 spark_llm-0.1.3/PKG-INFO
```

### Comparing `spark_llm-0.1.2/LICENSE` & `spark_llm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.2/README.md` & `spark_llm-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Spark-LLM
-
-Spark-LLM is a Python library that can assist in the development of Spark applications, including Spark Dataframe, Spark SQL, testings, and so on.
+# LLM Assistant for Apache Spark
 
 ## Installation
 
 ```bash
 pip install spark-llm
 ```
 
@@ -12,14 +10,15 @@
 ### Initialization
 ```python
 from langchain.chat_models import ChatOpenAI
 from spark_llm import SparkLLMAssistant
 
 llm = ChatOpenAI(model_name='gpt-4') # using gpt-4 can achieve better results
 assistant=SparkLLMAssistant(llm=llm)
+assistant.activate() # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 ```python
 auto_df=assistant.create_df("2022 USA national auto sales by brand")
 auto_df.show(n=5)
 ```
@@ -29,24 +28,24 @@
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
 | 4    | Honda     | 881201        | -33                  |
 | 5    | Hyundai   | 724265        | -2                   |
 
 ### DataFrame Transformation
 ```python
-auto_top_growth_df=assistant.transform_df(auto_df, "top brand with the highest growth")
+auto_top_growth_df=auto_df.llm_transform("top brand with the highest growth")
 auto_top_growth_df.show()
 ```
 | brand    | us_sales_2022 | sales_change_vs_2021 |
 |----------|---------------|----------------------|
 | Cadillac | 134726        | 14                   |
 
-### DataFrame Explaination
+### DataFrame Explanation
 ```python
-assistant.explain_df(auto_top_growth_df)
+auto_top_growth_df.llm_explain()
 ```
 
 > In summary, this dataframe is retrieving the brand with the highest sales change in 2022 compared to 2021. It presents the results sorted by sales change in descending order and only returns the top result.
 
 Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
```

### Comparing `spark_llm-0.1.2/pyproject.toml` & `spark_llm-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spark-llm"
-version = "0.1.2"
+version = "0.1.3"
 description = "LLM assistant for the development of Spark applications"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/gengliangwang/spark-llm"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `spark_llm-0.1.2/spark_llm/prompt.py` & `spark_llm-0.1.3/spark_llm/prompt.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.2/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.3/spark_llm/spark_llm_assistant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from functools import partial
 from typing import Callable, Optional, List
 from urllib.parse import urlparse
 
 import requests
 import tiktoken
 from bs4 import BeautifulSoup
 from langchain import LLMChain, GoogleSearchAPIWrapper
@@ -210,7 +211,14 @@
         )
         # If there is code block in the explain result, ignore it.
         if "```" in explain_result:
             summary = explain_result.split("```")[-1]
             return summary.strip()
         else:
             return explain_result
+
+    def activate(self):
+        """
+        Activates LLM utility functions for Spark DataFrame.
+        """
+        DataFrame.llm_transform = lambda df_instance, desc: self.transform_df(df_instance, desc)
+        DataFrame.llm_explain = lambda df_instance: self.explain_df(df_instance)
```

### Comparing `spark_llm-0.1.2/PKG-INFO` & `spark_llm-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-llm
-Version: 0.1.2
+Version: 0.1.3
 Summary: LLM assistant for the development of Spark applications
 Home-page: https://github.com/gengliangwang/spark-llm
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -24,17 +24,15 @@
 Requires-Dist: beautifulsoup4
 Requires-Dist: langchain
 Requires-Dist: pyspark
 Requires-Dist: requests
 Requires-Dist: tiktoken
 Description-Content-Type: text/markdown
 
-# Spark-LLM
-
-Spark-LLM is a Python library that can assist in the development of Spark applications, including Spark Dataframe, Spark SQL, testings, and so on.
+# LLM Assistant for Apache Spark
 
 ## Installation
 
 ```bash
 pip install spark-llm
 ```
 
@@ -42,14 +40,15 @@
 ### Initialization
 ```python
 from langchain.chat_models import ChatOpenAI
 from spark_llm import SparkLLMAssistant
 
 llm = ChatOpenAI(model_name='gpt-4') # using gpt-4 can achieve better results
 assistant=SparkLLMAssistant(llm=llm)
+assistant.activate() # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 ```python
 auto_df=assistant.create_df("2022 USA national auto sales by brand")
 auto_df.show(n=5)
 ```
@@ -59,24 +58,24 @@
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
 | 4    | Honda     | 881201        | -33                  |
 | 5    | Hyundai   | 724265        | -2                   |
 
 ### DataFrame Transformation
 ```python
-auto_top_growth_df=assistant.transform_df(auto_df, "top brand with the highest growth")
+auto_top_growth_df=auto_df.llm_transform("top brand with the highest growth")
 auto_top_growth_df.show()
 ```
 | brand    | us_sales_2022 | sales_change_vs_2021 |
 |----------|---------------|----------------------|
 | Cadillac | 134726        | 14                   |
 
-### DataFrame Explaination
+### DataFrame Explanation
 ```python
-assistant.explain_df(auto_top_growth_df)
+auto_top_growth_df.llm_explain()
 ```
 
 > In summary, this dataframe is retrieving the brand with the highest sales change in 2022 compared to 2021. It presents the results sorted by sales change in descending order and only returns the top result.
 
 Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
```

