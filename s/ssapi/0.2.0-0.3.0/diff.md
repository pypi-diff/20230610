# Comparing `tmp/ssapi-0.2.0.tar.gz` & `tmp/ssapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssapi-0.2.0.tar", last modified: Tue May  2 20:12:05 2023, max compression
+gzip compressed data, was "ssapi-0.3.0.tar", last modified: Sat Jun 10 16:28:58 2023, max compression
```

## Comparing `ssapi-0.2.0.tar` & `ssapi-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.477158 ssapi-0.2.0/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-05-02 20:12:05.477158 ssapi-0.2.0/PKG-INFO
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.474158 ssapi-0.2.0/scripts/
--rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.2.0/scripts/ssapi-web
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-05-02 20:12:05.477158 ssapi-0.2.0/setup.cfg
--rw-r--r--   0 zedr      (1000) zedr      (1000)      272 2023-05-02 20:11:58.000000 ssapi-0.2.0/setup.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.473158 ssapi-0.2.0/src/
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.476158 ssapi-0.2.0/src/ssapi/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.2.0/src/ssapi/__init__.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)     2596 2023-04-30 11:02:56.000000 ssapi-0.2.0/src/ssapi/db.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      202 2023-04-30 07:47:30.000000 ssapi-0.2.0/src/ssapi/defaults.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      715 2023-04-30 10:33:43.000000 ssapi-0.2.0/src/ssapi/entities.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.2.0/src/ssapi/env.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1309 2023-04-30 10:58:00.000000 ssapi-0.2.0/src/ssapi/relational.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      540 2023-04-30 11:18:15.000000 ssapi-0.2.0/src/ssapi/types.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)     1248 2023-04-30 13:51:41.000000 ssapi-0.2.0/src/ssapi/web.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      927 2023-04-30 10:39:01.000000 ssapi-0.2.0/src/ssapi/web_decorators.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      427 2023-04-30 09:55:14.000000 ssapi-0.2.0/src/ssapi/web_tools.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.477158 ssapi-0.2.0/src/ssapi.egg-info/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      400 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/SOURCES.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/dependency_links.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/requires.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/top_level.txt
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.291443 ssapi-0.3.0/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:28:58.291443 ssapi-0.3.0/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       30 2023-06-10 16:26:54.000000 ssapi-0.3.0/pyproject.toml
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.288443 ssapi-0.3.0/scripts/
+-rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.3.0/scripts/ssapi-web
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-06-10 16:28:58.291443 ssapi-0.3.0/setup.cfg
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      272 2023-06-10 16:28:55.000000 ssapi-0.3.0/setup.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.286443 ssapi-0.3.0/src/
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.290443 ssapi-0.3.0/src/ssapi/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.3.0/src/ssapi/__init__.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     3421 2023-06-10 16:27:44.000000 ssapi-0.3.0/src/ssapi/db.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1983 2023-06-10 16:27:44.000000 ssapi-0.3.0/src/ssapi/db_utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      201 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/defaults.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      688 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/entities.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.3.0/src/ssapi/env.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      363 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/exceptions.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     2397 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/relational.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      826 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/types.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1038 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     2353 2023-06-10 16:27:44.000000 ssapi-0.3.0/src/ssapi/web.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1305 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/web_decorators.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      760 2023-06-10 16:26:54.000000 ssapi-0.3.0/src/ssapi/web_tools.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:28:58.291443 ssapi-0.3.0/src/ssapi.egg-info/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      480 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/requires.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-06-10 16:28:58.000000 ssapi-0.3.0/src/ssapi.egg-info/top_level.txt
```

### Comparing `ssapi-0.2.0/src/ssapi/db.py` & `ssapi-0.3.0/src/ssapi/db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import typing as T
 
+from ssapi.types import Undefined
 from ssapi.entities import Sale, Return
 from ssapi.relational import Database
+from ssapi.db_utils import (
+    create_date_where_clause,
+    create_shop_where_clause,
+    WhereClause,
+)
 
 
 class ShopDatabase(Database):
     """A database that stores data about shops"""
 
     def _tables_init(self) -> None:
         """Initialize the tables"""
         self.conn.execute(
-            "CREATE TABLE IF NOT EXISTS shops"
-            "("
-            "name VARCHAR(255)"
-            ")"
+            "CREATE TABLE IF NOT EXISTS shops" "(" "name VARCHAR(255)" ")"
         )
         self.conn.execute(
             "CREATE TABLE IF NOT EXISTS sales"
             "("
             "id INTEGER PRIMARY KEY,"
             "product VARCHAR(255), "
             "shop VARCHAR(255), "
@@ -37,44 +40,64 @@
             ")"
         )
 
     def add_sales(self, *sales: Sale) -> int:
         """Record sale transactions and return the number of rows created"""
         cur = self.conn.executemany(
             "INSERT INTO sales VALUES(?, ?, ?, ?, ?, ?)",
-            (sale.as_tuple() for sale in sales)
+            (sale.as_tuple() for sale in sales),
         )
         self.conn.commit()
         return cur.rowcount
 
     def add_returns(self, *returns: Return) -> int:
         """Record sale transactions and return the number of rows created"""
         cur = self.conn.executemany(
             "INSERT INTO returns VALUES(?, ?, ?, ?, ?)",
-            (ret.as_tuple() for ret in returns)
+            (ret.as_tuple() for ret in returns),
         )
         self.conn.commit()
         return cur.rowcount
 
     def get_shops(self) -> T.Generator[str, None, None]:
         """Get all the shops"""
-        cur = self.conn.execute(
-            "SELECT DISTINCT shop FROM sales"
-        )
+        cur = self.conn.execute("SELECT DISTINCT shop FROM sales")
         for shop, *_ in cur.fetchall():
             yield shop
 
-    def get_sales(self,
-                  date_start=None,
-                  date_end=None) -> T.Generator[Sale, None, None]:
+    def get_sales(
+        self,
+        date_start="",
+        date_end="",
+        is_discounted=Undefined(),
+        shop="",
+    ) -> T.Generator[Sale, None, None]:
         """Get the sales according to the given criteria"""
-        cur = self.conn.execute("SELECT * FROM sales")
+        where = create_date_where_clause(date_start, date_end)
+        where = where.AND(create_shop_where_clause(shop))
+        where = where.AND(WhereClause.create(is_discounted=is_discounted))
+        cur = self.conn.execute(
+            f"SELECT * FROM sales {where.clause}", where.values
+        )
         for result in cur.fetchall():
             yield Sale(*result)
 
-    def get_returns(self,
-                    date_start=None,
-                    date_end=None) -> T.Generator[Return, None, None]:
+    def get_sale(self, id: int) -> T.Optional[Sale]:
+        """Get a specific sale by its id"""
+        cur = self.conn.execute("SELECT * FROM sales WHERE id=?", (id,))
+        if result := cur.fetchone():
+            return Sale(*result)
+        else:
+            return None
+
+    def get_returns(
+        self, date_start=None, date_end=None
+    ) -> T.Generator[Return, None, None]:
         """Get the sales according to the given criteria"""
         cur = self.conn.execute("SELECT * FROM returns")
         for result in cur.fetchall():
             yield Return(*result)
+
+    def get_products(self) -> T.Generator[tuple, None, None]:
+        cur = self.conn.execute("SELECT DISTINCT product FROM sales")
+        for item in cur.fetchall():
+            yield item[0]
```

### Comparing `ssapi-0.2.0/src/ssapi/entities.py` & `ssapi-0.3.0/src/ssapi/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import operator
-import typing as T
 from collections import namedtuple
 from dataclasses import dataclass
 
 from ssapi.relational import Table
 
 constraint = namedtuple("constraint", ("comparator", "value", "operator"))
 
 
 @dataclass
 class Transaction(Table):
     """A generic transaction"""
-    id: T.Optional[int]
+
+    id: int | None
     product: str
     shop: str
     quantity: int
-    date: T.Optional[str] = None
+    date: str | None = None
 
     class Constraints:
         product = constraint(len, 255, operator.lt)
         shop = constraint(len, 255, operator.lt)
 
 
 @dataclass
 class Sale(Transaction):
     """A sale of a certain amount of product"""
+
     is_discounted: bool = False
 
 
 class Return(Transaction):
     """A return of a certain amount of product"""
```

### Comparing `ssapi-0.2.0/src/ssapi/env.py` & `ssapi-0.3.0/src/ssapi/env.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.2.0/src/ssapi/types.py` & `ssapi-0.3.0/src/ssapi/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 import abc
-from typing import Iterable, Tuple, Union, Protocol, Any, Callable, Union
+import typing as T
+from typing import Iterable, Tuple, Protocol, Any, Union
+
+QueryType = T.TypeVar("QueryType", bound=dict[str, T.Union[str, int]])
 
 
 class Tabular(metaclass=abc.ABCMeta):
+    @property
+    @abc.abstractmethod
+    def columns(self) -> dict[str, T.Any]:
+        ...
+
     @abc.abstractmethod
     def as_map(self) -> Iterable[Tuple[str, Union[bool, int, float, str]]]:
         ...
 
     @abc.abstractmethod
     def as_tuple(self) -> tuple:
         ...
 
     class Constraints:
         ...
 
 
 class SingletonProtocol(Protocol):
     """"""
+
     _singleton: Any
 
     def __call__(self, *args, **kwargs):
         pass
 
 
 def provides_singleton(func: Any) -> SingletonProtocol:
     return func
+
+
+class Undefined:
+    """Singleton representing an undefined value"""
+
+    def __bool__(self):
+        return False
```

### Comparing `ssapi-0.2.0/src/ssapi/web_decorators.py` & `ssapi-0.3.0/src/ssapi/web_decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import sqlite3
 from functools import wraps
 
 from bottle import request, response
 
 from ssapi.defaults import DEFAULT_SSAPI_WEB_CONTENT_TYPE
 from ssapi.web_tools import camel_to_snake_case
 
@@ -11,23 +12,36 @@
     @wraps(callable)
     def wrapper(*args, **kwargs):
         if request.headers["content-type"] == DEFAULT_SSAPI_WEB_CONTENT_TYPE:
             try:
                 request.adapted_json = camel_to_snake_case(request.json)
             except json.JSONDecodeError as exc:
                 response.status = 400
-                return {
-                    "outcome": f"error: invalid JSON: {request.body}: {exc}"
-                }
+                return {"outcome": f"error: invalid JSON: {exc}"}
+        else:
+            response.status = 400
+            return {"outcome": "error: accepts only application/json"}
 
         return callable(*args, **kwargs)
 
     return wrapper
 
 
 def returns_json(callable):
     @wraps(callable)
-    def wrapper(*args, **kwargs):
+    def wrapper(*args, **kwargs) -> str:
         response.content_type = DEFAULT_SSAPI_WEB_CONTENT_TYPE
         return json.dumps(callable(*args, **kwargs))
 
     return wrapper
+
+
+def handles_db_errors(callable):
+    @wraps(callable)
+    def wrapper(*args, **kwargs):
+        try:
+            return callable(*args, **kwargs)
+        except sqlite3.Error as err:
+            response.status = 500
+            return {"outcome": f"error: db: {err}"}
+
+    return wrapper
```

