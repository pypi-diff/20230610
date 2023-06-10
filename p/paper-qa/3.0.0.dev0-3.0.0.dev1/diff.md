# Comparing `tmp/paper-qa-3.0.0.dev0.tar.gz` & `tmp/paper-qa-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.0.0.dev0.tar", last modified: Sat Jun 10 00:28:48 2023, max compression
+gzip compressed data, was "paper-qa-3.0.0.dev1.tar", last modified: Sat Jun 10 11:20:01 2023, max compression
```

## Comparing `paper-qa-3.0.0.dev0.tar` & `paper-qa-3.0.0.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.105593 paper-qa-3.0.0.dev0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20516 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/tests/test_paperqa.py
```

### Comparing `paper-qa-3.0.0.dev0/LICENSE` & `paper-qa-3.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/PKG-INFO` & `paper-qa-3.0.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev0
+Version: 3.0.0.dev1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,21 +24,20 @@
     - [Adjusting number of sources](#adjusting-number-of-sources)
     - [Using Code or HTML](#using-code-or-html)
   - [Version 3 Changes](#version-3-changes)
     - [New Features](#new-features)
     - [Naming](#naming)
     - [Breaking Changes](#breaking-changes)
   - [Notebooks](#notebooks)
-  - [Agents (experimental)](#agents-experimental)
   - [Where do I get papers?](#where-do-i-get-papers)
     - [Zotero](#zotero)
     - [Paper Scraper](#paper-scraper)
   - [PDF Reading Options](#pdf-reading-options)
   - [Typewriter View](#typewriter-view)
-  - [Caching](#caching-1)
+  - [LLM/Embedding Caching](#llmembedding-caching)
     - [Caching Embeddings](#caching-embeddings)
   - [Customizing Prompts](#customizing-prompts)
     - [Pre and Post Prompts](#pre-and-post-prompts)
   - [FAQ](#faq)
     - [How is this different from LlamaIndex?](#how-is-this-different-from-llamaindex)
     - [How is this different from LangChain?](#how-is-this-different-from-langchain)
     - [Can I use different LLMs?](#can-i-use-different-llms)
@@ -135,28 +134,24 @@
 
 
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
+import paperscraper
 from paperqa import Docs
 from langchain.llms import LlamaCpp
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
-from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.embeddings import LlamaCppEmbeddings
 
-# Callbacks support token-wise streaming
-callback_manager = CallbackManager([StreamingStdOutCallbackHandler()])
-# Verbose is required to pass to the callback manager
-
 # Make sure the model path is correct for your system!
 llm = LlamaCpp(
-    model_path="./ggml-model-q4_0.bin", callback_manager=callback_manager
+    model_path="./ggml-model-q4_0.bin", callbacks=[StreamingStdOutCallbackHandler()]
 )
 embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
 
 docs = Docs(llm=llm, embeddings=embeddings)
 
 keyword_search = 'bispecific antibody manufacture'
 papers = paperscraper.search_papers(keyword_search, limit=2)
@@ -187,15 +182,15 @@
 import glob
 
 source_files = glob.glob('**/*.js')
 
 docs = Docs()
 for f in source_files:
     # this assumes the file names are unique in code
-    docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
+    docs.add(f, citation='File ' + os.path.name(f), docname=os.path.name(f))
 answer = docs.query("Where is the search bar in the header defined?")
 print(answer)
 ```
 
 ## Version 3 Changes
 
 Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
@@ -252,25 +247,14 @@
 ```python
 import nest_asyncio
 nest_asyncio.apply()
 ```
 
 Also - if you know how to make this automated, please let me know!
 
-## Agents (experimental)
-
-You can try to automate the collection of papers and assessment of correctness of papers using an agent. This is experimental and requires installation of [paper-scraper](https://github.com/blackadad/paper-scraper).
-
-```python
-
-docs = paperqa.Docs()
-answer = paperqa.run_agent(docs, 'What compounds target AKT1')
-print(answer)
-```
-
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
 ### Zotero
 
 If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
@@ -304,15 +288,15 @@
 
 docs = paperqa.Docs()
 zotero = ZoteroDB(library_type="user")  # "group" if group library
 
 for item in zotero.iterate(limit=20):
     if item.num_pages > 30:
         continue  # skip long papers
-    docs.add(item.pdf, key=item.key)
+    docs.add(item.pdf, docname=item.key)
 ```
 
 which will download the first 20 papers in your Zotero database and add
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
 
@@ -321,15 +305,15 @@
         q="large language models",
         qmode="everything",
         sort="date",
         direction="desc",
         limit=100,
 ):
     print("Adding", item.title)
-    docs.add(item.pdf, key=item.key)
+    docs.add(item.pdf, docname=item.key)
 ```
 
 You can read more about the search syntax by typing `zotero.iterate?` in IPython.
 
 ### Paper Scraper
 
 If you want to search for papers outside of your own collection, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
@@ -359,21 +343,22 @@
 
 ## Typewriter View
 
 To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
 
 ```python
 from paperqa import Docs
+from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
 
-my_llm = ChatOpenAI(model='gpt-3.5-turbo', streaming=True)
+my_llm = ChatOpenAI(callbacks=[StreamingStdOutCallbackHandler()], streaming=True)
 docs = Docs(llm=my_llm)
 ```
 
-## Caching
+## LLM/Embedding Caching
 
 You can using the builtin langchain caching capabilities. Just run this code at the top of yours:
 
 ```py
 from langchain.cache import InMemoryCache
 langchain.llm_cache = InMemoryCache()
 ```
```

### Comparing `paper-qa-3.0.0.dev0/README.md` & `paper-qa-3.0.0.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     - [Adjusting number of sources](#adjusting-number-of-sources)
     - [Using Code or HTML](#using-code-or-html)
   - [Version 3 Changes](#version-3-changes)
     - [New Features](#new-features)
     - [Naming](#naming)
     - [Breaking Changes](#breaking-changes)
   - [Notebooks](#notebooks)
-  - [Agents (experimental)](#agents-experimental)
   - [Where do I get papers?](#where-do-i-get-papers)
     - [Zotero](#zotero)
     - [Paper Scraper](#paper-scraper)
   - [PDF Reading Options](#pdf-reading-options)
   - [Typewriter View](#typewriter-view)
-  - [Caching](#caching-1)
+  - [LLM/Embedding Caching](#llmembedding-caching)
     - [Caching Embeddings](#caching-embeddings)
   - [Customizing Prompts](#customizing-prompts)
     - [Pre and Post Prompts](#pre-and-post-prompts)
   - [FAQ](#faq)
     - [How is this different from LlamaIndex?](#how-is-this-different-from-llamaindex)
     - [How is this different from LangChain?](#how-is-this-different-from-langchain)
     - [Can I use different LLMs?](#can-i-use-different-llms)
@@ -121,28 +120,24 @@
 
 
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
+import paperscraper
 from paperqa import Docs
 from langchain.llms import LlamaCpp
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
-from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.embeddings import LlamaCppEmbeddings
 
-# Callbacks support token-wise streaming
-callback_manager = CallbackManager([StreamingStdOutCallbackHandler()])
-# Verbose is required to pass to the callback manager
-
 # Make sure the model path is correct for your system!
 llm = LlamaCpp(
-    model_path="./ggml-model-q4_0.bin", callback_manager=callback_manager
+    model_path="./ggml-model-q4_0.bin", callbacks=[StreamingStdOutCallbackHandler()]
 )
 embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
 
 docs = Docs(llm=llm, embeddings=embeddings)
 
 keyword_search = 'bispecific antibody manufacture'
 papers = paperscraper.search_papers(keyword_search, limit=2)
@@ -173,15 +168,15 @@
 import glob
 
 source_files = glob.glob('**/*.js')
 
 docs = Docs()
 for f in source_files:
     # this assumes the file names are unique in code
-    docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
+    docs.add(f, citation='File ' + os.path.name(f), docname=os.path.name(f))
 answer = docs.query("Where is the search bar in the header defined?")
 print(answer)
 ```
 
 ## Version 3 Changes
 
 Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
@@ -238,25 +233,14 @@
 ```python
 import nest_asyncio
 nest_asyncio.apply()
 ```
 
 Also - if you know how to make this automated, please let me know!
 
-## Agents (experimental)
-
-You can try to automate the collection of papers and assessment of correctness of papers using an agent. This is experimental and requires installation of [paper-scraper](https://github.com/blackadad/paper-scraper).
-
-```python
-
-docs = paperqa.Docs()
-answer = paperqa.run_agent(docs, 'What compounds target AKT1')
-print(answer)
-```
-
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
 ### Zotero
 
 If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
@@ -290,15 +274,15 @@
 
 docs = paperqa.Docs()
 zotero = ZoteroDB(library_type="user")  # "group" if group library
 
 for item in zotero.iterate(limit=20):
     if item.num_pages > 30:
         continue  # skip long papers
-    docs.add(item.pdf, key=item.key)
+    docs.add(item.pdf, docname=item.key)
 ```
 
 which will download the first 20 papers in your Zotero database and add
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
 
@@ -307,15 +291,15 @@
         q="large language models",
         qmode="everything",
         sort="date",
         direction="desc",
         limit=100,
 ):
     print("Adding", item.title)
-    docs.add(item.pdf, key=item.key)
+    docs.add(item.pdf, docname=item.key)
 ```
 
 You can read more about the search syntax by typing `zotero.iterate?` in IPython.
 
 ### Paper Scraper
 
 If you want to search for papers outside of your own collection, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
@@ -345,21 +329,22 @@
 
 ## Typewriter View
 
 To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
 
 ```python
 from paperqa import Docs
+from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
 
-my_llm = ChatOpenAI(model='gpt-3.5-turbo', streaming=True)
+my_llm = ChatOpenAI(callbacks=[StreamingStdOutCallbackHandler()], streaming=True)
 docs = Docs(llm=my_llm)
 ```
 
-## Caching
+## LLM/Embedding Caching
 
 You can using the builtin langchain caching capabilities. Just run this code at the top of yours:
 
 ```py
 from langchain.cache import InMemoryCache
 langchain.llm_cache = InMemoryCache()
 ```
```

### Comparing `paper-qa-3.0.0.dev0/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.0.0.dev1/paper_qa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev0
+Version: 3.0.0.dev1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,21 +24,20 @@
     - [Adjusting number of sources](#adjusting-number-of-sources)
     - [Using Code or HTML](#using-code-or-html)
   - [Version 3 Changes](#version-3-changes)
     - [New Features](#new-features)
     - [Naming](#naming)
     - [Breaking Changes](#breaking-changes)
   - [Notebooks](#notebooks)
-  - [Agents (experimental)](#agents-experimental)
   - [Where do I get papers?](#where-do-i-get-papers)
     - [Zotero](#zotero)
     - [Paper Scraper](#paper-scraper)
   - [PDF Reading Options](#pdf-reading-options)
   - [Typewriter View](#typewriter-view)
-  - [Caching](#caching-1)
+  - [LLM/Embedding Caching](#llmembedding-caching)
     - [Caching Embeddings](#caching-embeddings)
   - [Customizing Prompts](#customizing-prompts)
     - [Pre and Post Prompts](#pre-and-post-prompts)
   - [FAQ](#faq)
     - [How is this different from LlamaIndex?](#how-is-this-different-from-llamaindex)
     - [How is this different from LangChain?](#how-is-this-different-from-langchain)
     - [Can I use different LLMs?](#can-i-use-different-llms)
@@ -135,28 +134,24 @@
 
 
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
+import paperscraper
 from paperqa import Docs
 from langchain.llms import LlamaCpp
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
-from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.embeddings import LlamaCppEmbeddings
 
-# Callbacks support token-wise streaming
-callback_manager = CallbackManager([StreamingStdOutCallbackHandler()])
-# Verbose is required to pass to the callback manager
-
 # Make sure the model path is correct for your system!
 llm = LlamaCpp(
-    model_path="./ggml-model-q4_0.bin", callback_manager=callback_manager
+    model_path="./ggml-model-q4_0.bin", callbacks=[StreamingStdOutCallbackHandler()]
 )
 embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
 
 docs = Docs(llm=llm, embeddings=embeddings)
 
 keyword_search = 'bispecific antibody manufacture'
 papers = paperscraper.search_papers(keyword_search, limit=2)
@@ -187,15 +182,15 @@
 import glob
 
 source_files = glob.glob('**/*.js')
 
 docs = Docs()
 for f in source_files:
     # this assumes the file names are unique in code
-    docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
+    docs.add(f, citation='File ' + os.path.name(f), docname=os.path.name(f))
 answer = docs.query("Where is the search bar in the header defined?")
 print(answer)
 ```
 
 ## Version 3 Changes
 
 Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
@@ -252,25 +247,14 @@
 ```python
 import nest_asyncio
 nest_asyncio.apply()
 ```
 
 Also - if you know how to make this automated, please let me know!
 
-## Agents (experimental)
-
-You can try to automate the collection of papers and assessment of correctness of papers using an agent. This is experimental and requires installation of [paper-scraper](https://github.com/blackadad/paper-scraper).
-
-```python
-
-docs = paperqa.Docs()
-answer = paperqa.run_agent(docs, 'What compounds target AKT1')
-print(answer)
-```
-
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
 ### Zotero
 
 If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
@@ -304,15 +288,15 @@
 
 docs = paperqa.Docs()
 zotero = ZoteroDB(library_type="user")  # "group" if group library
 
 for item in zotero.iterate(limit=20):
     if item.num_pages > 30:
         continue  # skip long papers
-    docs.add(item.pdf, key=item.key)
+    docs.add(item.pdf, docname=item.key)
 ```
 
 which will download the first 20 papers in your Zotero database and add
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
 
@@ -321,15 +305,15 @@
         q="large language models",
         qmode="everything",
         sort="date",
         direction="desc",
         limit=100,
 ):
     print("Adding", item.title)
-    docs.add(item.pdf, key=item.key)
+    docs.add(item.pdf, docname=item.key)
 ```
 
 You can read more about the search syntax by typing `zotero.iterate?` in IPython.
 
 ### Paper Scraper
 
 If you want to search for papers outside of your own collection, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
@@ -359,21 +343,22 @@
 
 ## Typewriter View
 
 To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
 
 ```python
 from paperqa import Docs
+from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
 
-my_llm = ChatOpenAI(model='gpt-3.5-turbo', streaming=True)
+my_llm = ChatOpenAI(callbacks=[StreamingStdOutCallbackHandler()], streaming=True)
 docs = Docs(llm=my_llm)
 ```
 
-## Caching
+## LLM/Embedding Caching
 
 You can using the builtin langchain caching capabilities. Just run this code at the top of yours:
 
 ```py
 from langchain.cache import InMemoryCache
 langchain.llm_cache = InMemoryCache()
 ```
```

### Comparing `paper-qa-3.0.0.dev0/paperqa/chains.py` & `paper-qa-3.0.0.dev1/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/paperqa/contrib/zotero.py` & `paper-qa-3.0.0.dev1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/paperqa/docs.py` & `paper-qa-3.0.0.dev1/paperqa/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,28 +268,29 @@
         result = await chain.arun(  # type: ignore
             question=query, papers="\n".join(papers), callbacks=get_callbacks("filter")
         )
         return set([d.dockey for d in matched_docs if d.docname in result])
 
     def __getstate__(self):
         state = self.__dict__.copy()
-        if self.texts_index is not None:
+        if self.texts_index is not None and self.index_path is not None:
             state["texts_index"].save_local(self.index_path)
         del state["texts_index"]
         del state["doc_index"]
         return {"__dict__": state, "__fields_set__": self.__fields_set__}
 
     def __setstate__(self, state):
         object.__setattr__(self, "__dict__", state["__dict__"])
         object.__setattr__(self, "__fields_set__", state["__fields_set__"])
         try:
             self.texts_index = FAISS.load_local(self.index_path, self.embeddings)
         except Exception:
             # they use some special exception type, but I don't want to import it
             self.texts_index = None
+        self.doc_index = None
 
     def _build_texts_index(self):
         if self.texts_index is None:
             raw_texts = [t.text for t in self.texts]
             text_embeddings = [t.embeddings for t in self.texts]
             metadatas = [t.dict(exclude={"embeddings", "text"}) for t in self.texts]
             self.texts_index = FAISS.from_embeddings(
```

### Comparing `paper-qa-3.0.0.dev0/paperqa/prompts.py` & `paper-qa-3.0.0.dev1/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/paperqa/readers.py` & `paper-qa-3.0.0.dev1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/paperqa/types.py` & `paper-qa-3.0.0.dev1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/paperqa/utils.py` & `paper-qa-3.0.0.dev1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/setup.py` & `paper-qa-3.0.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev0/tests/test_paperqa.py` & `paper-qa-3.0.0.dev1/tests/test_paperqa.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,15 @@
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
         r = requests.get("https://en.wikipedia.org/wiki/Take_Your_Dog_to_Work_Day")
         f.write(r.text)
     llm = OpenAI(client=None, temperature=0.0, model="text-curie-001")
     docs = Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
+    os.remove(doc_path)
     docs_pickle = pickle.dumps(docs)
     docs2 = pickle.loads(docs_pickle)
     docs2.update_llm(llm)
     assert llm.model_name == docs2.llm.model_name
     assert docs2.summary_llm.model_name == docs2.llm.model_name
     assert len(docs.docs) == len(docs2.docs)
     context1, context2 = (
@@ -175,15 +176,16 @@
             k=3,
             max_sources=1,
         ).context,
     )
     print(context1)
     print(context2)
     assert strings_similarity(context1, context2) > 0.75
-    os.remove(doc_path)
+    # make sure we can query
+    docs.query("What date is bring your dog to work in the US?")
 
 
 def test_docs_pickle_no_faiss():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
         r = requests.get("https://en.wikipedia.org/wiki/Take_Your_Dog_to_Work_Day")
```

