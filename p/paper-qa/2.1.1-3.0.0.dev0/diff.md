# Comparing `tmp/paper-qa-2.1.1.tar.gz` & `tmp/paper-qa-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-2.1.1.tar", last modified: Wed Jun  7 03:17:44 2023, max compression
+gzip compressed data, was "paper-qa-3.0.0.dev0.tar", last modified: Sat Jun 10 00:28:48 2023, max compression
```

## Comparing `paper-qa-2.1.1.tar` & `paper-qa-3.0.0.dev0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 03:16:57.000000 paper-qa-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-07 03:17:44.571631 paper-qa-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-06-07 03:16:57.000000 paper-qa-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.567631 paper-qa-2.1.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22969 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:17:44.571631 paper-qa-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-07 03:16:57.000000 paper-qa-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-06-07 03:16:57.000000 paper-qa-2.1.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.105593 paper-qa-3.0.0.dev0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 00:28:48.000000 paper-qa-3.0.0.dev0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:28:48.109593 paper-qa-3.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-06-10 00:28:12.000000 paper-qa-3.0.0.dev0/tests/test_paperqa.py
```

### Comparing `paper-qa-2.1.1/LICENSE` & `paper-qa-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.1/PKG-INFO` & `paper-qa-3.0.0.dev0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,72 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.1.1
+Version: 3.0.0.dev0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Paper QA
+# Paper QA- [Paper QA](#paper-qa)
+- [Paper QA- Paper QA](#paper-qa--paper-qa)
+  - [Output Example](#output-example)
+    - [References](#references)
+  - [Hugging Face Demo](#hugging-face-demo)
+  - [Install](#install)
+  - [Usage](#usage)
+    - [Adding Documents](#adding-documents)
+    - [Choosing Model](#choosing-model)
+    - [Adjusting number of sources](#adjusting-number-of-sources)
+    - [Using Code or HTML](#using-code-or-html)
+  - [Version 3 Changes](#version-3-changes)
+    - [New Features](#new-features)
+    - [Naming](#naming)
+    - [Breaking Changes](#breaking-changes)
+  - [Notebooks](#notebooks)
+  - [Agents (experimental)](#agents-experimental)
+  - [Where do I get papers?](#where-do-i-get-papers)
+    - [Zotero](#zotero)
+    - [Paper Scraper](#paper-scraper)
+  - [PDF Reading Options](#pdf-reading-options)
+  - [Typewriter View](#typewriter-view)
+  - [Caching](#caching-1)
+    - [Caching Embeddings](#caching-embeddings)
+  - [Customizing Prompts](#customizing-prompts)
+    - [Pre and Post Prompts](#pre-and-post-prompts)
+  - [FAQ](#faq)
+    - [How is this different from LlamaIndex?](#how-is-this-different-from-llamaindex)
+    - [How is this different from LangChain?](#how-is-this-different-from-langchain)
+    - [Can I use different LLMs?](#can-i-use-different-llms)
+    - [Where do the documents come from?](#where-do-the-documents-come-from)
+    - [Can I save or load?](#can-i-save-or-load)
+
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
 
 This is a minimal package for doing question and answering from
-PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
-generate answers.
+PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations.
 
-It uses the process shown below:
+By default, it uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. However, via [langchain](https://github.com/hwchase17/langchain) you can use open-source models or embeddings (see details below).
 
-```
-embed docs into vectors -> embed query into vector -> search for top k passages in docs
+PaperQA uses the process shown below:
 
-create summary of each passage relevant to query -> put summaries into prompt -> generate answer
-```
-
-<img src="https://user-images.githubusercontent.com/908389/230854097-8fa96768-c694-45c0-bb04-3a7386facef3.jpeg" width="600" alt="Process of vector search, refinement, and answer with context">
+1. embed docs into vectors
+2. embed query into vector
+3. search for top k passages in docs
+4. create summary of each passage relevant to query
+5. put summaries into prompt
+6. generate answer with prompt
 
 ## Output Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
@@ -42,15 +74,14 @@
 
 Journet6644: Journet, Catherine, et al. "Large-scale production of single-walled carbon nanotubes by the electric-arc technique." nature 388.6644 (1997): 756-758.
 
 Tulevski2007: Tulevski, George S., et al. "Chemically assisted directed assembly of carbon nanotubes for the fabrication of large-scale device arrays." Journal of the American Chemical Society 129.39 (2007): 11964-11968.
 
 Chen2014: Chen, Haitian, et al. "Large-scale complementary macroelectronics using hybrid integration of carbon nanotubes and IGZO thin-film transistors." Nature communications 5.1 (2014): 4097.
 
-
 ## Hugging Face Demo
 
 [Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
 
 ## Install
 
 Install with pip:
@@ -77,28 +108,32 @@
 
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
+### Adding Documents
+
+`add` will add from paths. You can also use `add_file` (expects a file object) or `add_url` to work with other sources.
+
 ### Choosing Model
 
 By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
 
 ```py
 docs = Docs(llm='gpt-3.5-turbo')
 ```
 
 or you can use any other model available in [langchain](https://github.com/hwchase17/langchain):
 
 ```py
-from langchain.llms import Anthropic, OpenAIChat
-model = OpenAIChat(model='gpt-4')
-summary_model = Anthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
+from langchain.chat_models import ChatAnthropic, ChatOpenAI
+model = ChatOpenAI(model='gpt-4')
+summary_model = ChatAnthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
 docs = Docs(llm=model, summary_llm=summary_model)
 ```
 
 
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
@@ -157,14 +192,63 @@
 for f in source_files:
     # this assumes the file names are unique in code
     docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
 answer = docs.query("Where is the search bar in the header defined?")
 print(answer)
 ```
 
+## Version 3 Changes
+
+Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
+
+
+### New Features
+
+The following new features are in v3:
+
+1. `add_url` and `add_file` are now supported for adding from URLs and file objects
+2. Prompts can be customized, and now can be executed pre and post query
+3. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
+4. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
+5. Various simplifications, bug fixes, and performance improvements
+
+### Naming
+
+The following table shows the old names and the new names:
+
+| Old Name | New Name | Explanation |
+| :--- | :---: | ---: |
+| `key` | `name` | Name is a natural language name for text. |
+| `dockey` | `docname` | Docname is a natural language name for a document. |
+| `hash` | `dockey` | Dockey is a unique identifier for the document. |
+
+
+### Breaking Changes
+
+
+#### Pickled objects
+
+The pickled objects are not compatible with the new version.
+
+#### Agents
+
+The agent functionality has been removed, as it's not a core focus of the library
+
+#### Caching
+
+Caching has been removed because it's not a core focus of the library. See FAQ below for how to use caching.
+
+#### Answers
+
+Answers will not include passages, but instead return dockeys that can be used to retrieve the passages. Tokens/cost will also not be counted since that is built into langchain by default (see below for an example).
+
+#### Search Query
+
+The search query chain has been removed. You can use langchain directly to do this.
+
 ## Notebooks
 
 If you want to use this in an jupyter notebook or colab, you need to run the following command:
 
 ```python
 import nest_asyncio
 nest_asyncio.apply()
@@ -261,28 +345,88 @@
     except ValueError as e:
         # sometimes this happens if PDFs aren't downloaded or readable
         print('Could not read', path, e)
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer)
 ```
 
+## PDF Reading Options
+
+By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
+
+```sh
+pip install pymupdf
+```
+
+## Typewriter View
+
+To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
+
+```python
+from paperqa import Docs
+from langchain.chat_models import ChatOpenAI
+
+my_llm = ChatOpenAI(model='gpt-3.5-turbo', streaming=True)
+docs = Docs(llm=my_llm)
+```
+
+## Caching
+
+You can using the builtin langchain caching capabilities. Just run this code at the top of yours:
+
+```py
+from langchain.cache import InMemoryCache
+langchain.llm_cache = InMemoryCache()
+```
+
+### Caching Embeddings
+
+In general, embeddings are cached when you pickle a `Docs` regardless of what vector store you use. If you would like to manage caching embeddings via an external database or other strategy,
+you can populate a `Docs` object directly via
+the `add_texts` object. That can take chunked texts and documents, which are serializable objects, to populate `Docs`.
+
+You also can simply use a separate vector database by setting the `doc_index` and `texts_index` explicitly when building the `Docs` object.
+
+## Customizing Prompts
+
+You can customize any of the prompts, using the `PromptCollection` class. For example, if you want to change the prompt for the question, you can do:
+
+```python
+from paperqa import Docs, Answer, PromptCollection
+from langchain.prompts import PromptTemplate
+
+my_qaprompt = PromptTemplate(
+    input_variables=["context", "question"],
+    template="Answer the question '{question}' "
+    "Use the context below if helpful. "
+    "You can cite the context using the key "
+    "like (Example2012). "
+    "If there is insufficient context, write a poem "
+    "about how you cannot answer.\n\n"
+    "Context: {context}\n\n")
+prompts=PromptCollection(qa=my_qaprompt)
+docs = Docs(prompts=prompts)
+```
+
+### Pre and Post Prompts
+
+Following the syntax above, you can also include prompts that
+are executed after the query and before the query. For example, you can use this to critique the answer.
+
+
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
 It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
 
 ### How is this different from LangChain?
 
 It's not! We use langchain to abstract the LLMS, and the process is very similar to the `map_reduce` chain in LangChain.
 
-### Caching
-
-This code will cache responses from LLMS by default in `$HOME/.paperqa/llm_cache.db`. Delete this file to clear the cache.
-
 ### Can I use different LLMs?
 
 Yes, you can use any LLMs from [langchain](https://langchain.readthedocs.io/) by passing the `llm` argument to the `Docs` class. You can use different LLMs for summarization and for question answering too.
 
 ### Where do the documents come from?
 
 You can provide your own. I use some of my own code to pull papers from Google Scholar. This code is not included because it may enable people to violate Google's terms of service and publisher's terms of service.
@@ -298,19 +442,7 @@
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
-
-### PDF Reading Options
-
-By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
-
-```sh
-pip install pymupdf
-```
-
-### Callbacks
-
-TODO
```

### Comparing `paper-qa-2.1.1/README.md` & `paper-qa-3.0.0.dev0/paper_qa.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,72 @@
-# Paper QA
+Metadata-Version: 2.1
+Name: paper-qa
+Version: 3.0.0.dev0
+Summary: LLM Chain for answering questions from docs 
+Home-page: https://github.com/whitead/paper-qa
+Author: Andrew White
+Author-email: white.d.andrew@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Paper QA- [Paper QA](#paper-qa)
+- [Paper QA- Paper QA](#paper-qa--paper-qa)
+  - [Output Example](#output-example)
+    - [References](#references)
+  - [Hugging Face Demo](#hugging-face-demo)
+  - [Install](#install)
+  - [Usage](#usage)
+    - [Adding Documents](#adding-documents)
+    - [Choosing Model](#choosing-model)
+    - [Adjusting number of sources](#adjusting-number-of-sources)
+    - [Using Code or HTML](#using-code-or-html)
+  - [Version 3 Changes](#version-3-changes)
+    - [New Features](#new-features)
+    - [Naming](#naming)
+    - [Breaking Changes](#breaking-changes)
+  - [Notebooks](#notebooks)
+  - [Agents (experimental)](#agents-experimental)
+  - [Where do I get papers?](#where-do-i-get-papers)
+    - [Zotero](#zotero)
+    - [Paper Scraper](#paper-scraper)
+  - [PDF Reading Options](#pdf-reading-options)
+  - [Typewriter View](#typewriter-view)
+  - [Caching](#caching-1)
+    - [Caching Embeddings](#caching-embeddings)
+  - [Customizing Prompts](#customizing-prompts)
+    - [Pre and Post Prompts](#pre-and-post-prompts)
+  - [FAQ](#faq)
+    - [How is this different from LlamaIndex?](#how-is-this-different-from-llamaindex)
+    - [How is this different from LangChain?](#how-is-this-different-from-langchain)
+    - [Can I use different LLMs?](#can-i-use-different-llms)
+    - [Where do the documents come from?](#where-do-the-documents-come-from)
+    - [Can I save or load?](#can-i-save-or-load)
+
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
 
 This is a minimal package for doing question and answering from
-PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
-generate answers.
+PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations.
 
-It uses the process shown below:
+By default, it uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. However, via [langchain](https://github.com/hwchase17/langchain) you can use open-source models or embeddings (see details below).
 
-```
-embed docs into vectors -> embed query into vector -> search for top k passages in docs
+PaperQA uses the process shown below:
 
-create summary of each passage relevant to query -> put summaries into prompt -> generate answer
-```
-
-<img src="https://user-images.githubusercontent.com/908389/230854097-8fa96768-c694-45c0-bb04-3a7386facef3.jpeg" width="600" alt="Process of vector search, refinement, and answer with context">
+1. embed docs into vectors
+2. embed query into vector
+3. search for top k passages in docs
+4. create summary of each passage relevant to query
+5. put summaries into prompt
+6. generate answer with prompt
 
 ## Output Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
@@ -28,15 +74,14 @@
 
 Journet6644: Journet, Catherine, et al. "Large-scale production of single-walled carbon nanotubes by the electric-arc technique." nature 388.6644 (1997): 756-758.
 
 Tulevski2007: Tulevski, George S., et al. "Chemically assisted directed assembly of carbon nanotubes for the fabrication of large-scale device arrays." Journal of the American Chemical Society 129.39 (2007): 11964-11968.
 
 Chen2014: Chen, Haitian, et al. "Large-scale complementary macroelectronics using hybrid integration of carbon nanotubes and IGZO thin-film transistors." Nature communications 5.1 (2014): 4097.
 
-
 ## Hugging Face Demo
 
 [Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
 
 ## Install
 
 Install with pip:
@@ -63,28 +108,32 @@
 
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
+### Adding Documents
+
+`add` will add from paths. You can also use `add_file` (expects a file object) or `add_url` to work with other sources.
+
 ### Choosing Model
 
 By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
 
 ```py
 docs = Docs(llm='gpt-3.5-turbo')
 ```
 
 or you can use any other model available in [langchain](https://github.com/hwchase17/langchain):
 
 ```py
-from langchain.llms import Anthropic, OpenAIChat
-model = OpenAIChat(model='gpt-4')
-summary_model = Anthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
+from langchain.chat_models import ChatAnthropic, ChatOpenAI
+model = ChatOpenAI(model='gpt-4')
+summary_model = ChatAnthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
 docs = Docs(llm=model, summary_llm=summary_model)
 ```
 
 
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
@@ -143,14 +192,63 @@
 for f in source_files:
     # this assumes the file names are unique in code
     docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
 answer = docs.query("Where is the search bar in the header defined?")
 print(answer)
 ```
 
+## Version 3 Changes
+
+Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
+
+
+### New Features
+
+The following new features are in v3:
+
+1. `add_url` and `add_file` are now supported for adding from URLs and file objects
+2. Prompts can be customized, and now can be executed pre and post query
+3. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
+4. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
+5. Various simplifications, bug fixes, and performance improvements
+
+### Naming
+
+The following table shows the old names and the new names:
+
+| Old Name | New Name | Explanation |
+| :--- | :---: | ---: |
+| `key` | `name` | Name is a natural language name for text. |
+| `dockey` | `docname` | Docname is a natural language name for a document. |
+| `hash` | `dockey` | Dockey is a unique identifier for the document. |
+
+
+### Breaking Changes
+
+
+#### Pickled objects
+
+The pickled objects are not compatible with the new version.
+
+#### Agents
+
+The agent functionality has been removed, as it's not a core focus of the library
+
+#### Caching
+
+Caching has been removed because it's not a core focus of the library. See FAQ below for how to use caching.
+
+#### Answers
+
+Answers will not include passages, but instead return dockeys that can be used to retrieve the passages. Tokens/cost will also not be counted since that is built into langchain by default (see below for an example).
+
+#### Search Query
+
+The search query chain has been removed. You can use langchain directly to do this.
+
 ## Notebooks
 
 If you want to use this in an jupyter notebook or colab, you need to run the following command:
 
 ```python
 import nest_asyncio
 nest_asyncio.apply()
@@ -247,28 +345,88 @@
     except ValueError as e:
         # sometimes this happens if PDFs aren't downloaded or readable
         print('Could not read', path, e)
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer)
 ```
 
+## PDF Reading Options
+
+By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
+
+```sh
+pip install pymupdf
+```
+
+## Typewriter View
+
+To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
+
+```python
+from paperqa import Docs
+from langchain.chat_models import ChatOpenAI
+
+my_llm = ChatOpenAI(model='gpt-3.5-turbo', streaming=True)
+docs = Docs(llm=my_llm)
+```
+
+## Caching
+
+You can using the builtin langchain caching capabilities. Just run this code at the top of yours:
+
+```py
+from langchain.cache import InMemoryCache
+langchain.llm_cache = InMemoryCache()
+```
+
+### Caching Embeddings
+
+In general, embeddings are cached when you pickle a `Docs` regardless of what vector store you use. If you would like to manage caching embeddings via an external database or other strategy,
+you can populate a `Docs` object directly via
+the `add_texts` object. That can take chunked texts and documents, which are serializable objects, to populate `Docs`.
+
+You also can simply use a separate vector database by setting the `doc_index` and `texts_index` explicitly when building the `Docs` object.
+
+## Customizing Prompts
+
+You can customize any of the prompts, using the `PromptCollection` class. For example, if you want to change the prompt for the question, you can do:
+
+```python
+from paperqa import Docs, Answer, PromptCollection
+from langchain.prompts import PromptTemplate
+
+my_qaprompt = PromptTemplate(
+    input_variables=["context", "question"],
+    template="Answer the question '{question}' "
+    "Use the context below if helpful. "
+    "You can cite the context using the key "
+    "like (Example2012). "
+    "If there is insufficient context, write a poem "
+    "about how you cannot answer.\n\n"
+    "Context: {context}\n\n")
+prompts=PromptCollection(qa=my_qaprompt)
+docs = Docs(prompts=prompts)
+```
+
+### Pre and Post Prompts
+
+Following the syntax above, you can also include prompts that
+are executed after the query and before the query. For example, you can use this to critique the answer.
+
+
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
 It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
 
 ### How is this different from LangChain?
 
 It's not! We use langchain to abstract the LLMS, and the process is very similar to the `map_reduce` chain in LangChain.
 
-### Caching
-
-This code will cache responses from LLMS by default in `$HOME/.paperqa/llm_cache.db`. Delete this file to clear the cache.
-
 ### Can I use different LLMs?
 
 Yes, you can use any LLMs from [langchain](https://langchain.readthedocs.io/) by passing the `llm` argument to the `Docs` class. You can use different LLMs for summarization and for question answering too.
 
 ### Where do the documents come from?
 
 You can provide your own. I use some of my own code to pull papers from Google Scholar. This code is not included because it may enable people to violate Google's terms of service and publisher's terms of service.
@@ -284,19 +442,7 @@
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
-
-### PDF Reading Options
-
-By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
-
-```sh
-pip install pymupdf
-```
-
-### Callbacks
-
-TODO
```

### Comparing `paper-qa-2.1.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.0.0.dev0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,58 @@
-Metadata-Version: 2.1
-Name: paper-qa
-Version: 2.1.1
-Summary: LLM Chain for answering questions from docs 
-Home-page: https://github.com/whitead/paper-qa
-Author: Andrew White
-Author-email: white.d.andrew@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# Paper QA- [Paper QA](#paper-qa)
+- [Paper QA- Paper QA](#paper-qa--paper-qa)
+  - [Output Example](#output-example)
+    - [References](#references)
+  - [Hugging Face Demo](#hugging-face-demo)
+  - [Install](#install)
+  - [Usage](#usage)
+    - [Adding Documents](#adding-documents)
+    - [Choosing Model](#choosing-model)
+    - [Adjusting number of sources](#adjusting-number-of-sources)
+    - [Using Code or HTML](#using-code-or-html)
+  - [Version 3 Changes](#version-3-changes)
+    - [New Features](#new-features)
+    - [Naming](#naming)
+    - [Breaking Changes](#breaking-changes)
+  - [Notebooks](#notebooks)
+  - [Agents (experimental)](#agents-experimental)
+  - [Where do I get papers?](#where-do-i-get-papers)
+    - [Zotero](#zotero)
+    - [Paper Scraper](#paper-scraper)
+  - [PDF Reading Options](#pdf-reading-options)
+  - [Typewriter View](#typewriter-view)
+  - [Caching](#caching-1)
+    - [Caching Embeddings](#caching-embeddings)
+  - [Customizing Prompts](#customizing-prompts)
+    - [Pre and Post Prompts](#pre-and-post-prompts)
+  - [FAQ](#faq)
+    - [How is this different from LlamaIndex?](#how-is-this-different-from-llamaindex)
+    - [How is this different from LangChain?](#how-is-this-different-from-langchain)
+    - [Can I use different LLMs?](#can-i-use-different-llms)
+    - [Where do the documents come from?](#where-do-the-documents-come-from)
+    - [Can I save or load?](#can-i-save-or-load)
 
-# Paper QA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
 
 This is a minimal package for doing question and answering from
-PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
-generate answers.
+PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations.
 
-It uses the process shown below:
+By default, it uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. However, via [langchain](https://github.com/hwchase17/langchain) you can use open-source models or embeddings (see details below).
 
-```
-embed docs into vectors -> embed query into vector -> search for top k passages in docs
-
-create summary of each passage relevant to query -> put summaries into prompt -> generate answer
-```
+PaperQA uses the process shown below:
 
-<img src="https://user-images.githubusercontent.com/908389/230854097-8fa96768-c694-45c0-bb04-3a7386facef3.jpeg" width="600" alt="Process of vector search, refinement, and answer with context">
+1. embed docs into vectors
+2. embed query into vector
+3. search for top k passages in docs
+4. create summary of each passage relevant to query
+5. put summaries into prompt
+6. generate answer with prompt
 
 ## Output Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
@@ -42,15 +60,14 @@
 
 Journet6644: Journet, Catherine, et al. "Large-scale production of single-walled carbon nanotubes by the electric-arc technique." nature 388.6644 (1997): 756-758.
 
 Tulevski2007: Tulevski, George S., et al. "Chemically assisted directed assembly of carbon nanotubes for the fabrication of large-scale device arrays." Journal of the American Chemical Society 129.39 (2007): 11964-11968.
 
 Chen2014: Chen, Haitian, et al. "Large-scale complementary macroelectronics using hybrid integration of carbon nanotubes and IGZO thin-film transistors." Nature communications 5.1 (2014): 4097.
 
-
 ## Hugging Face Demo
 
 [Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
 
 ## Install
 
 Install with pip:
@@ -77,28 +94,32 @@
 
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
+### Adding Documents
+
+`add` will add from paths. You can also use `add_file` (expects a file object) or `add_url` to work with other sources.
+
 ### Choosing Model
 
 By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
 
 ```py
 docs = Docs(llm='gpt-3.5-turbo')
 ```
 
 or you can use any other model available in [langchain](https://github.com/hwchase17/langchain):
 
 ```py
-from langchain.llms import Anthropic, OpenAIChat
-model = OpenAIChat(model='gpt-4')
-summary_model = Anthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
+from langchain.chat_models import ChatAnthropic, ChatOpenAI
+model = ChatOpenAI(model='gpt-4')
+summary_model = ChatAnthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
 docs = Docs(llm=model, summary_llm=summary_model)
 ```
 
 
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
@@ -157,14 +178,63 @@
 for f in source_files:
     # this assumes the file names are unique in code
     docs.add(f, citation='File ' + os.path.name(f), key=os.path.name(f))
 answer = docs.query("Where is the search bar in the header defined?")
 print(answer)
 ```
 
+## Version 3 Changes
+
+Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
+
+
+### New Features
+
+The following new features are in v3:
+
+1. `add_url` and `add_file` are now supported for adding from URLs and file objects
+2. Prompts can be customized, and now can be executed pre and post query
+3. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
+4. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
+5. Various simplifications, bug fixes, and performance improvements
+
+### Naming
+
+The following table shows the old names and the new names:
+
+| Old Name | New Name | Explanation |
+| :--- | :---: | ---: |
+| `key` | `name` | Name is a natural language name for text. |
+| `dockey` | `docname` | Docname is a natural language name for a document. |
+| `hash` | `dockey` | Dockey is a unique identifier for the document. |
+
+
+### Breaking Changes
+
+
+#### Pickled objects
+
+The pickled objects are not compatible with the new version.
+
+#### Agents
+
+The agent functionality has been removed, as it's not a core focus of the library
+
+#### Caching
+
+Caching has been removed because it's not a core focus of the library. See FAQ below for how to use caching.
+
+#### Answers
+
+Answers will not include passages, but instead return dockeys that can be used to retrieve the passages. Tokens/cost will also not be counted since that is built into langchain by default (see below for an example).
+
+#### Search Query
+
+The search query chain has been removed. You can use langchain directly to do this.
+
 ## Notebooks
 
 If you want to use this in an jupyter notebook or colab, you need to run the following command:
 
 ```python
 import nest_asyncio
 nest_asyncio.apply()
@@ -261,28 +331,88 @@
     except ValueError as e:
         # sometimes this happens if PDFs aren't downloaded or readable
         print('Could not read', path, e)
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer)
 ```
 
+## PDF Reading Options
+
+By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
+
+```sh
+pip install pymupdf
+```
+
+## Typewriter View
+
+To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
+
+```python
+from paperqa import Docs
+from langchain.chat_models import ChatOpenAI
+
+my_llm = ChatOpenAI(model='gpt-3.5-turbo', streaming=True)
+docs = Docs(llm=my_llm)
+```
+
+## Caching
+
+You can using the builtin langchain caching capabilities. Just run this code at the top of yours:
+
+```py
+from langchain.cache import InMemoryCache
+langchain.llm_cache = InMemoryCache()
+```
+
+### Caching Embeddings
+
+In general, embeddings are cached when you pickle a `Docs` regardless of what vector store you use. If you would like to manage caching embeddings via an external database or other strategy,
+you can populate a `Docs` object directly via
+the `add_texts` object. That can take chunked texts and documents, which are serializable objects, to populate `Docs`.
+
+You also can simply use a separate vector database by setting the `doc_index` and `texts_index` explicitly when building the `Docs` object.
+
+## Customizing Prompts
+
+You can customize any of the prompts, using the `PromptCollection` class. For example, if you want to change the prompt for the question, you can do:
+
+```python
+from paperqa import Docs, Answer, PromptCollection
+from langchain.prompts import PromptTemplate
+
+my_qaprompt = PromptTemplate(
+    input_variables=["context", "question"],
+    template="Answer the question '{question}' "
+    "Use the context below if helpful. "
+    "You can cite the context using the key "
+    "like (Example2012). "
+    "If there is insufficient context, write a poem "
+    "about how you cannot answer.\n\n"
+    "Context: {context}\n\n")
+prompts=PromptCollection(qa=my_qaprompt)
+docs = Docs(prompts=prompts)
+```
+
+### Pre and Post Prompts
+
+Following the syntax above, you can also include prompts that
+are executed after the query and before the query. For example, you can use this to critique the answer.
+
+
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
 It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
 
 ### How is this different from LangChain?
 
 It's not! We use langchain to abstract the LLMS, and the process is very similar to the `map_reduce` chain in LangChain.
 
-### Caching
-
-This code will cache responses from LLMS by default in `$HOME/.paperqa/llm_cache.db`. Delete this file to clear the cache.
-
 ### Can I use different LLMs?
 
 Yes, you can use any LLMs from [langchain](https://langchain.readthedocs.io/) by passing the `llm` argument to the `Docs` class. You can use different LLMs for summarization and for question answering too.
 
 ### Where do the documents come from?
 
 You can provide your own. I use some of my own code to pull papers from Google Scholar. This code is not included because it may enable people to violate Google's terms of service and publisher's terms of service.
@@ -298,19 +428,7 @@
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
-
-### PDF Reading Options
-
-By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
-
-```sh
-pip install pymupdf
-```
-
-### Callbacks
-
-TODO
```

### Comparing `paper-qa-2.1.1/paperqa/contrib/zotero.py` & `paper-qa-3.0.0.dev0/paperqa/contrib/zotero.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,57 @@
 # This file gets PDF files from the user's Zotero library
 import logging
 import os
-from collections import namedtuple
 from pathlib import Path
-from typing import Optional, Union
+from typing import List, Optional, Union, cast
+
+from pydantic import BaseModel
 
 try:
     from pyzotero import zotero
 except ImportError:
     raise ImportError("Please install pyzotero: `pip install pyzotero`")
-from ..paths import CACHE_PATH
+from ..paths import PAPERQA_DIR
 from ..types import StrPath
 from ..utils import count_pdf_pages
 
-ZoteroPaper = namedtuple(
-    "ZoteroPaper", ["key", "title", "pdf", "num_pages", "zotero_key", "details"]
-)
-
 
-def _zotero_paper_repr(self) -> str:
-    return f'ZoteroPaper(\n    key = "{self.key}",\n    title = "{self.title}",\n    pdf = "{self.pdf}",\n    num_pages = {self.num_pages},\n    zotero_key = "{self.zotero_key}",\n    details = ...\n)'
+class ZoteroPaper(BaseModel):
+    """A paper from Zotero.
 
+    Attributes
+    ----------
+    key : str
+        The citation key.
+    title : str
+        The title of the item.
+    pdf : Path
+        The path to the PDF for the item (pass to `paperqa.Docs`)
+    num_pages : int
+        The number of pages in the PDF.
+    zotero_key : str
+        The Zotero key for the item.
+    details : dict
+        The full item details from Zotero.
+    """
 
-ZoteroPaper.__repr__ = _zotero_paper_repr
+    key: str
+    title: str
+    pdf: Path
+    num_pages: int
+    zotero_key: str
+    details: dict
+
+    def __str__(self) -> str:
+        """Return the title of the paper."""
+        return (
+            f'ZoteroPaper(\n    key = "{self.key}",\n'
+            f'title = "{self.title}",\n    pdf = "{self.pdf}",\n    '
+            f'num_pages = {self.num_pages},\n    zotero_key = "{self.zotero_key}",\n    details = ...\n)'
+        )
 
 
 class ZoteroDB(zotero.Zotero):
     """An extension of pyzotero.zotero.Zotero to interface with paperqa.
 
     This class automatically reads in your `ZOTERO_USER_ID` and `ZOTERO_API_KEY`
     from your environment variables. If you do not have these, see
@@ -71,15 +96,15 @@
                 )
             else:
                 api_key = os.environ["ZOTERO_API_KEY"]
 
         self.logger.info(f"Using library ID: {library_id} with type: {library_type}.")
 
         if storage is None:
-            storage = CACHE_PATH.parent / "zotero"
+            storage = PAPERQA_DIR / "zotero"
 
         self.logger.info(f"Using cache location: {storage}")
         self.storage = storage
 
         super().__init__(
             library_type=library_type, library_id=library_id, api_key=api_key, **kwargs
         )
@@ -100,15 +125,15 @@
             raise TypeError("Pass the full item of the paper. The item must be a dict.")
 
         pdf_key = _extract_pdf_key(item)
 
         if pdf_key is None:
             return None
 
-        pdf_path = self.storage / (pdf_key + ".pdf")
+        pdf_path: Path = Path(self.storage / (pdf_key + ".pdf"))  # type: ignore
 
         if not pdf_path.exists():
             pdf_path.parent.mkdir(parents=True, exist_ok=True)
             self.logger.info(f"|  Downloading PDF for: {_get_citation_key(item)}")
             self.dump(pdf_key, pdf_path)
 
         return pdf_path
@@ -182,19 +207,19 @@
         if collection_name is not None and len(query_kwargs) > 0:
             raise ValueError(
                 "You cannot specify a `collection_name` and search query simultaneously!"
             )
 
         max_limit = 100
 
-        items = []
-        pdfs = []
+        items: List = []
+        pdfs: List[Path] = []
         i = 0
         actual_i = 0
-        num_remaining = limit - len(items)
+        num_remaining = limit
 
         collection_id = None
         if collection_name:
             collection_id = self._get_collection_id(
                 collection_name
             )  # raise error if not found
 
@@ -218,15 +243,15 @@
             # Filter:
             for item, pdf in zip(_items, _pdfs):
                 no_pdf = item is None or pdf is None
                 is_duplicate = pdf in pdfs
 
                 if no_pdf or is_duplicate:
                     continue
-
+                pdf = cast(Path, pdf)
                 title = item["data"]["title"] if "title" in item["data"] else ""
                 if len(items) >= start:
                     yield ZoteroPaper(
                         key=_get_citation_key(item),
                         title=title,
                         pdf=pdf,
                         num_pages=count_pdf_pages(pdf),
@@ -298,15 +323,15 @@
     short_title = "".join([c for c in short_title if c.isalnum()])
     last_name = "".join([c for c in last_name if c.isalnum()])
     date = "".join([c for c in date if c.isalnum()])
 
     return f"{last_name}_{short_title}_{date}_{item['key']}".replace(" ", "")
 
 
-def _extract_pdf_key(item: dict) -> str:
+def _extract_pdf_key(item: dict) -> Union[str, None]:
     """Extract the PDF key from a Zotero item."""
 
     if "links" not in item:
         return None
 
     if "attachment" not in item["links"]:
         return None
```

### Comparing `paper-qa-2.1.1/paperqa/docs.py` & `paper-qa-3.0.0.dev0/paperqa/docs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,344 +1,315 @@
 import asyncio
 import os
 import re
 import sys
+import tempfile
 from datetime import datetime
-from functools import reduce
+from io import BytesIO
 from pathlib import Path
-from typing import Callable, List, Optional, Tuple, Union
+from typing import BinaryIO, Dict, List, Optional, Set, Union, cast
 
-import langchain
-from langchain.cache import SQLiteCache
-from langchain.callbacks import OpenAICallbackHandler, get_openai_callback
-from langchain.callbacks.base import AsyncCallbackHandler
-from langchain.callbacks.manager import AsyncCallbackManager
+from langchain.base_language import BaseLanguageModel
 from langchain.chat_models import ChatOpenAI
-from langchain.docstore.document import Document
 from langchain.embeddings.base import Embeddings
 from langchain.embeddings.openai import OpenAIEmbeddings
-from langchain.llms.base import LLM
-from langchain.vectorstores import FAISS
+from langchain.vectorstores import FAISS, VectorStore
+from pydantic import BaseModel, validator
 
-from .paths import CACHE_PATH
-from .qaprompts import (
-    citation_prompt,
-    make_chain,
-    qa_prompt,
-    search_prompt,
-    select_paper_prompt,
-    summary_prompt,
-    get_score,
-)
+from .chains import get_score, make_chain
+from .paths import PAPERQA_DIR
 from .readers import read_doc
-from .types import Answer, Context
-from .utils import maybe_is_text, md5sum, gather_with_concurrency, guess_is_4xx
-
-os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
-langchain.llm_cache = SQLiteCache(CACHE_PATH)
+from .types import Answer, CallbackFactory, Context, Doc, DocKey, PromptCollection, Text
+from .utils import (
+    gather_with_concurrency,
+    guess_is_4xx,
+    maybe_is_html,
+    maybe_is_pdf,
+    maybe_is_text,
+    md5sum,
+    name_in_text,
+)
 
 
-class Docs:
+class Docs(BaseModel, arbitrary_types_allowed=True, smart_union=True):
     """A collection of documents to be used for answering questions."""
 
-    def __init__(
-        self,
-        chunk_size_limit: int = 3000,
-        llm: Optional[Union[LLM, str]] = None,
-        summary_llm: Optional[Union[LLM, str]] = None,
-        name: str = "default",
-        index_path: Optional[Path] = None,
-        embeddings: Optional[Embeddings] = None,
-        max_concurrent: int = 5,
-    ) -> None:
-        """Initialize the collection of documents.
-
-        Args:
-            chunk_size_limit: The maximum number of characters to use for a single chunk of text.
-            llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
-            summary_llm: The language model to use for summarizing documents. If None, llm is used.
-            name: The name of the collection.
-            index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
-            embeddings: The embeddings to use for indexing documents. Default - OpenAI embeddings
-            max_concurrent: Number of concurrent LLM model calls to make
-        """
-        self.docs = []
-        self.chunk_size_limit = chunk_size_limit
-        self.keys = set()
-        self._faiss_index = None
-        self._doc_index = None
-        self.update_llm(llm, summary_llm)
-        if index_path is None:
-            index_path = Path.home() / ".paperqa" / name
-        self.index_path = index_path
-        self.name = name
-        if embeddings is None:
-            embeddings = OpenAIEmbeddings()
-        self.embeddings = embeddings
-        self.max_concurrent = max_concurrent
-        self._deleted_keys = set()
+    docs: Dict[DocKey, Doc] = {}
+    texts: List[Text] = []
+    docnames: Set[str] = set()
+    texts_index: Optional[VectorStore] = None
+    doc_index: Optional[VectorStore] = None
+    llm: Union[str, BaseLanguageModel] = ChatOpenAI(
+        temperature=0.1, model="gpt-3.5-turbo", client=None
+    )
+    summary_llm: Optional[Union[str, BaseLanguageModel]] = None
+    name: str = "default"
+    index_path: Optional[Path] = PAPERQA_DIR / name
+    embeddings: Embeddings = OpenAIEmbeddings(client=None)
+    max_concurrent: int = 5
+    deleted_dockeys: Set[DocKey] = set()
+    prompts: PromptCollection = PromptCollection()
+
+    # TODO: Not sure how to get this to work
+    # while also passing mypy checks
+    @validator("llm", "summary_llm")
+    def check_llm(cls, v: Union[BaseLanguageModel, str]) -> BaseLanguageModel:
+        if type(v) is str:
+            return ChatOpenAI(temperature=0.1, model=v, client=None)
+        return v
+
+    @validator("summary_llm", always=True)
+    def copy_llm_if_not_set(cls, v, values):
+        return v or values["llm"]
 
     def update_llm(
         self,
-        llm: Optional[Union[LLM, str]] = None,
-        summary_llm: Optional[Union[LLM, str]] = None,
+        llm: Union[BaseLanguageModel, str],
+        summary_llm: Optional[Union[BaseLanguageModel, str]] = None,
     ) -> None:
         """Update the LLM for answering questions."""
-        if llm is None and os.environ.get("OPENAI_API_KEY") is not None:
-            llm = "gpt-3.5-turbo"
         if type(llm) is str:
-            llm = ChatOpenAI(temperature=0.1, model_name=llm)
+            llm = ChatOpenAI(temperature=0.1, model=llm, client=None)
         if type(summary_llm) is str:
-            summary_llm = ChatOpenAI(temperature=0.1, model_name=summary_llm)
-        self.llm = llm
+            summary_llm = ChatOpenAI(temperature=0.1, model=summary_llm, client=None)
+        self.llm = cast(BaseLanguageModel, llm)
         if summary_llm is None:
             summary_llm = llm
-        self.summary_llm = summary_llm
+        self.summary_llm = cast(BaseLanguageModel, summary_llm)
 
-    def get_unique_key(self, key: str) -> str:
-        """Create a unique key given proposed key"""
+    def get_unique_name(self, docname: str) -> str:
+        """Create a unique name given proposed name"""
         suffix = ""
-        while key + suffix in self.keys:
+        while docname + suffix in self.docnames:
             # move suffix to next letter
             if suffix == "":
                 suffix = "a"
             else:
                 suffix = chr(ord(suffix) + 1)
-        key += suffix
-        return key
+        docname += suffix
+        return docname
 
-    def add(
+    def add_file(
         self,
-        path: str,
+        file: BinaryIO,
         citation: Optional[str] = None,
-        key: Optional[str] = None,
-        disable_check: bool = False,
-        chunk_chars: Optional[int] = 3000,
+        docname: Optional[str] = None,
+        dockey: Optional[DocKey] = None,
+        chunk_chars: int = 3000,
     ) -> str:
         """Add a document to the collection."""
+        # just put in temp file and use existing method
+        suffix = ".txt"
+        if maybe_is_pdf(file):
+            suffix = ".pdf"
+        elif maybe_is_html(file):
+            suffix = ".html"
+
+        with tempfile.NamedTemporaryFile(suffix=suffix) as f:
+            f.write(file.read())
+            f.seek(0)
+            return self.add(
+                Path(f.name),
+                citation=citation,
+                docname=docname,
+                dockey=dockey,
+                chunk_chars=chunk_chars,
+            )
 
-        # first check to see if we already have this document
-        # this way we don't make api call to create citation on file we already have
-        hash = md5sum(path)
-        if hash in [d["hash"] for d in self.docs]:
-            raise ValueError(f"Document {path} already in collection.")
+    def add_url(
+        self,
+        url: str,
+        citation: Optional[str] = None,
+        docname: Optional[str] = None,
+        dockey: Optional[DocKey] = None,
+        chunk_chars: int = 3000,
+    ) -> str:
+        """Add a document to the collection."""
+        import urllib.request
+
+        with urllib.request.urlopen(url) as f:
+            # need to wrap to enable seek
+            file = BytesIO(f.read())
+            return self.add_file(
+                file,
+                citation=citation,
+                docname=docname,
+                dockey=dockey,
+                chunk_chars=chunk_chars,
+            )
 
+    def add(
+        self,
+        path: Path,
+        citation: Optional[str] = None,
+        docname: Optional[str] = None,
+        disable_check: bool = False,
+        dockey: Optional[DocKey] = None,
+        chunk_chars: int = 3000,
+    ) -> str:
+        """Add a document to the collection."""
+        if dockey is None:
+            dockey = md5sum(path)
         if citation is None:
             # skip system because it's too hesitant to answer
             cite_chain = make_chain(
-                prompt=citation_prompt, llm=self.summary_llm, skip_system=True
+                prompt=self.prompts.cite,
+                llm=cast(BaseLanguageModel, self.summary_llm),
+                skip_system=True,
             )
             # peak first chunk
-            texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
+            fake_doc = Doc(docname="", citation="", dockey=dockey)
+            texts = read_doc(path, fake_doc, chunk_chars=chunk_chars, overlap=100)
             if len(texts) == 0:
                 raise ValueError(f"Could not read document {path}. Is it empty?")
-            citation = cite_chain.run(texts[0])
+            citation = cite_chain.run(texts[0].text)
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
-        if key is None:
+        if docname is None:
             # get first name and year from citation
-            try:
-                author = re.search(r"([A-Z][a-z]+)", citation).group(1)
-            except AttributeError:
+            match = re.search(r"([A-Z][a-z]+)", citation)
+            if match is not None:
+                author = match.group(1)  # type: ignore
+            else:
                 # panicking - no word??
                 raise ValueError(
-                    f"Could not parse key from citation {citation}. Consider just passing key explicitly - e.g. docs.py (path, citation, key='mykey')"
+                    f"Could not parse docname from citation {citation}. "
+                    "Consider just passing key explicitly - e.g. docs.py "
+                    "(path, citation, key='mykey')"
                 )
-            try:
-                year = re.search(r"(\d{4})", citation).group(1)
-            except AttributeError:
-                year = ""
-            key = f"{author}{year}"
-        key = self.get_unique_key(key)
-        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
+            year = ""
+            match = re.search(r"(\d{4})", citation)
+            if match is not None:
+                year = match.group(1)  # type: ignore
+            docname = f"{author}{year}"
+        docname = self.get_unique_name(docname)
+        doc = Doc(docname=docname, citation=citation, dockey=dockey)
+        texts = read_doc(path, doc, chunk_chars=chunk_chars, overlap=100)
         # loose check to see if document was loaded
-        #
-        if len("".join(texts)) < 10 or (
-            not disable_check and not maybe_is_text("".join(texts))
+        if len(texts[0].text) < 10 or (
+            not disable_check and not maybe_is_text(texts[0].text)
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
             )
-        self.add_texts(texts, metadata, hash)
-        return key
+        self.add_texts(texts, doc)
+        return docname
 
     def add_texts(
         self,
-        texts: List[str],
-        metadatas: List[dict],
-        hash: str,
-        text_embeddings: Optional[List[List[float]]] = None,
+        texts: List[Text],
+        doc: Doc,
     ):
-        """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself.
-
-        The metadatas should have the following keys: citation, dockey (same as key arg), and key (unique key for each chunk).
-        The hash is a unique identifier for the document. It is used to check if the document has already been added.
-        """
-        if len(texts) != len(metadatas):
-            raise ValueError("texts and metadatas must have the same length.")
-
-        if hash in [d["hash"] for d in self.docs]:
-            raise ValueError(f"Document already in collection.")
-
-        key = metadatas[0]["dockey"]
-        citation = metadatas[0]["citation"]
-        if key in self.keys:
-            new_key = self.get_unique_key(key)
-            for metadata in metadatas:
-                metadata["dockey"] = new_key
-                metadata["key"] = metadata["key"].replace(key, new_key)
-            key = new_key
-        if text_embeddings is None:
-            text_embeddings = self.embeddings.embed_documents(texts)
-        if self._faiss_index is not None:
-            self._faiss_index.add_embeddings(
-                list(zip(texts, text_embeddings)), metadatas=metadatas
-            )
-        if self._doc_index is not None:
-            self._doc_index.add_texts([citation], metadatas=[{"key": key}])
-        self.docs.append(
-            dict(
-                texts=texts,
-                metadata=metadatas,
-                key=key,
-                hash=hash,
-                text_embeddings=text_embeddings,
-            )
-        )
-        self.keys.add(key)
+        """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself."""
+        if doc.dockey in self.docs:
+            raise ValueError("Document already in collection.")
+        if len(texts) == 0:
+            raise ValueError("No texts to add.")
+        if doc.docname in self.docnames:
+            new_docname = self.get_unique_name(doc.docname)
+            for t in texts:
+                t.name = t.name.replace(doc.docname, new_docname)
+            doc.docname = new_docname
+        if texts[0].embeddings is None:
+            text_embeddings = self.embeddings.embed_documents([t.text for t in texts])
+            for i, t in enumerate(texts):
+                t.embeddings = text_embeddings[i]
+        else:
+            text_embeddings = cast(List[List[float]], [t.embeddings for t in texts])
+        if self.texts_index is not None:
+            try:
+                self.texts_index.add_embeddings(  # type: ignore
+                    list(zip(texts, text_embeddings)),
+                    metadatas=[
+                        t.dict(exclude={"embeddings", "text"}) for t in self.texts
+                    ],
+                )
+            except AttributeError:
+                raise ValueError("Need a vector store that supports adding embeddings.")
+        if self.doc_index is not None:
+            self.doc_index.add_texts([doc.citation], metadatas=[{"dockey": doc.dockey}])
+        self.docs[doc.dockey] = doc
+        self.texts += texts
+        self.docnames.add(doc.docname)
 
-    def delete(self, key: str) -> None:
+    def delete(
+        self, name: Optional[str] = None, dockey: Optional[DocKey] = None
+    ) -> None:
         """Delete a document from the collection."""
-        if key not in self.keys:
-            return
-        self.keys.remove(key)
-        self.docs = [doc for doc in self.docs if doc["key"] != key]
-        self._deleted_keys.add(key)
-
-    def clear(self) -> None:
-        """Clear the collection of documents."""
-        self.docs = []
-        self.keys = set()
-        self._faiss_index = None
-        self._doc_index = None
-        # delete index file
-        pkl = self.index_path / "index.pkl"
-        if pkl.exists():
-            pkl.unlink()
-        fs = self.index_path / "index.faiss"
-        if fs.exists():
-            fs.unlink()
-
-    def doc_previews(self) -> List[Tuple[int, str, str]]:
-        """Return a list of tuples of (key, citation) for each document."""
-        return [
-            (
-                len(doc["texts"]),
-                doc["metadata"][0]["dockey"],
-                doc["metadata"][0]["citation"],
-                doc["hash"],
-            )
-            for doc in self.docs
-        ]
+        if name is not None:
+            doc = next((doc for doc in self.docs.values() if doc.docname == name), None)
+            if doc is None:
+                return
+            self.docnames.remove(doc.docname)
+            dockey = doc.dockey
+        del self.docs[dockey]
+        self.deleted_dockeys.add(dockey)
 
     async def adoc_match(
-        self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
-    ) -> List[str]:
-        """Return a list of documents that match the query."""
+        self, query: str, k: int = 25, get_callbacks: CallbackFactory = lambda x: None
+    ) -> Set[DocKey]:
+        """Return a list of dockeys that match the query."""
         if len(self.docs) == 0:
-            return ""
-        if self._doc_index is None:
-            texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
-            self._doc_index = FAISS.from_texts(
+            return set()
+        if self.doc_index is None:
+            texts = [doc.citation for doc in self.docs.values()]
+            metadatas = [d.dict() for d in self.docs.values()]
+            self.doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
-        docs = self._doc_index.max_marginal_relevance_search(
-            query, k=k + len(self._deleted_keys)
+        matches = self.doc_index.max_marginal_relevance_search(
+            query, k=k + len(self.deleted_dockeys)
         )
-        docs = [doc for doc in docs if doc.metadata["key"] not in self._deleted_keys]
-        chain = make_chain(select_paper_prompt, self.summary_llm)
-        papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
-        result = await chain.arun(
-            question=query, papers="\n".join(papers), callbacks=callbacks
+        matched_docs = [self.docs[m.metadata["dockey"]] for m in matches]
+        chain = make_chain(
+            self.prompts.select, cast(BaseLanguageModel, self.summary_llm)
         )
-        return result
-
-    def doc_match(
-        self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
-    ) -> List[str]:
-        """Return a list of documents that match the query."""
-        if len(self.docs) == 0:
-            return ""
-        if self._doc_index is None:
-            texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
-            self._doc_index = FAISS.from_texts(
-                texts, metadatas=metadatas, embedding=self.embeddings
-            )
-        docs = self._doc_index.max_marginal_relevance_search(
-            query, k=k + len(self._deleted_keys)
+        papers = [f"{d.docname}: {d.citation}" for d in matched_docs]
+        result = await chain.arun(  # type: ignore
+            question=query, papers="\n".join(papers), callbacks=get_callbacks("filter")
         )
-        docs = [doc for doc in docs if doc.metadata["key"] not in self._deleted_keys]
-        chain = make_chain(select_paper_prompt, self.summary_llm)
-        papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
-        result = chain.run(
-            question=query, papers="\n".join(papers), callbacks=callbacks
-        )
-        return result
+        return set([d.dockey for d in matched_docs if d.docname in result])
 
     def __getstate__(self):
         state = self.__dict__.copy()
-        if self._faiss_index is not None:
-            state["_faiss_index"].save_local(self.index_path)
-        del state["_faiss_index"]
-        del state["_doc_index"]
-        return state
+        if self.texts_index is not None:
+            state["texts_index"].save_local(self.index_path)
+        del state["texts_index"]
+        del state["doc_index"]
+        return {"__dict__": state, "__fields_set__": self.__fields_set__}
 
     def __setstate__(self, state):
-        self.__dict__.update(state)
+        object.__setattr__(self, "__dict__", state["__dict__"])
+        object.__setattr__(self, "__fields_set__", state["__fields_set__"])
         try:
-            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
-        except:
+            self.texts_index = FAISS.load_local(self.index_path, self.embeddings)
+        except Exception:
             # they use some special exception type, but I don't want to import it
-            self._faiss_index = None
-        if not hasattr(self, "_doc_index"):
-            self._doc_index = None
-        # must be a better way to have backwards compatibility
-        if not hasattr(self, "_deleted_keys"):
-            self._deleted_keys = set()
-        if not hasattr(self, "max_concurrent"):
-            self.max_concurrent = 5
-        self.update_llm(None, None)
-
-    def _build_faiss_index(self):
-        if self._faiss_index is None:
-            texts = reduce(lambda x, y: x + y, [doc["texts"] for doc in self.docs], [])
-            text_embeddings = reduce(
-                lambda x, y: x + y, [doc["text_embeddings"] for doc in self.docs], []
-            )
-            metadatas = reduce(
-                lambda x, y: x + y, [doc["metadata"] for doc in self.docs], []
-            )
-            self._faiss_index = FAISS.from_embeddings(
+            self.texts_index = None
+
+    def _build_texts_index(self):
+        if self.texts_index is None:
+            raw_texts = [t.text for t in self.texts]
+            text_embeddings = [t.embeddings for t in self.texts]
+            metadatas = [t.dict(exclude={"embeddings", "text"}) for t in self.texts]
+            self.texts_index = FAISS.from_embeddings(
                 # wow adding list to the zip was tricky
-                text_embeddings=list(zip(texts, text_embeddings)),
+                text_embeddings=list(zip(raw_texts, text_embeddings)),
                 embedding=self.embeddings,
                 metadatas=metadatas,
             )
 
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
-        key_filter: Optional[List[str]] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+        get_callbacks: CallbackFactory = lambda x: None,
     ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
@@ -348,156 +319,128 @@
             asyncio.set_event_loop(loop)
         return loop.run_until_complete(
             self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
-                key_filter=key_filter,
                 get_callbacks=get_callbacks,
             )
         )
 
     async def aget_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
-        key_filter: Optional[List[str]] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+        get_callbacks: CallbackFactory = lambda x: None,
     ) -> Answer:
         if len(self.docs) == 0:
             return answer
-        if key_filter is not None:
-            answer.key_filter = key_filter
-        if self._faiss_index is None:
-            self._build_faiss_index()
+        if self.texts_index is None:
+            self._build_texts_index()
+        self.texts_index = cast(VectorStore, self.texts_index)
         _k = k
-        if answer.key_filter is not None:
+        if answer.dockey_filter is not None:
             _k = k * 10  # heuristic
         # want to work through indices but less k
         if marginal_relevance:
-            docs = self._faiss_index.max_marginal_relevance_search(
+            matches = self.texts_index.max_marginal_relevance_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
         else:
-            docs = self._faiss_index.similarity_search(
+            matches = self.texts_index.similarity_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
         # ok now filter
-        if answer.key_filter is not None:
-            # I realize that by testing for existence
-            # in strings that weird cases can
-            # happen - like FooBar can match FooBar2023
-            # but remember there are later checks
-            # The risk of explicitly parsing is that the
-            # language model may not give back in predictable
-            # format (e.g., - "FooBar and BarSoo are good papers")
-            docs = [doc for doc in docs if doc.metadata["dockey"] in answer.key_filter][
-                :k
+        if answer.dockey_filter is not None:
+            matches = [
+                m
+                for m in matches
+                if m.metadata["doc"]["dockey"] in answer.dockey_filter
             ]
 
-        async def process(doc):
-            if doc.metadata["dockey"] in self._deleted_keys:
-                return None, None
-            # check if it is already in answer (possible in agent setting)
-            if doc.metadata["key"] in [c.key for c in answer.contexts]:
-                return None, None
-            callbacks = [OpenAICallbackHandler()] + get_callbacks(
-                "evidence:" + doc.metadata["key"]
-            )
-            summary_chain = make_chain(summary_prompt, self.summary_llm)
+        # check if it is deleted
+        matches = [
+            m
+            for m in matches
+            if m.metadata["doc"]["dockey"] not in self.deleted_dockeys
+        ]
+
+        # check if it is already in answer
+        cur_names = [c.text.name for c in answer.contexts]
+        matches = [m for m in matches if m.metadata["name"] not in cur_names]
+
+        # now finally cut down
+        matches = matches[:k]
+
+        async def process(match):
+            callbacks = get_callbacks("evidence:" + match.metadata["name"])
+            summary_chain = make_chain(self.prompts.summary, self.summary_llm)
             # This is dangerous because it
-            # could mask errors that are important
+            # could mask errors that are important- like auth errors
             # I also cannot know what the exception
             # type is because any model could be used
             # my best idea is see if there is a 4XX
             # http code in the exception
             try:
                 context = await summary_chain.arun(
                     question=answer.question,
-                    context_str=doc.page_content,
-                    citation=doc.metadata["citation"],
+                    citation=match.metadata["doc"]["citation"],
+                    summary_length=answer.summary_length,
+                    text=match.page_content,
                     callbacks=callbacks,
                 )
             except Exception as e:
                 if guess_is_4xx(e):
-                    return None, None
+                    return None
                 raise e
+            if "not applicable" in context.lower():
+                return None
             c = Context(
-                key=doc.metadata["key"],
-                citation=doc.metadata["citation"],
                 context=context,
-                text=doc.page_content,
+                text=Text(
+                    text=match.page_content,
+                    name=match.metadata["name"],
+                    doc=Doc(**match.metadata["doc"]),
+                ),
                 score=get_score(context),
-                dockey=doc.metadata["dockey"],
             )
-            if "not applicable" not in c.context.casefold():
-                return c, callbacks[0]
-            return None, None
+            return c
 
         results = await gather_with_concurrency(
-            self.max_concurrent, *[process(doc) for doc in docs]
+            self.max_concurrent, *[process(m) for m in matches]
         )
         # filter out failures
-        results = [r for r in results if r[0] is not None]
-        answer.tokens += sum([cb.total_tokens for _, cb in results])
-        answer.cost += sum([cb.total_cost for _, cb in results])
-        contexts = [c for c, _ in results if c is not None]
+        contexts = [c for c in results if c is not None]
         if len(contexts) == 0:
             return answer
         contexts = sorted(contexts, key=lambda x: x.score, reverse=True)
         contexts = contexts[:max_sources]
-        # add to answer (if not already there)
-        keys = [c.key for c in answer.contexts]
-        for c in contexts:
-            if c.key not in keys:
-                answer.contexts.append(c)
-
+        # add to answer contexts
+        answer.contexts += contexts
         context_str = "\n\n".join(
-            [
-                f"{c.key}: {c.context}"
-                for c in answer.contexts
-                if "Not applicable" not in c.context
-            ]
+            [f"{c.text.name}: {c.context}" for c in answer.contexts]
         )
-        valid_keys = [
-            c.key for c in answer.contexts if "Not applicable" not in c.context
-        ]
-        if len(valid_keys) > 0:
-            context_str += "\n\nValid keys: " + ", ".join(valid_keys)
+        valid_names = [c.text.name for c in answer.contexts]
+        context_str += "\n\nValid keys: " + ", ".join(valid_names)
         answer.context = context_str
         return answer
 
-    def generate_search_query(self, query: str) -> List[str]:
-        """Generate a list of search strings that can be used to find
-        relevant papers.
-
-        Args:
-            query (str): The query to generate search strings for.
-        """
-
-        search_chain = make_chain(prompt=search_prompt, llm=self.summary_llm)
-        search_query = search_chain.run(question=query)
-        queries = [s for s in search_query.split("\n") if len(s) > 3]
-        # remove 2., 3. from queries
-        queries = [re.sub(r"^\d+\.\s*", "", q) for q in queries]
-        return queries
-
     def query(
         self,
         query: str,
         k: int = 10,
         max_sources: int = 5,
-        length_prompt: str = "about 100 words",
+        length_prompt="about 100 words",
         marginal_relevance: bool = True,
         answer: Optional[Answer] = None,
         key_filter: Optional[bool] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+        get_callbacks: CallbackFactory = lambda x: None,
     ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
@@ -523,71 +466,78 @@
         query: str,
         k: int = 10,
         max_sources: int = 5,
         length_prompt: str = "about 100 words",
         marginal_relevance: bool = True,
         answer: Optional[Answer] = None,
         key_filter: Optional[bool] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+        get_callbacks: CallbackFactory = lambda x: None,
     ) -> Answer:
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
         if answer is None:
-            answer = Answer(query)
+            answer = Answer(question=query, answer_length=length_prompt)
         if len(answer.contexts) == 0:
+            # this is heuristic - max_sources and len(docs) are not
+            # comparable - one is chunks and one is docs
             if key_filter or (key_filter is None and len(self.docs) > max_sources):
-                callbacks = [OpenAICallbackHandler()] + get_callbacks("filter")
-                keys = await self.adoc_match(answer.question, callbacks=callbacks)
-                answer.tokens += callbacks[0].total_tokens
-                answer.cost += callbacks[0].total_cost
-                key_filter = True if len(keys) > 0 else False
-                answer.key_filter = keys
+                keys = await self.adoc_match(
+                    answer.question, get_callbacks=get_callbacks
+                )
+                if len(keys) > 0:
+                    answer.dockey_filter = keys
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 get_callbacks=get_callbacks,
             )
-        context_str, contexts = answer.context, answer.contexts
+        if self.prompts.pre is not None:
+            chain = make_chain(self.prompts.pre, self.llm)
+            pre = await chain.arun(
+                question=answer.question, callbacks=get_callbacks("pre")
+            )
+            answer.context = pre + "\n\n" + answer.context
         bib = dict()
-        passages = dict()
-        if len(context_str) < 10:
+        if len(answer.context) < 10:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
-            cb = OpenAICallbackHandler()
-            callbacks = [cb] + get_callbacks("answer")
-            qa_chain = make_chain(qa_prompt, self.llm)
+            callbacks = get_callbacks("answer")
+            qa_chain = make_chain(self.prompts.qa, self.llm)
+            print(self.prompts.qa)
             answer_text = await qa_chain.arun(
-                question=query,
-                context_str=context_str,
-                length=length_prompt,
+                context=answer.context,
+                answer_length=answer.answer_length,
+                question=answer.question,
                 callbacks=callbacks,
             )
-            answer.tokens += cb.total_tokens
-            answer.cost += cb.total_cost
-        # it still happens lol
+        # it still happens
         if "(Example2012)" in answer_text:
             answer_text = answer_text.replace("(Example2012)", "")
-        for c in contexts:
-            key = c.key
-            text = c.context
-            citation = c.citation
+        for c in answer.contexts:
+            name = c.text.name
+            citation = c.text.doc.citation
             # do check for whole key (so we don't catch Callahan2019a with Callahan2019)
-            skey = key.split(" ")[0]
-            if skey + " " in answer_text or skey + ")" or skey + "," in answer_text:
-                bib[skey] = citation
-                passages[key] = text
+            if name_in_text(name, answer_text):
+                bib[name] = citation
         bib_str = "\n\n".join(
             [f"{i+1}. ({k}): {c}" for i, (k, c) in enumerate(bib.items())]
         )
         formatted_answer = f"Question: {query}\n\n{answer_text}\n"
         if len(bib) > 0:
             formatted_answer += f"\nReferences\n\n{bib_str}\n"
-        formatted_answer += f"\nTokens Used: {answer.tokens} Cost: ${answer.cost:.2f}"
         answer.answer = answer_text
         answer.formatted_answer = formatted_answer
         answer.references = bib_str
-        answer.passages = passages
+
+        if self.prompts.post is not None:
+            chain = make_chain(self.prompts.post, self.llm)
+            post = await chain.arun(**answer.dict(), callbacks=get_callbacks("post"))
+            answer.answer = post
+            answer.formatted_answer = f"Question: {query}\n\n{post}\n"
+            if len(bib) > 0:
+                answer.formatted_answer += f"\nReferences\n\n{bib_str}\n"
+
         return answer
```

### Comparing `paper-qa-2.1.1/setup.py` & `paper-qa-3.0.0.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from setuptools import setup
 
+# for typing
+__version__ = ""
 exec(open("paperqa/version.py").read())
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="paper-qa",
@@ -12,21 +14,20 @@
     author="Andrew White",
     author_email="white.d.andrew@gmail.com",
     url="https://github.com/whitead/paper-qa",
     license="MIT",
     packages=["paperqa", "paperqa.contrib"],
     install_requires=[
         "pypdf",
-        "langchain>=0.0.172",
-        "openai>=0.27.0",
+        "langchain>=0.0.195",
+        "openai >= 0.27.8",
         "faiss-cpu",
         "PyCryptodome",
         "html2text",
         "tiktoken",
-        "rmrkl>=0.0.2",
     ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

