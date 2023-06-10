# Comparing `tmp/acb-0.1.5.tar.gz` & `tmp/acb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.1.5.tar", last modified: Sat May 27 21:19:36 2023, max compression
+gzip compressed data, was "acb-0.1.6.tar", last modified: Sat Jun 10 17:07:28 2023, max compression
```

## Comparing `acb-0.1.5.tar` & `acb-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1001 2023-05-27 13:27:12.641564 acb-0.1.5/README.md
--rw-r--r--   0        0        0      140 2023-05-27 20:21:40.115629 acb-0.1.5/acb/__init__.py
--rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.5/acb/actions/__init__.py
--rw-r--r--   0        0        0     1387 2023-05-27 21:16:17.114056 acb-0.1.5/acb/actions/debug.py
--rw-r--r--   0        0        0     3249 2023-05-27 21:05:57.372642 acb-0.1.5/acb/actions/encode.py
--rw-r--r--   0        0        0      877 2023-05-07 15:46:56.099014 acb-0.1.5/acb/actions/hash.py
--rw-r--r--   0        0        0       77 2023-05-26 17:34:58.552486 acb-0.1.5/acb/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.5/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-27 19:19:32.332620 acb-0.1.5/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.5/acb/adapters/database/__init__.py
--rw-r--r--   0        0        0       97 2023-05-27 21:16:18.244974 acb-0.1.5/acb/adapters/database/redis_om.py
--rw-r--r--   0        0        0    16459 2023-05-26 14:44:49.878690 acb-0.1.5/acb/adapters/database/sqlalchemy.py
--rw-r--r--   0        0        0     1848 2023-05-27 13:27:44.420088 acb-0.1.5/acb/adapters/database/sqlmodel.py
--rw-r--r--   0        0        0        0 2023-05-27 19:13:35.056779 acb-0.1.5/acb/adapters/debug/__init__.py
--rw-r--r--   0        0        0      471 2023-05-27 21:16:52.557919 acb-0.1.5/acb/adapters/debug/sentry.py
--rw-r--r--   0        0        0     4770 2023-05-27 21:01:37.006314 acb-0.1.5/acb/adapters/dns/cloud_dns.py
--rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.5/acb/adapters/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 20:21:31.954823 acb-0.1.5/acb/adapters/mail/gmail.py
--rw-r--r--   0        0        0     9799 2023-05-27 21:01:36.998525 acb-0.1.5/acb/adapters/mail/mailgun.py
--rw-r--r--   0        0        0        0 2023-05-27 13:39:02.267034 acb-0.1.5/acb/adapters/requests/__init__.py
--rw-r--r--   0        0        0      687 2023-05-27 21:16:18.575095 acb-0.1.5/acb/adapters/requests/httpx.py
--rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.5/acb/adapters/secret/__init__.py
--rw-r--r--   0        0        0     7078 2023-05-27 13:27:14.023615 acb-0.1.5/acb/adapters/secret/google.py
--rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.5/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     4675 2023-04-29 15:06:51.116866 acb-0.1.5/acb/adapters/storage/google.py
--rw-r--r--   0        0        0     6392 2023-04-26 17:21:57.767534 acb-0.1.5/acb/adapters/storage/universal.py
--rw-r--r--   0        0        0     3836 2023-05-27 21:15:49.356733 acb-0.1.5/acb/config.py
--rw-r--r--   0        0        0     3434 2023-05-27 21:16:13.327412 acb-0.1.5/acb/logger.py
--rw-r--r--   0        0        0     1839 2023-05-27 21:19:36.544613 acb-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 acb-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1001 2023-05-27 13:27:12.641564 acb-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 17:02:37.330792 acb-0.1.6/acb/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.6/acb/actions/__init__.py
+-rw-r--r--   0        0        0     3302 2023-06-10 16:40:53.286529 acb-0.1.6/acb/actions/encode.py
+-rw-r--r--   0        0        0      893 2023-05-28 11:01:16.821596 acb-0.1.6/acb/actions/hash.py
+-rw-r--r--   0        0        0       86 2023-06-08 13:59:12.603285 acb-0.1.6/acb/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.6/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1566 2023-05-28 09:13:29.665468 acb-0.1.6/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.6/acb/adapters/database/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-27 21:16:18.244974 acb-0.1.6/acb/adapters/database/redis_om.py
+-rw-r--r--   0        0        0    16633 2023-05-28 11:24:26.304819 acb-0.1.6/acb/adapters/database/sqlalchemy.py
+-rw-r--r--   0        0        0     1848 2023-05-27 13:27:44.420088 acb-0.1.6/acb/adapters/database/sqlmodel.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:13:35.056779 acb-0.1.6/acb/adapters/debug/__init__.py
+-rw-r--r--   0        0        0      471 2023-05-27 21:16:52.557919 acb-0.1.6/acb/adapters/debug/sentry.py
+-rw-r--r--   0        0        0     4764 2023-05-28 09:40:25.073871 acb-0.1.6/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.6/acb/adapters/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:21:31.954823 acb-0.1.6/acb/adapters/mail/gmail.py
+-rw-r--r--   0        0        0     9916 2023-06-01 13:42:09.249464 acb-0.1.6/acb/adapters/mail/mailgun.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:39:02.267034 acb-0.1.6/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-27 21:16:18.575095 acb-0.1.6/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.6/acb/adapters/secrets/__init__.py
+-rw-r--r--   0        0        0     7058 2023-06-08 14:00:12.903726 acb-0.1.6/acb/adapters/secrets/secret_manager.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.6/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     4938 2023-05-28 08:44:28.039395 acb-0.1.6/acb/adapters/storage/cloud_storage.py
+-rw-r--r--   0        0        0     6374 2023-05-28 09:26:16.911587 acb-0.1.6/acb/adapters/storage/universal.py
+-rw-r--r--   0        0        0     4807 2023-06-09 15:16:58.144879 acb-0.1.6/acb/config.py
+-rw-r--r--   0        0        0     3439 2023-06-08 14:34:18.922003 acb-0.1.6/acb/logger.py
+-rw-r--r--   0        0        0     1722 2023-06-10 17:07:28.954622 acb-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 acb-0.1.6/PKG-INFO
```

### Comparing `acb-0.1.5/README.md` & `acb-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `acb-0.1.5/acb/actions/encode.py` & `acb-0.1.6/acb/actions/encode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 import linecache
 import sys
-import tomllib
+import typing as t
 from os import PathLike
 from re import search
+from types import FrameType
 from warnings import warn
 
 import dill as pickle
 import msgspec
-import tomlkit
 from aiopath import AsyncPath
 from blake3 import blake3  # type: ignore
 from itsdangerous import Serializer as SecureSerializer
 
 
 class AcbEncoder:
+    serializers: dict = dict(
+        json=msgspec.json,
+        yaml=msgspec.yaml,
+        msgpack=msgspec.msgpack,
+        pickle=pickle,
+        toml=msgspec.toml,
+    )
+
     def __init__(self) -> None:
-        self.serializers = dict(
-            json=msgspec.json,
-            yaml=msgspec.yaml,
-            msgpack=msgspec.msgpack,
-            pickle=pickle,
-            toml=tomllib,
-        )
         pickle.encode = pickle.dumps
         pickle.decode = pickle.loads
-        tomllib.encode = tomlkit.dumps
-        tomllib.dumps = tomlkit.dumps
-        tomllib.decode = tomllib.loads
         for s in self.serializers.keys():
             setattr(self, s, self.__call__)
 
     async def process(
         self,
         obj: bytes | str | AsyncPath,
         path: AsyncPath,
-        action,
-        serializer,
-        sort_keys,
-        use_list,
+        action: str,
+        serializer: t.Any,
+        # sort_keys: bool,
+        use_list: bool,
         **kwargs,
     ) -> int | bytes:
         if action in ("load", "decode"):
             if serializer is msgspec.msgpack:
-                kwargs.use_list = use_list
+                kwargs["use_list"] = use_list
             if isinstance(obj, AsyncPath):
                 obj = await obj.read_text()
             return serializer.decode(obj, **kwargs)
         elif action in ("dump", "encode"):
-            if serializer is msgspec.yaml:
-                kwargs.sort_keys = sort_keys
+            # if serializer is msgspec.yaml:
+            #     kwargs["sort_keys"] = sort_keys
             data = serializer.encode(obj, **kwargs)
             if isinstance(path, AsyncPath):
-                return await path.write_text(data)
+                return await path.write_bytes(data)
             return data
 
-    def get_vars(self, frame):
+    def get_vars(self, frame: FrameType):
         code_context = linecache.getline(frame.f_code.co_filename, frame.f_lineno)
         calling_method = search("await\s(\w+)\.(\w+)\(", code_context)
         return calling_method.group(1), self.serializers[calling_method.group(2)]
 
     def get_serializer(self, serializer, secret_key, secure_salt):
         secure = secret_key and secure_salt
         return (
@@ -71,16 +69,16 @@
             if secure
             else serializer
         )
 
     async def __call__(
         self,
         obj: str | PathLike | dict,
-        path: AsyncPath | str | None = None,
-        sort_keys: bool = True,
+        path: t.Optional[AsyncPath] = None,
+        # sort_keys: bool = True,
         use_list: bool = False,
         secret_key: str = None,
         secure_salt: str = None,
         **kwargs,
     ) -> dict | bytes:
         # obj = obj if not isinstance(obj, AsyncPath) else AsyncPath(obj)
         # path = AsyncPath(path) if isinstance(path, Path | str) else path
@@ -88,12 +86,18 @@
         if (secret_key and not secure_salt) or (secure_salt and not secret_key):
             warn(
                 f"{serializer} serializer won't sign objects unless both "
                 f"secret_key and secure_salt are set"
             )
         serializer = self.get_serializer(serializer, secret_key, secure_salt)
         return await self.process(
-            obj, path, action, serializer, sort_keys, use_list, **kwargs
+            obj,
+            path,
+            action,
+            serializer,
+            use_list,
+            **kwargs
+            # obj, path, action, serializer, sort_keys, use_list, **kwargs
         )
 
 
 dump = load = encode = decode = AcbEncoder()
```

### Comparing `acb-0.1.5/acb/actions/hash.py` & `acb-0.1.6/acb/actions/hash.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import PathLike
 
 import arrow
 from aiopath import AsyncPath
-from blake3 import blake3 as hash_blake3
+from blake3 import blake3 as hash_blake3  # type: ignore
 from google_crc32c import value as hash_crc32c
 
 
 class Hash:
     @staticmethod
     async def blake3(obj: PathLike | list | bytes | str) -> str:
         if not obj:
```

### Comparing `acb-0.1.5/acb/adapters/cache/redis.py` & `acb-0.1.6/acb/adapters/cache/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class CacheSettings(AppSettings):
     namespace = ac.app.name
     default_timeout = 86400
     template_timeout = 300 if ac.deployed else 1
     media_timeout = 15_768_000
-    media_control = f"max-age={str(media_timeout)} public"
+    media_control = f"max-age={media_timeout} public"
     secret_key = ac.secrets.app_secret_key or None
     secure_salt = ac.secrets.app_secure_salt or None
     host: IPv4Address = ac.secrets.redis_host if ac.deployed else ac.app.localhost
     password: str = ac.secrets.redis_password or ""
     port = 6379
     db = 1
     health_check_interval = 15
```

### Comparing `acb-0.1.5/acb/adapters/database/sqlalchemy.py` & `acb-0.1.6/acb/adapters/database/sqlalchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 from datetime import timedelta
 from functools import lru_cache
 from itertools import chain
 from pathlib import Path
 from re import search
 from typing import Any
 
-# from sqlalchemy.orm.exc import UnmappedInstanceError
-from storage import stor
-
 import arrow
-
-# from re import sub
-# from adapters.database_ import async_session
-from acb.adapters.database.sqlmodel import AppBaseModel
 from acb import ac
 from acb import AppSettings
 from acb import logger
 from acb.actions.debug import apformat
+
+# from re import sub
+# from adapters.database_ import async_session
+from acb.adapters.database.sqlmodel import AppBaseModel
 from aioconsole import ainput
 from aioconsole import aprint
 
+# from sqlalchemy.orm.exc import UnmappedInstanceError
+# from storage import stor
+from aiopath import AsyncPath
+
 # from plugins import plugin_source
 from pydantic import BaseModel
 from sqlalchemy import inspect
 from sqlalchemy import text
 from sqlalchemy.engine import URL
 from sqlalchemy.ext.asyncio import create_async_engine
 
@@ -43,19 +44,21 @@
 from sqlalchemy.pool import NullPool
 from sqlalchemy_utils import create_database
 from sqlalchemy_utils import database_exists
 from sqlalchemy_utils import drop_database
 from sqlmodel import select
 from sqlmodel import SQLModel
 from sqlmodel.ext.asyncio.session import AsyncSession
-
+from pydantic import create_model
 
 # from actions.load import load
 # from resize import clear_resized_images
 
+stor = create_model("Storage", __base__=BaseModel, **dict(db=None))
+
 
 class DatabaseSettings(AppSettings):
     host: str = ac.secrets.database_host if ac.deployed else "127.0.0.1"
     user: str = ac.secrets.database_user
     port = 3306
     async_url: t.Optional[URL]
     url: t.Optional[URL]
@@ -74,14 +77,15 @@
         self.async_url = URL.create(**self.async_url_kwargs)
         self.url_kwargs = dict(drivername="mysql+mysqldb")
         self.url = URL.create(**{**self.async_url_kwargs, **self.url_kwargs})
 
 
 class Database:
     engine: t.Any = None
+
     # session: t.Any = None
 
     async def create(self, demo: bool = False) -> None:
         exists = database_exists(ac.db.url)
         if exists:
             logger.debug("Database exists.")
 
@@ -111,15 +115,15 @@
             logger.info("Database created.")
 
     @lru_cache
     async def get_async_session(self):
         return AsyncSession(self.engine, expire_on_commit=False)
 
     @asynccontextmanager
-    async def session(self) -> AsyncSession:
+    async def session(self) -> t.AsyncGenerator:
         async with self.get_async_session() as sess:
             yield sess
 
     @staticmethod
     def get_table_names(conn):
         inspector = inspect(conn)
         return inspector.get_table_names()
@@ -160,15 +164,15 @@
             if self.get_timestamp(blob.name):
                 yield blob.name
 
     def get_timestamps(self):
         if not self.files:
             self.files = tuple(self.get_files())
 
-        different_timestamps = list()
+        different_timestamps = []
         for name in self.files:
             timestamp = self.get_timestamp(name)
             if timestamp and timestamp not in different_timestamps:
                 different_timestamps.append(timestamp)
         return different_timestamps
 
     def by_timestamp(self, timestamp):
@@ -251,16 +255,16 @@
             )
         )
         diff_as_list = [d for d in self.dates if d not in self.white_list]
         self.black_list.extend(sorted(diff_as_list, reverse=True))
 
 
 class BackupDb(BackupDbDates, BackupDbUtils):
-    do_not_backup = list()
-    models = list()
+    do_not_backup = []
+    models = []
 
     def show(self):
         return [
             m
             for m in SQLModel.metadata.schema
             if isinstance(m, type) and issubclass(m, AppBaseModel)
         ]
@@ -273,15 +277,15 @@
         if model.__subclasses__():
             for submodel in model.__subclasses__():
                 self.add_subclasses(submodel)
         else:
             self.models.append(model)
 
     def get_data(self):
-        data = dict()
+        data = {}
         async with db.session() as session:
             for model in self.get_mapped_classes():
                 query = select(model)
                 results = session.exec(query)
                 data[model.__name__] = sdumps(results)
         return data
 
@@ -304,24 +308,24 @@
         now = arrow.utcnow().int_timestamp
 
         for class_name in data.keys():
             path = self.get_path(class_name, now)
             logger.debug(f"Backing up - {path.name}")
             await self.backup(class_name, data[class_name], now)
 
-    def get_backups(self):
+    async def get_backups(self):
         timestamps = self.get_timestamps()
-        backups = dict()
+        backups = {}
         for timestamp in timestamps:
             adate = arrow.Arrow.fromtimestamp(timestamp)
             date_formatted = adate.humanize()
             backups[timestamp] = []
-            fps = [Path(b) for b in stor.db.list() if timestamp in b.name]
+            fps = [AsyncPath(b) for b in stor.db.list() if timestamp in b.name]
             for fp in fps:
-                if stor.db.exists(fp):
+                if await stor.db.exists(fp):
                     backups[timestamp].append(fp.name)
             adate_formatted = adate.format("MM-DD-YYYY HH:mm:ss ZZ")
             logger.debug(f"{date_formatted} ==> {adate_formatted}:")
         return sorted(backups, reverse=True)
 
     def get_last_backup(self):
         timestamps = self.get_timestamps()
@@ -359,15 +363,16 @@
         #                     with suppress(UnmappedInstanceError):
         #                         self.async_session.merge(row)
         #                     self.async_session.commit()
         #                 except (IntegrityError, InvalidRequestError) as err:
         #                     self.async_session.rollback()
         #                     fails.append(row)
         #             status = "partially" if len(fails) else "totally"
-        #             status = f"\t==> {path.name} {status} restored{':' if len(fails) else '.'}"
+        #             status = f"\t==> {path.name} {status} " \
+        #                      f"restored{':' if len(fails) else '.'}"
         #         else:
         #             status = f"\t!=> No or bad data for {model}."
         #     else:
         #         status = f"\t!=> File {path.name} does not exist."
         # except Exception as err:
         #     status = err
         # return status, fails
@@ -414,38 +419,38 @@
         for timestamp in white_list:
             date_formatted = arrow.Arrow.fromtimestamp(timestamp).humanize()
             logger.debug(f"ID: {timestamp} (from {date_formatted})")
             if ac.debug.database:
                 for f in self.by_timestamp(timestamp):
                     logger.debug(f)
 
-        delete_list = list()
+        delete_list = []
         logger.debug(f"==> {len(black_list)} backups will be deleted:")
         for timestamp in black_list:
             date_formatted = arrow.Arrow.fromtimestamp(timestamp).humanize()
             logger.debug(f"ID: {timestamp} (from {date_formatted})")
             for f in self.by_timestamp(timestamp):
                 if ac.debug.database:
                     logger.debug(f)
                 delete_list.append(f)
 
         self.delete_backups(delete_list)
         return "cleandb"
 
-    def run(self) -> None:
-        if not ac.app.is_deployed:
+    async def run(self) -> None:
+        if not ac.deployed:
             last_backup = self.get_last_backup()
             if ac.debug.database and sure_delete:
                 blobs = [b.name for b in stor.db.list()]
                 for b in blobs:
                     stor.db.delete(b)
                 # clear_resized_images()
                 last_backup = None
             if not last_backup:
-                self.save()
+                await self.save()
             elif last_backup and ac.debug.database and not sure_delete:
                 logger.info(f"Restoring last backup - {last_backup}")
                 self.restore_backup(last_backup)
             self.clean()
             logger.info("Backups complete.")
```

### Comparing `acb-0.1.5/acb/adapters/database/sqlmodel.py` & `acb-0.1.6/acb/adapters/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.5/acb/adapters/dns/cloud_dns.py` & `acb-0.1.6/acb/adapters/dns/cloud_dns.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 splashstand_zone = dns_client.zone("sstand", "splashstand.com.")
 
 
 class DnsRecord(BaseModel):
     name: str = ac.mail_domain
     type: str = "TXT"
     ttl: int = 300
-    rrdata: str | list = ""
+    rrdata: str | list = None
 
 
 class GoogleDNS:
     @staticmethod
     def create_dns_zone() -> None:
         if not dns_zone.exists():
             print(f"Creating gdns zone '{ac.app_name}...")
@@ -48,15 +48,15 @@
             )
             for record in records
         ]
         if ac.debug.dns or ac.debug.mail:
             await apformat(records)
         return records
 
-    def create_dns_records(
+    async def create_dns_records(
         self, records: list | DnsRecord, zone: DnsClient.zone = dns_zone
     ):
         if type(records) == DnsRecord:
             records = [records]
         changes = zone.changes()
         current_record_sets = []
         new_record_sets = []
@@ -95,36 +95,36 @@
                 name=record.name,
                 record_type=record.type,
                 ttl=record.ttl,
                 rrdatas=record.rrdata,
             )
             new_record_sets.append(record_set)
             print(f"Creating - {record}")
-        if len(current_record_sets):
+        if current_record_sets:
             for set in current_record_sets:
                 changes.delete_record_set(set)
             changes.create()  # API request
             print("Deleting record sets", end="")
             while changes.status != "done":
                 print(".", end="")
                 sleep(5)
                 changes.reload()  # API request
-            print("")
+            print()
         changes = zone.changes()
-        if len(new_record_sets):
+        if new_record_sets:
             for set in new_record_sets:
                 changes.add_record_set(set)
             try:
                 changes.create()  # API request
                 print("Creating record sets", end="")
                 while changes.status != "done":
                     print(".", end="")
                     sleep(5)
                     changes.reload()  # API request
-                print("")
+                print()
             except (Conflict, BadRequest) as err:
                 if not changes.additions[0].name.split(".")[1] == "splashstand":
                     raise err
                 print("SplashStand development domain detected. No changes made.")
         else:
             print("No DNS changes detected.")
```

### Comparing `acb-0.1.5/acb/adapters/mail/mailgun.py` & `acb-0.1.6/acb/adapters/mail/mailgun.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+import sys
 import typing as t
 from asyncio import gather
 from pprint import pformat
 from pprint import pprint
 from re import search
 
-from acb import ac
-from acb import AppSettings
-from acb.actions import load
-from acb.adapters.dns.cloud_dns import DnsRecord
-from acb.adapters.dns.cloud_dns import gdns
-from acb.config import inspect_
 from aiopath import AsyncPath
 from httpx import AsyncClient
 from loguru import logger
 from pydantic import BaseModel
+from pydantic import EmailStr
+from pydantic import AnyUrl
+from ..dns.cloud_dns import DnsRecord
+from ..dns.cloud_dns import gdns
+from ... import ac
+from ... import AppSettings
+from ...actions import load
 
 
 class MailSettings(AppSettings):
     # MAIL_USERNAME: str
     # MAIL_PASSWORD: str
     # MAIL_PORT: int = 465
     # MAIL_SERVER: str
@@ -27,26 +29,26 @@
     # MAIL_FROM: EmailStr
     # MAIL_FROM_NAME: Optional[str] = None
     # TEMPLATE_FOLDER: Optional[DirectoryAsyncPath] = None
     # SUPPRESS_SEND: conint(gt=-1, lt=2) = 0  # type: ignore
     # USE_CREDENTIALS: bool = True
     # VALIDATE_CERTS: bool = True
 
-    enabled = (not ac.app.mail_provider == "gmail",)
+    enabled = not ac.app.mail_provider == "gmail"
     debug = ac.debug.mail
-    domain = f"mail@{ac.app.domain}"
-    server = "smpt.mailgun.com"
+    domain: EmailStr = f"mail@{ac.app.domain}"
+    server: AnyUrl = "smtp.mailgun.com"
     port = "587"
     username = f"postmaster@{ac.app.domain}"
     password = ac.secrets.app_mail_password
     api_url = ("https://api.mailgun.net/v3/domains",)
     api_key = (ac.secrets.mailgun_api_key,)
-    default_from = f"info@{ac.app.domain}"
+    default_from: EmailStr = f"info@{ac.app.domain}"
     default_from_name = ac.app.title
-    test_receiver = "email@splashstand.org"
+    test_receiver: EmailStr = None
     tls = True
     ssl = False
     template_folder: t.Optional[AsyncPath]
     gmail = dict(
         enabled=ac.app.mail_provider == "gmail",
         mx_servers=[
             "1 aspmx.l.google.com.",
@@ -72,15 +74,15 @@
     #     MAIL_SSL=False,
     #     TEMPLATE_FOLDER=theme.path / "utility" / "mail",
     # )
 
     async def get_response(
         self, req_type: str, domain=None, data=None, params=None
     ) -> dict:
-        caller = inspect_.calling_function()
+        caller: str = sys._getframe().f_back.f_code.co_name
         match caller:
             case search(caller, "domain"):
                 caller = "domain"
             case search(caller, "route"):
                 caller = "route"
         url = "/".join([ac.mailgun.api_url, caller, domain])
         data = dict(auth=("api", ac.mailgun.api_key), params=params, data=data)
@@ -95,15 +97,15 @@
                 case "post":
                     url = "".join([url, "/connection"])
                     resp = await client.post(url, data=data)
                 case "delete":
                     resp = await client.delete(url)
         if ac.debug.mail:
             print(resp)
-        return load.json(resp.json())
+        return await load.json(resp.json())
 
     async def list_domains(self):
         resp = await self.get_response("get", params={"skip": 0, "limit": 1000})
         domains = [d["name"] for d in resp["items"]]
         return domains
 
     async def get_domain(self, domain):
@@ -182,15 +184,15 @@
             logger.debug(len(resp["items"]))
             logger.debug(pformat(domain_routes))
             logger.debug(len(domain_routes))
 
         return domain_routes
 
     async def delete_route(self, route):
-        with AsyncClient() as client:
+        async with AsyncClient() as client:
             resp = await client.delete("delete", domain={route["id"]})
         logger.info(f"Deleted route for {route['description']}")
         return resp
 
     @staticmethod
     def get_name(address: str):
         name = search("'(.+)@.+", address)
@@ -251,29 +253,27 @@
         resp = await self.get_response("post", data=route)
         logger.info(
             f"Created route for {domain_address}  ==> "
             f" {', '.join(forwarding_addresses)}"
         )
         return resp
 
-
-async def create_routes(self, ordered: bool = True) -> None:
-    if ac.mail.mailgun.gmail.enabled:
-        logger.info("Using gmail mx servers. No routes created.")
-        return
-    else:
-        forwards = await load.yaml(AsyncPath("mail.yml"), ordered=ordered)
-        async for k, v in forwards.items():
-            await self.create_route(k, v)
-
-
-def setup_mail(self) -> bool:
-    self.create_dns_records()
-
-    if not (AsyncPath("mail.yml").exists()):
-        logger.info("No mail routes to configre - mail.yml not found.")
-        return False
-    self.delete_routes(delete_all=False)
-    self.create_routes()
+    async def create_routes(self, ordered: bool = True) -> None:
+        if ac.mail.mailgun.gmail.enabled:
+            logger.info("Using gmail mx servers. No routes created.")
+            return
+        else:
+            forwards = await load.yaml(AsyncPath("mail.yml"), ordered=ordered)
+            async for k, v in forwards.items():
+                await self.create_route(k, v)
+
+    async def setup_mail(self) -> None:
+        await self.create_dns_records()
+
+        if not (AsyncPath("mail.yml").exists()):
+            logger.info("No mail routes to configre - mail.yml not found.")
+            return
+        await self.delete_routes()
+        await self.create_routes()
 
 
 mailgun = Mailgun()
```

### Comparing `acb-0.1.5/acb/adapters/requests/httpx.py` & `acb-0.1.6/acb/adapters/requests/httpx.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.5/acb/adapters/secret/google.py` & `acb-0.1.6/acb/adapters/secrets/secret_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from string import punctuation
 from typing import Any
 from typing import Optional
 from warnings import catch_warnings
 from warnings import filterwarnings
 
 from acb.config import ac
-from acb.adapters.logging.loguru import logger
+from acb.logger import logger
 from aiopath import AsyncPath
 from google.api_core.exceptions import AlreadyExists
 from google.auth import default
 from google.auth.transport.requests import AuthorizedSession
 from google.auth.transport.requests import Request
 from google.cloud.secretmanager import SecretManagerServiceClient
 from google.oauth2.credentials import Credentials
@@ -72,15 +72,15 @@
     creds: Optional[Credentials]
     # target_audience: Optional[str]
     # projects: Optional[list]
     project: Optional[str] = ac.app.project
     # domain: Optional[str] = settings.domain
     prefix: Optional[str] = ac.app.name
     parent: Optional[str] = f"projects/{ac.app.project}"
-    secret_dir: str = ac.tmp / "secrets"
+    secret_dir: AsyncPath = ac.tmp / "secrets"
 
     class Config:
         arbitrary_types_allowed = True
 
     @staticmethod
     def extract_secret_name(secret: str) -> str:
         return Path(secret).parts[-1]
@@ -101,27 +101,27 @@
 
     async def verify_access_token(self, token: str) -> bool:
         verified = compare_digest(self.creds.token, token)
         if ac.debug.secret_manager:
             logger.debug(f"Secrets access token verified - {verified}")
         return verified
 
-    async def list(self):
+    async def list(self) -> list:
         secrets = self.client.list_secrets(request={"parent": self.parent})
         secrets = [self.extract_secret_name(secret.name) for secret in secrets]
-        secrets = [s for s in secrets if s.split("_")[0] in [ac.app.name, "000"]]
+        secrets = [s for s in secrets if s.split("_")[0] in (ac.app.name, "000")]
         # if not deployed and debug.secret_manager:
         #     await apformat(secrets)
         return secrets
 
     async def get(self, name: str) -> str:
         name = self.get_name(name)
         path = f"projects/{self.project}/secrets/{name}/versions/latest"
         version = self.client.access_secret_version(request={"name": path})
-        payload = str(version.payload.data.decode())
+        payload = version.payload.data.decode()
         if not deployed:
             logger.info(f"Fetched secret - {name.removeprefix('000_')}")
         return payload
 
     async def create(self, name: str, value: str) -> None:
         name = self.get_name(name)
         parent = f"projects/{self.project}"
@@ -163,31 +163,29 @@
 
     async def load(self, name: str, secrets, cls_dict) -> str:
         if name not in secrets:
             await self.create(name, cls_dict[name])
         secret = await self.get(name)
         return secret
 
-    async def load_all(self, cls_dict):
+    async def load_all(self, cls_dict) -> dict:
         secrets = await self.list()
         data = {}
-        secret_dir = AsyncPath(self.secret_dir)
-        await secret_dir.mkdir()
+        await self.secret_dir.mkdir(exist_ok=True)
         for name in cls_dict.keys():
             secret = await self.load(name, secrets, cls_dict)
             data[name] = secret
-            secret_path = secret_dir / name
+            secret_path = self.secret_dir / name
             await secret_path.write_text(secret)
         return data
 
-    async def init(self):
+    async def init(self) -> BaseSettings | dict:
         if not await AsyncPath(self.secret_dir).exists():
             return await self.load_all(AppSecrets().dict())
-        else:
-            return AppSecrets(_secrets_dir=self.secret_dir)
+        return AppSecrets(_secrets_dir=self.secret_dir)
 
     def __init__(self) -> None:
         super().__init__()
         self.debug = None
         # self.target_audience = f"https://{self.domain}"
         with catch_warnings():
             filterwarnings("ignore", category=Warning)
```

### Comparing `acb-0.1.5/acb/adapters/storage/google.py` & `acb-0.1.6/acb/adapters/storage/cloud_storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-import typing as t
-from pathlib import Path
-
-from acb.actions.log import logger
-
-from acb.actions.debug import ic
-from acb.config import AppSettings
-
-# from aiologger import Logger
-from acb.config import tmp
-from aiopath import AsyncPath
-from google.cloud.exceptions import NotFound
-from pathy import Pathy
-from pathy import set_client_params
-from pathy import use_fs_cache
-from pydantic import BaseModel
-from pydantic import BaseSettings
-
-
-# from gcloud.aio.storage import Storage
-
-# from google.cloud.storage import Blob
-# from google.cloud.storage import Bucket
-# from actions.compress import compress
-# from actions.compress import decompress
-# from cloudpathlib import CloudPath
-
-
-# Credentials for upload to Cloud Storage
-# CORS policy for upload bucket
-
+# import typing as t
+# from pathlib import Path
 #
-# upload-cors.json
+# from acb.actions.log import logger
 #
-# [
-#     {
-#       "origin": ["*"],
-#       "method": ["*"],
-#       "responseHeader": ["*"],
-#       "maxAgeSeconds": 600
-#     }
-# ]
-
-
-# async with Storage() as client:
-#     ...
-
-
-class StorageSettings(AppSettings):
-    class Bucket(BaseSettings):
-        media = "7e1028ec-569c-4aad-ac5c-824aa56382d6"
-        upload = "3f3a5536-e1d7-430a-a478-39794fa864a3"
-
-    class Cache(BaseSettings):
-        control = ac.cache.media_control
-        timeout = ac.cache.media_timeout
-
-    bucket = Bucket()
-    cache = Cache()
-
-
-class CloudStorageBucket(BaseModel):
-    prefix: str = ac.app.name
-    cache_control: t.Optional[str] = None
-    user_project: str = ac.app.name  # used for billing
-    bucket: t.Optional[str]
-    path: t.Optional[Pathy]
-    logger: Logger = None
-    ic: t.Any = None
-    pf: t.Any = None
-
-    class Config:
-        arbitrary_types_allowed = True
-
-    def __init__(self, bucket: str, prefix: str = None, **data: t.Any) -> None:
-        super().__init__(**data)
-
-    self.prefix = prefix if prefix else self.prefix
-    self.bucket = (
-        f"splashstand-{bucket}"
-        if bucket not in [ac.storage.bucket.media, ac.storage.bucket.upload]
-        else bucket
-    )
-    self.path = Pathy(f"gs://{self.bucket}/{self.prefix}/")
-
-    def save(self, obj_path: AsyncPath, data: t.Any) -> None:
-        self.get_path(obj_path)
-
-    logger.debug(f"Saving {stor_path}...")
-    if isinstance(data, bytes):
-        stor_path.write_bytes(data)
-    else:
-        stor_path.write_text(data)
-    logger.debug(f"Saved - {stor_path}")
-
-    def get(self, obj_path: AsyncPath):
-        stor_path = self.get_path(obj_path)
-        logger.debug(f"Getting {stor_path}...")
-        try:
-            data = stor_path.read_text()
-        except NotFound:
-            raise FileNotFoundError
-        logger.debug(f"Got - {stor_path}")
-        return data
-
-    def stat(self, obj_path: AsyncPath):
-        return self.get_path(obj_path).stat()
-
-    def list(self, dir_path: AsyncPath):
-        return self.get_path(dir_path).rglob("*")
-
-    def exists(self, obj_path: AsyncPath):
-        return self.get_path(obj_path).exists()
-
-    def get_path(self, obj_path: AsyncPath) -> Path:
-        ic(self.path / "/".join(obj_path.parts[1:]))
-        return self.path / "/".join(obj_path.parts[1:])
-
-    async def get_url(self, obj_path: AsyncPath):
-        return str(self.get_path(obj_path).resolve()).replace(
-            "gs://", "https://storage.cloud.google.com/"
-        )
-
-
-class AppStorage:
-    logger: t.Optional[Logger]
-    stock_media = CloudStorageBucket(ac.storage.bucket.media, "stock")
-    media = CloudStorageBucket(ac.storage.bucket.media)
-    upload = CloudStorageBucket(ac.storage.bucket.upload)
-    database = CloudStorageBucket("database")
-    settings = CloudStorageBucket("settings")
-    plugins = CloudStorageBucket("plugins")
-    migrations = CloudStorageBucket("migrations")
-    theme = CloudStorageBucket("theme")
-
-    async def init(self) -> None:
-        set_client_params("gs", project=ac.app.project)
-
-    use_fs_cache(root=tmp / "storage")
-
-    for bucket in [
-        b for b in self.__dict__.values() if isinstance(b, CloudStorageBucket)
-    ]:
-        ic(type(bucket))
-        logger.debug(f"{bucket.__name__.title()} initialized.")
-    logger.info("Storage initialized.")
-
-
-stor = AppStorage()
+# from acb.actions.debug import ic
+# from acb.config import AppSettings
+#
+# # from aiologger import Logger
+# from acb.config import tmp
+# from aiopath import AsyncPath
+# from google.cloud.exceptions import NotFound
+# from pathy import Pathy
+# from pathy import set_client_params
+# from pathy import use_fs_cache
+# from pydantic import BaseModel
+# from pydantic import BaseSettings
+#
+#
+# # from gcloud.aio.storage import Storage
+#
+# # from google.cloud.storage import Blob
+# # from google.cloud.storage import Bucket
+# # from actions.compress import compress
+# # from actions.compress import decompress
+# # from cloudpathlib import CloudPath
+#
+#
+# # Credentials for upload to Cloud Storage
+# # CORS policy for upload bucket
+#
+# #
+# # upload-cors.json
+# #
+# # [
+# #     {
+# #       "origin": ["*"],
+# #       "method": ["*"],
+# #       "responseHeader": ["*"],
+# #       "maxAgeSeconds": 600
+# #     }
+# # ]
+#
+#
+# # async with Storage() as client:
+# #     ...
+#
+#
+# class StorageSettings(AppSettings):
+#     class Bucket(BaseSettings):
+#         media = "7e1028ec-569c-4aad-ac5c-824aa56382d6"
+#         upload = "3f3a5536-e1d7-430a-a478-39794fa864a3"
+#
+#     class Cache(BaseSettings):
+#         control = ac.cache.media_control
+#         timeout = ac.cache.media_timeout
+#
+#     bucket = Bucket()
+#     cache = Cache()
+#
+#
+# class CloudStorageBucket(BaseModel):
+#     prefix: str = ac.app.name
+#     cache_control: t.Optional[str] = None
+#     user_project: str = ac.app.name  # used for billing
+#     bucket: t.Optional[str]
+#     path: t.Optional[Pathy]
+#     logger: Logger = None
+#     ic: t.Any = None
+#     pf: t.Any = None
+#
+#     class Config:
+#         arbitrary_types_allowed = True
+#
+#     def __init__(self, bucket: str, prefix: str = None, **data: t.Any) -> None:
+#         super().__init__(**data)
+#
+#     self.prefix = prefix if prefix else self.prefix
+#     self.bucket = (
+#         f"splashstand-{bucket}"
+#         if bucket not in [ac.storage.bucket.media, ac.storage.bucket.upload]
+#         else bucket
+#     )
+#     self.path = Pathy(f"gs://{self.bucket}/{self.prefix}/")
+#
+#     def save(self, obj_path: AsyncPath, data: t.Any) -> None:
+#         self.get_path(obj_path)
+#
+#     logger.debug(f"Saving {stor_path}...")
+#     if isinstance(data, bytes):
+#         stor_path.write_bytes(data)
+#     else:
+#         stor_path.write_text(data)
+#     logger.debug(f"Saved - {stor_path}")
+#
+#     def get(self, obj_path: AsyncPath):
+#         stor_path = self.get_path(obj_path)
+#         logger.debug(f"Getting {stor_path}...")
+#         try:
+#             data = stor_path.read_text()
+#         except NotFound:
+#             raise FileNotFoundError
+#         logger.debug(f"Got - {stor_path}")
+#         return data
+#
+#     def stat(self, obj_path: AsyncPath):
+#         return self.get_path(obj_path).stat()
+#
+#     def list(self, dir_path: AsyncPath):
+#         return self.get_path(dir_path).rglob("*")
+#
+#     def exists(self, obj_path: AsyncPath):
+#         return self.get_path(obj_path).exists()
+#
+#     def get_path(self, obj_path: AsyncPath) -> Path:
+#         ic(self.path / "/".join(obj_path.parts[1:]))
+#         return self.path / "/".join(obj_path.parts[1:])
+#
+#     async def get_url(self, obj_path: AsyncPath):
+#         return str(self.get_path(obj_path).resolve()).replace(
+#             "gs://", "https://storage.cloud.google.com/"
+#         )
+#
+#
+# class AppStorage:
+#     logger: t.Optional[Logger]
+#     stock_media = CloudStorageBucket(ac.storage.bucket.media, "stock")
+#     media = CloudStorageBucket(ac.storage.bucket.media)
+#     upload = CloudStorageBucket(ac.storage.bucket.upload)
+#     database = CloudStorageBucket("database")
+#     settings = CloudStorageBucket("settings")
+#     plugins = CloudStorageBucket("plugins")
+#     migrations = CloudStorageBucket("migrations")
+#     theme = CloudStorageBucket("theme")
+#
+#     async def init(self) -> None:
+#         set_client_params("gs", project=ac.app.project)
+#
+#     use_fs_cache(root=tmp / "storage")
+#
+#     for bucket in [
+#         b for b in self.__dict__.values() if isinstance(b, CloudStorageBucket)
+#     ]:
+#         ic(type(bucket))
+#         logger.debug(f"{bucket.__name__.title()} initialized.")
+#     logger.info("Storage initialized.")
+#
+#
+# stor = AppStorage()
 
 # return blob(f"{url_pre}/{url_path.name}").public_url
 # return f"https://storage.cloud.google.com/{stor.media.name}/{ac.app_name}/{path}"
 
 
 # CORS policy for upload bucket
 #
```

### Comparing `acb-0.1.5/acb/adapters/storage/universal.py` & `acb-0.1.6/acb/adapters/storage/universal.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
 
     for sep in os.path.sep, os.path.altsep:
         if sep:
             filename = filename.replace(sep, " ")
 
     normalized_filename = _filename_ascii_strip_re.sub("", "_".join(filename.split()))
-    filename = str(normalized_filename).strip("._")
+    filename = normalized_filename.strip("._")
     return filename
 
 
 class BaseStorage:  # pragma: no cover
     def get_name(self, name: str) -> str:
         ...
 
@@ -196,15 +196,15 @@
     """
     Google Cloud Storage backend.
     You might want to use this with the `FileType` type.
     """
 
     def __init__(self, path: str) -> None:
         super().__init__(path)
-        self.bucket = Pathy.from_bucket(self.bucket, scheme="gs")
+        self.bucket = Pathy.from_bucket(self.bucket)
         self._path = self.bucket / self._path
         from google.oauth2 import service_account
 
         _creds = os.environ.get("GCS_CREDENTIALS", "")
         account = service_account.Credentials
         with suppress(TypeError, OSError, FileNotFoundError):
             _creds = Path(_creds).read_text()
```

### Comparing `acb-0.1.5/acb/config.py` & `acb-0.1.6/acb/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,148 @@
 import typing as t
 from importlib import import_module
-from inspect import getargvalues
-from inspect import getmodule
-from inspect import getouterframes
-from inspect import getsourcelines
-from inspect import stack
+from inspect import getsource
+from pprint import pprint
+import sys
 
-from acb.actions import dump
-from acb.actions import load
 from aiopath import AsyncPath
 from inflection import camelize
 from inflection import titleize
 from inflection import underscore
-from pydantic import BaseModel
 from pydantic import BaseSettings
 from pydantic import Extra
+from .actions import dump
+from .actions import load
 
 
 class AppSettings(BaseSettings):
     class Config:
         extra = Extra.allow
         arbitrary_types_allowed = True
 
-    async def __call__(self) -> None:
+    async def __call__(self) -> "AppSettings":
         adapter_name = underscore(self.__class__.__name__.replace("Settings", ""))
         yml_path = ac.settings_path / adapter_name
         if not await yml_path.exists() and not ac.deployed:
-            await dump.yml(self.dict(), yml_path)
-        yml_settings = await load.yml(yml_path)
+            await dump.yaml(self.dict(), yml_path)
+        yml_settings = await load.yaml(yml_path)
         if adapter_name == "debug":
-            app_mods = [path.stem async for path in ac.basedir.rglob("*.py")]
-            all_mods = app_mods + list(ac.app.adapters)
-            for mod in [mod for mod in all_mods if mod not in yml_settings]:
-                yml_settings[mod] = False
+            for adptr in [
+                adptr
+                for adptr in ac.enabled_adapters
+                if adptr not in yml_settings.keys()
+            ]:
+                yml_settings[adptr] = False
         super().__init__(**yml_settings)
+        print(1, yml_settings)
         setattr(ac, adapter_name, self)
         if not ac.deployed:
-            await dump.yml(yml_settings, yml_path)
+            await dump.yaml(yml_settings, yml_path)
+        return self
 
 
 class Debug(AppSettings):
     production = False
     main = False
     logger = False
     database = False
     cache = False
+    mail = False
 
 
 class App(AppSettings):
-    project: str = "acb"
-    name: str = "acb-app"
-    title: str = None
-    adapters: dict = {}
+    project = "acb-project"
+    name = "acb-app"
+    title: t.Optional[str]
+    adapters = {}
 
     def __init__(self, **values: t.Any) -> None:
         super().__init__(**values)
         self.title = self.title or titleize(self.name)
 
 
 class AppConfig(BaseSettings):
-    deployed = False
-    basedir: AsyncPath = None
-    tmp: AsyncPath = "tmp"
-    config_path: AsyncPath = None
-    settings_path: AsyncPath = None
-    debug: Debug = Debug()
-    app: App = App()
+    pkgdir = AsyncPath(__file__).parent
+    deployed: bool = False
+    basedir: t.Optional[AsyncPath]
+    tmp: t.Optional[AsyncPath]
+    config_path: t.Optional[AsyncPath]
+    settings_path: t.Optional[AsyncPath]
+    adapter_categories = []
+    enabled_adapters = []
 
     async def __call__(self, deployed: bool = False) -> None:
         self.basedir = AsyncPath().cwd()
         self.tmp = self.basedir / "tmp"
         self.config_path = self.basedir / "config.py"
         self.settings_path = self.basedir / "settings"
         await self.settings_path.mkdir(exist_ok=True)
+        await self.tmp.mkdir(exist_ok=True)
         self.deployed = True if self.basedir.name == "app" else deployed
         # deployed = True if basedir.name == "srv" else False
         # self.debug = False if deployed else True
         # self.secrets = await SecretManager().init()
-        print(getsourcelines(App))
+        mod_dir = self.basedir / "__pypackages__"
+        sys.path.append(str(mod_dir))
         if not await self.config_path.exists():
             await self.config_path.write_text(
-                f"from acb.config import AppSettings\n\n{getsourcelines(App)}"
+                f"import typing as t\n"
+                f"from inflection import titleize\n"
+                f"from acb.config import AppSettings\n"
+                f"from acb.config import ac\n\n"
+                f"{getsource(App)}"
             )
         # configs = dict()
+        self.app = await App()()
+        print(2, type(self.app), self.app)
         if self.basedir.name != "acb":
             app_settings = import_module("config")
-            await app_settings.App()()
-        await self.debug()
-        for cat, adapter in self.app.adapters:
-            module = import_module(".".join(["acb", "adapters", cat, adapter]))
+            self.app = await app_settings.App()()
+            self.debug = await Debug()()
+            self.adapter_categories = [
+                path.stem
+                async for path in (ac.pkgdir / "adapters").iterdir()
+                if path.is_dir and not path.name.startswith("__")
+            ]
+            print(3, self.adapter_categories)
+            # all_mods = app_mods + list(ac.app.adapters)
+            self.enabled_adapters = [
+                adptr
+                for adptr in self.app.adapters.items()
+                if adptr in self.adapter_categories
+            ]
+            print(4, self.enabled_adapters)
+        for category, adapter in self.app.adapters.items():
+            module = import_module(".".join(["acb", "adapters", category, adapter]))
             adapter_settings = getattr(module, f"{camelize(adapter)}Settings")
             await adapter_settings()()
+        pprint(self.dict())
         # super().__init__(**configs)
 
     class Config:
         extra = "allow"
         arbitrary_types_allowed = False
 
 
 ac = AppConfig()
 
 
-class InspectStack(BaseModel):
-    @staticmethod
-    def calling_function():
-        frm = stack()[2]
-        return AsyncPath(getmodule(frm[0]).__file__).stem
-
-    @staticmethod
-    def calling_page(calling_frame):
-        calling_stack = getouterframes(calling_frame)
-        page = ""
-        for f in calling_stack:
-            if f[3] == "render_template_string":
-                page = getargvalues(f[0]).locals["context"]["page"]
-        return page
+# asyncio.run(ac())
 
 
-inspect_ = InspectStack()
+# class InspectStack(BaseModel):
+#     @staticmethod
+#     def calling_function():
+#         frm = stack()[2]
+#         return AsyncPath(getmodule(frm[0]).__file__).stem
+#
+#     @staticmethod
+#     def calling_page(calling_frame):
+#         calling_stack = getouterframes(calling_frame)
+#         page = ""
+#         for f in calling_stack:
+#             if f[3] == "render_template_string":
+#                 page = getargvalues(f[0]).locals["context"]["page"]
+#         return page
+#
+#
+# inspect_ = InspectStack()
```

### Comparing `acb-0.1.5/acb/logger.py` & `acb-0.1.6/acb/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 from inspect import getmodule
 from inspect import stack
 from pathlib import Path
 from pprint import pformat
 from pprint import pprint
-from time import time
+from time import perf_counter
 
 from acb.config import ac
 from aioconsole import aprint
 from icecream import colorizedStderrPrint
 from icecream import ic
 from loguru import logger
 
@@ -40,17 +40,17 @@
     mod = get_mod()
     if not ac.deployed and not ac.debug.production and ac.debug[mod.name]:
         await aprint(pformat(obj, sort_dicts=sort_dicts))
 
 
 def timeit(func):
     def wrapped(*args, **kwargs):
-        start = time()
+        start = perf_counter()
         result = func(*args, **kwargs)
-        end = time()
+        end = perf_counter()
         logger.debug(f"Function '{func.__name__}' executed in {end - start} s")
         return result
 
     return wrapped
 
 
 class InterceptHandler(logging.Handler):
@@ -102,15 +102,15 @@
             "sqlalchemy.engine",
             "sqlalchemy.orm",
             "sqlalchemy.pool",
             "sqlalchemy.dialects",
         ]
     )
 if ac.debug.cache:
-    _loggers.extend(["starlette_cache", "httpx_caching"])
+    _loggers.extend(["httpx_caching"])
 for _log in _loggers:
     _logger = logging.getLogger(_log)
     _logger.handlers.clear()
     _logger.handlers = [InterceptHandler(_logger.name)]
 
 if ac.debug.logger:
     logger.debug("debug")
```

### Comparing `acb-0.1.5/pyproject.toml` & `acb-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.0",
-    "icecream>=2.1.3",
     "pre-commit>=3.2.2",
     "crackerjack>=0.2.0",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
@@ -23,46 +22,41 @@
 convention = "google"
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
-[tool.mypy]
-strict = false
-pretty = true
-ignore_missing_imports = false
-plugins = [
-    "pydantic.mypy",
-]
-
 [tool.refurb]
 enable_all = true
 
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "acb"
-version = "0.1.5"
+version = "0.1.6"
 description = "Asynchronus Code Base"
 dependencies = [
-    "pydantic>=1.10.7",
     "itsdangerous>=2.1.2",
     "msgspec>=0.14.1",
     "aiopath>=0.6.11",
     "arrow>=1.2.3",
     "google-crc32c>=1.5.0",
     "icecream>=2.1.3",
     "pathy>=0.10.1",
     "dill>=0.3.6",
     "blake3>=0.3.3",
     "python-ulid>=1.1.0",
+    "loguru>=0.7.0",
+    "google-api-core>=2.11.0",
+    "google-cloud-secret-manager>=2.16.1",
+    "pydantic>=2.0b2",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 
@@ -77,34 +71,29 @@
 [project.optional-dependencies]
 cache = [
     "cashews[redis]>=6.0.2",
 ]
 storage = [
     "google-cloud-storage>=2.8.0",
 ]
-secret = [
-    "google-cloud-secret-manager>=2.16.1",
-]
 dns = [
     "google-cloud-dns>=0.34.1",
     "validators>=0.20.0",
 ]
-logging = [
-    "loguru>=0.7.0",
-]
 database = [
-    "sqlmodel>=0.0.8",
     "sqlalchemy>=1.4.41",
     "sqlalchemy-utils>=0.41.1",
-    "redis-om>=0.1.2",
 ]
 requests = [
     "httpx>=0.24.1",
     "httpx-cache>=0.10.0",
 ]
 mail = []
+secrets = [
+    "google-cloud-secret-manager>=2.16.1",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `acb-0.1.5/PKG-INFO` & `acb-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronus Code Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/acb
 Project-URL: Documentation, https://github.com/lesleslie/acb
 Project-URL: Repository, https://github.com/lesleslie/acb
 Requires-Python: >=3.11
-Requires-Dist: pydantic>=1.10.7
 Requires-Dist: itsdangerous>=2.1.2
 Requires-Dist: msgspec>=0.14.1
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: arrow>=1.2.3
 Requires-Dist: google-crc32c>=1.5.0
 Requires-Dist: icecream>=2.1.3
 Requires-Dist: pathy>=0.10.1
 Requires-Dist: dill>=0.3.6
 Requires-Dist: blake3>=0.3.3
 Requires-Dist: python-ulid>=1.1.0
+Requires-Dist: loguru>=0.7.0
+Requires-Dist: google-api-core>=2.11.0
+Requires-Dist: google-cloud-secret-manager>=2.16.1
+Requires-Dist: pydantic>=2.0b2
 Requires-Dist: cashews[redis]>=6.0.2; extra == "cache"
 Requires-Dist: google-cloud-storage>=2.8.0; extra == "storage"
-Requires-Dist: google-cloud-secret-manager>=2.16.1; extra == "secret"
 Requires-Dist: google-cloud-dns>=0.34.1; extra == "dns"
 Requires-Dist: validators>=0.20.0; extra == "dns"
-Requires-Dist: loguru>=0.7.0; extra == "logging"
-Requires-Dist: sqlmodel>=0.0.8; extra == "database"
 Requires-Dist: sqlalchemy>=1.4.41; extra == "database"
 Requires-Dist: sqlalchemy-utils>=0.41.1; extra == "database"
-Requires-Dist: redis-om>=0.1.2; extra == "database"
 Requires-Dist: httpx>=0.24.1; extra == "requests"
 Requires-Dist: httpx-cache>=0.10.0; extra == "requests"
+Requires-Dist: google-cloud-secret-manager>=2.16.1; extra == "secrets"
 Provides-Extra: cache
 Provides-Extra: storage
-Provides-Extra: secret
 Provides-Extra: dns
-Provides-Extra: logging
 Provides-Extra: database
 Provides-Extra: requests
+Provides-Extra: secrets
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://drive.google.com/uc?id=1pMUqyvgMkhGYoLz3jBibZDl3J63HEcCC">
 </p>
 
 # <u>A</u>synchronous <u>C</u>omponent <u>B</u>ase
```

