# Comparing `tmp/langkit-0.0.1b4.tar.gz` & `tmp/langkit-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1b4.tar", max compression
+gzip compressed data, was "langkit-0.0.1b5.tar", max compression
```

## Comparing `langkit-0.0.1b4.tar` & `langkit-0.0.1b5.tar`

### file list

```diff
@@ -1,21 +1,44 @@
--rw-r--r--   0        0        0     2259 2023-05-26 20:55:15.988991 langkit-0.0.1b4/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b4/LICENSE
--rw-r--r--   0        0        0      706 2023-05-19 23:22:41.142537 langkit-0.0.1b4/langkit/__init__.py
--rw-r--r--   0        0        0    16075 2023-05-26 20:49:07.178991 langkit-0.0.1b4/langkit/examples/GPT_Intro_to_LangKit.ipynb
--rw-r--r--   0        0        0      750 2023-05-26 20:48:57.228991 langkit-0.0.1b4/langkit/injections.py
--rw-r--r--   0        0        0     1047 2023-05-26 04:00:38.203377 langkit-0.0.1b4/langkit/input_output.py
--rw-r--r--   0        0        0      778 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2962 2023-05-26 20:48:57.228991 langkit-0.0.1b4/langkit/regexes.py
--rw-r--r--   0        0        0      451 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/sentiment.py
--rw-r--r--   0        0        0      714 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/tests/conftest.py
--rw-r--r--   0        0        0     2152 2023-05-26 20:49:07.188991 langkit-0.0.1b4/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2150 2023-05-26 04:00:38.203377 langkit-0.0.1b4/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/tests/test_themes.py
--rw-r--r--   0        0        0     3235 2023-05-26 20:48:57.228991 langkit-0.0.1b4/langkit/textstat.py
--rw-r--r--   0        0        0     8896 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/themes.json.txt
--rw-r--r--   0        0        0     2869 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/themes.py
--rw-r--r--   0        0        0      728 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/transformer.py
--rw-r--r--   0        0        0      753 2023-05-26 20:54:04.228991 langkit-0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 langkit-0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b5/LICENSE
+-rw-r--r--   0        0        0     2852 2023-06-09 23:51:13.157907 langkit-0.0.1b5/README.md
+-rw-r--r--   0        0        0      998 2023-06-09 23:51:13.157907 langkit-0.0.1b5/langkit/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-09 23:51:13.157907 langkit-0.0.1b5/langkit/all_metrics.py
+-rw-r--r--   0        0        0      140 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/config/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/config/environment.py
+-rw-r--r--   0        0        0     1260 2023-06-09 23:51:13.157907 langkit-0.0.1b5/langkit/docs/features/quality.md
+-rw-r--r--   0        0        0     1768 2023-06-09 23:51:13.157907 langkit-0.0.1b5/langkit/docs/features/relevance.md
+-rw-r--r--   0        0        0     1886 2023-06-07 22:19:42.247907 langkit-0.0.1b5/langkit/docs/features/security.md
+-rw-r--r--   0        0        0     1364 2023-06-07 22:19:42.247907 langkit-0.0.1b5/langkit/docs/features/sentiment.md
+-rw-r--r--   0        0        0    10756 2023-06-09 23:51:13.157907 langkit-0.0.1b5/langkit/docs/modules.md
+-rw-r--r--   0        0        0     9284 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0     7194 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/examples/Intro_to_Langkit.ipynb
+-rw-r--r--   0        0        0   262428 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0    21888 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     5449 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0     1362 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/injections.py
+-rw-r--r--   0        0        0     2210 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/input_output.py
+-rw-r--r--   0        0        0      297 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/light_metrics.py
+-rw-r--r--   0        0        0      499 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/llm_metrics.py
+-rw-r--r--   0        0        0       75 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/openai/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/openai/openai.py
+-rw-r--r--   0        0        0     1741 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/openai_wrapper.py
+-rw-r--r--   0        0        0      793 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2962 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/regexes.py
+-rw-r--r--   0        0        0      943 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/sentiment.py
+-rw-r--r--   0        0        0     3970 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     1078 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/tests/test_injections.py
+-rw-r--r--   0        0        0     2308 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0     2150 2023-05-26 04:00:38.203377 langkit-0.0.1b5/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b5/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0      798 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/tests/test_toxicity.py
+-rw-r--r--   0        0        0     3781 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/textstat.py
+-rw-r--r--   0        0        0     8896 2023-05-19 23:17:27.872537 langkit-0.0.1b5/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b5/langkit/themes.json.txt
+-rw-r--r--   0        0        0     3652 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/themes.py
+-rw-r--r--   0        0        0      679 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/topics.py
+-rw-r--r--   0        0        0     1305 2023-06-09 23:51:13.167907 langkit-0.0.1b5/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b5/langkit/transformer.py
+-rw-r--r--   0        0        0    23462 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/whylogs/reference_chats.json
+-rw-r--r--   0        0        0      474 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/whylogs/rolling_logger.py
+-rw-r--r--   0        0        0      993 2023-06-10 01:05:05.107906 langkit-0.0.1b5/langkit/whylogs/samples.py
+-rw-r--r--   0        0        0      902 2023-06-10 01:05:05.117906 langkit-0.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 langkit-0.0.1b5/PKG-INFO
```

### Comparing `langkit-0.0.1b4/DESCRIPTION.md` & `langkit-0.0.1b5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # LangKit
 
+![LangKit graphic](static/img/LangKit_graphic.png)
+
 **LangKit** is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
 The generated profiles can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
 
 ## Motivation
 
 Productionizing language models, including LLMs, comes with a range of risks due to the infinite amount of input combinations, which can elicit an infinite amount of outputs. The unstructured nature of text poses a challenge in the ML observability space - a challenge worth solving, since the lack of visibility on the model's behavior can have serious consequences.
 
 ## Features
 
 The currently supported metrics include:
 
-- readability score
-- complexity and grade scores
-- sentiment analysis
-- patterns - count of strings matching a user-defined regex pattern group
-- jailbreaks - similarity scores with respect to known jailbreak attempts and prompt injection attacks
-- refusals - similarity scores with respect to known LLM refusal of service responses
+- [Text Quality](langkit/docs/features/quality.md)
+  - readability score
+  - complexity and grade scores
+- [Text Relevance](langkit/docs/features/relevance.md)
+  - Similarity scores between prompt/responses
+  - Similarity scores against user-defined themes
+- [Security and Privacy](langkit/docs/features/security.md)
+  - patterns - count of strings matching a user-defined regex pattern group
+  - jailbreaks - similarity scores with respect to known jailbreak attempts
+  - prompt injection - similarity scores with respect to known prompt injection attacks
+  - refusals - similarity scores with respect to known LLM refusal of service responses
+- [Sentiment and Toxicity](langkit/docs/features/sentiment.md)
+  - sentiment analysis
+  - toxicity analysis
 
 ## Installation
 
 To install LangKit, use the Python Package Index (PyPI) as follows:
 
 ```bash
 pip install langkit
@@ -35,14 +45,18 @@
 from whylogs.experimental.core.metrics.udf_metric import generate_udf_schema
 from whylogs.core.schema import DeclarativeSchema
 import whylogs as why
 from langkit.sentiment import *
 from langkit.textstat import *
 
 text_schema = DeclarativeSchema(generate_udf_schema())
-results = why.log({"prompt": "Hello,", "response": "World!"}, schema=text_schema)
+results = why.log({"prompt": "hello!", "response": "world!"}, schema=text_schema)
 
 ```
 
 The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules.
 
 More examples are available [here](https://github.com/whylabs/LanguageToolkit/tree/main/langkit/examples).
+
+## Modules
+
+You can have more information about the different modules and their metrics [here](langkit/docs/modules.md).
```

### Comparing `langkit-0.0.1b4/LICENSE` & `langkit-0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b4/langkit/input_output.py` & `langkit-0.0.1b5/langkit/input_output.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,64 @@
+from logging import getLogger
 from typing import Optional
+import pandas as pd
 
 from sentence_transformers import util
 from whylogs.experimental.core.udf_schema import register_dataset_udf
 
 from langkit.transformer import load_model
 
 from . import LangKitConfig
 
 lang_config = LangKitConfig()
 _transformer_model = None
 _transformer_name = None
 
+diagnostic_logger = getLogger(__name__)
+
 
 def init(transformer_name: Optional[str] = None):
     global _transformer_model, _transformer_name
     if transformer_name is None:
         transformer_name = lang_config.transformer_name
     _transformer_model = load_model(transformer_name)
     _transformer_name = transformer_name
 
 
 init()
 
 
 @register_dataset_udf(["prompt", "response"], "response.relevance_to_prompt")
 def similarity_MiniLM_L6_v2(text):
-    x = text["prompt"]
-    y = text["response"]
-    # below assumes text is Dict[str, str], no pandas support
-    embedding_1 = _transformer_model.encode(x, convert_to_tensor=True)
-    embedding_2 = _transformer_model.encode(y, convert_to_tensor=True)
-    similarity = util.pytorch_cos_sim(embedding_1, embedding_2)
-    return similarity.item()
+    if _transformer_model is None:
+        raise ValueError(
+            "response.relevance_to_prompt must have a transformer model initialized before use."
+        )
+
+    if not isinstance(text, pd.DataFrame):
+        result = None
+        try:
+            x = text["prompt"]
+            y = text["response"]
+            embedding_1 = _transformer_model.encode(x, convert_to_tensor=True)
+            embedding_2 = _transformer_model.encode(y, convert_to_tensor=True)
+            similarity = util.pytorch_cos_sim(embedding_1, embedding_2)
+            result = similarity.item()
+        except Exception as e:
+            diagnostic_logger.warning(
+                f"Message({text}) caused similarity_MiniLM_L6_v2 to encounter error: {e}"
+            )
+        return result
+    else:
+        series_result = []
+        for x, y in zip(text["prompt"], text["response"]):
+            try:
+                embedding_1 = _transformer_model.encode(x, convert_to_tensor=True)
+                embedding_2 = _transformer_model.encode(y, convert_to_tensor=True)
+                similarity = util.pytorch_cos_sim(embedding_1, embedding_2)
+                series_result.append(similarity.item())
+            except Exception as e:
+                diagnostic_logger.warning(
+                    f"pandas {text} caused similarity_MiniLM_L6_v2 to encounter error: {e}"
+                )
+        return series_result
+    return 0
```

### Comparing `langkit-0.0.1b4/langkit/pattern_groups.json` & `langkit-0.0.1b5/langkit/pattern_groups.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {'0': "{'expressions': ['\\\\b\\\\d{4}[- ]?(\\\\d{4}[- ]?){2,3}\\\\d{4}\\\\b']}",*

 * * 'delete': '[0]',*

 * * 'insert': "[(4, OrderedDict([('expressions', "*

 * *           '["[A-Za-z0-9._+\\\\-\\\\\']+@[A-Za-z0-9.\\\\-]+\\\\.[A-Za-z]{2,}"]), (\'name\', '*

 * *           "'email address')]))]"}*

```diff
@@ -1,17 +1,11 @@
 [
     {
         "expressions": [
-            "[A-Za-z0-9._+\\-\\']+@[A-Za-z0-9.\\-]+\\.[A-Za-z]{2,}"
-        ],
-        "name": "email address"
-    },
-    {
-        "expressions": [
-            "\\b(?:\\d[ -]*?){13,16}\\b"
+            "\\b\\d{4}[- ]?(\\d{4}[- ]?){2,3}\\d{4}\\b"
         ],
         "name": "credit card number"
     },
     {
         "expressions": [
             "(?!(\\d){3}(-| |)\\1{2}\\2\\1{4})(?!666|000|9\\d{2})(\\b\\d{3}(-| |)(?!00)\\d{2}\\4(?!0{4})\\d{4}\\b)"
         ],
@@ -24,9 +18,15 @@
         "name": "phone number"
     },
     {
         "expressions": [
             "\\d+(\\s+(N|S|E|W|NE|NW|SE|SW)\\.?)?\\s+[0-9]{0,5}[a-zA-Z]+\\s+(?:Street|St|Road|Rd|Avenue|Ave|Boulevard|Blvd|Drive|Dr|Court|Ct|Lane|Ln|Square|Sq)"
         ],
         "name": "mailing address"
+    },
+    {
+        "expressions": [
+            "[A-Za-z0-9._+\\-\\']+@[A-Za-z0-9.\\-]+\\.[A-Za-z]{2,}"
+        ],
+        "name": "email address"
     }
 ]
```

### Comparing `langkit-0.0.1b4/langkit/regexes.py` & `langkit-0.0.1b5/langkit/regexes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b4/langkit/tests/test_input_output.py` & `langkit-0.0.1b5/langkit/tests/test_input_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         if {"prompt", "response"}.issubset(set(interaction.keys())):
             similarity_median = (
                 result.view()
                 .get_column(column_name)
                 .get_metric("distribution")
                 .to_summary_dict()["median"]
             )
+            if similarity_median is None:
+                print(interaction)
+                print(result.view().get_column(column_name).to_summary_dict())
             assert (similarity_median is None and not texty(interaction)) or (
                 texty(interaction) and (-1.1 <= similarity_median <= 1.1)
             )
             assert (
                 "frequent_items/frequent_strings"
                 not in result.view().get_column("prompt").to_summary_dict()
             )
```

### Comparing `langkit-0.0.1b4/langkit/tests/test_patterns.py` & `langkit-0.0.1b5/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b4/langkit/tests/test_themes.py` & `langkit-0.0.1b5/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b4/langkit/textstat.py` & `langkit-0.0.1b5/langkit/textstat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,89 @@
+from logging import getLogger
 import textstat
 from whylogs.core.datatypes import String
 from whylogs.experimental.core.metrics.udf_metric import register_metric_udf
 
+
+diagnostic_logger = getLogger(__name__)
+
 # score metrics
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="text_standard_component")
 def flesch_kincaid_grade(text: str) -> float:
     return textstat.textstat.flesch_kincaid_grade(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="text_standard_component")
 def flesch_reading_ease(text: str) -> float:
     return textstat.textstat.flesch_reading_ease(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="text_standard_component")
 def smog_index(text: str) -> float:
     return textstat.textstat.smog_index(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="text_standard_component")
 def coleman_liau_index(text: str) -> float:
     return textstat.textstat.coleman_liau_index(text)
 
 
 @register_metric_udf(col_type=String)
 def automated_readability_index(text: str) -> float:
     return textstat.textstat.automated_readability_index(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="text_standard_component")
 def dale_chall_readability_score(text: str) -> float:
     return textstat.textstat.dale_chall_readability_score(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="text_standard_component")
 def linsear_write_formula(text: str) -> float:
     return textstat.textstat.linsear_write_formula(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="text_standard_component")
 def gunning_fog(text: str) -> float:
     return textstat.textstat.gunning_fog(text)
 
 
 @register_metric_udf(col_type=String)
 def aggregate_reading_level(text: str) -> float:
-    return textstat.textstat.text_standard(text)
+    return textstat.textstat.text_standard(text, float_output=True)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="es")
 def fernandez_huerta(text: str) -> float:
     return textstat.textstat.fernandez_huerta(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="es")
 def szigriszt_pazos(text: str) -> float:
     return textstat.textstat.szigriszt_pazos(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="es")
 def gutierrez_polini(text: str) -> float:
     return textstat.textstat.gutierrez_polini(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="es")
 def crawford(text: str) -> float:
     return textstat.textstat.crawford(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="it")
 def gulpease_index(text: str) -> float:
     return textstat.textstat.gulpease_index(text)
 
 
-@register_metric_udf(col_type=String)
+@register_metric_udf(col_type=String, schema_name="ar")
 def osman(text: str) -> float:
     return textstat.textstat.osman(text)
 
 
 # count metrics
 
 
@@ -117,7 +121,11 @@
 def monosyllable_count(text: str) -> float:
     return textstat.textstat.monosyllabcount(text)
 
 
 @register_metric_udf(col_type=String)
 def difficult_words(text: str) -> float:
     return textstat.textstat.difficult_words(text)
+
+
+def init():
+    diagnostic_logger.info("Initialized textstat metrics.")
```

### Comparing `langkit-0.0.1b4/langkit/themes.json` & `langkit-0.0.1b5/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b4/langkit/themes.py` & `langkit-0.0.1b5/langkit/themes.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,31 +24,37 @@
         jailbreak_embeddings = [
             _transformer_model.encode(s, convert_to_tensor=True)
             for s in _theme_groups["jailbreaks"]
         ]
 
         @register_metric_udf(col_type=String)
         def jailbreak_similarity(text: str) -> float:
+            if _transformer_model is None:
+                raise ValueError("Must initialize a transformer before calling encode!")
             similarities = []
+            text_embedding = _transformer_model.encode(text, convert_to_tensor=True)
             for embedding in jailbreak_embeddings:
-                similarity = get_subject_similarity(text, embedding)
+                similarity = get_embeddings_similarity(text_embedding, embedding)
                 similarities.append(similarity)
             return max(similarities)
 
     if "refusals" in _theme_groups:
         refusal_embeddings = [
             _transformer_model.encode(s, convert_to_tensor=True)
             for s in _theme_groups["refusals"]
         ]
 
         @register_metric_udf(col_type=String)
         def refusal_similarity(text: str) -> float:
+            if _transformer_model is None:
+                raise ValueError("Must initialize a transformer before calling encode!")
             similarities = []
+            text_embedding = _transformer_model.encode(text, convert_to_tensor=True)
             for embedding in refusal_embeddings:
-                similarity = get_subject_similarity(text, embedding)
+                similarity = get_embeddings_similarity(text_embedding, embedding)
                 similarities.append(similarity)
             return max(similarities)
 
 
 def load_themes(json_path: str):
     try:
         skip = False
@@ -84,8 +90,17 @@
     if _transformer_model is None:
         raise ValueError("Must initialize a transformer before calling encode!")
     embedding = _transformer_model.encode(text, convert_to_tensor=True)
     similarity = util.pytorch_cos_sim(embedding, comparison_embedding)
     return similarity.item()
 
 
+def get_embeddings_similarity(
+    text_embedding: Tensor, comparison_embedding: Tensor
+) -> float:
+    if _transformer_model is None:
+        raise ValueError("Must initialize a transformer before calling encode!")
+    similarity = util.pytorch_cos_sim(text_embedding, comparison_embedding)
+    return similarity.item()
+
+
 init()
```

### Comparing `langkit-0.0.1b4/pyproject.toml` & `langkit-0.0.1b5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.1b4"
+version = "0.0.1b5"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
-readme = "DESCRIPTION.md"
+readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-whylogs = {version = "1.1.43.dev0"}
+whylogs = {version = "1.1.45.dev3"}
 textstat = "^0.7.3"
-sentence-transformers = "^2.2.2"
-nltk = "^3.8.1"
 pandas = "*"
-datasets = "*"
+
 
 # optional dependencies
 torch = {version = "*", optional = true}
-openai = {version = "*", optional = true}
+datasets = {version ="^2.12.0", optional = true}
+openai = {version ="^0.27.6", optional = true}
+nltk = {version ="^3.8.1", optional = true}
+sentence-transformers = {version ="^2.2.2", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.0"
 pytest = "^7.3.1"
 
 
 [tool.poetry.extras]
 all = [
     "torch",
-    "openai"
+    "datasets",
+    "openai",
+    "nltk",
+    "sentence-transformers",
 ]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langkit-0.0.1b4/PKG-INFO` & `langkit-0.0.1b5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
-Requires-Dist: datasets
-Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: openai ; extra == "all"
+Requires-Dist: datasets (>=2.12.0,<3.0.0) ; extra == "all"
+Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "all"
+Requires-Dist: openai (>=0.27.6,<0.28.0) ; extra == "all"
 Requires-Dist: pandas
-Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "all"
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch ; extra == "all"
-Requires-Dist: whylogs (==1.1.43.dev0)
+Requires-Dist: whylogs (==1.1.45.dev3)
 Description-Content-Type: text/markdown
 
 # LangKit
 
+![LangKit graphic](static/img/LangKit_graphic.png)
+
 **LangKit** is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
 The generated profiles can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
 
 ## Motivation
 
 Productionizing language models, including LLMs, comes with a range of risks due to the infinite amount of input combinations, which can elicit an infinite amount of outputs. The unstructured nature of text poses a challenge in the ML observability space - a challenge worth solving, since the lack of visibility on the model's behavior can have serious consequences.
 
 ## Features
 
 The currently supported metrics include:
 
-- readability score
-- complexity and grade scores
-- sentiment analysis
-- patterns - count of strings matching a user-defined regex pattern group
-- jailbreaks - similarity scores with respect to known jailbreak attempts and prompt injection attacks
-- refusals - similarity scores with respect to known LLM refusal of service responses
+- [Text Quality](langkit/docs/features/quality.md)
+  - readability score
+  - complexity and grade scores
+- [Text Relevance](langkit/docs/features/relevance.md)
+  - Similarity scores between prompt/responses
+  - Similarity scores against user-defined themes
+- [Security and Privacy](langkit/docs/features/security.md)
+  - patterns - count of strings matching a user-defined regex pattern group
+  - jailbreaks - similarity scores with respect to known jailbreak attempts
+  - prompt injection - similarity scores with respect to known prompt injection attacks
+  - refusals - similarity scores with respect to known LLM refusal of service responses
+- [Sentiment and Toxicity](langkit/docs/features/sentiment.md)
+  - sentiment analysis
+  - toxicity analysis
 
 ## Installation
 
 To install LangKit, use the Python Package Index (PyPI) as follows:
 
 ```bash
 pip install langkit
@@ -60,15 +70,19 @@
 from whylogs.experimental.core.metrics.udf_metric import generate_udf_schema
 from whylogs.core.schema import DeclarativeSchema
 import whylogs as why
 from langkit.sentiment import *
 from langkit.textstat import *
 
 text_schema = DeclarativeSchema(generate_udf_schema())
-results = why.log({"prompt": "Hello,", "response": "World!"}, schema=text_schema)
+results = why.log({"prompt": "hello!", "response": "world!"}, schema=text_schema)
 
 ```
 
 The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules.
 
 More examples are available [here](https://github.com/whylabs/LanguageToolkit/tree/main/langkit/examples).
 
+## Modules
+
+You can have more information about the different modules and their metrics [here](langkit/docs/modules.md).
+
```

