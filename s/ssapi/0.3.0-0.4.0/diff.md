# Comparing `tmp/ssapi-0.3.0.tar.gz` & `tmp/ssapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssapi-0.3.0.tar", last modified: Sat Jun 10 16:28:58 2023, max compression
+gzip compressed data, was "ssapi-0.4.0.tar", last modified: Sat Jun 10 16:36:40 2023, max compression
```

## Comparing `ssapi-0.3.0.tar` & `ssapi-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.291443 ssapi-0.3.0/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:28:58.291443 ssapi-0.3.0/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       30 2023-06-10 16:26:54.000000 ssapi-0.3.0/pyproject.toml
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.288443 ssapi-0.3.0/scripts/
--rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.3.0/scripts/ssapi-web
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-06-10 16:28:58.291443 ssapi-0.3.0/setup.cfg
--rw-r--r--   0 zedr      (1000) zedr      (1000)      272 2023-06-10 16:28:55.000000 ssapi-0.3.0/setup.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.286443 ssapi-0.3.0/src/
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.290443 ssapi-0.3.0/src/ssapi/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.3.0/src/ssapi/__init__.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     3421 2023-06-10 16:27:44.000000 ssapi-0.3.0/src/ssapi/db.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1983 2023-06-10 16:27:44.000000 ssapi-0.3.0/src/ssapi/db_utils.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      201 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/defaults.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      688 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/entities.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.3.0/src/ssapi/env.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      363 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/exceptions.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     2397 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/relational.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      826 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/types.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1038 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/utils.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     2353 2023-06-10 16:27:44.000000 ssapi-0.3.0/src/ssapi/web.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1305 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/web_decorators.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      760 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/web_tools.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.291443 ssapi-0.3.0/src/ssapi.egg-info/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      480 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/SOURCES.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/dependency_links.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/requires.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/top_level.txt
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:36:40.646378 ssapi-0.4.0/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:36:40.645378 ssapi-0.4.0/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       30 2023-06-10 16:26:54.000000 ssapi-0.4.0/pyproject.toml
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:36:40.642378 ssapi-0.4.0/scripts/
+-rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.4.0/scripts/ssapi-web
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-06-10 16:36:40.646378 ssapi-0.4.0/setup.cfg
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      272 2023-06-10 16:36:32.000000 ssapi-0.4.0/setup.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:36:40.642378 ssapi-0.4.0/src/
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:36:40.644378 ssapi-0.4.0/src/ssapi/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.4.0/src/ssapi/__init__.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     3466 2023-06-10 16:35:29.000000 ssapi-0.4.0/src/ssapi/db.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1984 2023-06-10 16:35:29.000000 ssapi-0.4.0/src/ssapi/db_utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      201 2023-06-10 16:26:54.000000 ssapi-0.4.0/src/ssapi/defaults.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      722 2023-06-10 16:35:56.000000 ssapi-0.4.0/src/ssapi/entities.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.4.0/src/ssapi/env.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      363 2023-06-10 16:26:54.000000 ssapi-0.4.0/src/ssapi/exceptions.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     2397 2023-06-10 16:26:54.000000 ssapi-0.4.0/src/ssapi/relational.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      826 2023-06-10 16:26:54.000000 ssapi-0.4.0/src/ssapi/types.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1038 2023-06-10 16:26:54.000000 ssapi-0.4.0/src/ssapi/utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     2357 2023-06-10 16:35:29.000000 ssapi-0.4.0/src/ssapi/web.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1305 2023-06-10 16:26:54.000000 ssapi-0.4.0/src/ssapi/web_decorators.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      760 2023-06-10 16:26:54.000000 ssapi-0.4.0/src/ssapi/web_tools.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:36:40.645378 ssapi-0.4.0/src/ssapi.egg-info/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:36:40.000000 ssapi-0.4.0/src/ssapi.egg-info/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      480 2023-06-10 16:36:40.000000 ssapi-0.4.0/src/ssapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-06-10 16:36:40.000000 ssapi-0.4.0/src/ssapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-06-10 16:36:40.000000 ssapi-0.4.0/src/ssapi.egg-info/requires.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-06-10 16:36:40.000000 ssapi-0.4.0/src/ssapi.egg-info/top_level.txt
```

### Comparing `ssapi-0.3.0/src/ssapi/db.py` & `ssapi-0.4.0/src/ssapi/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ssapi.types import Undefined
 from ssapi.entities import Sale, Return
 from ssapi.relational import Database
 from ssapi.db_utils import (
     create_date_where_clause,
     create_shop_where_clause,
-    WhereClause,
+    WhereClause
 )
 
 
 class ShopDatabase(Database):
     """A database that stores data about shops"""
 
     def _tables_init(self) -> None:
@@ -61,19 +61,19 @@
     def get_shops(self) -> T.Generator[str, None, None]:
         """Get all the shops"""
         cur = self.conn.execute("SELECT DISTINCT shop FROM sales")
         for shop, *_ in cur.fetchall():
             yield shop
 
     def get_sales(
-        self,
-        date_start="",
-        date_end="",
-        is_discounted=Undefined(),
-        shop="",
+            self,
+            date_start="",
+            date_end="",
+            is_discounted=Undefined(),
+            shop="",
     ) -> T.Generator[Sale, None, None]:
         """Get the sales according to the given criteria"""
         where = create_date_where_clause(date_start, date_end)
         where = where.AND(create_shop_where_clause(shop))
         where = where.AND(WhereClause.create(is_discounted=is_discounted))
         cur = self.conn.execute(
             f"SELECT * FROM sales {where.clause}", where.values
@@ -86,18 +86,20 @@
         cur = self.conn.execute("SELECT * FROM sales WHERE id=?", (id,))
         if result := cur.fetchone():
             return Sale(*result)
         else:
             return None
 
     def get_returns(
-        self, date_start=None, date_end=None
+            self, date_start=None, date_end=None
     ) -> T.Generator[Return, None, None]:
         """Get the sales according to the given criteria"""
         cur = self.conn.execute("SELECT * FROM returns")
         for result in cur.fetchall():
             yield Return(*result)
 
     def get_products(self) -> T.Generator[tuple, None, None]:
-        cur = self.conn.execute("SELECT DISTINCT product FROM sales")
+        cur = self.conn.execute(
+            "SELECT DISTINCT product FROM sales"
+        )
         for item in cur.fetchall():
             yield item[0]
```

### Comparing `ssapi-0.3.0/src/ssapi/db_utils.py` & `ssapi-0.4.0/src/ssapi/db_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,25 @@
             return self
         else:
             return WhereClause(
                 clause=(
                     f"WHERE ({self._bare_clause}) "
                     f"AND ({other_where._bare_clause})"
                 ),
-                values=self.values + other_where.values,
+                values=self.values + other_where.values
+
             )
 
     @property
     def _bare_clause(self) -> str:
         return self.clause.removeprefix("WHERE").lstrip()
 
     @classmethod
-    def create(
-        cls, **kwargs: Union[Undefined, dict[str, str]]
-    ) -> "WhereClause":
+    def create(cls,
+               **kwargs: Union[Undefined, dict[str, str]]) -> "WhereClause":
         """Create a new WHERE clause using the given key and value"""
         if len(kwargs) != 1:
             raise ValueError("Only one key/value pair supported")
 
         key, value = list(kwargs.items())[0]
 
         if isinstance(value, Undefined):
```

### Comparing `ssapi-0.3.0/src/ssapi/env.py` & `ssapi-0.4.0/src/ssapi/env.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.3.0/src/ssapi/relational.py` & `ssapi-0.4.0/src/ssapi/relational.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.3.0/src/ssapi/types.py` & `ssapi-0.4.0/src/ssapi/types.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.3.0/src/ssapi/utils.py` & `ssapi-0.4.0/src/ssapi/utils.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.3.0/src/ssapi/web.py` & `ssapi-0.4.0/src/ssapi/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     return [
         dict(sale.as_map())
         for sale in get_env_database().get_sales(
             date_start=start,
             date_end=end,
             shop=shop,
             is_discounted=(
-                Undefined()
-                if is_discounted is None
-                else literal_eval(is_discounted)
-            ),
+                Undefined() if is_discounted is None else literal_eval(
+                    is_discounted
+                )
+            )
         )
     ]
 
 
 @get("/sales/<id:int>")
 @returns_json
 def get_sale(id: int) -> dict:
@@ -79,15 +79,14 @@
     else:
         db = get_env_database()
         count = db.add_sales(new_sale)
         outcome = f"creation ({count}) succeeded in database at: {db.name}"
 
     return {"outcome": outcome}
 
-
 @get("/products")
 @returns_json
 def get_products():
     return tuple(get_env_database().get_products())
 
 
 @post("/drop")
```

### Comparing `ssapi-0.3.0/src/ssapi/web_decorators.py` & `ssapi-0.4.0/src/ssapi/web_decorators.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.3.0/src/ssapi/web_tools.py` & `ssapi-0.4.0/src/ssapi/web_tools.py`

 * *Files identical despite different names*

