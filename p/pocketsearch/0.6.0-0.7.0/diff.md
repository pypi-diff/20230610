# Comparing `tmp/pocketsearch-0.6.0.tar.gz` & `tmp/pocketsearch-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.6.0.tar", last modified: Sat Jun 10 10:05:26 2023, max compression
+gzip compressed data, was "pocketsearch-0.7.0.tar", last modified: Sat Jun 10 19:33:07 2023, max compression
```

## Comparing `pocketsearch-0.6.0.tar` & `pocketsearch-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.034794 pocketsearch-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-10 10:05:26.034794 pocketsearch-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 10:05:26.034794 pocketsearch-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.026794 pocketsearch-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.030794 pocketsearch-0.6.0/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20037 2023-06-10 10:05:08.000000 pocketsearch-0.6.0/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:05:26.030794 pocketsearch-0.6.0/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 10:05:26.000000 pocketsearch-0.6.0/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.813548 pocketsearch-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-10 19:33:07.809548 pocketsearch-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:33:07.813548 pocketsearch-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.805548 pocketsearch-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.809548 pocketsearch-0.7.0/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    41876 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.809548 pocketsearch-0.7.0/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.6.0/LICENSE` & `pocketsearch-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.6.0/PKG-INFO` & `pocketsearch-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.6.0
+Version: 0.7.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -161,14 +161,16 @@
     filename = Text(is_id_field=True)
 
 # create pocketsearch instance and provide schema
 pocket_search.PocketSearch(schema=FileContents)
 pocket_search.insert(text="Hello world",filename="a.txt")
 ```
 
+## Fields
+
 Following fields are available:
 
 | Field        | SQLite data type | 
 |--------------|-----------|
 | Text         | TEXT   |
 | Int          | INTEGER  |
 | Real         | REAL  |
@@ -210,15 +212,17 @@
     print(result.text)
 ```
 
 The result will contain all documents containing either "world" or where the filename is "a.text".
 
 This option is currently experimental and still has issues, espcially when accessing results through indexing. 
 
-# Handling updates and deletes
+# Inserting, updating and deleting data
+
+## Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
 pocket_search.update(rowid=1, text="The updated text.")
 ```
 
@@ -226,15 +230,15 @@
 
 To delete a document, use:
 
 ```Python
 pocket_search.delete(rowid=1)
 ```
 
-# Using index readers to insert data
+## Using index readers to insert data
 
 Normally we have a data source at hand (e.g. files in a file system or a source database) that we use to read 
 data from. IndexReader classes can be used to build an index from such a data source. Assume, you want to 
 index text files from a directory, we first define a schema:
 
 ```Python
 class FileSchema(Schema):
@@ -256,15 +260,31 @@
 inserted otherwise. 
 
 Currently, the FileSystemReader is the only implementation provided, however you can easily implement your own 
 by implementing the abstract class IndexError implementing a .read method. The .read method should return an 
 iterable containing dictionaries whereas the dictionary's keys correspond to schema fields and its values 
 the data you want to insert for the document. 
 
-# Searching numeric data
+## Optimizing the index for query performance
+If you have inserted a large volume of new documents, it might be sensible 
+to optimize the index for query performance. This can be achieved by 
+running VACUUM ANALYSE on the database, pocketsearch has a convenience 
+method for this, that can be run e.g. after the indexing process is 
+complete:
+
+```Python
+pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
+pocket_search.optimize()
+```
+
+Note, that this will close the current database connection and establish a new one. 
+
+# More search options
+
+## Searching numeric data
 
 You can also search for numeric data:
 
 ```Python
 class Product(Schema):
 
     price = Int()
@@ -285,15 +305,15 @@
 pocket_search.search(price__lte=3)
 # Matches products with price greater than equal 3
 pocket_search.search(price__gte=3)
 # Matches products with price greater than equal 3 AND where the description contains "apple".
 pocket_search.search(price__gte=3,description="apple")
 ```
 
-# Searching date fields
+## Searching date fields
 
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
     published=Datetime()
```

### Comparing `pocketsearch-0.6.0/README.md` & `pocketsearch-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,16 @@
     filename = Text(is_id_field=True)
 
 # create pocketsearch instance and provide schema
 pocket_search.PocketSearch(schema=FileContents)
 pocket_search.insert(text="Hello world",filename="a.txt")
 ```
 
+## Fields
+
 Following fields are available:
 
 | Field        | SQLite data type | 
 |--------------|-----------|
 | Text         | TEXT   |
 | Int          | INTEGER  |
 | Real         | REAL  |
@@ -186,15 +188,17 @@
     print(result.text)
 ```
 
 The result will contain all documents containing either "world" or where the filename is "a.text".
 
 This option is currently experimental and still has issues, espcially when accessing results through indexing. 
 
-# Handling updates and deletes
+# Inserting, updating and deleting data
+
+## Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
 pocket_search.update(rowid=1, text="The updated text.")
 ```
 
@@ -202,15 +206,15 @@
 
 To delete a document, use:
 
 ```Python
 pocket_search.delete(rowid=1)
 ```
 
-# Using index readers to insert data
+## Using index readers to insert data
 
 Normally we have a data source at hand (e.g. files in a file system or a source database) that we use to read 
 data from. IndexReader classes can be used to build an index from such a data source. Assume, you want to 
 index text files from a directory, we first define a schema:
 
 ```Python
 class FileSchema(Schema):
@@ -232,15 +236,31 @@
 inserted otherwise. 
 
 Currently, the FileSystemReader is the only implementation provided, however you can easily implement your own 
 by implementing the abstract class IndexError implementing a .read method. The .read method should return an 
 iterable containing dictionaries whereas the dictionary's keys correspond to schema fields and its values 
 the data you want to insert for the document. 
 
-# Searching numeric data
+## Optimizing the index for query performance
+If you have inserted a large volume of new documents, it might be sensible 
+to optimize the index for query performance. This can be achieved by 
+running VACUUM ANALYSE on the database, pocketsearch has a convenience 
+method for this, that can be run e.g. after the indexing process is 
+complete:
+
+```Python
+pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
+pocket_search.optimize()
+```
+
+Note, that this will close the current database connection and establish a new one. 
+
+# More search options
+
+## Searching numeric data
 
 You can also search for numeric data:
 
 ```Python
 class Product(Schema):
 
     price = Int()
@@ -261,15 +281,15 @@
 pocket_search.search(price__lte=3)
 # Matches products with price greater than equal 3
 pocket_search.search(price__gte=3)
 # Matches products with price greater than equal 3 AND where the description contains "apple".
 pocket_search.search(price__gte=3,description="apple")
 ```
 
-# Searching date fields
+## Searching date fields
 
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
     published=Datetime()
```

### Comparing `pocketsearch-0.6.0/setup.py` & `pocketsearch-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.6.0",
+    version = "0.7.0",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
```

### Comparing `pocketsearch-0.6.0/src/pocketsearch/__init__.py` & `pocketsearch-0.7.0/src/pocketsearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -901,30 +901,42 @@
         def __init__(self, names, value):
             self.names = names
             self.value = value
 
     def __init__(self, db_name=None,
                  index_name="documents",
                  schema=DefaultSchema,
-                 writeable=False):
+                 writeable=False,
+                 write_buffer_size=1):
         self.db_name = db_name
-        self.schema = schema(index_name)
-        if db_name is None:
-            self.connection = sqlite3.connect(":memory:", detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES)
-        else:
-            self.connection = sqlite3.connect(self.db_name, detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES)
-        self.connection.row_factory = sqlite3.Row
+        self.connection = self._open()
         self.cursor = self.connection.cursor()
+        self.schema = schema(index_name)
         self.db_name = db_name
         self.writeable = writeable
+        self.write_buffer=0 # keep a record of writes performed by insert statement
+        self.write_buffer_size=write_buffer_size
         if writeable or db_name is None:
             # If it is an in-memory database, we allow writes by default
             self.writeable = True
             self._create_table(self.schema.name)
 
+    def _open(self):
+        if self.db_name is None:
+            connection = sqlite3.connect(":memory:", detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES)
+        else:
+            connection = sqlite3.connect(self.db_name, detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES)
+        connection.row_factory = sqlite3.Row
+        return connection
+
+    def _close(self):
+        if self.connection:
+            self.connection.close()
+            self.connection = None
+
     def assure_writeable(self):
         '''
         Tests, if the index is writable.
         '''
         if not(self.writeable):
             raise self.IndexError(
                 "Index '{schema_name}' has been opened in read-only mode. Cannot write changes to index.".format(schema_name=self.schema.name))
@@ -973,30 +985,30 @@
                     index_fields.append(field)
                 elif field.index and not(field.fts_enabled()):
                     default_index_fields.append(field)
                 fields.append(field)
         if len(index_fields) == 0:
             raise IndexError("Schema does not have a single indexable field.")
         sql_table = '''
-        CREATE TABLE %s(%s)
+        CREATE TABLE IF NOT EXISTS %s(%s)
         ''' % (index_name, ", ".join([field.to_sql() for field in fields]))
         sql_virtual_table = '''
-        CREATE VIRTUAL TABLE %s_fts USING fts5(%s, content='%s', content_rowid='id' %s);
+        CREATE VIRTUAL TABLE IF NOT EXISTS %s_fts USING fts5(%s, content='%s', content_rowid='id' %s);
         ''' % (index_name, ", ".join([field.to_sql(index_table=True) for field in fields if field.fts_enabled()]), index_name, self._create_additional_options())
         # Trigger definitions:
         sql_trigger_insert = '''
-        CREATE TRIGGER {index_name}_ai AFTER INSERT ON {index_name} BEGIN
+        CREATE TRIGGER IF NOT EXISTS {index_name}_ai AFTER INSERT ON {index_name} BEGIN
         INSERT INTO {index_name}_fts(rowid, {cols}) VALUES (new.id, {new_cols});
         END;'''
         sql_trigger_delete = '''
-        CREATE TRIGGER {index_name}_ad AFTER DELETE ON {index_name} BEGIN
+        CREATE TRIGGER IF NOT EXISTS {index_name}_ad AFTER DELETE ON {index_name} BEGIN
         INSERT INTO {index_name}_fts({index_name}_fts, rowid, {cols}) VALUES('delete', old.id, {old_cols});
         END;'''
         sql_trigger_update = '''
-        CREATE TRIGGER {index_name}_au AFTER UPDATE ON {index_name} BEGIN
+        CREATE TRIGGER IF NOT EXISTS {index_name}_au AFTER UPDATE ON {index_name} BEGIN
         INSERT INTO {index_name}_fts({index_name}_fts, rowid, {cols}) VALUES('delete', old.id, {old_cols});
         INSERT INTO {index_name}_fts(rowid, {cols}) VALUES (new.id, {new_cols});
         END;
         '''
         self.cursor.execute(sql_table)
         self.cursor.execute(sql_virtual_table)
         self.cursor.execute(self._format_sql(index_name, fields, sql_trigger_insert))
@@ -1061,31 +1073,54 @@
                                                               ",".join(placeholder_values))
         try:
             self.cursor.execute(sql, values)
         except Exception as sql_error:
             raise self.DatabaseError(sql_error)
         self.connection.commit()
 
+    def commit(self):
+        '''
+        Commit current changes to database. Commits are only performed 
+        when the buffer is full.
+        '''
+        if self.write_buffer > self.write_buffer_size:
+            self.write_buffer=0 # reset buffer
+            self.connection.commit()
+
+    def optimize(self):
+        '''
+        Runs table optimization that can be run after a huge amount 
+        of data has been inserted to the database.
+        Technically, this runs a VACUUM ANALYSE command on the 
+        database, resulting in potential query speed ups.
+        '''
+        self.assure_writeable()
+        self._close() # close old connection, so we do not have any conflicts
+        connection = self._open()
+        connection.cursor().execute("VACUUM")
+        connection.close()
+
     def insert(self, *args, **kwargs):
         '''
         Inserts a new document to the search index.
         '''
         self.assure_writeable()
+        self.write_buffer = self.write_buffer + 1
         arguments = self.get_arguments(kwargs, for_search=False)
         joined_fields = ",".join([f for f in arguments])
         values = [argument.lookups[0].value for argument in arguments.values()]
         placeholder_values = "?" * len(values)
         sql = "insert into %s (%s) values (%s)" % (self.schema.name,
                                                    joined_fields,
                                                    ",".join(placeholder_values))
         try:
             self.cursor.execute(sql, values)
         except Exception as sql_error:
             raise self.DatabaseError(sql_error)
-        self.connection.commit()
+        self.commit()
 
     def get(self, rowid):
         '''
         Get a document from the index. rowid is the integer id of the document.
         '''
         sql = "select * from %s  where id=?" % (self.schema.name,)
         fields = self.schema.get_fields()
@@ -1107,25 +1142,28 @@
         arguments = self.get_arguments(kwargs, for_search=False)
         values = [argument.lookups[0].value for argument in arguments.values()] + [docid]
         stmt = []
         for f in arguments:
             stmt.append("%s=?" % f)
         sql = "update %s set %s where id=?" % (self.schema.name, ",".join(stmt))
         self.cursor.execute(sql, values)
-        self.connection.commit()
+        if self.write_buffer > self.write_buffer_size:
+            self.write_buffer=0
+            self.connection.commit()        
+        self.commit()
 
     def delete(self, rowid):
         '''
         Deletes a document. A rowid keyword argument must be provided. If the
         the rowid is not found, no deletion is done and no error is thrown.
         '''
         self.assure_writeable()
         sql = "delete from %s where id = ?" % (self.schema.name)
         self.cursor.execute(sql, (rowid,))
-        self.connection.commit()
+        self.commit()
 
     def search(self, **kwargs):
         '''
         Searches the index. Keyword arguments must correspond to
         '''
         arguments = self.get_arguments(kwargs)
         return Query(self, arguments)
```

### Comparing `pocketsearch-0.6.0/src/pocketsearch/tests.py` & `pocketsearch-0.7.0/src/pocketsearch/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,23 @@
 
     def test_write_to_read_only_index(self):
         pocket_search = PocketSearch(writeable=False)
         pocket_search.writeable = False  # in.memory dbs are writeable by default so we set the flag manually
         with self.assertRaises(pocket_search.IndexError):
             pocket_search.insert(text="21")
 
+    def test_optimize_within_tranascation(self):
+        pocket_search = PocketSearch()
+        pocket_search.insert(text="123")        
+        pocket_search.commit()
+        #with self.assertRaises(Exception):
+        # this should not work, as vacuum is not allowed at this stage
+        pocket_search.optimize()
+
+
     def test_use_insert_update_with_lookups(self):
         pocket_search = PocketSearch()
         with self.assertRaises(pocket_search.FieldError):
             pocket_search.insert(text__allow_boolean="123")
         pocket_search.insert(text="123")
         with self.assertRaises(pocket_search.FieldError):
             pocket_search.update(rowid=1, text__allow_boolean="The DOG jumped over the fence. Now he is beyond the fence.")
```

### Comparing `pocketsearch-0.6.0/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.7.0/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.6.0
+Version: 0.7.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -161,14 +161,16 @@
     filename = Text(is_id_field=True)
 
 # create pocketsearch instance and provide schema
 pocket_search.PocketSearch(schema=FileContents)
 pocket_search.insert(text="Hello world",filename="a.txt")
 ```
 
+## Fields
+
 Following fields are available:
 
 | Field        | SQLite data type | 
 |--------------|-----------|
 | Text         | TEXT   |
 | Int          | INTEGER  |
 | Real         | REAL  |
@@ -210,15 +212,17 @@
     print(result.text)
 ```
 
 The result will contain all documents containing either "world" or where the filename is "a.text".
 
 This option is currently experimental and still has issues, espcially when accessing results through indexing. 
 
-# Handling updates and deletes
+# Inserting, updating and deleting data
+
+## Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
 pocket_search.update(rowid=1, text="The updated text.")
 ```
 
@@ -226,15 +230,15 @@
 
 To delete a document, use:
 
 ```Python
 pocket_search.delete(rowid=1)
 ```
 
-# Using index readers to insert data
+## Using index readers to insert data
 
 Normally we have a data source at hand (e.g. files in a file system or a source database) that we use to read 
 data from. IndexReader classes can be used to build an index from such a data source. Assume, you want to 
 index text files from a directory, we first define a schema:
 
 ```Python
 class FileSchema(Schema):
@@ -256,15 +260,31 @@
 inserted otherwise. 
 
 Currently, the FileSystemReader is the only implementation provided, however you can easily implement your own 
 by implementing the abstract class IndexError implementing a .read method. The .read method should return an 
 iterable containing dictionaries whereas the dictionary's keys correspond to schema fields and its values 
 the data you want to insert for the document. 
 
-# Searching numeric data
+## Optimizing the index for query performance
+If you have inserted a large volume of new documents, it might be sensible 
+to optimize the index for query performance. This can be achieved by 
+running VACUUM ANALYSE on the database, pocketsearch has a convenience 
+method for this, that can be run e.g. after the indexing process is 
+complete:
+
+```Python
+pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
+pocket_search.optimize()
+```
+
+Note, that this will close the current database connection and establish a new one. 
+
+# More search options
+
+## Searching numeric data
 
 You can also search for numeric data:
 
 ```Python
 class Product(Schema):
 
     price = Int()
@@ -285,15 +305,15 @@
 pocket_search.search(price__lte=3)
 # Matches products with price greater than equal 3
 pocket_search.search(price__gte=3)
 # Matches products with price greater than equal 3 AND where the description contains "apple".
 pocket_search.search(price__gte=3,description="apple")
 ```
 
-# Searching date fields
+## Searching date fields
 
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
     published=Datetime()
```

