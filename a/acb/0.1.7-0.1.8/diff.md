# Comparing `tmp/acb-0.1.7.tar.gz` & `tmp/acb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.1.7.tar", last modified: Sat Jun 10 17:25:32 2023, max compression
+gzip compressed data, was "acb-0.1.8.tar", last modified: Sat Jun 10 17:43:24 2023, max compression
```

## Comparing `acb-0.1.7.tar` & `acb-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1001 2023-05-27 13:27:12.641564 acb-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-06-10 17:02:37.330792 acb-0.1.7/acb/__init__.py
--rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.7/acb/actions/__init__.py
--rw-r--r--   0        0        0     3302 2023-06-10 16:40:53.286529 acb-0.1.7/acb/actions/encode.py
--rw-r--r--   0        0        0      893 2023-05-28 11:01:16.821596 acb-0.1.7/acb/actions/hash.py
--rw-r--r--   0        0        0       86 2023-06-08 13:59:12.603285 acb-0.1.7/acb/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.7/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0     1566 2023-05-28 09:13:29.665468 acb-0.1.7/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.7/acb/adapters/database/__init__.py
--rw-r--r--   0        0        0       97 2023-05-27 21:16:18.244974 acb-0.1.7/acb/adapters/database/redis_om.py
--rw-r--r--   0        0        0    16633 2023-05-28 11:24:26.304819 acb-0.1.7/acb/adapters/database/sqlalchemy.py
--rw-r--r--   0        0        0     1848 2023-05-27 13:27:44.420088 acb-0.1.7/acb/adapters/database/sqlmodel.py
--rw-r--r--   0        0        0        0 2023-05-27 19:13:35.056779 acb-0.1.7/acb/adapters/debug/__init__.py
--rw-r--r--   0        0        0      471 2023-05-27 21:16:52.557919 acb-0.1.7/acb/adapters/debug/sentry.py
--rw-r--r--   0        0        0     4764 2023-05-28 09:40:25.073871 acb-0.1.7/acb/adapters/dns/cloud_dns.py
--rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.7/acb/adapters/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 20:21:31.954823 acb-0.1.7/acb/adapters/mail/gmail.py
--rw-r--r--   0        0        0     9916 2023-06-01 13:42:09.249464 acb-0.1.7/acb/adapters/mail/mailgun.py
--rw-r--r--   0        0        0        0 2023-05-27 13:39:02.267034 acb-0.1.7/acb/adapters/requests/__init__.py
--rw-r--r--   0        0        0      687 2023-05-27 21:16:18.575095 acb-0.1.7/acb/adapters/requests/httpx.py
--rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.7/acb/adapters/secrets/__init__.py
--rw-r--r--   0        0        0     7058 2023-06-08 14:00:12.903726 acb-0.1.7/acb/adapters/secrets/secret_manager.py
--rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.7/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     4938 2023-05-28 08:44:28.039395 acb-0.1.7/acb/adapters/storage/cloud_storage.py
--rw-r--r--   0        0        0     6374 2023-05-28 09:26:16.911587 acb-0.1.7/acb/adapters/storage/universal.py
--rw-r--r--   0        0        0     4807 2023-06-09 15:16:58.144879 acb-0.1.7/acb/config.py
--rw-r--r--   0        0        0     3439 2023-06-08 14:34:18.922003 acb-0.1.7/acb/logger.py
--rw-r--r--   0        0        0     1722 2023-06-10 17:25:32.383123 acb-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 acb-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1001 2023-06-10 17:41:43.826515 acb-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 17:02:37.330792 acb-0.1.8/acb/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.8/acb/actions/__init__.py
+-rw-r--r--   0        0        0     3153 2023-06-10 17:42:03.837454 acb-0.1.8/acb/actions/encode.py
+-rw-r--r--   0        0        0      893 2023-05-28 11:01:16.821596 acb-0.1.8/acb/actions/hash.py
+-rw-r--r--   0        0        0       86 2023-06-08 13:59:12.603285 acb-0.1.8/acb/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.8/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1566 2023-06-10 17:27:46.952606 acb-0.1.8/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.8/acb/adapters/database/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-27 21:16:18.244974 acb-0.1.8/acb/adapters/database/redis_om.py
+-rw-r--r--   0        0        0    16594 2023-06-10 17:27:46.947799 acb-0.1.8/acb/adapters/database/sqlalchemy.py
+-rw-r--r--   0        0        0     1848 2023-06-10 17:27:46.961838 acb-0.1.8/acb/adapters/database/sqlmodel.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:13:35.056779 acb-0.1.8/acb/adapters/debug/__init__.py
+-rw-r--r--   0        0        0      472 2023-06-10 17:27:46.956693 acb-0.1.8/acb/adapters/debug/sentry.py
+-rw-r--r--   0        0        0     4764 2023-05-28 09:40:25.073871 acb-0.1.8/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.8/acb/adapters/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:21:31.954823 acb-0.1.8/acb/adapters/mail/gmail.py
+-rw-r--r--   0        0        0     9778 2023-06-10 17:27:46.939885 acb-0.1.8/acb/adapters/mail/mailgun.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:39:02.267034 acb-0.1.8/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-27 21:16:18.575095 acb-0.1.8/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.8/acb/adapters/secrets/__init__.py
+-rw-r--r--   0        0        0     6804 2023-06-10 17:27:46.943788 acb-0.1.8/acb/adapters/secrets/secret_manager.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.8/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     4938 2023-05-28 08:44:28.039395 acb-0.1.8/acb/adapters/storage/cloud_storage.py
+-rw-r--r--   0        0        0     6374 2023-05-28 09:26:16.911587 acb-0.1.8/acb/adapters/storage/universal.py
+-rw-r--r--   0        0        0     4806 2023-06-10 17:27:46.966071 acb-0.1.8/acb/config.py
+-rw-r--r--   0        0        0     3439 2023-06-08 14:34:18.922003 acb-0.1.8/acb/logger.py
+-rw-r--r--   0        0        0     1722 2023-06-10 17:43:24.562914 acb-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 acb-0.1.8/PKG-INFO
```

### Comparing `acb-0.1.7/README.md` & `acb-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `acb-0.1.7/acb/actions/encode.py` & `acb-0.1.8/acb/actions/encode.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,16 +76,14 @@
         path: t.Optional[AsyncPath] = None,
         # sort_keys: bool = True,
         use_list: bool = False,
         secret_key: str = None,
         secure_salt: str = None,
         **kwargs,
     ) -> dict | bytes:
-        # obj = obj if not isinstance(obj, AsyncPath) else AsyncPath(obj)
-        # path = AsyncPath(path) if isinstance(path, Path | str) else path
         action, serializer = self.get_vars(sys._getframe(1))
         if (secret_key and not secure_salt) or (secure_salt and not secret_key):
             warn(
                 f"{serializer} serializer won't sign objects unless both "
                 f"secret_key and secure_salt are set"
             )
         serializer = self.get_serializer(serializer, secret_key, secure_salt)
```

### Comparing `acb-0.1.7/acb/actions/hash.py` & `acb-0.1.8/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.7/acb/adapters/cache/redis.py` & `acb-0.1.8/acb/adapters/cache/redis.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing as t
+from ipaddress import IPv4Address
 
 from acb import ac
 from acb import AppSettings
 from acb.actions import dump
 from acb.actions import load
 from cashews import cache
 from cashews.serialize import register_type
-from ipaddress import IPv4Address
 
 
 class CacheSettings(AppSettings):
     namespace = ac.app.name
     default_timeout = 86400
     template_timeout = 300 if ac.deployed else 1
     media_timeout = 15_768_000
```

### Comparing `acb-0.1.7/acb/adapters/database/sqlalchemy.py` & `acb-0.1.8/acb/adapters/database/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,49 +10,46 @@
 from datetime import timedelta
 from functools import lru_cache
 from itertools import chain
 from pathlib import Path
 from re import search
 from typing import Any
 
+from acb.actions.debug import apformat
+from sqlmodel.ext.asyncio.session import AsyncSession
+
 import arrow
 from acb import ac
 from acb import AppSettings
 from acb import logger
-from acb.actions.debug import apformat
-
 # from re import sub
 # from adapters.database_ import async_session
 from acb.adapters.database.sqlmodel import AppBaseModel
 from aioconsole import ainput
 from aioconsole import aprint
-
 # from sqlalchemy.orm.exc import UnmappedInstanceError
 # from storage import stor
 from aiopath import AsyncPath
-
 # from plugins import plugin_source
 from pydantic import BaseModel
+from pydantic import create_model
 from sqlalchemy import inspect
 from sqlalchemy import text
 from sqlalchemy.engine import URL
 from sqlalchemy.ext.asyncio import create_async_engine
-
 # from sqlalchemy.exc import IntegrityError
 # from sqlalchemy.exc import InvalidRequestError
 from sqlalchemy.ext.serializer import dumps as sdumps
 from sqlalchemy.ext.serializer import loads as sloads
 from sqlalchemy.pool import NullPool
 from sqlalchemy_utils import create_database
 from sqlalchemy_utils import database_exists
 from sqlalchemy_utils import drop_database
 from sqlmodel import select
 from sqlmodel import SQLModel
-from sqlmodel.ext.asyncio.session import AsyncSession
-from pydantic import create_model
 
 # from actions.load import load
 # from resize import clear_resized_images
 
 stor = create_model("Storage", __base__=BaseModel, **dict(db=None))
 
 
@@ -61,42 +58,42 @@
     user: str = ac.secrets.database_user
     port = 3306
     async_url: t.Optional[URL]
     url: t.Optional[URL]
     engine_kwargs = dict(poolclass=NullPool, pool_pre_ping=True)
 
     def __init__(self, **data: t.Any) -> None:
-        super().__init__(**data)
-        self.async_url_kwargs = dict(
-            drivername="mysql+asyncmy",
-            username=ac.secrets.database_user,
-            password=ac.secrets.database_password,
-            port=self.port,
-            host=self.host,
-            database=ac.app.name,
-        )
-        self.async_url = URL.create(**self.async_url_kwargs)
-        self.url_kwargs = dict(drivername="mysql+mysqldb")
-        self.url = URL.create(**{**self.async_url_kwargs, **self.url_kwargs})
+    super().__init__(**data)
+    self.async_url_kwargs = dict(
+        drivername="mysql+asyncmy",
+        username=ac.secrets.database_user,
+        password=ac.secrets.database_password,
+        port=self.port,
+        host=self.host,
+        database=ac.app.name,
+    )
+    self.async_url = URL.create(**self.async_url_kwargs)
+    self.url_kwargs = dict(drivername="mysql+mysqldb")
+    self.url = URL.create(**{**self.async_url_kwargs, **self.url_kwargs})
 
 
 class Database:
     engine: t.Any = None
 
     # session: t.Any = None
 
     async def create(self, demo: bool = False) -> None:
         exists = database_exists(ac.db.url)
         if exists:
             logger.debug("Database exists.")
 
         if (
-            (ac.debug.database or ac.debug.models)
-            and not (ac.app.is_deployed or ac.debug.production)
-            and exists
+                (ac.debug.database or ac.debug.models)
+                and not (ac.app.is_deployed or ac.debug.production)
+                and exists
         ):
             msg = (
                 "\n\nRESETTING THE DATABASE WILL CAUSE ALL OF YOUR"
                 " CURRENT DATA TO BE LOST!\n"
             )
             if demo:
                 msg = (
```

### Comparing `acb-0.1.7/acb/adapters/database/sqlmodel.py` & `acb-0.1.8/acb/adapters/database/sqlmodel.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
-from acb.actions import dump
-from acb.actions import load
-from acb.adapters.database.sqlalchemy import db
 from adapters.firebase import current_user
 
 import arrow
+from acb.actions import dump
+from acb.actions import load
+from acb.adapters.database.sqlalchemy import db
 from inflection import underscore
 from sqlalchemy import Column
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.orm import declared_attr
 from sqlalchemy_utils import ArrowType
 from sqlmodel import Field
 from sqlmodel import SQLModel
```

### Comparing `acb-0.1.7/acb/adapters/dns/cloud_dns.py` & `acb-0.1.8/acb/adapters/dns/cloud_dns.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.7/acb/adapters/mail/mailgun.py` & `acb-0.1.8/acb/adapters/mail/mailgun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import sys
 import typing as t
-from asyncio import gather
 from pprint import pformat
 from pprint import pprint
 from re import search
 
 from aiopath import AsyncPath
 from httpx import AsyncClient
 from loguru import logger
+from pydantic import AnyUrl
 from pydantic import BaseModel
 from pydantic import EmailStr
-from pydantic import AnyUrl
 from ..dns.cloud_dns import DnsRecord
 from ..dns.cloud_dns import gdns
 from ... import ac
 from ... import AppSettings
 from ...actions import load
 
 
@@ -72,15 +71,15 @@
     #     MAIL_FROM="info@{app.domain}",
     #     MAIL_TLS=True,
     #     MAIL_SSL=False,
     #     TEMPLATE_FOLDER=theme.path / "utility" / "mail",
     # )
 
     async def get_response(
-        self, req_type: str, domain=None, data=None, params=None
+            self, req_type: str, domain=None, data=None, params=None
     ) -> dict:
         caller: str = sys._getframe().f_back.f_code.co_name
         match caller:
             case search(caller, "domain"):
                 caller = "domain"
             case search(caller, "route"):
                 caller = "route"
@@ -117,15 +116,15 @@
             data={
                 "name": domain,
                 "smtp_password": ac.mail.password,
                 "web_scheme": "https",
             },
         )
         if ac.debug.mail:
-            logger.debug(resp)
+    logger.debug(resp)
         resp = await self.get_response(
             "put", data={"require_tls": True, "skip_verification": True}
         )
         return resp
 
     async def delete_domain(self, domain):
         return await self.get_response("delete", domain=domain)
@@ -155,39 +154,39 @@
         records.append(record)
         for r in sending_records:
             record = DnsRecord(name=r["name"], type=r["record_type"], rrdata=r["value"])
             records.append(record)
         return records
 
     async def create_dns_records(self) -> None:
-        # if not ac.mail.mailgun.domain in list_domains(self):
-        await self.create_domain(ac.mail.mailgun.domain)
-        await self.create_domain_credentials(ac.mail.mailgun.domain)
-        records = await self.get_dns_records(ac.mail.mailgun.domain)
-        if ac.mail.mailgun.gmail.enabled:
-            await self.delete_domain(ac.mail.mailgun.domain)
-            rrdata = ac.mail.gmail.mx_servers
-            record = DnsRecord(name=ac.mail.mailgun.domain, type="MX", rrdata=rrdata)
-            records.append(record)
-        else:
-            await self.delete_domain(ac.mail.mailgun.domain)
-        if ac.debug.mail:
-            pprint(records)
+    # if not ac.mail.mailgun.domain in list_domains(self):
+    await self.create_domain(ac.mail.mailgun.domain)
+    await self.create_domain_credentials(ac.mail.mailgun.domain)
+    records = await self.get_dns_records(ac.mail.mailgun.domain)
+    if ac.mail.mailgun.gmail.enabled:
+        await self.delete_domain(ac.mail.mailgun.domain)
+        rrdata = ac.mail.gmail.mx_servers
+        record = DnsRecord(name=ac.mail.mailgun.domain, type="MX", rrdata=rrdata)
+        records.append(record)
+    else:
+        await self.delete_domain(ac.mail.mailgun.domain)
+    if ac.debug.mail:
+        pprint(records)
         await gdns.create_dns_records(records)
 
     async def list_routes(self):
         resp = await self.get_response("get", params={"skip": 0, "limit": 1000})
         domain_routes = [
             r for r in resp["items"] if ac.mail.mailgun.domain in r["expression"]
         ]
         if ac.debug.mail:
-            logger.debug(pformat(resp["items"]))
-            logger.debug(len(resp["items"]))
-            logger.debug(pformat(domain_routes))
-            logger.debug(len(domain_routes))
+    logger.debug(pformat(resp["items"]))
+    logger.debug(len(resp["items"]))
+    logger.debug(pformat(domain_routes))
+    logger.debug(len(domain_routes))
 
         return domain_routes
 
     async def delete_route(self, route):
         async with AsyncClient() as client:
             resp = await client.delete("delete", domain={route["id"]})
         logger.info(f"Deleted route for {route['description']}")
@@ -209,30 +208,30 @@
             pprint(deletes)
         for f in forwards:
             fs = [r for r in routes if self.get_name(r["expression"]) == f]
             deletes.extend(fs[1:])
         if delete_all or ac.mail.mailgun.gmail.enabled:
             deletes = [r for r in routes if len(self.get_name(r["expression"]))]
         if ac.debug.mail:
-            pprint(deletes)
-            print(len(deletes))
+    pprint(deletes)
+    print(len(deletes))
         else:
             for d in deletes:
                 await self.delete_route(d)
 
     async def create_route(self, domain_address, forwarding_addresses):
         domain_address = f"{domain_address}@{ac.mail.mailgun.domain}"
         if not isinstance(forwarding_addresses, list):
             forwarding_addresses = [forwarding_addresses]
         actions = ["stop(self)"]
 
         for addr in forwarding_addresses:
             actions.insert(0, f"forward('{addr}')")
         if ac.debug.mail:
-            print(actions)
+    print(actions)
         route = {
             "priority": 0,
             "description": domain_address,
             "expression": f"match_recipient('{domain_address}')",
             "action": actions,
         }
         routes = await self.list_routes()
@@ -262,14 +261,15 @@
             logger.info("Using gmail mx servers. No routes created.")
             return
         else:
             forwards = await load.yaml(AsyncPath("mail.yml"), ordered=ordered)
             async for k, v in forwards.items():
                 await self.create_route(k, v)
 
+
     async def setup_mail(self) -> None:
         await self.create_dns_records()
 
         if not (AsyncPath("mail.yml").exists()):
             logger.info("No mail routes to configre - mail.yml not found.")
             return
         await self.delete_routes()
```

### Comparing `acb-0.1.7/acb/adapters/requests/httpx.py` & `acb-0.1.8/acb/adapters/requests/httpx.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.7/acb/adapters/secrets/secret_manager.py` & `acb-0.1.8/acb/adapters/secrets/secret_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from contextlib import suppress
 from pathlib import Path
 from random import choice
 from secrets import compare_digest
 from secrets import token_bytes
 from secrets import token_urlsafe
 from string import ascii_letters
 from string import digits
@@ -11,15 +10,14 @@
 from typing import Optional
 from warnings import catch_warnings
 from warnings import filterwarnings
 
 from acb.config import ac
 from acb.logger import logger
 from aiopath import AsyncPath
-from google.api_core.exceptions import AlreadyExists
 from google.auth import default
 from google.auth.transport.requests import AuthorizedSession
 from google.auth.transport.requests import Request
 from google.cloud.secretmanager import SecretManagerServiceClient
 from google.oauth2.credentials import Credentials
 from pydantic import BaseSettings
 
@@ -56,15 +54,15 @@
     recaptcha_dev_key: Optional[str]
     recaptcha_production_key: Optional[str]
     app_secret_key = token_urlsafe(32)
     app_secure_salt: Optional[str] = str(token_bytes(32))
     app_mail_password: Optional[str] = gen_password(10)
 
     def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
+    super().__init__(**data)
 
     class Config:
         extra = "forbid"
 
 
 class SecretManager:
     client: Optional[SecretManagerServiceClient]
@@ -92,84 +90,84 @@
             else f"000_{name}"
         )
         return name
 
     async def get_access_token(self) -> str:
         self.creds.refresh(Request())
         if ac.debug.secret_manager:
-            logger.debug(f"Secrets access token:\n{self.creds.token}")
+    logger.debug(f"Secrets access token:\n{self.creds.token}")
         return self.creds.token
 
     async def verify_access_token(self, token: str) -> bool:
         verified = compare_digest(self.creds.token, token)
         if ac.debug.secret_manager:
-            logger.debug(f"Secrets access token verified - {verified}")
+    logger.debug(f"Secrets access token verified - {verified}")
         return verified
 
     async def list(self) -> list:
-        secrets = self.client.list_secrets(request={"parent": self.parent})
-        secrets = [self.extract_secret_name(secret.name) for secret in secrets]
-        secrets = [s for s in secrets if s.split("_")[0] in (ac.app.name, "000")]
-        # if not deployed and debug.secret_manager:
-        #     await apformat(secrets)
-        return secrets
+    secrets = self.client.list_secrets(request={"parent": self.parent})
+    secrets = [self.extract_secret_name(secret.name) for secret in secrets]
+    secrets = [s for s in secrets if s.split("_")[0] in (ac.app.name, "000")]
+    # if not deployed and debug.secret_manager:
+    #     await apformat(secrets)
+    return secrets
 
     async def get(self, name: str) -> str:
         name = self.get_name(name)
         path = f"projects/{self.project}/secrets/{name}/versions/latest"
         version = self.client.access_secret_version(request={"name": path})
         payload = version.payload.data.decode()
         if not deployed:
             logger.info(f"Fetched secret - {name.removeprefix('000_')}")
         return payload
 
     async def create(self, name: str, value: str) -> None:
-        name = self.get_name(name)
-        parent = f"projects/{self.project}"
-        with suppress(AlreadyExists):
-            version = self.client.create_secret(
-                request={
-                    "parent": parent,
-                    "secret_id": name,
-                    "secret": {"replication": {"automatic": {}}},
-                }
-            )
+    name = self.get_name(name)
+    parent = f"projects/{self.project}"
+    with suppress(AlreadyExists):
+        version = self.client.create_secret(
+            request={
+                "parent": parent,
+                "secret_id": name,
+                "secret": {"replication": {"automatic": {}}},
+            }
+        )
             self.client.add_secret_version(
                 request={
                     "parent": version.name,
                     "payload": {"data": f"{value}".encode()},
                 }
             )
             if not deployed:
                 logger.debug(f"Created secret - {name}")
 
     async def update(self, name: str, value: str) -> None:
-        name = self.get_name(name)
-        secret = self.client.secret_path(self.project, name)
-        self.client.add_secret_version(
-            request={
-                "parent": secret,
-                "payload": {"data": f"{value}".encode()},
-            }
-        )
-        if not deployed:
-            logger.debug(f"Updated secret - {name}")
+    name = self.get_name(name)
+    secret = self.client.secret_path(self.project, name)
+    self.client.add_secret_version(
+        request={
+            "parent": secret,
+            "payload": {"data": f"{value}".encode()},
+        }
+    )
+    if not deployed:
+        logger.debug(f"Updated secret - {name}")
 
     async def delete(self, name: str) -> None:
-        name = self.get_name(name)
-        secret = self.client.secret_path(self.project, name)
-        self.client.delete_secret(request={"name": secret})
-        if not deployed:
-            logger.debug(f"Deleted secret - {secret}")
+    name = self.get_name(name)
+    secret = self.client.secret_path(self.project, name)
+    self.client.delete_secret(request={"name": secret})
+    if not deployed:
+        logger.debug(f"Deleted secret - {secret}")
 
     async def load(self, name: str, secrets, cls_dict) -> str:
-        if name not in secrets:
-            await self.create(name, cls_dict[name])
-        secret = await self.get(name)
-        return secret
+    if name not in secrets:
+        await self.create(name, cls_dict[name])
+    secret = await self.get(name)
+    return secret
 
     async def load_all(self, cls_dict) -> dict:
         secrets = await self.list()
         data = {}
         await self.secret_dir.mkdir(exist_ok=True)
         for name in cls_dict.keys():
             secret = await self.load(name, secrets, cls_dict)
@@ -191,11 +189,10 @@
             filterwarnings("ignore", category=Warning)
             creds, projects = default()
         self.creds = creds
         self.projects = projects
         self.client = SecretManagerServiceClient(credentials=self.creds)
         self.authed_session = AuthorizedSession(self.creds)
         if ac.debug.secret:
-            Path(secret_dir).rmdir()
-
+    Path(secret_dir).rmdir()
 
 # secret_manager = SecretManager()
```

### Comparing `acb-0.1.7/acb/adapters/storage/cloud_storage.py` & `acb-0.1.8/acb/adapters/storage/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.7/acb/adapters/storage/universal.py` & `acb-0.1.8/acb/adapters/storage/universal.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.7/acb/config.py` & `acb-0.1.8/acb/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import sys
 import typing as t
 from importlib import import_module
 from inspect import getsource
 from pprint import pprint
-import sys
 
 from aiopath import AsyncPath
 from inflection import camelize
 from inflection import titleize
 from inflection import underscore
 from pydantic import BaseSettings
 from pydantic import Extra
@@ -121,15 +121,14 @@
     class Config:
         extra = "allow"
         arbitrary_types_allowed = False
 
 
 ac = AppConfig()
 
-
 # asyncio.run(ac())
 
 
 # class InspectStack(BaseModel):
 #     @staticmethod
 #     def calling_function():
 #         frm = stack()[2]
```

### Comparing `acb-0.1.7/acb/logger.py` & `acb-0.1.8/acb/logger.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.7/pyproject.toml` & `acb-0.1.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "acb"
-version = "0.1.7"
+version = "0.1.8"
 description = "Asynchronus Code Base"
 dependencies = [
     "itsdangerous>=2.1.2",
     "msgspec>=0.14.1",
     "aiopath>=0.6.11",
     "arrow>=1.2.3",
     "google-crc32c>=1.5.0",
```

### Comparing `acb-0.1.7/PKG-INFO` & `acb-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.1.7
+Version: 0.1.8
 Summary: Asynchronus Code Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/acb
 Project-URL: Documentation, https://github.com/lesleslie/acb
 Project-URL: Repository, https://github.com/lesleslie/acb
 Requires-Python: >=3.11
```

