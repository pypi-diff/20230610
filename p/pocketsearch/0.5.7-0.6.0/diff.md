# Comparing `tmp/pocketsearch-0.5.7.tar.gz` & `tmp/pocketsearch-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.5.7.tar", last modified: Fri Jun  9 19:10:10 2023, max compression
+gzip compressed data, was "pocketsearch-0.6.0.tar", last modified: Sat Jun 10 10:05:26 2023, max compression
```

## Comparing `pocketsearch-0.5.7.tar` & `pocketsearch-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:10:10.106531 pocketsearch-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 19:10:01.000000 pocketsearch-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-09 19:10:10.106531 pocketsearch-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-06-09 19:10:01.000000 pocketsearch-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:10:10.106531 pocketsearch-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 19:10:01.000000 pocketsearch-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:10:10.102531 pocketsearch-0.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:10:10.102531 pocketsearch-0.5.7/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 19:10:01.000000 pocketsearch-0.5.7/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 19:10:01.000000 pocketsearch-0.5.7/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:10:10.102531 pocketsearch-0.5.7/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-09 19:10:10.000000 pocketsearch-0.5.7/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 19:10:10.000000 pocketsearch-0.5.7/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:10:10.000000 pocketsearch-0.5.7/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 19:10:10.000000 pocketsearch-0.5.7/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.034794 pocketsearch-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-10 10:05:26.034794 pocketsearch-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 10:05:26.034794 pocketsearch-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.026794 pocketsearch-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.030794 pocketsearch-0.6.0/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20037 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.030794 pocketsearch-0.6.0/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.5.7/LICENSE` & `pocketsearch-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.7/PKG-INFO` & `pocketsearch-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.7
+Version: 0.6.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
+Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -22,25 +23,29 @@
 License-File: LICENSE
 
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
 - Support for full text search
 - A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
-- Support for text, numeric and date search
+- Support for multi-field indices including text, numeric and date search
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
+pocketsearch is currently being tested on data from Wikipedia, indexing more than 6 million abstracts. If you 
+are interested in preliminary performance tests, have a look at https://github.com/kaykay-dv/pocketsearch/tree/development/tests.
+
 # Status
 The package is currently in Beta status.
 
 ![Unit tests main](https://github.com/kaykay-dv/pocketsearch/actions/workflows/unittests-main.yml/badge.svg)
 ![Unit tests development](https://github.com/kaykay-dv/pocketsearch/actions/workflows/unittests-development.yml/badge.svg)
 
+
 # Installation
 
 Run 
 
 ```Shell
 pip install pocketsearch
 ```
@@ -221,16 +226,43 @@
 
 To delete a document, use:
 
 ```Python
 pocket_search.delete(rowid=1)
 ```
 
-Please note that by default an AND query is performed, thus only documents are
-matched where text contains the word "world" and the filename is "a.txt"
+# Using index readers to insert data
+
+Normally we have a data source at hand (e.g. files in a file system or a source database) that we use to read 
+data from. IndexReader classes can be used to build an index from such a data source. Assume, you want to 
+index text files from a directory, we first define a schema:
+
+```Python
+class FileSchema(Schema):
+
+        text = Text(index=True)
+        filename = Text(is_id_field=True) 
+```
+
+Next, we create a PocketSearch and 
+
+```Python
+from pocketsearch import FileSystemReader
+pocket_search = PocketSearch(schema=FileSchema)
+reader = FileSystemReader(base_dir="/some/directory", file_extensions=[".txt"])
+pocket_search.build(reader)
+```
+
+This will build the index. If a document has already been seen it will be updated, a new document will be 
+inserted otherwise. 
+
+Currently, the FileSystemReader is the only implementation provided, however you can easily implement your own 
+by implementing the abstract class IndexError implementing a .read method. The .read method should return an 
+iterable containing dictionaries whereas the dictionary's keys correspond to schema fields and its values 
+the data you want to insert for the document. 
 
 # Searching numeric data
 
 You can also search for numeric data:
 
 ```Python
 class Product(Schema):
```

### Comparing `pocketsearch-0.5.7/README.md` & `pocketsearch-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
 - Support for full text search
 - A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
-- Support for text, numeric and date search
+- Support for multi-field indices including text, numeric and date search
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
+pocketsearch is currently being tested on data from Wikipedia, indexing more than 6 million abstracts. If you 
+are interested in preliminary performance tests, have a look at https://github.com/kaykay-dv/pocketsearch/tree/development/tests.
+
 # Status
 The package is currently in Beta status.
 
 ![Unit tests main](https://github.com/kaykay-dv/pocketsearch/actions/workflows/unittests-main.yml/badge.svg)
 ![Unit tests development](https://github.com/kaykay-dv/pocketsearch/actions/workflows/unittests-development.yml/badge.svg)
 
+
 # Installation
 
 Run 
 
 ```Shell
 pip install pocketsearch
 ```
@@ -198,16 +202,43 @@
 
 To delete a document, use:
 
 ```Python
 pocket_search.delete(rowid=1)
 ```
 
-Please note that by default an AND query is performed, thus only documents are
-matched where text contains the word "world" and the filename is "a.txt"
+# Using index readers to insert data
+
+Normally we have a data source at hand (e.g. files in a file system or a source database) that we use to read 
+data from. IndexReader classes can be used to build an index from such a data source. Assume, you want to 
+index text files from a directory, we first define a schema:
+
+```Python
+class FileSchema(Schema):
+
+        text = Text(index=True)
+        filename = Text(is_id_field=True) 
+```
+
+Next, we create a PocketSearch and 
+
+```Python
+from pocketsearch import FileSystemReader
+pocket_search = PocketSearch(schema=FileSchema)
+reader = FileSystemReader(base_dir="/some/directory", file_extensions=[".txt"])
+pocket_search.build(reader)
+```
+
+This will build the index. If a document has already been seen it will be updated, a new document will be 
+inserted otherwise. 
+
+Currently, the FileSystemReader is the only implementation provided, however you can easily implement your own 
+by implementing the abstract class IndexError implementing a .read method. The .read method should return an 
+iterable containing dictionaries whereas the dictionary's keys correspond to schema fields and its values 
+the data you want to insert for the document. 
 
 # Searching numeric data
 
 You can also search for numeric data:
 
 ```Python
 class Product(Schema):
```

### Comparing `pocketsearch-0.5.7/setup.py` & `pocketsearch-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.5.7",
+    version = "0.6.0",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
         "Bug Tracker": "https://github.com/kaykay-dv/pocketsearch/issues",
+        "Change log" : "https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md"
     },
     classifiers = [
         "Development Status :: 4 - Beta",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `pocketsearch-0.5.7/src/pocketsearch/__init__.py` & `pocketsearch-0.6.0/src/pocketsearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,37 +19,44 @@
     '''
     A helper class that displays
     a progress bar in console.
     '''
 
     def __init__(self, precision=5):
         self.start = time.time()
+        self.stop = self.start
         self.precision = precision
         self.total_time = 0
         self.laps = []
         self.snapshots = 0
 
     def lap(self, name):
         '''
         Add a lap to the timer. A lap has a name and is automatically
         associated with the the current time.
         '''
         if len(self.laps) > 0:
             self.total_time += time.time()-self.laps[-1:][0][1]
         self.laps.append((name, time.time()))
 
+    def get_its(self):
+        '''
+        Returns current number of iterations per second
+        '''
+        return round(1/((self.stop-self.start)/self.snapshots), self.precision)
+
     def snapshot(self, more_info=""):
         '''
         Prints out the current iteration and statistics on time consumed.
         more_info maybe used on what is actually done.
         '''
-        stop = time.time()
+        self.stop = time.time()
         self.snapshots = self.snapshots+1
-        its = round(1/((stop-self.start)/self.snapshots), self.precision)
-        out = "%s iterations %s it/s %s s elapsed %s%s" % (self.snapshots, its, round(stop-self.start, self.precision), more_info, " "*15)
+        its = self.get_its()
+        out = "%s iterations %s it/s %s s elapsed %s%s" % (self.snapshots, its, round(self.stop-self.start, self.precision), more_info, " "*15)
         print(out, end="\r", flush=True)
 
     def done(self):
         '''
         Prints a newline on console.
         '''
         print()
@@ -1026,14 +1033,22 @@
         for field in self.schema:
             if field.name not in referenced_fields and not(for_search) and field.name not in ["id", "rank"]:
                 raise self.FieldError("Missing field '%s' in keyword arguments." % field.name)
             if field.name in referenced_fields:
                 arguments[field.name] = self.Argument(field, referenced_fields[field.name])
         return arguments
 
+    def build(self,index_reader):
+        '''
+        Create an index reading a document from an index_builder instance.
+        '''
+        self.assure_writeable()
+        for elem in index_reader.read():
+            self.insert_or_update(**elem)
+
     def insert_or_update(self, *args, **kwargs):
         '''
         Insert or updates a new document if it already exists.
         '''
         self.assure_writeable()
         if self.schema.id_field is None:
             raise self.DatabaseError("No IDFIeld has been defined in the schema - cannot perform insert_or_update.")
@@ -1112,15 +1127,15 @@
         '''
         Searches the index. Keyword arguments must correspond to
         '''
         arguments = self.get_arguments(kwargs)
         return Query(self, arguments)
 
 
-class Index(abc.ABC):
+class IndexReader(abc.ABC):
     '''
     An abstract base class for index readers. Reader classes
     scan through a source (e.g. the file system or some web site)
     and retrieve documents that should be indexed.
     '''
 
     def read(self):
@@ -1128,57 +1143,45 @@
         Subclasses need to implement this method.
         It should return a list of dictionaries
         where each dictionary entry represents
         a document in the schema.
         '''
         raise NotImplementedError()
 
-    def search(self, *args, **kwargs):
-        '''
-        Wrapper method around the local pocket_search
-        object instance.
-        '''
-        return self.pocket_search.search(*args, **kwargs)
-
-    def build(self):
-        '''
-        Populate the index in the given pocket_search
-        instance.
-        '''
-        for elem in self.read():
-            self.pocket_search.insert_or_update(**elem)
-
-class FileSystemIndex(Index):
+class FileSystemReader(IndexReader):
     '''
     Index files and their contents from a directory.
     The FileSystemReader expects a schema containing
     following fields:
 
     - filename (TEXT, unique=True)
     - text (TEXT, index=True)
 
     '''
 
-    class FileContents(Schema):
+    encoding = "utf-8"
 
-        text = Text(index=True)
-        filename = Text(is_id_field=True)
-
-    def __init__(self, base_dir="./", file_extensions=[".txt"]):
+    def __init__(self, base_dir="./", file_extensions=None,**kwargs):
+        if file_extensions is None:
+            self.file_extensions = [".txt"]
+        else:
+            self.file_extensions = file_extensions
         self.base_dir = base_dir
-        self.file_extensions = file_extensions
-        self.pocket_search = PocketSearch(schema=self.FileContents, writeable=True)
 
     def file_to_dict(self, file_path, file):
         '''
         Open the file and transform it to a dictionary.
         '''
         return {"filename": file_path, "text": file.read()}
 
     def read(self):
-        for root, dirs, files in os.walk(self.base_dir):
+        '''
+        Traverse directory and yield files found matching 
+        the given extensions. This expects
+        '''
+        for root, _ , files in os.walk(self.base_dir):
             for file in files:
                 for extension in self.file_extensions:
                     if file.endswith(extension):
                         file_path = os.path.join(root, file)
-                        with open(file_path, 'r') as file:
+                        with open(file_path, 'r',encoding=self.encoding) as file:
                             yield(self.file_to_dict(file_path, file))
```

### Comparing `pocketsearch-0.5.7/src/pocketsearch/tests.py` & `pocketsearch-0.6.0/src/pocketsearch/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 import unittest
 import tempfile
 import datetime
 
-from pocketsearch import FileSystemIndex, Text, PocketSearch, Schema, Query, Field, Int, Real, Blob, Date, Datetime, IdField
+from pocketsearch import FileSystemReader, Text, PocketSearch, Schema, Query, Field, Int, Real, Blob, Date, Datetime, IdField
 
 
 class Movie(Schema):
     '''
     A simple movie schema we use for tests.
     '''
 
@@ -490,31 +490,37 @@
 
     def test_filter_combined_and_or(self):
         self.assertEqual(self.pocket_search.search(price__lte=4, description__allow_boolean="apple OR Orange").count(), 2)
 
 
 class FileSystemReaderTests(unittest.TestCase):
 
+    class FileSchema(Schema):
+
+        text = Text(index=True)
+        filename = Text(is_id_field=True)    
+
     def test_build_index(self):
         self.files_to_index = []
         with tempfile.TemporaryDirectory() as tmpdirname:
             for file_name, contents in [
                 ("a.txt", "Hello world !"),
                 ("b.txt", "Good bye world !"),
                 ("c.txt", "Hello again, world !"),
             ]:
-                f = open(os.path.join(tmpdirname, file_name), "w")
+                f = open(os.path.join(tmpdirname, file_name), "w", encoding="utf-8")
                 f.write(contents)
                 f.close()
-            index = FileSystemIndex(base_dir=tmpdirname, file_extensions=[".txt"])
-            index.build()
-            self.assertEqual(index.search(text="world").count(), 3)
-            self.assertEqual(index.search(text="bye").count(), 1)
-            self.assertEqual(index.search(filename="d.txt").count(), 0)
+            pocket_search = PocketSearch(schema=self.FileSchema)
+            reader = FileSystemReader(base_dir=tmpdirname, file_extensions=[".txt"])
+            pocket_search.build(reader)
+            self.assertEqual(pocket_search.search(text="world").count(), 3)
+            self.assertEqual(pocket_search.search(text="bye").count(), 1)
+            self.assertEqual(pocket_search.search(filename="d.txt").count(), 0)
             # rebuild the index, the number of documents should not
             # change as they have only been updated
-            index.build()
-            self.assertEqual(index.search(text="world").count(), 3)
+            pocket_search.build(reader)
+            self.assertEqual(pocket_search.search(text="world").count(), 3)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pocketsearch-0.5.7/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.6.0/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.7
+Version: 0.6.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
+Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -22,25 +23,29 @@
 License-File: LICENSE
 
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
 - Support for full text search
 - A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
-- Support for text, numeric and date search
+- Support for multi-field indices including text, numeric and date search
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
+pocketsearch is currently being tested on data from Wikipedia, indexing more than 6 million abstracts. If you 
+are interested in preliminary performance tests, have a look at https://github.com/kaykay-dv/pocketsearch/tree/development/tests.
+
 # Status
 The package is currently in Beta status.
 
 ![Unit tests main](https://github.com/kaykay-dv/pocketsearch/actions/workflows/unittests-main.yml/badge.svg)
 ![Unit tests development](https://github.com/kaykay-dv/pocketsearch/actions/workflows/unittests-development.yml/badge.svg)
 
+
 # Installation
 
 Run 
 
 ```Shell
 pip install pocketsearch
 ```
@@ -221,16 +226,43 @@
 
 To delete a document, use:
 
 ```Python
 pocket_search.delete(rowid=1)
 ```
 
-Please note that by default an AND query is performed, thus only documents are
-matched where text contains the word "world" and the filename is "a.txt"
+# Using index readers to insert data
+
+Normally we have a data source at hand (e.g. files in a file system or a source database) that we use to read 
+data from. IndexReader classes can be used to build an index from such a data source. Assume, you want to 
+index text files from a directory, we first define a schema:
+
+```Python
+class FileSchema(Schema):
+
+        text = Text(index=True)
+        filename = Text(is_id_field=True) 
+```
+
+Next, we create a PocketSearch and 
+
+```Python
+from pocketsearch import FileSystemReader
+pocket_search = PocketSearch(schema=FileSchema)
+reader = FileSystemReader(base_dir="/some/directory", file_extensions=[".txt"])
+pocket_search.build(reader)
+```
+
+This will build the index. If a document has already been seen it will be updated, a new document will be 
+inserted otherwise. 
+
+Currently, the FileSystemReader is the only implementation provided, however you can easily implement your own 
+by implementing the abstract class IndexError implementing a .read method. The .read method should return an 
+iterable containing dictionaries whereas the dictionary's keys correspond to schema fields and its values 
+the data you want to insert for the document. 
 
 # Searching numeric data
 
 You can also search for numeric data:
 
 ```Python
 class Product(Schema):
```

