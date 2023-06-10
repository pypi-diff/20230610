# Comparing `tmp/vector_vault-2.0.6.tar.gz` & `tmp/vector_vault-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.6.tar", last modified: Fri Jun  9 23:05:34 2023, max compression
+gzip compressed data, was "vector_vault-2.0.7.tar", last modified: Sat Jun 10 04:18:06 2023, max compression
```

## Comparing `vector_vault-2.0.6.tar` & `vector_vault-2.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 23:05:34.887707 vector_vault-2.0.6/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.6/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20846 2023-06-09 23:05:34.887574 vector_vault-2.0.6/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20121 2023-06-09 23:05:24.000000 vector_vault-2.0.6/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-09 23:05:34.887744 vector_vault-2.0.6/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-09 23:05:32.000000 vector_vault-2.0.6/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 23:05:34.884055 vector_vault-2.0.6/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20846 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-09 23:05:34.000000 vector_vault-2.0.6/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 23:05:34.887255 vector_vault-2.0.6/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.0.6/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.6/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1954 2023-06-09 19:11:10.000000 vector_vault-2.0.6/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.6/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.6/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.6/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2398 2023-06-08 04:57:38.000000 vector_vault-2.0.6/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.6/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    30807 2023-06-09 19:58:53.000000 vector_vault-2.0.6/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.6/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.6/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-10 04:18:06.337669 vector_vault-2.0.7/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.7/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    19254 2023-06-10 04:18:06.337479 vector_vault-2.0.7/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    18529 2023-06-10 00:06:46.000000 vector_vault-2.0.7/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-10 04:18:06.337707 vector_vault-2.0.7/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-10 04:17:45.000000 vector_vault-2.0.7/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-10 04:18:06.333311 vector_vault-2.0.7/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    19254 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-10 04:18:06.337080 vector_vault-2.0.7/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.0.7/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.7/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1954 2023-06-09 19:11:10.000000 vector_vault-2.0.7/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.7/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.7/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.7/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2398 2023-06-08 04:57:38.000000 vector_vault-2.0.7/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.7/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    30807 2023-06-09 19:58:53.000000 vector_vault-2.0.7/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.7/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.7/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.6/LICENSE` & `vector_vault-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/PKG-INFO` & `vector_vault-2.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: vector_vault
-Version: 2.0.6
-Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
-Home-page: https://github.com/John-Rood/VectorVault
-Author: VectorVault.io
-Author-email: john@johnrood.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud with under one second response times.
 
 The `vectorvault` package comes with extensive chat functionality, so that you don't have to think about the details and can make smooth chat applications with ease. Speaking of smooth chat experiences, `vectorvault` also comes with chat streaming built-in. Simply use the `get_chat_stream()` function that works just like the regular `get_chat()` but with streaming. 
 
 `langchain` is a popular package for building functionality with llms, but when it comes to referencing vector databases, the database retrieval and chat integration can be complicated and difficult. This is one of the reasons we built `vectorvault`. We've integrated all the chat options people like to use with `langchain`, but made them all easier and more straight forward to use. Now with Vector Vault, integrating vector database results into generative chat applications is not only easy, it's the default. You also have total control over every aspect with parameters. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you.
@@ -62,37 +43,37 @@
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
 ### Get Your Vector Vault API Key:
-```
+```python
 from vectorvault import register
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
 ```
 The api key will be sent to your email.
 
 <br>
 
 # Build The Vault:
 
 Set your openai key as an envorionment variable
-```
+```python
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
 4. Get vectors embeddings 
 5. Save to the cloud vault
 
-```
+```python
 from vectorvault import Vault
 
 vault = Vault(user='your@email.com', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
@@ -102,15 +83,15 @@
 vault.save()
 ```
 
 <br>
 <br>
 
 Now that you have saved some data to the vault, you can add more at anytime. `vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed. `vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
-```
+```python
 vault.add(very_large_text)
 vault.get_vectors() 
 vault.save() 
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
@@ -133,50 +114,50 @@
         "vault": "your_vault_name",
         "text": "Your text input"
      }'
 ```
 >> {"results":[{"data":"NASA Mars Exploration... **shortend for brevity**","metadata":{"created_at":"2023-05-29T19:21:20.846023","item_id":0,"name":"webdump-0","updated_at":"2023-05-29T19:21:20.846028"}}]}
     
 This is the same exact call, but in Python:
-```
+```python
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
 ```
 >> NASA Mars Exploration... NASA To Host Briefing... Program studies Mars... A Look at a Steep North Polar...
 
 ^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
 `similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of 4.
 
 <br>
 
 Print the metadata:
-```
+```python
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 >> NASA Mars Exploration... {"created_at":"2023-05-29T19...} NASA To Host Briefing... {"created_at":"2023-05-29T19...} Program studies Mars... {"created_at":"2023-05-29T19...} A Look at a Steep North Polar... {"created_at":"2023-05-29T19...}
 
 <br>
 <br>
 
 ### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
 Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
-```
+```python
 question = "Should I use Vector Vault for my next generative ai application"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
-```
+```python
 answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
@@ -208,15 +189,15 @@
 `response = vault.get_chat(text, chat_history, get_context=True)`
 
 - Example Context-Response with Context Samples Returned:
 `vault_response = vault.get_chat(text, get_context=True, return_context=True)`
 <br>
 
 Response from ChatGPT in string format, unless `return_context=True` is passed, then response will be a dictionary containing the results - response from ChatGPT, and the vault data.
-```
+```python
 # print response:
 print(vault_response['response'])
 
 # print context:
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
@@ -227,21 +208,21 @@
 
 # Summarize Anything:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
 </p>
 
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
-```
+```python
 summary = vault.get_chat(text, summary=True)
 ```
 <br>
 
 want to make a summary of a certain length?...
-```
+```python
 summary = vault.get_chat(text, summary=True)
 
 while len(summary) > 1000:
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
@@ -249,66 +230,42 @@
 <br>
 <br>
 
 # Streaming:
 Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-![Alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/559fd0ea-8fa7-40a2-9260-c5b0f4b063b5/Streaming+Demo+Offish.gif)
+![Alt text](https://github.com/John-Rood/VectorVault/blob/778c11dfc8b71675d704c5f559c3452dc65b910a/digital%20assets/Streaming%20Demo%20Offish.gif)
 
 ## get_chat_stream():
+See it in action. Check our [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) that has Colab notebooks you can be running in the browser seconds from now.
 
-Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
-Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
-`cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
-`print_stream()` is for local console printing.
-
-Example Signle Usage: 
-`response = vault.print_stream(vault.get_chat_stream(text))`
-
-Example Chat: 
-`response = vault.print_stream(vault.get_chat_stream(text, chat_history))`
 
-Example Summary: 
-`summary = vault.print_stream(vault.get_chat_stream(text, summary=True))`
+`get_chat()` function returns the whole message at once. `get_chat_stream` yields each word as it it received.
 
-Example Context-Based Response:
-`response = vault.print_stream(vault.get_chat_stream(text, get_context = True))`
-
-Example Context-Based Response w/ Chat History:
-`response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True))`
-
-Example Context-Response with Context Samples Returned:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True))`
-
-Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
-
-Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
-
-Response is a always a stream
-`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message to show their difference:
-
-```
+```python
 ## get_chat()
 print(vault.get_chat(text, history))
 
 ## get_chat_stream()
 for word in vault.get_chat_stream(text, history):
         print(word)
 ```
-This will take each word yielded and print it as it comes in. However, it's best to use the built in print function `print_stream`. 
-```
+
+```python
+# But it's best to use the built in print function print_stream() function
 vault.print_stream(vault.get_chat_stream(text, history))
 ```
 <br>
 
-Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
-This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
+Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: 
+```python
+return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')
+```
+This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq). Check out our [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) that has notebooks you can run in the browser with Google Colab.
 
 
 <br>
 <br> 
 
 
 
@@ -323,15 +280,15 @@
 <br>
 
 In the following code, we will add all of a company's past support conversations to a cloud Vault. (We load the company support texts from a .txt file, vectorize them, then add them to the Vault). As new people message in, we will vector search the Vault for similar questions and answers. We take the past answers returned from the Vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
-```
+```python
 from vectorvault import Vault
 
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
 
 with open('customer_service.txt', 'r') as f:
@@ -342,15 +299,15 @@
 vault.save()
 ```
 
 <br>
 
 And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
-```
+```python
 question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 <br>
 
 That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
@@ -395,9 +352,7 @@
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets.
 
 <br>
 
 ### What if I'm a large company with very large data
 If you need to store more than 1 gig of data in single vaults for any reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need. It is always active and scalable to terabytes. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up ~8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
 
-
-
```

### Comparing `vector_vault-2.0.6/README.md` & `vector_vault-2.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: vector_vault
+Version: 2.0.7
+Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
+Home-page: https://github.com/John-Rood/VectorVault
+Author: VectorVault.io
+Author-email: john@johnrood.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud with under one second response times.
 
 The `vectorvault` package comes with extensive chat functionality, so that you don't have to think about the details and can make smooth chat applications with ease. Speaking of smooth chat experiences, `vectorvault` also comes with chat streaming built-in. Simply use the `get_chat_stream()` function that works just like the regular `get_chat()` but with streaming. 
 
 `langchain` is a popular package for building functionality with llms, but when it comes to referencing vector databases, the database retrieval and chat integration can be complicated and difficult. This is one of the reasons we built `vectorvault`. We've integrated all the chat options people like to use with `langchain`, but made them all easier and more straight forward to use. Now with Vector Vault, integrating vector database results into generative chat applications is not only easy, it's the default. You also have total control over every aspect with parameters. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you.
@@ -43,37 +62,37 @@
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
 ### Get Your Vector Vault API Key:
-```
+```python
 from vectorvault import register
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
 ```
 The api key will be sent to your email.
 
 <br>
 
 # Build The Vault:
 
 Set your openai key as an envorionment variable
-```
+```python
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
 4. Get vectors embeddings 
 5. Save to the cloud vault
 
-```
+```python
 from vectorvault import Vault
 
 vault = Vault(user='your@email.com', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
@@ -83,15 +102,15 @@
 vault.save()
 ```
 
 <br>
 <br>
 
 Now that you have saved some data to the vault, you can add more at anytime. `vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed. `vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
-```
+```python
 vault.add(very_large_text)
 vault.get_vectors() 
 vault.save() 
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
@@ -114,50 +133,50 @@
         "vault": "your_vault_name",
         "text": "Your text input"
      }'
 ```
 >> {"results":[{"data":"NASA Mars Exploration... **shortend for brevity**","metadata":{"created_at":"2023-05-29T19:21:20.846023","item_id":0,"name":"webdump-0","updated_at":"2023-05-29T19:21:20.846028"}}]}
     
 This is the same exact call, but in Python:
-```
+```python
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
 ```
 >> NASA Mars Exploration... NASA To Host Briefing... Program studies Mars... A Look at a Steep North Polar...
 
 ^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
 `similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of 4.
 
 <br>
 
 Print the metadata:
-```
+```python
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 >> NASA Mars Exploration... {"created_at":"2023-05-29T19...} NASA To Host Briefing... {"created_at":"2023-05-29T19...} Program studies Mars... {"created_at":"2023-05-29T19...} A Look at a Steep North Polar... {"created_at":"2023-05-29T19...}
 
 <br>
 <br>
 
 ### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
 Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
-```
+```python
 question = "Should I use Vector Vault for my next generative ai application"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
-```
+```python
 answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
@@ -189,15 +208,15 @@
 `response = vault.get_chat(text, chat_history, get_context=True)`
 
 - Example Context-Response with Context Samples Returned:
 `vault_response = vault.get_chat(text, get_context=True, return_context=True)`
 <br>
 
 Response from ChatGPT in string format, unless `return_context=True` is passed, then response will be a dictionary containing the results - response from ChatGPT, and the vault data.
-```
+```python
 # print response:
 print(vault_response['response'])
 
 # print context:
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
@@ -208,21 +227,21 @@
 
 # Summarize Anything:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
 </p>
 
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
-```
+```python
 summary = vault.get_chat(text, summary=True)
 ```
 <br>
 
 want to make a summary of a certain length?...
-```
+```python
 summary = vault.get_chat(text, summary=True)
 
 while len(summary) > 1000:
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
@@ -230,66 +249,42 @@
 <br>
 <br>
 
 # Streaming:
 Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-![Alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/559fd0ea-8fa7-40a2-9260-c5b0f4b063b5/Streaming+Demo+Offish.gif)
+![Alt text](https://github.com/John-Rood/VectorVault/blob/778c11dfc8b71675d704c5f559c3452dc65b910a/digital%20assets/Streaming%20Demo%20Offish.gif)
 
 ## get_chat_stream():
+See it in action. Check our [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) that has Colab notebooks you can be running in the browser seconds from now.
 
-Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
-Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
-`cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
-`print_stream()` is for local console printing.
-
-Example Signle Usage: 
-`response = vault.print_stream(vault.get_chat_stream(text))`
-
-Example Chat: 
-`response = vault.print_stream(vault.get_chat_stream(text, chat_history))`
 
-Example Summary: 
-`summary = vault.print_stream(vault.get_chat_stream(text, summary=True))`
+`get_chat()` function returns the whole message at once. `get_chat_stream` yields each word as it it received.
 
-Example Context-Based Response:
-`response = vault.print_stream(vault.get_chat_stream(text, get_context = True))`
-
-Example Context-Based Response w/ Chat History:
-`response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True))`
-
-Example Context-Response with Context Samples Returned:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True))`
-
-Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
-
-Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
-
-Response is a always a stream
-`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message to show their difference:
-
-```
+```python
 ## get_chat()
 print(vault.get_chat(text, history))
 
 ## get_chat_stream()
 for word in vault.get_chat_stream(text, history):
         print(word)
 ```
-This will take each word yielded and print it as it comes in. However, it's best to use the built in print function `print_stream`. 
-```
+
+```python
+# But it's best to use the built in print function print_stream() function
 vault.print_stream(vault.get_chat_stream(text, history))
 ```
 <br>
 
-Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
-This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
+Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: 
+```python
+return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')
+```
+This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq). Check out our [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) that has notebooks you can run in the browser with Google Colab.
 
 
 <br>
 <br> 
 
 
 
@@ -304,15 +299,15 @@
 <br>
 
 In the following code, we will add all of a company's past support conversations to a cloud Vault. (We load the company support texts from a .txt file, vectorize them, then add them to the Vault). As new people message in, we will vector search the Vault for similar questions and answers. We take the past answers returned from the Vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
-```
+```python
 from vectorvault import Vault
 
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
 
 with open('customer_service.txt', 'r') as f:
@@ -323,15 +318,15 @@
 vault.save()
 ```
 
 <br>
 
 And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
-```
+```python
 question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 <br>
 
 That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
@@ -376,7 +371,9 @@
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets.
 
 <br>
 
 ### What if I'm a large company with very large data
 If you need to store more than 1 gig of data in single vaults for any reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need. It is always active and scalable to terabytes. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up ~8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
 
+
+
```

### Comparing `vector_vault-2.0.6/setup.py` & `vector_vault-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.6",
+    version="2.0.7",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.6/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.7/vector_vault.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.0.6
+Version: 2.0.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -62,37 +62,37 @@
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
 ### Get Your Vector Vault API Key:
-```
+```python
 from vectorvault import register
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
 ```
 The api key will be sent to your email.
 
 <br>
 
 # Build The Vault:
 
 Set your openai key as an envorionment variable
-```
+```python
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
 4. Get vectors embeddings 
 5. Save to the cloud vault
 
-```
+```python
 from vectorvault import Vault
 
 vault = Vault(user='your@email.com', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
@@ -102,15 +102,15 @@
 vault.save()
 ```
 
 <br>
 <br>
 
 Now that you have saved some data to the vault, you can add more at anytime. `vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed. `vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
-```
+```python
 vault.add(very_large_text)
 vault.get_vectors() 
 vault.save() 
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
@@ -133,50 +133,50 @@
         "vault": "your_vault_name",
         "text": "Your text input"
      }'
 ```
 >> {"results":[{"data":"NASA Mars Exploration... **shortend for brevity**","metadata":{"created_at":"2023-05-29T19:21:20.846023","item_id":0,"name":"webdump-0","updated_at":"2023-05-29T19:21:20.846028"}}]}
     
 This is the same exact call, but in Python:
-```
+```python
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
 ```
 >> NASA Mars Exploration... NASA To Host Briefing... Program studies Mars... A Look at a Steep North Polar...
 
 ^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
 `similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of 4.
 
 <br>
 
 Print the metadata:
-```
+```python
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 >> NASA Mars Exploration... {"created_at":"2023-05-29T19...} NASA To Host Briefing... {"created_at":"2023-05-29T19...} Program studies Mars... {"created_at":"2023-05-29T19...} A Look at a Steep North Polar... {"created_at":"2023-05-29T19...}
 
 <br>
 <br>
 
 ### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
 Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
-```
+```python
 question = "Should I use Vector Vault for my next generative ai application"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
-```
+```python
 answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
@@ -208,15 +208,15 @@
 `response = vault.get_chat(text, chat_history, get_context=True)`
 
 - Example Context-Response with Context Samples Returned:
 `vault_response = vault.get_chat(text, get_context=True, return_context=True)`
 <br>
 
 Response from ChatGPT in string format, unless `return_context=True` is passed, then response will be a dictionary containing the results - response from ChatGPT, and the vault data.
-```
+```python
 # print response:
 print(vault_response['response'])
 
 # print context:
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
@@ -227,21 +227,21 @@
 
 # Summarize Anything:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
 </p>
 
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
-```
+```python
 summary = vault.get_chat(text, summary=True)
 ```
 <br>
 
 want to make a summary of a certain length?...
-```
+```python
 summary = vault.get_chat(text, summary=True)
 
 while len(summary) > 1000:
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
@@ -249,66 +249,42 @@
 <br>
 <br>
 
 # Streaming:
 Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-![Alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/559fd0ea-8fa7-40a2-9260-c5b0f4b063b5/Streaming+Demo+Offish.gif)
+![Alt text](https://github.com/John-Rood/VectorVault/blob/778c11dfc8b71675d704c5f559c3452dc65b910a/digital%20assets/Streaming%20Demo%20Offish.gif)
 
 ## get_chat_stream():
+See it in action. Check our [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) that has Colab notebooks you can be running in the browser seconds from now.
 
-Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
-Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
-`cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
-`print_stream()` is for local console printing.
-
-Example Signle Usage: 
-`response = vault.print_stream(vault.get_chat_stream(text))`
-
-Example Chat: 
-`response = vault.print_stream(vault.get_chat_stream(text, chat_history))`
 
-Example Summary: 
-`summary = vault.print_stream(vault.get_chat_stream(text, summary=True))`
+`get_chat()` function returns the whole message at once. `get_chat_stream` yields each word as it it received.
 
-Example Context-Based Response:
-`response = vault.print_stream(vault.get_chat_stream(text, get_context = True))`
-
-Example Context-Based Response w/ Chat History:
-`response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True))`
-
-Example Context-Response with Context Samples Returned:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True))`
-
-Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
-
-Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
-`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
-
-Response is a always a stream
-`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message to show their difference:
-
-```
+```python
 ## get_chat()
 print(vault.get_chat(text, history))
 
 ## get_chat_stream()
 for word in vault.get_chat_stream(text, history):
         print(word)
 ```
-This will take each word yielded and print it as it comes in. However, it's best to use the built in print function `print_stream`. 
-```
+
+```python
+# But it's best to use the built in print function print_stream() function
 vault.print_stream(vault.get_chat_stream(text, history))
 ```
 <br>
 
-Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
-This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
+Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: 
+```python
+return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')
+```
+This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq). Check out our [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) that has notebooks you can run in the browser with Google Colab.
 
 
 <br>
 <br> 
 
 
 
@@ -323,15 +299,15 @@
 <br>
 
 In the following code, we will add all of a company's past support conversations to a cloud Vault. (We load the company support texts from a .txt file, vectorize them, then add them to the Vault). As new people message in, we will vector search the Vault for similar questions and answers. We take the past answers returned from the Vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
-```
+```python
 from vectorvault import Vault
 
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
 
 with open('customer_service.txt', 'r') as f:
@@ -342,15 +318,15 @@
 vault.save()
 ```
 
 <br>
 
 And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
-```
+```python
 question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 <br>
 
 That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
```

### Comparing `vector_vault-2.0.6/vectorvault/ai.py` & `vector_vault-2.0.7/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/cloud_api.py` & `vector_vault-2.0.7/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/cloudmanager.py` & `vector_vault-2.0.7/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/creds.py` & `vector_vault-2.0.7/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/download.py` & `vector_vault-2.0.7/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/itemize.py` & `vector_vault-2.0.7/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/tools_gpt.py` & `vector_vault-2.0.7/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/vault.py` & `vector_vault-2.0.7/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.6/vectorvault/vecreq.py` & `vector_vault-2.0.7/vectorvault/vecreq.py`

 * *Files identical despite different names*

