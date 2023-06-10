# Comparing `tmp/xtdb-0.5.0.tar.gz` & `tmp/xtdb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtdb-0.5.0.tar", max compression
+gzip compressed data, was "xtdb-0.6.0.tar", max compression
```

## Comparing `xtdb-0.5.0.tar` & `xtdb-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-06-05 17:21:07.892303 xtdb-0.5.0/LICENSE
--rw-r--r--   0        0        0     4797 2023-06-05 17:21:07.892303 xtdb-0.5.0/README.md
--rw-r--r--   0        0        0     1567 2023-06-05 17:21:07.896303 xtdb-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/__init__.py
--rw-r--r--   0        0        0      211 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/__main__.py
--rw-r--r--   0        0        0    14264 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/datalog.py
--rw-r--r--   0        0        0      120 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/exceptions.py
--rw-r--r--   0        0        0     1711 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/orm.py
--rw-r--r--   0        0        0     6391 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/query.py
--rw-r--r--   0        0        0    12148 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/session.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 xtdb-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-10 08:15:27.079638 xtdb-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4977 2023-06-10 08:15:27.079638 xtdb-0.6.0/README.md
+-rw-r--r--   0        0        0     1567 2023-06-10 08:15:27.083638 xtdb-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 08:15:27.083638 xtdb-0.6.0/xtdb/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-10 08:15:27.083638 xtdb-0.6.0/xtdb/__main__.py
+-rw-r--r--   0        0        0    16276 2023-06-10 08:15:27.083638 xtdb-0.6.0/xtdb/datalog.py
+-rw-r--r--   0        0        0      120 2023-06-10 08:15:27.083638 xtdb-0.6.0/xtdb/exceptions.py
+-rw-r--r--   0        0        0     1711 2023-06-10 08:15:27.083638 xtdb-0.6.0/xtdb/orm.py
+-rw-r--r--   0        0        0     6391 2023-06-10 08:15:27.083638 xtdb-0.6.0/xtdb/query.py
+-rw-r--r--   0        0        0    13348 2023-06-10 08:15:27.083638 xtdb-0.6.0/xtdb/session.py
+-rw-r--r--   0        0        0     5657 1970-01-01 00:00:00.000000 xtdb-0.6.0/PKG-INFO
```

### Comparing `xtdb-0.5.0/LICENSE` & `xtdb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtdb-0.5.0/README.md` & `xtdb-0.6.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -31,45 +31,45 @@
 ```
 
 ### Using the Client
 
 The `XTDBClient` supports the full [HTTP API spec](https://docs.xtdb.com/clients/http/).
 
 ```python3
->>> import os
->>> from xtdb.session import XTDBClient, Operation
->>>
->>> client = XTDBClient(os.environ["XTDB_URI"])
->>> client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
->>>
->>> client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
+>> > import os
+>> > from xtdb.session import XTDBClient, Operation
+>> >
+>> > client = XTDBClient(os.environ["XTDB_URI"])
+>> > client.submit_tx([Operation.put({"xt/id": "123", "name": "fred"})])
+>> >
+>> > client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
 [[{'name': 'fred', 'xt/id': '123'}]]
->>>
->>> client.get_entity("123")
+>> >
+>> > client.get_entity("123")
 {'name': 'fred', 'xt/id': '123'}
 ```
 
 Take a look at the spec to see the full range of functionality that maps directly to the client.
 
 ### Using the Datalog module
 
-The [datalog](xtdb/datalog.py) module also provides a layer to construct queries with more easily.
-Given the data from [the cities example](examples/cities) has been seeded:
+The [datalog](https://github.com/Donnype/xtdb-py/blob/main/xtdb/datalog.py) module also provides a layer to construct queries with more easily.
+Given the data from [the cities example](https://github.com/Donnype/xtdb-py/blob/main/examples/cities) has been seeded:
 ```python3
 >>> from xtdb.datalog import Find, Where
 >>>
 >>> query = Find("(pull Country [*])") & Find("City") & (Where("City", "City/country", "Country") & Where("City", "City/name", '"Rome"'))
 >>> str(query)
 {:query {:find [ (pull Country [*]) City] :where [ [ City :City/country Country ] [ City :City/name "Rome" ]]}}
 >>>
 >>> client.query(query)
 [[{'type': 'Country', 'Country/name': 'Italy', 'xt/id': 'c095839f-031f-46ad-85e1-097f634ba4f0'}, '33aa7fa6-b752-4982-a772-d2dbaeda58ae']]
 ```
 
-To see more datalog query examples, check out the [unit tests](tests/test_datalog.py).
+To see more datalog query examples, check out the [unit tests](https://github.com/Donnype/xtdb-py/blob/main/tests/test_datalog.py).
 
 ### Using the ORM and Session
 
 Below is an example of how to use the ORM functionality.
 
 ```python3
 import os
@@ -98,15 +98,15 @@
 
 query = Query(TestEntity).where(TestEntity, name="test")
 result = session.query(query)
 
 result[0].dict() #  {"TestEntity/name": "test", "type": "TestEntity", "xt/id": "fe2a3ee0-9254-41dc-91cc-74ad9e2a16db"}
 ```
 
-To see more examples, check out the [examples directory](examples).
+To see more examples, check out the [examples directory](https://github.com/Donnype/xtdb-py/blob/main/examples).
 Don't hesitate to add your own examples!
 
 ### Using the CLI for querying
 
 This package also comes with an easy CLI tool to query XTDB.
 To query XTDB using a plain query you can run
```

### Comparing `xtdb-0.5.0/pyproject.toml` & `xtdb-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtdb"
-version = "0.5.0"
+version = "0.6.0"
 packages = [{ include = "xtdb" }]
 include  = ["xtdb/**"]
 exclude = [
     "**/.idea",
     "**/.git*",
     "**/.*ignore",
     "**/.flake8",
```

### Comparing `xtdb-0.5.0/xtdb/datalog.py` & `xtdb-0.6.0/xtdb/datalog.py`

 * *Files 15% similar despite different names*

```diff
@@ -80,25 +80,25 @@
             collected = list(set(collected))
         if all(clause.commutative for clause in self.clauses):
             collected = sorted(collected)
 
         return collected
 
     def _or(self, other: Clause) -> "Clause":
-        if isinstance(other, Where):
+        if isinstance(other, (Where, WherePredicate)):
             raise XTDBException("Cannot | on a single where, use & instead")
 
         return Or([self, other])
 
     def _and(self, other: Clause) -> Clause:
         if self.query_section != "find" and issubclass(type(other), Find):
             raise XTDBException("Cannot perform a where-find. User find-where instead.")
         if self.query_section == "find" and isinstance(other, And) and other.query_section != "find":
             return FindWhere(self, other)
-        if self.query_section == "find" and isinstance(other, (Where, Or, Not)):
+        if self.query_section == "find" and isinstance(other, (Where, Or, Not, NotJoin, WherePredicate)):
             return FindWhere(self, other)
 
         return And(self.clauses + [other], self.query_section)
 
     def __invert__(self):
         return Not(self.clauses)
 
@@ -158,14 +158,72 @@
     def _or(self, other: Clause) -> Clause:
         return Or(self.clauses + [other])
 
     def __invert__(self):
         return And(self.clauses)
 
 
+class NotJoin(Clause):
+    def __init__(self, variable: str, clauses: Optional[List] = None):
+        self.variable = variable
+        self.clauses = clauses or []
+
+    def compile(self, root: bool = True, *, separator=" ") -> str:
+        collected = []
+
+        for clause in self.clauses:
+            collected.append(clause.compile(root=False, separator=separator))
+
+        if all(clause.idempotent for clause in self.clauses):
+            collected = list(set(collected))
+
+        if all(clause.commutative for clause in self.clauses):
+            collected = sorted(collected)
+
+        if root:
+            return f":where [(not-join{separator}[{self.variable}] {separator.join(collected)})]"
+
+        return f"(not-join{separator}[{self.variable}] {separator.join(collected)})"
+
+    def _and(self, other: Clause) -> Clause:
+        return NotJoin(self.variable, self.clauses + [other])
+
+    def __invert__(self):
+        raise XTDBException("Cannot use ~ on not-join")
+
+
+class OrJoin(Clause):
+    def __init__(self, variable: str, clauses: Optional[List] = None):
+        self.variable = variable
+        self.clauses = clauses or []
+
+    def compile(self, root: bool = True, *, separator=" ") -> str:
+        collected = []
+
+        for clause in self.clauses:
+            collected.append(clause.compile(root=False, separator=separator))
+
+        if all(clause.idempotent for clause in self.clauses):
+            collected = list(set(collected))
+
+        if all(clause.commutative for clause in self.clauses):
+            collected = sorted(collected)
+
+        if root:
+            return f":where [(or-join{separator}[{self.variable}] {separator.join(collected)})]"
+
+        return f"(or-join{separator}[{self.variable}] {separator.join(collected)})"
+
+    def _and(self, other: Clause) -> Clause:
+        return OrJoin(self.variable, self.clauses + [other])
+
+    def __invert__(self):
+        raise XTDBException("Cannot use ~ on or-join")
+
+
 class Where(Clause):
     def __init__(self, document: str, field: str, value: Any = ""):
         self.document = document
         self.field = field
         self.value = value
 
     def compile(self, root: bool = True, *, separator=" ") -> str:
@@ -260,15 +318,15 @@
             return f":find [{self.expression}]"
 
         return str(self.expression)
 
     def _and(self, other: Clause) -> Clause:
         if isinstance(other, And) and other.query_section != "find":
             return FindWhere(self, other)
-        if isinstance(other, (Where, Or, Not)):
+        if isinstance(other, (Where, Or, Not, WherePredicate)):
             return FindWhere(self, other)
 
         return And([self, other], "find")
 
 
 class In(QueryKey):
     def __init__(self, in_args: Union[str, List[str], List[List[str]]], values: Union[str, List[str], List[List[str]]]):
```

### Comparing `xtdb-0.5.0/xtdb/orm.py` & `xtdb-0.6.0/xtdb/orm.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.5.0/xtdb/query.py` & `xtdb-0.6.0/xtdb/query.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.5.0/xtdb/session.py` & `xtdb-0.6.0/xtdb/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime, timezone
 from enum import Enum
+from json import JSONDecodeError
 from typing import Any, Dict, List, Literal, Optional, Type, Union
 
 from requests import HTTPError, Response, Session
 from requests.adapters import DEFAULT_POOLBLOCK, DEFAULT_POOLSIZE, HTTPAdapter
+from requests.exceptions import ConnectionError
 from urllib3 import Retry
 
 from xtdb.datalog import Clause, FindWhere
 from xtdb.exceptions import XTDBException
 from xtdb.orm import Base, Fn
 from xtdb.query import Query
 
@@ -94,28 +96,36 @@
         pool_connections: int = DEFAULT_POOLSIZE,
         pool_maxsize: int = DEFAULT_POOLSIZE,
         pool_block: bool = DEFAULT_POOLBLOCK,
         retries: int = 6,
         backoff_factor: float = 0.5,
     ):
         self.base_url = base_url
-        self._session = Session()
-
-        adapter = HTTPAdapter(
+        self.adapter = HTTPAdapter(
             pool_connections=pool_connections,
             pool_maxsize=pool_maxsize,
             pool_block=pool_block,
-            max_retries=Retry(total=retries, backoff_factor=backoff_factor),
+            max_retries=Retry(total=retries, backoff_factor=backoff_factor, connect=3),
         )
-        self._session.mount("http://", adapter)
-        self._session.mount("https://", adapter)
-        self._session.headers["Accept"] = "application/json"
-        self._session.hooks["response"] = self._verify_response
+        self._session = self.get_session()
+
+    def get_session(self) -> Session:
+        session = Session()
+
+        session.mount("http://", self.adapter)
+        session.mount("https://", self.adapter)
+        session.headers["Accept"] = "application/json"
+        session.hooks["response"] = self._verify_response
+
+        logger.debug("Initialized new HTTP session")
+
+        return session
 
-        logger.debug("Initialized HTTP session to %s", self.base_url)
+    def refresh(self):
+        self._session = self.get_session()
 
     @staticmethod
     def _verify_response(response: Response, *args, **kwargs) -> None:
         logger.debug('"%s %s" %s', response.request.method, response.request.url, response.status_code)
 
         try:
             response.raise_for_status()
@@ -195,25 +205,39 @@
     def query(
         self,
         query: Union[str, Query, Clause],
         *,
         valid_time: Optional[datetime] = None,
         tx_time: Optional[datetime] = None,
         tx_id: Optional[int] = None,
+        tries: int = 0,
     ) -> Union[List, Dict]:
         if not isinstance(query, (str, Query)) and not issubclass(type(query), FindWhere):
             raise XTDBException("Cannot query using incomplete clause")
 
         params = self._format_parameter("valid-time", valid_time)
         params = self._format_parameter("tx-time", tx_time, params)
         params = self._format_parameter("tx-id", tx_id, params)
 
-        return self._session.post(
-            f"{self.base_url}/query", str(query), params=params, headers={"Content-Type": "application/edn"}
-        ).json()
+        try:
+            return self._session.post(
+                f"{self.base_url}/query", str(query), params=params, headers={"Content-Type": "application/edn"}
+            ).json()
+        except JSONDecodeError as e:
+            if e.msg == "Expecting value":
+                # Empty bodies are returned when you do strange queries such as Sum(x) where x is not numerical.
+                raise XTDBException("Bad XTDB response: query probably failed") from e
+            raise
+        except ConnectionError:
+            if tries > 0:
+                raise
+
+            # Bad queries cleave connections in a bad state, which is fixed by creating a new requests.Session()
+            self.refresh()
+            return self.query(query, valid_time=valid_time, tx_time=tx_time, tx_id=tx_id, tries=1)
 
     def await_transaction(self, tx_id: int, timeout: Optional[int] = None) -> None:
         params = self._format_parameter("timeout", timeout)
         params = self._format_parameter("tx-id", tx_id, params)
 
         self._session.get(f"{self.base_url}/await-tx", params=params)
 
@@ -225,21 +249,29 @@
 
     def get_transaction_log(self, after_tx_id: Optional[int] = None, with_ops: Optional[bool] = None):
         params = self._format_parameter("after-tx-id", after_tx_id)
         params = self._format_parameter("with-ops?", with_ops, params)
 
         return self._session.get(f"{self.base_url}/tx-log", params=params).json()
 
-    def submit_transaction(self, transaction: Union[Transaction, List]) -> None:
+    def submit_tx(self, transaction: Union[Transaction, List], tries: int = 0) -> None:
         if isinstance(transaction, list):
             transaction = Transaction(operations=transaction)
 
-        res = self._session.post(
-            f"{self.base_url}/submit-tx", transaction.json(), headers={"Content-Type": "application/json"}
-        )
+        try:
+            res = self._session.post(
+                f"{self.base_url}/submit-tx", transaction.json(), headers={"Content-Type": "application/json"}
+            )
+        except ConnectionError:
+            if tries > 0:
+                raise
+
+            # Bad queries cleave connections in a bad state, which is fixed by creating a new requests.Session()
+            self.refresh()
+            return self.submit_tx(transaction, tries=1)
 
         self.await_transaction(res.json()["txId"])
 
     def get_transaction_committed(self, tx_id: int):
         return self._session.get(f"{self.base_url}/tx-committed", params=self._format_parameter("tx-id", tx_id)).json()
 
     def get_latest_completed_transaction(self):
@@ -311,11 +343,11 @@
         self._transaction.add(Operation.fn(function.identifier, *args))
 
     def commit(self) -> None:
         if operation_count := len(self._transaction.operations) == 0:
             return
 
         try:
-            self.client.submit_transaction(self._transaction)
+            self.client.submit_tx(self._transaction)
             logger.debug("Committed %s operations", operation_count)
         finally:
             self._transaction = Transaction()
```

### Comparing `xtdb-0.5.0/PKG-INFO` & `xtdb-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python ORM for XTDB.
 Home-page: https://github.com/Donnype/xtdb-py
 Author: Donny Peeters
 Author-email: donny.peeters@hotmail.com
 Maintainer: Donny Peeters
 Maintainer-email: donny.peeters@hotmail.com
 Requires-Python: >=3.8,<4.0
@@ -50,45 +50,45 @@
 ```
 
 ### Using the Client
 
 The `XTDBClient` supports the full [HTTP API spec](https://docs.xtdb.com/clients/http/).
 
 ```python3
->>> import os
->>> from xtdb.session import XTDBClient, Operation
->>>
->>> client = XTDBClient(os.environ["XTDB_URI"])
->>> client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
->>>
->>> client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
+>> > import os
+>> > from xtdb.session import XTDBClient, Operation
+>> >
+>> > client = XTDBClient(os.environ["XTDB_URI"])
+>> > client.submit_tx([Operation.put({"xt/id": "123", "name": "fred"})])
+>> >
+>> > client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
 [[{'name': 'fred', 'xt/id': '123'}]]
->>>
->>> client.get_entity("123")
+>> >
+>> > client.get_entity("123")
 {'name': 'fred', 'xt/id': '123'}
 ```
 
 Take a look at the spec to see the full range of functionality that maps directly to the client.
 
 ### Using the Datalog module
 
-The [datalog](xtdb/datalog.py) module also provides a layer to construct queries with more easily.
-Given the data from [the cities example](examples/cities) has been seeded:
+The [datalog](https://github.com/Donnype/xtdb-py/blob/main/xtdb/datalog.py) module also provides a layer to construct queries with more easily.
+Given the data from [the cities example](https://github.com/Donnype/xtdb-py/blob/main/examples/cities) has been seeded:
 ```python3
 >>> from xtdb.datalog import Find, Where
 >>>
 >>> query = Find("(pull Country [*])") & Find("City") & (Where("City", "City/country", "Country") & Where("City", "City/name", '"Rome"'))
 >>> str(query)
 {:query {:find [ (pull Country [*]) City] :where [ [ City :City/country Country ] [ City :City/name "Rome" ]]}}
 >>>
 >>> client.query(query)
 [[{'type': 'Country', 'Country/name': 'Italy', 'xt/id': 'c095839f-031f-46ad-85e1-097f634ba4f0'}, '33aa7fa6-b752-4982-a772-d2dbaeda58ae']]
 ```
 
-To see more datalog query examples, check out the [unit tests](tests/test_datalog.py).
+To see more datalog query examples, check out the [unit tests](https://github.com/Donnype/xtdb-py/blob/main/tests/test_datalog.py).
 
 ### Using the ORM and Session
 
 Below is an example of how to use the ORM functionality.
 
 ```python3
 import os
@@ -117,15 +117,15 @@
 
 query = Query(TestEntity).where(TestEntity, name="test")
 result = session.query(query)
 
 result[0].dict() #  {"TestEntity/name": "test", "type": "TestEntity", "xt/id": "fe2a3ee0-9254-41dc-91cc-74ad9e2a16db"}
 ```
 
-To see more examples, check out the [examples directory](examples).
+To see more examples, check out the [examples directory](https://github.com/Donnype/xtdb-py/blob/main/examples).
 Don't hesitate to add your own examples!
 
 ### Using the CLI for querying
 
 This package also comes with an easy CLI tool to query XTDB.
 To query XTDB using a plain query you can run
```

