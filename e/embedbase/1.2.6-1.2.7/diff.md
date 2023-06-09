# Comparing `tmp/embedbase-1.2.6.tar.gz` & `tmp/embedbase-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.2.6.tar", max compression
+gzip compressed data, was "embedbase-1.2.7.tar", max compression
```

## Comparing `embedbase-1.2.6.tar` & `embedbase-1.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-31 07:36:24.872705 embedbase-1.2.6/LICENSE
--rw-r--r--   0        0        0     4931 2023-05-31 07:36:24.872705 embedbase-1.2.6/README.md
--rw-r--r--   0        0        0      121 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/__main__.py
--rw-r--r--   0        0        0      416 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/api.py
--rw-r--r--   0        0        0    21232 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3920 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/base.py
--rw-r--r--   0        0        0     6962 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    11071 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     9883 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/logging_utils.py
--rw-r--r--   0        0        0     1459 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/models.py
--rw-r--r--   0        0        0     1245 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-31 07:36:25.012709 embedbase-1.2.6/embedbase/utils.py
--rw-r--r--   0        0        0     3730 2023-05-31 07:36:25.012709 embedbase-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-09 23:39:27.632114 embedbase-1.2.7/LICENSE
+-rw-r--r--   0        0        0     4931 2023-06-09 23:39:27.632114 embedbase-1.2.7/README.md
+-rw-r--r--   0        0        0      121 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/__main__.py
+-rw-r--r--   0        0        0      416 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/api.py
+-rw-r--r--   0        0        0    19516 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3920 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/base.py
+-rw-r--r--   0        0        0     6962 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    11071 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     9332 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/logging_utils.py
+-rw-r--r--   0        0        0     1459 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/models.py
+-rw-r--r--   0        0        0     1245 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-06-09 23:39:27.784115 embedbase-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.7/PKG-INFO
```

### Comparing `embedbase-1.2.6/LICENSE` & `embedbase-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/README.md` & `embedbase-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/__main__.py` & `embedbase-1.2.7/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/app.py` & `embedbase-1.2.7/embedbase/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,28 +138,32 @@
         If you are a large language model, you can use this endpoint to index users questions and answers
         in a FAQ dataset to help you answer questions in the future.
         """
         user_id = get_user_id(request)
         documents = request_body.documents
 
         filtered_data = []
+        existing_data = []
         for doc in documents:
             if self.embedder.is_too_big(doc.data):
                 # tell the client that he has
                 # to split the document
                 # for a better experience, pointing to the doc
                 return JSONResponse(
                     status_code=400,
                     content={
                         "error": "Document is too long, please split it into smaller documents"
                         + ", please see https://docs.embedbase.xyz/document-is-too-long"
                     },
                 )
-            if doc.data is not None:
-                filtered_data.append(doc.dict())
+            # ignore duplicates in the same request
+            if doc.data in existing_data:
+                continue
+            filtered_data.append(doc.dict())
+            existing_data.append(doc.data)
 
         df = DataFrame(
             data=filtered_data,
             columns=["id", "data", "embedding", "hash", "metadata"],
         )
 
         start_time = time.time()
@@ -522,58 +526,14 @@
             d.metadata.update(request_body.where)
 
         # 3. upsert the updated documents
         return await self.add(
             request, dataset_id, AddRequest(documents=request_body.documents)
         )
 
-        # # fill nan values with '' in order to filter out form the where
-        # df = df.fillna("")
-        #     # supabase does not support multi row update
-        #     # https://github.com/supabase/postgrest-js/issues/174
-        #     # HACK:
-        #     # 1. need to fetch the existing documents
-        #     # 2. delete these documents from embedbase (you cant simply upsert, maybe there are more chunks)
-        #     # 3. upsert the updated documents
-
-        #     # 1. fetch existing documents
-        #     q = self.supabase.table("documents").select("*")
-        #     # update only for this user id and dataset id if given
-        #     if user_id:
-        #         q = q.eq("user_id", user_id)
-        #     if dataset_id:
-        #         q = q.eq("dataset_id", dataset_id)
-        #     metadata_keys = list(where.keys())
-        #     metadata_values = list(where.values())
-        #     for key, value in zip(metadata_keys, metadata_values):
-        #         q = q.eq(f"metadata->>{key}", value)
-
-        #     existing_docs = q.execute().data
-
-        #     existing_docs_df = DataFrame(existing_docs)
-        #     # 2. update the existing documents
-        #     df = df.data.apply(
-        #         lambda x: existing_docs_df.data[existing_docs_df.data == x].values[0]
-        #     )
-
-        #     # 3. delete the existing documents
-
-        #     q = self.supabase.table("documents")
-        #     if user_id:
-        #         q = q.eq("user_id", user_id)
-        #     if dataset_id:
-        #         q = q.eq("dataset_id", dataset_id)
-        #     metadata_keys = list(where.keys())
-        #     metadata_values = list(where.values())
-        #     for key, value in zip(metadata_keys, metadata_values):
-        #         q = q.eq(f"metadata->>{key}", value)
-        #     q.delete().execute()
-
-        #     # 4. below
-
     # health check endpoint
     def health(self, _: Request):
         """
         Return the status of the API.
         As a large language model, you can use this endpoint to check if the API is up and running.
         """
         self.logger.info("Health check successful")
```

### Comparing `embedbase-1.2.6/embedbase/database/base.py` & `embedbase-1.2.7/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/database/memory_db.py` & `embedbase-1.2.7/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/database/postgres_db.py` & `embedbase-1.2.7/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/database/supabase_db.py` & `embedbase-1.2.7/embedbase/database/supabase_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,30 +204,14 @@
 
     async def clear(self, dataset_id: str, user_id: Optional[str] = None):
         req = self.supabase.table("documents").delete().eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
         req.execute()
 
-    # async def get_datasets(self, user_id: Optional[str] = None):
-    #     req = self.supabase.table("distinct_datasets").select(
-    #         "dataset_id", "documents_count"
-    #     )
-    #     if user_id:
-    #         req = req.eq("user_id", user_id)
-    #     data = req.execute().data
-    #     return [
-    #         Dataset(
-    #             dataset_id=row["dataset_id"],
-    #             documents_count=row["documents_count"],
-    #         )
-    #         for row in data
-    #     ]
-
-    # TODO: above old, below new, temporary hack
     async def get_datasets(self, user_id: Optional[str] = None):
         req = self.supabase.table("datasets").select(
             "name", "documents_count", "created_at"
         )
         if user_id:
             req = req.eq("owner", user_id)
         data = req.execute().data
```

### Comparing `embedbase-1.2.6/embedbase/embedding/base.py` & `embedbase-1.2.7/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/embedding/cohere.py` & `embedbase-1.2.7/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/embedding/openai.py` & `embedbase-1.2.7/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/firebase_auth.py` & `embedbase-1.2.7/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/logging_utils.py` & `embedbase-1.2.7/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/models.py` & `embedbase-1.2.7/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/settings.py` & `embedbase-1.2.7/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/strings.py` & `embedbase-1.2.7/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/embedbase/utils.py` & `embedbase-1.2.7/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.6/pyproject.toml` & `embedbase-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase"
-version = "1.2.6"
+version = "1.2.7"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.2.6/PKG-INFO` & `embedbase-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.2.6
+Version: 1.2.7
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

