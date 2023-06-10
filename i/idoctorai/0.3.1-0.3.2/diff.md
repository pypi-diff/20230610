# Comparing `tmp/idoctorai-0.3.1.tar.gz` & `tmp/idoctorai-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.3.1.tar", max compression
+gzip compressed data, was "idoctorai-0.3.2.tar", max compression
```

## Comparing `idoctorai-0.3.1.tar` & `idoctorai-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.1/LICENSE
--rw-r--r--   0        0        0    19001 2023-06-08 05:58:42.811892 idoctorai-0.3.1/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.1/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2332 2023-06-09 12:47:59.549794 idoctorai-0.3.1/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11261 2023-06-09 13:00:38.629850 idoctorai-0.3.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3209 2023-06-09 10:29:55.340192 idoctorai-0.3.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1454 2023-06-09 13:01:37.250641 idoctorai-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.1/README.md
--rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 idoctorai-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.2/LICENSE
+-rw-r--r--   0        0        0    19100 2023-06-10 07:53:33.608323 idoctorai-0.3.2/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.2/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.2/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.2/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.2/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.2/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.2/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2881 2023-06-10 09:03:03.357210 idoctorai-0.3.2/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.2/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11323 2023-06-10 09:13:47.773963 idoctorai-0.3.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.2/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.2/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3240 2023-06-10 07:56:37.939765 idoctorai-0.3.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.2/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.2/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.2/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.2/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.2/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.2/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.2/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.2/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1454 2023-06-10 09:14:05.013893 idoctorai-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.2/README.md
+-rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 idoctorai-0.3.2/PKG-INFO
```

### Comparing `idoctorai-0.3.1/LICENSE` & `idoctorai-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/__init__.py` & `idoctorai-0.3.2/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
+        history: list = None,
     ) -> Union[str, pd.DataFrame]:
         """
         Run the PandasAI to make Dataframes Conversational.
 
         Args:
             data_frame (pd.Dataframe): A pandas Dataframe
             prompt (str): A prompt to query about the Dataframe
@@ -225,14 +226,15 @@
                         else dataframe.head(rows_to_display)
                         for dataframe in data_frame
                     ]
 
                     code = self._llm.generate_code(
                         MultipleDataframesPrompt(dataframes=heads),
                         prompt,
+                        history,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": heads,
                         "rows_to_display": rows_to_display,
                     }
@@ -247,14 +249,15 @@
                             prompt=prompt,
                             df_head=df_head,
                             num_rows=data_frame.shape[0],
                             num_columns=data_frame.shape[1],
                             rows_to_display=rows_to_display,
                         ),
                         prompt,
+                        history,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": df_head,
                         "num_rows": data_frame.shape[0],
                         "num_columns": data_frame.shape[1],
```

### Comparing `idoctorai-0.3.1/pandasai/constants.py` & `idoctorai-0.3.2/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/exceptions.py` & `idoctorai-0.3.2/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/helpers/_optional.py` & `idoctorai-0.3.2/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/helpers/anonymizer.py` & `idoctorai-0.3.2/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/helpers/cache.py` & `idoctorai-0.3.2/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/helpers/from_excel.py` & `idoctorai-0.3.2/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/helpers/notebook.py` & `idoctorai-0.3.2/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/helpers/save_chart.py` & `idoctorai-0.3.2/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/langchain/__init__.py` & `idoctorai-0.3.2/pandasai/langchain/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,39 +12,52 @@
 
 
 class LangChain:
 
     api_token: str
     conversation: ConversationChain
     llm: OpenAI
+    model_name: str = "gpt-3.5-turbo"
+    k: int = 2
 
     template = """Assistant is a large language model trained by OpenAI.
 
 Assistant is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, Assistant is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
 
 Assistant is constantly learning and improving, and its capabilities are constantly evolving. It is able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. Additionally, Assistant is able to generate its own text based on the input it receives, allowing it to engage in discussions and provide explanations and descriptions on a wide range of topics.
 
 Overall, Assistant is a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether you need help with a specific question or just want to have a conversation about a particular topic, Assistant is here to assist.
 
+{history}
 Human: {human_input}
 Assistant:"""
 
     def __init__(self, api_token: Optional[str] = None, **kwargs,):
         self.api_token = api_token or None
         self.llm = OpenAI(openai_api_key=self.api_token, temperature=0, max_tokens=512)
         prompt = PromptTemplate(
-            input_variables=["human_input"], 
+            input_variables=["history","human_input"], 
             template=self.template
         )
+
+        memory = ConversationBufferWindowMemory(k=self.k)
+        # memory = ConversationBufferMemory(memory_key="history", memory_size=3)
+        # memory.save_context({"input": "hi"}, {"output": "whats up"})
+        # memory.save_context({"input": "not much you"}, {"output": "not much"})
+
         chatgpt_chain = LLMChain(
             llm=self.llm, 
             prompt=prompt, 
             verbose=True, 
-            memory=ConversationBufferWindowMemory(k=2),
+            memory=memory,
         )
 
         self.conversation =  chatgpt_chain
 
-    def __call__(self, prompt: str, **kwargs) -> str:
+    def __call__(self, prompt: str, history:list = None, **kwargs) -> str:
+        if history is not None:
+            self.conversation.memory.k = len(history)
+            for sec in history:
+                self.conversation.memory.save_context(*sec)
         return self.conversation.predict(human_input=prompt)
```

### Comparing `idoctorai-0.3.1/pandasai/llm/azure_openai.py` & `idoctorai-0.3.2/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/llm/base.py` & `idoctorai-0.3.2/pandasai/llm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,22 +124,22 @@
             suffix (str, optional): Suffix. Defaults to "".
 
         Raises:
             MethodNotImplementedError: Call method has not been implemented
         """
         raise MethodNotImplementedError("Call method has not been implemented")
 
-    def generate_code(self, instruction: Prompt, prompt: str) -> str:
+    def generate_code(self, instruction: Prompt, prompt: str, history: list) -> str:
         """
         Generate the code based on the instruction and the given prompt.
 
         Returns:
             str: Code
         """
-        return self._extract_code(self.call(instruction, prompt, suffix="\n\nCode:\n"))
+        return self._extract_code(self.call(instruction, prompt, suffix="\n\nCode:\n", history=history))
 
 
 class BaseOpenAI(LLM, ABC):
     """Base class to implement a new OpenAI LLM
     LLM base class, this class is extended to be used with OpenAI API.
 
     """
@@ -237,16 +237,16 @@
         if self.stop is not None:
             params["stop"] = [self.stop]
       
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
     
-    def langchain_input(self, value:str) -> str:
-        response = self.langchain.__call__(value)
+    def langchain_input(self, value:str, history:list = None) -> str:
+        response = self.langchain.__call__(value, history)
         # print(response)
         return response
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
```

### Comparing `idoctorai-0.3.1/pandasai/llm/fake.py` & `idoctorai-0.3.2/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/llm/google_palm.py` & `idoctorai-0.3.2/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/llm/open_assistant.py` & `idoctorai-0.3.2/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/llm/openai.py` & `idoctorai-0.3.2/pandasai/llm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API"""
         return {
             **super()._default_params,
             "model": self.model,
         }
 
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+    def call(self, instruction: Prompt, value: str, suffix: str = "", history: list = None) -> str:
         """
         Call the OpenAI LLM.
 
         Args:
             instruction (Prompt): Instruction to pass
             value (str): Value to pass
             suffix (str): Suffix to pass
@@ -96,15 +96,15 @@
         """
         self.last_prompt = str(instruction) + str(value)
 
         if self.model in self._supported_completion_models:
             response = self.completion(str(instruction) + str(value) + suffix)
         elif self.model in self._supported_chat_models:
             # response = self.chat_completion(str(instruction) + str(value) + suffix)
-            response = self.langchain_input(str(instruction) + str(value) + suffix)
+            response = self.langchain_input(str(instruction) + str(value) + suffix, history)
         else:
             raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
     def type(self) -> str:
```

### Comparing `idoctorai-0.3.1/pandasai/llm/starcoder.py` & `idoctorai-0.3.2/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/prompts/base.py` & `idoctorai-0.3.2/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.3.2/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.3.2/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/prompts/generate_python_code.py` & `idoctorai-0.3.2/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/prompts/generate_response.py` & `idoctorai-0.3.2/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.3.2/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.1/pyproject.toml` & `idoctorai-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.3.1"
+version = "0.3.2"
 description = "this is idoctorai, Generate code with natural speech"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
```

### Comparing `idoctorai-0.3.1/PKG-INFO` & `idoctorai-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.3.1
+Version: 0.3.2
 Summary: this is idoctorai, Generate code with natural speech
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

