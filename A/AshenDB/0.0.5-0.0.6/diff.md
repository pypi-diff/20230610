# Comparing `tmp/AshenDB-0.0.5.tar.gz` & `tmp/AshenDB-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshenDB-0.0.5.tar", last modified: Wed May  3 10:06:17 2023, max compression
+gzip compressed data, was "AshenDB-0.0.6.tar", last modified: Sat Jun 10 01:26:46 2023, max compression
```

## Comparing `AshenDB-0.0.5.tar` & `AshenDB-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 10:06:17.056774 AshenDB-0.0.5/
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 10:06:17.055774 AshenDB-0.0.5/AshenDB.egg-info/
--rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/SOURCES.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/dependency_links.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/entry_points.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/requires.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/top_level.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.5/LICENSE
--rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-05-03 10:06:17.056774 AshenDB-0.0.5/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2080 2023-05-03 08:58:55.000000 AshenDB-0.0.5/README.rst
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 10:06:17.056774 AshenDB-0.0.5/ashendb/
--rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-04-26 01:59:48.000000 AshenDB-0.0.5/ashendb/__init__.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     6886 2023-04-29 23:18:14.000000 AshenDB-0.0.5/ashendb/client.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     9216 2023-05-03 01:37:15.000000 AshenDB-0.0.5/ashendb/collection.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     7751 2023-04-29 23:18:41.000000 AshenDB-0.0.5/ashendb/database.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1257 2023-05-03 00:01:33.000000 AshenDB-0.0.5/ashendb/document.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.5/ashendb/exception.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)    10256 2023-05-03 10:05:21.000000 AshenDB-0.0.5/ashendb/helper.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-05-03 10:02:22.000000 AshenDB-0.0.5/pyproject.toml
--rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-05-03 10:06:17.056774 AshenDB-0.0.5/setup.cfg
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-06-10 01:26:46.893619 AshenDB-0.0.6/
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-06-10 01:26:46.892619 AshenDB-0.0.6/AshenDB.egg-info/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/SOURCES.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/dependency_links.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/entry_points.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/requires.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/top_level.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.6/LICENSE
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-06-10 01:26:46.893619 AshenDB-0.0.6/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     2080 2023-05-04 20:45:32.000000 AshenDB-0.0.6/README.rst
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-06-10 01:26:46.893619 AshenDB-0.0.6/ashendb/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-05-04 20:43:34.000000 AshenDB-0.0.6/ashendb/__init__.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     6934 2023-05-06 10:06:48.000000 AshenDB-0.0.6/ashendb/client.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)    11191 2023-05-27 22:40:56.000000 AshenDB-0.0.6/ashendb/collection.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7746 2023-05-04 20:46:23.000000 AshenDB-0.0.6/ashendb/database.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1257 2023-05-03 00:01:33.000000 AshenDB-0.0.6/ashendb/document.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.6/ashendb/exception.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)    10541 2023-06-10 01:06:02.000000 AshenDB-0.0.6/ashendb/helper.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-06-10 01:22:41.000000 AshenDB-0.0.6/pyproject.toml
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-06-10 01:26:46.893619 AshenDB-0.0.6/setup.cfg
```

### Comparing `AshenDB-0.0.5/AshenDB.egg-info/PKG-INFO` & `AshenDB-0.0.6/AshenDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.5
+Version: 0.0.6
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.5/LICENSE` & `AshenDB-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.5/PKG-INFO` & `AshenDB-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.5
+Version: 0.0.6
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.5/README.rst` & `AshenDB-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.5/ashendb/__init__.py` & `AshenDB-0.0.6/ashendb/__init__.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.5/ashendb/client.py` & `AshenDB-0.0.6/ashendb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import aiofiles
 import aiofiles.os as aios
 from typing import Generator
 
 from .database import Database
 from .exception import *
 
 
 # Client Class
-class AshenDB(str):
+class AshenDB:
     """
     Entry point for AshenDB. This class is used to create, get, and delete databases.
 
     """
 
     base: str = ".ashendb/"
 
@@ -26,14 +25,15 @@
             NotFound: If the database does not exist.
 
         Example:
             >>> db = await AshenDB.get_db("test")
             >>> db
             <Database: test>
         """
+        db_name = str(db_name)
         for name in await aios.listdir(cls.base):
             if name == db_name:
                 return Database(cls.base + name + "/")
         raise NotFound(f"Database '{db_name}' does not exist.")
 
     @classmethod
     async def get_dbs(cls, db_names: list[str] = None) -> list[Database]:
@@ -96,28 +96,29 @@
         elif isinstance(db_names, list) and len(db_names) > 0:
             for name in db_names:
                 yield await cls.get_db(name)
         else:
             raise InvalidArgumentType(f"Expected list, got {type(db_names)}.")
 
     @classmethod
-    async def create_db(cls, db_name: str) -> Database:
+    async def create_db(cls, db_name: str or int) -> Database:
         """Creates a single database.
 
         Args:
             db_name: The name of the database.
 
         Raises:
             AlreadyExists: If the database already exists.
 
         Example:
             >>> db = await AshenDB.create_db("test")
             >>> db
             <Database: test>
         """
+        db_name = str(db_name)
         path = cls.base + db_name
         if await aios.path.exists(path):
             raise AlreadyExists(f"Database '{db_name}' already exists.")
         else:
             await aios.mkdir(path)
             return Database(path + "/")
```

### Comparing `AshenDB-0.0.5/ashendb/collection.py` & `AshenDB-0.0.6/ashendb/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import aiofiles, json
+import aiofiles, json, urllib, httpx, subprocess
 import aiofiles.os as aios
 from typing import Generator
 from uuid import uuid4
 
 from .helper import match_data, update_data
 from .document import Document
 from .exception import *
@@ -17,14 +17,49 @@
     return str(uuid4())
 
 
 class Collection:
     def __init__(self, path):
         self.path = path
 
+    async def w3m(self) -> None:
+        """Show the collection in w3m.
+
+        Note:
+            Your system must have w3m installed.
+        """
+
+        json_data = []
+        for file in await aios.scandir(self.path):
+            async with aiofiles.open(file.path, "r") as f:
+                json_data.append(json.loads(await f.read()))
+
+        safe_data = urllib.parse.quote(str(json_data).replace("'", '"'))
+        safe_data = safe_data.replace("%20", "+")
+        data = "jsonData=" + safe_data
+
+        async with httpx.AsyncClient() as client:
+            response = await client.post(
+                url="https://tools.atatus.com/tools/json-to-html",
+                data=data,
+                headers={
+                    "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8"
+                },
+            )
+            response.raise_for_status()
+
+        subprocess.run(
+            ["w3m", "-dump", "-T", "text/html", "-cols", "1000"],
+            input=response.text.replace(
+                "<table>", '<table  border="1" cellpadding="10">'
+            ),
+            encoding="utf-8",
+        )
+        return None
+
     async def get_doc(self, *, id: str or int = None, query: dict = None) -> Document:
         """Get a single document.
 
         You can pass either an id or a query. If both are passed then the id will be used.
 
         Args:
             id: The id of the document.
@@ -39,14 +74,15 @@
             >>> doc
             <Document: 1>
 
             >>> doc = await coll.get_doc(query={"name": "test"})
             >>> print(doc)
             {"name": "test"}
         """
+        id = str(id)
         try:
             # check if the "{self.path}/{id}.json" file exists
             path = f"{self.path}/{id}.json"
             if not await aios.path.exists(path):
                 raise NotFound("No document found")
             doc = Document(path)
             await doc.__ainit__()
@@ -104,15 +140,15 @@
             if len(final) == 0 or len(final[0]) == 0:
                 raise NotFound("No documents found")
             return final
         else:
             raise ValueError("Either ids or query must be provided")
 
     async def iterate_docs(
-        self, ids: list[str or int], query: dict = None
+        self, *, ids: list[str or int] = None, query: dict = None
     ) -> Generator[Document, None, None]:
         """Iterate over multiple documents.
 
         You can pass either a list of ids or a query. If both are passed then the ids will be used.
 
         Args:
             ids: The ids of the documents.
@@ -147,15 +183,20 @@
                 async with aiofiles.open(file.path, "r") as f:
                     data = json.loads(await f.read())
                     if await match_data(data, query):
                         doc = Document(file.path)
                         await doc.__ainit__()
                         yield doc
         else:
-            raise ValueError("Either ids or query must be provided")
+            for file in await aios.scandir(self.path):
+                async with aiofiles.open(file.path, "r") as f:
+                    data = json.loads(await f.read())
+                    doc = Document(file.path)
+                    await doc.__ainit__()
+                    yield doc
 
     async def create_doc(self, data: dict) -> Document:
         """Create a document.
 
         Args:
             data: The data to be stored in the document.
 
@@ -167,23 +208,28 @@
             >>> doc
             <Document: 1>
         """
         if not isinstance(data, dict):
             raise TypeError("Data must be a dict")
 
         try:
-            id = str(data.get("_id"))
-        except:
+            id = str(data["_id"])
+        except KeyError:
             id = gen_id()
-
+            data["_id"] = id
+        # Check if already exist
+        if await aios.path.exists(f"{self.path}/{id}.json"):
+            raise AlreadyExists("Document already exist")
         async with aiofiles.open(f"{self.path}/{id}.json", "w") as f:
             await f.write(json.dumps(data))
-        return Document(f"{self.path}/{id}.json")
+        document = Document(f"{self.path}/{id}.json")
+        await document.__ainit__()
+        return document
 
-    async def create_doc(self, datas: list[dict]) -> list[Document]:
+    async def create_docs(self, datas: list[dict]) -> list[Document]:
         """Create multiple documents.
 
         Args:
             datas: The data to be stored in the documents.
 
         Raises:
             TypeError: If datas is not a list.
@@ -277,7 +323,19 @@
             >>> new_doc = await coll.get_doc(query={"name": "test2"})
             >>> new_doc
             {"name": "test2"}
         """
         doc = await self.get_doc(id=id, query=query)
         new_doc = await update_data(doc, data)
         return new_doc
+
+    async def count_docs(self) -> int:
+        """Count the number of documents in the collection.
+
+        Example:
+            >>> await coll.count_docs()
+            3
+        """
+        count = 0
+        for _ in await aios.scandir(self.path):
+            count += 1
+        return count
```

### Comparing `AshenDB-0.0.5/ashendb/database.py` & `AshenDB-0.0.6/ashendb/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Generator
 
 from .collection import Collection
 from .exception import *
 
 
 # Database Class
-class Database(str):
+class Database:
     def __init__(self, db_path: str):
         super().__init__()
         self.path = db_path
 
     async def get_coll(self, collection_name: str) -> Collection:
         """Get a single collection.
```

### Comparing `AshenDB-0.0.5/ashendb/document.py` & `AshenDB-0.0.6/ashendb/document.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.5/ashendb/helper.py` & `AshenDB-0.0.6/ashendb/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,32 +296,34 @@
             key, parent_key[key][:-1]
         )
         if value == -1
         else parent_key.__setitem__(key, parent_key[key][1:])
         if value == 1
         else parent_key,
         "$pull": lambda parent_key, key, value: parent_key.__setitem__(
-            key, [item for item in parent_key[key] if item != value]
+            key,
+            [
+                item
+                for item in parent_key[key]
+                if not (
+                    isinstance(item, dict)
+                    and all(k in item and item[k] == v for k, v in value.items())
+                )
+            ],
         )
         if isinstance(value, dict)
         else parent_key.__setitem__(
-            key, [item for item in parent_key[key] if item not in value]
-        )
-        if isinstance(value, list)
-        else parent_key.__setitem__(
-            key, [item for item in parent_key[key] if item != value]
-        )
-        if isinstance(value, str)
-        else parent_key,
-        "$push": lambda parent_key, key, value: parent_key.__setitem__(
             key,
-            parent_key.get(key, []) + value,
+            [item for item in parent_key[key] if item not in value],
+        ),
+        "$push": lambda parent_key, key, value: parent_key.__setitem__(
+            key, parent_key[key].extend(value)
         )
-        if parent_key.get(key)
-        else parent_key,
+        if key in parent_key and hasattr(value, "__iter__")
+        else parent_key.__setitem__(key, value if isinstance(value, list) else [value]),
         "$pullAll": lambda parent_key, key, value: parent_key.__setitem__(
             key, [item for item in parent_key[key] if item not in value]
         )
         if isinstance(value, list)
         else parent_key,
     }
 
@@ -336,17 +338,22 @@
         **field_operators,
         **array_operators,
         **modification_operators,
     }
 
     for operator, data in update.items():
         for key, value in data.items():
-            keys = key.split(".")
             temp = document
+            keys = key.split(".")
             for key in keys[:-1]:
-                temp = temp.setdefault(key, {})
+                if "[" in key:
+                    key, index = key.split("[")
+                    index = int(index[:-1])
+                    temp = temp[key][index]
+                else:
+                    temp = temp.setdefault(key, {})
 
             if operator in update_operators:
                 update_operators[operator](temp, keys[-1], value)
 
     await document.save()
     return document
```

### Comparing `AshenDB-0.0.5/pyproject.toml` & `AshenDB-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AshenDB"
-version = "0.0.5"
+version = "0.0.6"
 description = "Another stupid library for using json as Database"
 readme = "README.rst"
 authors = [{name = "Abdullah Al Muaz", email = "abdullahalmuaz15@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: MIT License",
```

