# Comparing `tmp/panml-1.0.0.tar.gz` & `tmp/panml-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-1.0.0.tar", last modified: Thu Jun  8 13:10:00 2023, max compression
+gzip compressed data, was "panml-1.0.1.tar", last modified: Sat Jun 10 00:05:25 2023, max compression
```

## Comparing `panml-1.0.0.tar` & `panml-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.564454 panml-1.0.0/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.0/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-08 13:10:00.564832 panml-1.0.0/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.0/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.557697 panml-1.0.0/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.0/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.560836 panml-1.0.0/panml/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.0/panml/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.0/panml/clustering/faiss.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.0/panml/constants.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.0/panml/environments.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.562576 panml-1.0.0/panml/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.0/panml/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    23699 2023-06-08 13:09:32.000000 panml-1.0.0/panml/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    15676 2023-06-08 13:09:32.000000 panml-1.0.0/panml/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-08 13:09:32.000000 panml-1.0.0/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.0/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.559790 panml-1.0.0/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-08 13:10:00.566014 panml-1.0.0/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-08 13:09:32.000000 panml-1.0.0/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.563851 panml-1.0.0/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.0/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.0/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 00:05:25.099917 panml-1.0.1/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.1/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-10 00:05:25.100464 panml-1.0.1/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.1/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 00:05:25.089076 panml-1.0.1/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.1/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 00:05:25.093259 panml-1.0.1/panml/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.1/panml/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.1/panml/clustering/faiss.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.1/panml/constants.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.1/panml/environments.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 00:05:25.095901 panml-1.0.1/panml/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.1/panml/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    24033 2023-06-10 00:04:43.000000 panml-1.0.1/panml/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    15676 2023-06-08 13:09:32.000000 panml-1.0.1/panml/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-08 13:09:32.000000 panml-1.0.1/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.1/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 00:05:25.092089 panml-1.0.1/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-10 00:05:24.000000 panml-1.0.1/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-10 00:05:25.000000 panml-1.0.1/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-10 00:05:24.000000 panml-1.0.1/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-10 00:05:24.000000 panml-1.0.1/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-10 00:05:24.000000 panml-1.0.1/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-10 00:05:25.101733 panml-1.0.1/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-10 00:04:43.000000 panml-1.0.1/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 00:05:25.098816 panml-1.0.1/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.1/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.1/test/test_VectorEngine.py
```

### Comparing `panml-1.0.0/LICENSE` & `panml-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/PKG-INFO` & `panml-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.0
+Version: 1.0.1
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.0/README.md` & `panml-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/panml/clustering/faiss.py` & `panml-1.0.1/panml/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/panml/constants.py` & `panml-1.0.1/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/panml/environments.py` & `panml-1.0.1/panml/environments.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/panml/llm/huggingface.py` & `panml-1.0.1/panml/llm/huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,16 @@
             self.tokenizer = AutoTokenizer.from_pretrained(self.peft_config.base_model_name_or_path)
         else:
             # Set non-LoRA trained model's tokenizer
             if self.model_hf.config.tokenizer_class:
                 self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
             else:
                 self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
+        if self.tokenizer.pad_token is None:
+            self.tokenizer.pad_token = self.model_hf.config.eos_token_id
 
         # Set LoRA for training
         if len(peft_lora_args) > 0 and load_peft_lora is False:
             if self.model_name in self.supported_models_peft_lora:
                 if 'flan' in self.model_name:
                     self.peft_config = LoraConfig(task_type=TaskType['SEQ_2_SEQ_LM'], **peft_lora_args)
                 else:
@@ -411,18 +413,19 @@
                 eval_dataset=tokenized_data.remove_columns(['text']),
                 data_collator=data_collator,
             )
 
         trainer.train() # Execute training
 
         print('Getting evaluations...')
-        self.evaluation_result = trainer.evaluate() # Save evaluation result
+        self.evaluation_result = trainer.evaluate() # save evaluation result
         
         if train_args['save_model']:
-            trainer.save_model(f'./results/model_{train_args["title"]}') # Save trained model
+            trainer.save_model(f'./results/model_{train_args["title"]}') # save trained model
+            self.tokenizer._tokenizer.save(f'./results/model_{train_args["title"]}/tokenizer.json') # save tokenizer
 
         print('Task completed')
         
     # Save model
     def save(self, save_dir: str=None) -> None:
         '''
         Save the model on demand
@@ -431,8 +434,9 @@
         save_dir: relative path of the file. If directory is not provided, the default directory is set to ".results/model_<model_name>"
 
         Returns:
         None. File is saved at the specified location
         '''
         if save_dir is None:
             save_dir = f'./results/model_{self.model_name}'
-        self.model_hf.save_pretrained(save_dir)
+        self.model_hf.save_pretrained(save_dir) # save model
+        self.tokenizer._tokenizer.save(f'{save_dir}/tokenizer.json') # save tokenizer
```

### Comparing `panml-1.0.0/panml/llm/openai.py` & `panml-1.0.1/panml/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/panml/models.py` & `panml-1.0.1/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/panml/search.py` & `panml-1.0.1/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/panml.egg-info/PKG-INFO` & `panml-1.0.1/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.0
+Version: 1.0.1
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.0/setup.py` & `panml-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '1.0.0', # version
+  version = '1.0.1', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-1.0.0/test/test_ModelPack.py` & `panml-1.0.1/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.0/test/test_VectorEngine.py` & `panml-1.0.1/test/test_VectorEngine.py`

 * *Files identical despite different names*

