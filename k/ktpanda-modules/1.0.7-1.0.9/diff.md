# Comparing `tmp/ktpanda_modules-1.0.7-py3-none-any.whl.zip` & `tmp/ktpanda_modules-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 12442 bytes, number of entries: 10
--rw-rw-r--  2.0 unx        0 b- defN 22-Aug-09 19:58 ktpanda/__init__.py
--rw-rw-r--  2.0 unx     4186 b- defN 22-Aug-15 07:09 ktpanda/hotload.py
--rw-rw-r--  2.0 unx     3974 b- defN 22-Aug-14 16:58 ktpanda/object_pool.py
--rw-rw-r--  2.0 unx    10202 b- defN 22-Aug-24 08:25 ktpanda/sqlite_helper.py
--rw-rw-r--  2.0 unx     5944 b- defN 22-Aug-24 08:24 ktpanda/threadpool.py
--rw-rw-r--  2.0 unx     1074 b- defN 22-Aug-24 08:27 ktpanda_modules-1.0.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2218 b- defN 22-Aug-24 08:27 ktpanda_modules-1.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-24 08:27 ktpanda_modules-1.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 22-Aug-24 08:27 ktpanda_modules-1.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      812 b- defN 22-Aug-24 08:27 ktpanda_modules-1.0.7.dist-info/RECORD
-10 files, 28510 bytes uncompressed, 11054 bytes compressed:  61.2%
+Zip file size: 15619 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx        0 b- defN 22-Aug-25 09:43 ktpanda/__init__.py
+-rw-rw-r--  2.0 unx     4182 b- defN 22-Aug-25 09:43 ktpanda/hotload.py
+-rw-rw-r--  2.0 unx     3970 b- defN 22-Aug-25 09:43 ktpanda/object_pool.py
+-rw-rw-r--  2.0 unx    10650 b- defN 22-Aug-25 09:43 ktpanda/sqlite_helper.py
+-rw-rw-r--  2.0 unx     8902 b- defN 22-Aug-25 09:46 ktpanda/textcolor.py
+-rw-rw-r--  2.0 unx     5940 b- defN 22-Aug-25 09:43 ktpanda/threadpool.py
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Aug-25 09:47 ktpanda_modules-1.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2218 b- defN 22-Aug-25 09:47 ktpanda_modules-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Aug-25 09:47 ktpanda_modules-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 22-Aug-25 09:47 ktpanda_modules-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      889 b- defN 22-Aug-25 09:47 ktpanda_modules-1.0.9.dist-info/RECORD
+11 files, 37925 bytes uncompressed, 14115 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -6,26 +6,29 @@
 
 Filename: ktpanda/object_pool.py
 Comment: 
 
 Filename: ktpanda/sqlite_helper.py
 Comment: 
 
+Filename: ktpanda/textcolor.py
+Comment: 
+
 Filename: ktpanda/threadpool.py
 Comment: 
 
-Filename: ktpanda_modules-1.0.7.dist-info/LICENSE
+Filename: ktpanda_modules-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: ktpanda_modules-1.0.7.dist-info/METADATA
+Filename: ktpanda_modules-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: ktpanda_modules-1.0.7.dist-info/WHEEL
+Filename: ktpanda_modules-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: ktpanda_modules-1.0.7.dist-info/top_level.txt
+Filename: ktpanda_modules-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ktpanda_modules-1.0.7.dist-info/RECORD
+Filename: ktpanda_modules-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ktpanda/hotload.py

```diff
@@ -1,10 +1,10 @@
 # hotload.py
 #
-# Copyright (C) 2021 Katie Stafford (katie@ktpanda.org)
+# Copyright (C) 2022 Katie Rust (katie@ktpanda.org)
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

## ktpanda/object_pool.py

```diff
@@ -1,10 +1,10 @@
 # object_pool.py
 #
-# Copyright (C) 2021 Katie Stafford (katie@ktpanda.org)
+# Copyright (C) 2022 Katie Rust (katie@ktpanda.org)
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

## ktpanda/sqlite_helper.py

```diff
@@ -1,10 +1,10 @@
 # sqlite_helper.py
 #
-# Copyright (C) 2021 Katie Stafford (katie@ktpanda.org)
+# Copyright (C) 2022 Katie Rust (katie@ktpanda.org)
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -29,15 +29,14 @@
 various helper methods.
 '''
 
 import sys
 import sqlite3
 import functools
 import urllib.parse
-from contextlib import contextmanager
 from pathlib import Path
 
 def retry(func, *args):
     while True:
         try:
             return func(*args)
         except sqlite3.OperationalError as err:
@@ -71,14 +70,35 @@
         kw['immutable'] = 'true'
 
     uri = f'file://{urllib.parse.quote(str(Path(path).resolve()))}'
     if kw:
         uri += '?' + '&'.join(f'{urllib.parse.quote_plus(key)}={urllib.parse.quote_plus(val)}' for key, val in kw.items())
     return uri
 
+class Cursor(sqlite3.Cursor):
+    '''Subclass of sqlite3.Cursor which supports use as a context manager.'''
+    _helper_db = None
+    def execute(self, sql, parameters=()):
+        if self._helper_db and self._helper_db.explain:
+            self._helper_db._do_explain(sql, parameters)
+
+        return super().execute(sql, parameters)
+
+    def executemany(self, sql, parameters):
+        if self._helper_db and self._helper_db.explain:
+            self._helper_db._do_explain(sql, parameters)
+
+        return super().executemany(sql, parameters)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        self.close()
+
 class SQLiteDB:
     PRAGMA_journal_mode = 'WAL'
     PRAGMA_synchronous = 'NORMAL'
     PRAGMA_page_size = 8192
     PRAGMA_recursive_triggers = True
     PRAGMA_legacy_file_format = False
     PRAGMA_foreign_keys = True
@@ -177,29 +197,14 @@
                                  (prefix + old + suffix, prefix + new + suffix) + args)
 
         self.backend.execute(f'PRAGMA schema_version = {sqlite_schema_version + 1}')
         self.backend.execute('PRAGMA writable_schema = OFF')
         if check:
             self.backend.execute('PRAGMA integrity_check')
 
-    @contextmanager
-    def cursor(self, sql=None, args=()):
-        '''Helper to allow the use of the `with` statement to auto-close a cursor. Creates
-        a cursor and optionally runs an SQL query with it.'''
-        if sql is not None and self.explain:
-            self._do_explain(sql, args)
-
-        curs = self.backend.cursor()
-        try:
-            if sql is not None:
-                curs.execute(sql, args)
-            yield curs
-        finally:
-            curs.close()
-
     def commit(self):
         return self.backend.commit()
 
     def rollback(self):
         self.backend.execute('ROLLBACK')
 
     def _do_explain(self, q, args):
@@ -208,59 +213,69 @@
         self.explained.add(q)
         print()
         print('=== ' + q)
         for row in self.backend.execute('EXPLAIN QUERY PLAN ' + q, args):
             print(f'   {row!r}')
         print()
 
+    def cursor(self):
+        curs = self.backend.cursor(Cursor)
+        curs._helper_db = self
+        return curs
+
+    def execute(self, sql, parameters=()):
+        curs = self.backend.cursor(Cursor)
+        curs._helper_db = self
+        curs.execute(sql, parameters)
+        return curs
+
+    def executemany(self, sql, parameters):
+        curs = self.backend.cursor(Cursor)
+        curs._helper_db = self
+        curs.executemany(sql, parameters)
+        return curs
+
+    def execute_nonquery(self, q, args=()):
+        '''Execute a statement that will update rows but not return them, like 'INSERT',
+        'UPDATE', or 'DELETE'. Returns a tuple of (rowcount, last_insert_rowid).'''
+        if self.readonly:
+            return 0, None
+
+        with self.execute(q, args) as curs:
+            return curs.rowcount, curs.lastrowid
+
     def query_list(self, q, args=()):
         '''Runs the given query in full and returns rows as a list.'''
-        with self.cursor(q, args) as curs:
+        with self.execute(q, args) as curs:
             rows = list(curs)
         return rows
 
     def query_one(self, q, args=(), default=None):
         '''Returns a single row from the query. If the query returns no rows, returns `default`.'''
-        with self.cursor(q, args) as curs:
+        with self.execute(q, args) as curs:
             row = curs.fetchone()
         if row is not None:
             return row
         return default
 
     def query_scalar(self, q, args=(), default=None):
         '''Returns a single column from a single row. If the query returns no rows, returns `default`.'''
         return self.query_one(q, args, (default,))[0]
 
-    def execute_modify(self, q, args=()):
-        '''Execute a statement that will update rows but not return them, like 'INSERT',
-        'UPDATE', or 'DELETE'. Returns a tuple of (rowcount, last_insert_rowid).'''
-        if self.readonly:
-            return 0, None
-
-        with self.cursor(q, args) as curs:
-            return curs.rowcount, curs.lastrowid
-
-    def execute_many(self, sql, arg_sequence):
-        if self.readonly:
-            return
-
-        with self.cursor() as curs:
-            curs.executemany(sql, arg_sequence)
-
     def close(self):
         self.backend.close()
 
     def getvar(self, name, default=None):
         row = self.query_scalar('SELECT value FROM vars WHERE name = ?', (name,)).fetchone()
         if row:
             return row[0]
         return default
 
     def setvar(self, name, val):
-        self.execute_modify('INSERT OR REPLACE INTO vars VALUES(?, ?)', (name, val))
+        self.execute_nonquery('INSERT OR REPLACE INTO vars VALUES(?, ?)', (name, val))
 
     def retry_transaction(self, func, *a, **kw):
         '''Begin a transaction and run func(). If the database is locked, rolls back and
         runs func() again until it succeeds. If it fails with any other exception, the
         database is rolled back
         '''
         mode = kw.pop('mode', 'DEFERRED')
```

## ktpanda/threadpool.py

```diff
@@ -1,10 +1,10 @@
 # threadpool.py
 #
-# Copyright (C) 2021 Katie Stafford (katie@ktpanda.org)
+# Copyright (C) 2022 Katie Rust (katie@ktpanda.org)
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

## Comparing `ktpanda_modules-1.0.7.dist-info/LICENSE` & `ktpanda_modules-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ktpanda_modules-1.0.7.dist-info/METADATA` & `ktpanda_modules-1.0.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktpanda-modules
-Version: 1.0.7
+Version: 1.0.9
 Summary: A collection of miscellaneous utility modules
 Author-email: Katie Rust <katie@ktpanda.org>
 License: Copyright (C) 2022 Katie Rust (katie@ktpanda.org)        
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

