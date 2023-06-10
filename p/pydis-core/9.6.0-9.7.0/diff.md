# Comparing `tmp/pydis_core-9.6.0.tar.gz` & `tmp/pydis_core-9.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydis_core-9.6.0.tar", max compression
+gzip compressed data, was "pydis_core-9.7.0.tar", max compression
```

## Comparing `pydis_core-9.6.0.tar` & `pydis_core-9.7.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1071 2022-03-31 15:49:16.729733 pydis_core-9.6.0/LICENSE
--rw-r--r--   0        0        0      331 2023-02-09 21:50:49.567310 pydis_core-9.6.0/pydis_core/__init__.py
--rw-r--r--   0        0        0    11450 2023-05-06 12:14:38.832461 pydis_core-9.6.0/pydis_core/_bot.py
--rw-r--r--   0        0        0     1917 2023-02-09 21:50:49.567310 pydis_core-9.6.0/pydis_core/async_stats.py
--rw-r--r--   0        0        0      104 2022-11-05 14:18:24.787185 pydis_core-9.6.0/pydis_core/exts/__init__.py
--rw-r--r--   0        0        0     6349 2023-02-09 21:50:49.609519 pydis_core-9.6.0/pydis_core/site_api.py
--rw-r--r--   0        0        0     1314 2023-02-09 21:50:49.609519 pydis_core-9.6.0/pydis_core/utils/__init__.py
--rw-r--r--   0        0        0     1680 2022-11-05 14:18:24.788185 pydis_core-9.6.0/pydis_core/utils/_extensions.py
--rw-r--r--   0        0        0     2740 2022-11-05 14:18:24.789186 pydis_core-9.6.0/pydis_core/utils/_monkey_patches.py
--rw-r--r--   0        0        0     1810 2022-11-05 14:18:24.789186 pydis_core-9.6.0/pydis_core/utils/caching.py
--rw-r--r--   0        0        0     1705 2023-02-09 21:50:49.610663 pydis_core-9.6.0/pydis_core/utils/channel.py
--rw-r--r--   0        0        0     1521 2022-11-05 14:18:24.790186 pydis_core-9.6.0/pydis_core/utils/commands.py
--rw-r--r--   0        0        0     7725 2023-02-09 21:50:49.667635 pydis_core-9.6.0/pydis_core/utils/cooldown.py
--rw-r--r--   0        0        0     4267 2022-11-11 15:00:18.292347 pydis_core-9.6.0/pydis_core/utils/function.py
--rw-r--r--   0        0        0     4468 2023-02-09 21:50:49.674633 pydis_core-9.6.0/pydis_core/utils/interactions.py
--rw-r--r--   0        0        0     1432 2022-11-06 00:01:44.084076 pydis_core-9.6.0/pydis_core/utils/logging.py
--rw-r--r--   0        0        0     1995 2023-02-09 21:50:49.689686 pydis_core-9.6.0/pydis_core/utils/members.py
--rw-r--r--   0        0        0     2397 2022-11-05 14:18:24.793186 pydis_core-9.6.0/pydis_core/utils/regex.py
--rw-r--r--   0        0        0    10227 2023-02-09 21:50:49.689686 pydis_core-9.6.0/pydis_core/utils/scheduling.py
--rw-r--r--   0        0        0     2196 2023-05-06 12:14:38.832461 pydis_core-9.6.0/pyproject.toml
--rw-r--r--   0        0        0      120 2022-05-31 19:45:29.494670 pydis_core-9.6.0/README.md
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 pydis_core-9.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-03-31 15:49:16.729733 pydis_core-9.7.0/LICENSE
+-rw-r--r--   0        0        0      320 2023-06-10 18:44:50.836639 pydis_core-9.7.0/pydis_core/__init__.py
+-rw-r--r--   0        0        0    11394 2023-06-10 18:44:50.836639 pydis_core-9.7.0/pydis_core/_bot.py
+-rw-r--r--   0        0        0     1886 2023-06-10 18:44:50.837639 pydis_core-9.7.0/pydis_core/async_stats.py
+-rw-r--r--   0        0        0       93 2023-06-10 18:44:50.837639 pydis_core-9.7.0/pydis_core/exts/__init__.py
+-rw-r--r--   0        0        0     6309 2023-06-10 18:44:50.837639 pydis_core-9.7.0/pydis_core/site_api.py
+-rw-r--r--   0        0        0     1336 2023-06-10 18:49:04.940072 pydis_core-9.7.0/pydis_core/utils/__init__.py
+-rw-r--r--   0        0        0     1680 2022-11-05 14:18:24.788185 pydis_core-9.7.0/pydis_core/utils/_extensions.py
+-rw-r--r--   0        0        0     2749 2023-06-10 18:44:50.838639 pydis_core-9.7.0/pydis_core/utils/_monkey_patches.py
+-rw-r--r--   0        0        0     1810 2022-11-05 14:18:24.789186 pydis_core-9.7.0/pydis_core/utils/caching.py
+-rw-r--r--   0        0        0     1705 2023-06-04 20:04:18.921646 pydis_core-9.7.0/pydis_core/utils/channel.py
+-rw-r--r--   0        0        0     1490 2023-06-10 18:44:50.839639 pydis_core-9.7.0/pydis_core/utils/commands.py
+-rw-r--r--   0        0        0     7740 2023-06-10 18:44:50.839639 pydis_core-9.7.0/pydis_core/utils/cooldown.py
+-rw-r--r--   0        0        0     1253 2023-06-10 18:49:04.941072 pydis_core-9.7.0/pydis_core/utils/error_handling.py
+-rw-r--r--   0        0        0     4253 2023-06-10 18:44:50.839639 pydis_core-9.7.0/pydis_core/utils/function.py
+-rw-r--r--   0        0        0     4465 2023-06-10 18:44:50.840639 pydis_core-9.7.0/pydis_core/utils/interactions.py
+-rw-r--r--   0        0        0     1422 2023-06-10 18:44:50.840639 pydis_core-9.7.0/pydis_core/utils/logging.py
+-rw-r--r--   0        0        0     1985 2023-06-10 18:44:50.840639 pydis_core-9.7.0/pydis_core/utils/members.py
+-rw-r--r--   0        0        0     3958 2023-06-10 18:44:50.841639 pydis_core-9.7.0/pydis_core/utils/paste_service.py
+-rw-r--r--   0        0        0     2397 2022-11-05 14:18:24.793186 pydis_core-9.7.0/pydis_core/utils/regex.py
+-rw-r--r--   0        0        0    10730 2023-06-10 18:49:04.941072 pydis_core-9.7.0/pydis_core/utils/scheduling.py
+-rw-r--r--   0        0        0     2872 2023-06-10 18:48:16.993938 pydis_core-9.7.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2022-05-31 19:45:29.494670 pydis_core-9.7.0/README.md
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pydis_core-9.7.0/PKG-INFO
```

### Comparing `pydis_core-9.6.0/LICENSE` & `pydis_core-9.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydis_core-9.6.0/pydis_core/_bot.py` & `pydis_core-9.7.0/pydis_core/_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import socket
 import types
 import warnings
 from contextlib import suppress
-from typing import Optional
 
 import aiohttp
 import discord
 from discord.ext import commands
 
 from pydis_core.async_stats import AsyncStatsClient
 from pydis_core.site_api import APIClient
@@ -15,15 +14,15 @@
 from pydis_core.utils._extensions import walk_extensions
 from pydis_core.utils.logging import get_logger
 
 try:
     from async_rediscache import RedisSession
     REDIS_AVAILABLE = True
 except ImportError:
-    RedisSession = None
+    RedisSession = object
     REDIS_AVAILABLE = False
 
 log = get_logger()
 
 
 class StartupError(Exception):
     """Exception class for startup errors."""
@@ -38,17 +37,17 @@
 
     def __init__(
         self,
         *args,
         guild_id: int,
         allowed_roles: list,
         http_session: aiohttp.ClientSession,
-        redis_session: Optional[RedisSession] = None,
-        api_client: Optional[APIClient] = None,
-        statsd_url: Optional[str] = None,
+        redis_session: RedisSession | None = None,
+        api_client: APIClient | None = None,
+        statsd_url: str | None = None,
         **kwargs,
     ):
         """
         Initialise the base bot instance.
 
         Args:
             guild_id: The ID of the guild used for :func:`wait_until_guild_available`.
@@ -73,24 +72,24 @@
         self.statsd_url = statsd_url
 
         if redis_session and not REDIS_AVAILABLE:
             warnings.warn("redis_session kwarg passed, but async-rediscache not installed!", stacklevel=2)
         elif redis_session:
             self.redis_session = redis_session
 
-        self._resolver: Optional[aiohttp.AsyncResolver] = None
-        self._connector: Optional[aiohttp.TCPConnector] = None
+        self._resolver: aiohttp.AsyncResolver | None = None
+        self._connector: aiohttp.TCPConnector | None = None
 
-        self._statsd_timerhandle: Optional[asyncio.TimerHandle] = None
-        self._guild_available: Optional[asyncio.Event] = None
+        self._statsd_timerhandle: asyncio.TimerHandle | None = None
+        self._guild_available: asyncio.Event | None = None
         self._extension_loading_task: asyncio.Task | None = None
 
-        self.stats: Optional[AsyncStatsClient] = None
+        self.stats: AsyncStatsClient | None = None
 
-        self.all_extensions: Optional[frozenset[str]] = None
+        self.all_extensions: frozenset[str] | None = None
 
     def _connect_statsd(
         self,
         statsd_url: str,
         loop: asyncio.AbstractEventLoop,
         retry_after: int = 2,
         attempt: int = 1
@@ -115,15 +114,15 @@
                 statsd_url,
                 retry_after * 2,
                 attempt + 1
             )
 
     async def _load_extensions(self, module: types.ModuleType) -> None:
         """Load all the extensions within the given module and save them to ``self.all_extensions``."""
-        log.info("Waiting for guild %d to be avialable before loading extensions.", self.guild_id)
+        log.info("Waiting for guild %d to be available before loading extensions.", self.guild_id)
 
         await self.wait_until_guild_available()
         log.info("Loading extensions...")
         self.all_extensions = walk_extensions(module)
 
         for extension in self.all_extensions:
             scheduling.create_task(self.load_extension(extension))
@@ -172,15 +171,15 @@
         log.info(f"Cog loaded: {cog.qualified_name}")
 
     def add_command(self, command: commands.Command) -> None:
         """Add ``command`` as normal and then add its root aliases to the bot."""
         super().add_command(command)
         self._add_root_aliases(command)
 
-    def remove_command(self, name: str) -> Optional[commands.Command]:
+    def remove_command(self, name: str) -> commands.Command | None:
         """
         Remove a command/alias as normal and then remove its root aliases from the bot.
 
         Individual root aliases cannot be removed by this function.
         To remove them, either remove the entire command or manually edit `bot.all_commands`.
         """
         command = super().remove_command(name)
```

### Comparing `pydis_core-9.6.0/pydis_core/async_stats.py` & `pydis_core-9.7.0/pydis_core/async_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """An async transport method for statsd communication."""
 
 import asyncio
 import socket
-from typing import Optional
 
 from statsd.client.base import StatsClientBase
 
 from pydis_core.utils import scheduling
 
 
 class AsyncStatsClient(StatsClientBase):
     """An async implementation of :obj:`statsd.client.base.StatsClientBase` that supports async stat communication."""
 
     def __init__(
         self,
         loop: asyncio.AbstractEventLoop,
-        host: str = 'localhost',
+        host: str = "localhost",
         port: int = 8125,
         prefix: str = None
     ):
         """
         Create a new :obj:`AsyncStatsClient`.
 
         Args:
@@ -31,15 +30,15 @@
         """
         _, _, _, _, addr = socket.getaddrinfo(
             host, port, socket.AF_INET, socket.SOCK_DGRAM
         )[0]
         self._addr = addr
         self._prefix = prefix
         self._loop = loop
-        self._transport: Optional[asyncio.DatagramTransport] = None
+        self._transport: asyncio.DatagramTransport | None = None
 
     async def create_socket(self) -> None:
         """Use :obj:`asyncio.loop.create_datagram_endpoint` from the loop given on init to create a socket."""
         self._transport, _ = await self._loop.create_datagram_endpoint(
             asyncio.DatagramProtocol,
             family=socket.AF_INET,
             remote_addr=self._addr
@@ -47,11 +46,11 @@
 
     def _send(self, data: str) -> None:
         """Start an async task to send data to statsd."""
         scheduling.create_task(self._async_send(data), event_loop=self._loop)
 
     async def _async_send(self, data: str) -> None:
         """Send data to the statsd server using the async transport."""
-        self._transport.sendto(data.encode('ascii'), self._addr)
+        self._transport.sendto(data.encode("ascii"), self._addr)
 
 
-__all__ = ['AsyncStatsClient']
+__all__ = ["AsyncStatsClient"]
```

### Comparing `pydis_core-9.6.0/pydis_core/site_api.py` & `pydis_core-9.7.0/pydis_core/site_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """An API wrapper around the Site API."""
 
 import asyncio
-from typing import Optional
 from urllib.parse import quote as quote_url
 
 import aiohttp
 
 from pydis_core.utils.logging import get_logger
 
 log = get_logger(__name__)
@@ -13,16 +12,16 @@
 
 class ResponseCodeError(ValueError):
     """Raised in :meth:`APIClient.request` when a non-OK HTTP response is received."""
 
     def __init__(
         self,
         response: aiohttp.ClientResponse,
-        response_json: Optional[dict] = None,
-        response_text: Optional[str] = None
+        response_json: dict | None = None,
+        response_text: str | None = None
     ):
         """
         Initialize a new :obj:`ResponseCodeError` instance.
 
         Args:
             response (:obj:`aiohttp.ClientResponse`): The response object from the request.
             response_json: The JSON response returned from the request, if any.
@@ -38,36 +37,36 @@
         response = self.response_json or self.response_text
         return f"Status: {self.status} Response: {response}"
 
 
 class APIClient:
     """A wrapper for the Django Site API."""
 
-    session: Optional[aiohttp.ClientSession] = None
+    session: aiohttp.ClientSession | None = None
     loop: asyncio.AbstractEventLoop = None
 
     def __init__(self, site_api_url: str, site_api_token: str, **session_kwargs):
         """
         Initialize a new :obj:`APIClient` instance.
 
         Args:
             site_api_url: The URL of the site API.
             site_api_token: The token to use for authentication.
             session_kwargs: Keyword arguments to pass to the :obj:`aiohttp.ClientSession` constructor.
         """
         self.site_api_url = site_api_url
 
         auth_headers = {
-            'Authorization': f"Token {site_api_token}"
+            "Authorization": f"Token {site_api_token}"
         }
 
-        if 'headers' in session_kwargs:
-            session_kwargs['headers'].update(auth_headers)
+        if "headers" in session_kwargs:
+            session_kwargs["headers"].update(auth_headers)
         else:
-            session_kwargs['headers'] = auth_headers
+            session_kwargs["headers"] = auth_headers
 
         # aiohttp will complain if APIClient gets instantiated outside a coroutine. Thankfully, we
         # don't and shouldn't need to do that, so we can avoid scheduling a task to create it.
         self.session = aiohttp.ClientSession(**session_kwargs)
 
     def _url_for(self, endpoint: str) -> str:
         return f"{self.site_api_url}/{quote_url(endpoint)}"
@@ -130,15 +129,15 @@
         """Equivalent to :meth:`APIClient.request` with POST passed as the method."""
         return await self.request("POST", endpoint, raise_for_status=raise_for_status, **kwargs)
 
     async def put(self, endpoint: str, *, raise_for_status: bool = True, **kwargs) -> dict:
         """Equivalent to :meth:`APIClient.request` with PUT passed as the method."""
         return await self.request("PUT", endpoint, raise_for_status=raise_for_status, **kwargs)
 
-    async def delete(self, endpoint: str, *, raise_for_status: bool = True, **kwargs) -> Optional[dict]:
+    async def delete(self, endpoint: str, *, raise_for_status: bool = True, **kwargs) -> dict | None:
         """
         Send a DELETE request to the site API and return the JSON response.
 
         Args:
             endpoint: The endpoint to send the request to.
             raise_for_status: Whether or not to raise an exception if the response is not OK.
             **kwargs: Any extra keyword arguments to pass to :func:`aiohttp.request`.
@@ -150,8 +149,8 @@
             if resp.status == 204:
                 return None
 
             await self.maybe_raise_for_status(resp, raise_for_status)
             return await resp.json()
 
 
-__all__ = ['APIClient', 'ResponseCodeError']
+__all__ = ["APIClient", "ResponseCodeError"]
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/__init__.py` & `pydis_core-9.7.0/pydis_core/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 """Useful utilities and tools for Discord bot development."""
 
 from pydis_core.utils import (
-    _monkey_patches,
-    caching,
-    channel,
-    commands,
-    cooldown,
-    function,
-    interactions,
-    logging,
-    members,
-    regex,
-    scheduling,
+    _monkey_patches, caching, channel, commands, cooldown, error_handling, function, interactions, logging, members,
+    paste_service, regex, scheduling
 )
 from pydis_core.utils._extensions import unqualify
 
 
 def apply_monkey_patches() -> None:
     """
     Applies all common monkey patches for our bots.
@@ -34,17 +25,19 @@
 
 __all__ = [
     apply_monkey_patches,
     caching,
     channel,
     commands,
     cooldown,
+    error_handling,
     function,
     interactions,
     logging,
     members,
+    paste_service,
     regex,
     scheduling,
     unqualify,
 ]
 
-__all__ = list(map(lambda module: module.__name__, __all__))
+__all__ = [module.__name__ for module in __all__]
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/_extensions.py` & `pydis_core-9.7.0/pydis_core/utils/_extensions.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.6.0/pydis_core/utils/_monkey_patches.py` & `pydis_core-9.7.0/pydis_core/utils/_monkey_patches.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Contains all common monkey patches, used to alter discord to fit our needs."""
 
 import logging
-import typing
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from functools import partial, partialmethod
 
 from discord import Forbidden, http
 from discord.ext import commands
 
 log = logging.getLogger(__name__)
 
@@ -20,15 +19,15 @@
     also named ``root_aliases``.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.root_aliases = kwargs.get("root_aliases", [])
 
-        if not isinstance(self.root_aliases, (list, tuple)):
+        if not isinstance(self.root_aliases, list | tuple):
             raise TypeError("Root aliases of a command must be a list or a tuple of strings.")
 
 
 class _Group(commands.Group, _Command):
     """
     A :obj:`discord.ext.commands.Group` subclass which supports root aliases.
 
@@ -43,25 +42,25 @@
     Sometimes Discord turns off typing events by throwing 403s.
 
     Handle those issues by patching discord's internal ``send_typing`` method so it ignores 403s in general.
     """
     log.debug("Patching send_typing, which should fix things breaking when Discord disables typing events. Stay safe!")
 
     original = http.HTTPClient.send_typing
-    last_403: typing.Optional[datetime] = None
+    last_403: datetime | None = None
 
     async def honeybadger_type(self: http.HTTPClient, channel_id: int) -> None:
         nonlocal last_403
-        if last_403 and (datetime.utcnow() - last_403) < timedelta(minutes=5):
+        if last_403 and (datetime.now(tz=timezone.utc) - last_403) < timedelta(minutes=5):
             log.warning("Not sending typing event, we got a 403 less than 5 minutes ago.")
             return
         try:
             await original(self, channel_id)
         except Forbidden:
-            last_403 = datetime.utcnow()
+            last_403 = datetime.now(tz=timezone.utc)
             log.warning("Got a 403 from typing event!")
 
     http.HTTPClient.send_typing = honeybadger_type
 
 
 def _apply_monkey_patches() -> None:
     """This is surfaced directly in pydis_core.utils.apply_monkey_patches()."""
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/caching.py` & `pydis_core-9.7.0/pydis_core/utils/caching.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.6.0/pydis_core/utils/channel.py` & `pydis_core-9.7.0/pydis_core/utils/channel.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.6.0/pydis_core/utils/commands.py` & `pydis_core-9.7.0/pydis_core/utils/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Optional
 
 from discord import Message
 from discord.ext.commands import BadArgument, Context, clean_content
 
 
-async def clean_text_or_reply(ctx: Context, text: Optional[str] = None) -> str:
+async def clean_text_or_reply(ctx: Context, text: str | None = None) -> str:
     """
     Cleans a text argument or replied message's content.
 
     Args:
         ctx: The command's context
         text: The provided text argument of the command (if given)
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/cooldown.py` & `pydis_core-9.7.0/pydis_core/utils/cooldown.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 _KEYWORD_SEP_SENTINEL = object()
 
 _ArgsList = list[object]
 _HashableArgsTuple = tuple[Hashable, ...]
 
 if typing.TYPE_CHECKING:
     import typing_extensions
+
     from pydis_core import BotBase
 
 P = typing.ParamSpec("P")
 """The command's signature."""
 R = typing.TypeVar("R")
 """The command's return value."""
 
 
-class CommandOnCooldown(CommandError, typing.Generic[P, R]):
+class CommandOnCooldown(CommandError, typing.Generic[P, R]):  # noqa: N818
     """Raised when a command is invoked while on cooldown."""
 
     def __init__(
         self,
         message: str | None,
         function: Callable[P, Awaitable[R]],
         /,
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/function.py` & `pydis_core-9.7.0/pydis_core/utils/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         assigned: Sequence of attribute names that are directly assigned from ``wrapped`` to ``wrapper``.
         updated: Sequence of attribute names that are ``.update``d on ``wrapper`` from the attributes on ``wrapped``.
         ignored_conflict_names: A set of names to ignore if a conflict between them is found.
 
     Returns:
         A decorator that behaves like :func:`functools.wraps`,
         with the wrapper replaced with the function :func:`update_wrapper_globals` returned.
-    """  # noqa: D200
+    """
     def decorator(wrapper: Callable[_P, _R]) -> Callable[_P, _R]:
         return functools.update_wrapper(
             update_wrapper_globals(wrapper, wrapped, ignored_conflict_names=ignored_conflict_names),
             wrapped,
             assigned,
             updated,
         )
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/interactions.py` & `pydis_core-9.7.0/pydis_core/utils/interactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Literal, Optional, Sequence
+from collections.abc import Sequence
+from typing import Literal
 
 from discord import ButtonStyle, HTTPException, Interaction, Message, NotFound, ui
 
 from pydis_core.utils.logging import get_logger
 
 log = get_logger(__name__)
 
@@ -39,16 +40,16 @@
     """
 
     def __init__(
         self,
         *,
         allowed_users: Sequence[int],
         allowed_roles: Sequence[int],
-        timeout: Optional[float] = 180.0,
-        message: Optional[Message] = None
+        timeout: float | None = 180.0,
+        message: Message | None = None
     ) -> None:
         super().__init__(timeout=timeout)
         self.allowed_users = allowed_users
         self.allowed_roles = allowed_roles
         self.message = message
 
     async def interaction_check(self, interaction: Interaction) -> bool:
@@ -93,15 +94,15 @@
 
     See :obj:`pydis_core.utils.interactions.ViewWithUserAndRoleCheck` for a view that implements basic checks.
 
     Args:
         style (:literal-url:`ButtonStyle <https://discordpy.readthedocs.io/en/latest/interactions/api.html#discord.ButtonStyle>`):
             The style of the button, set to ``ButtonStyle.secondary`` if not specified.
         label: The label of the button, set to "Delete" if not specified.
-    """  # noqa: E501
+    """
 
     def __init__(
         self,
         *,
         style: ButtonStyle = ButtonStyle.secondary,
         label: str = "Delete",
         **kwargs
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/logging.py` & `pydis_core-9.7.0/pydis_core/utils/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             msg: The message to be logged.
             args, kwargs: Passed to the base log function as is.
         """
         if self.isEnabledFor(TRACE_LEVEL):
             self.log(TRACE_LEVEL, msg, *args, **kwargs)
 
 
-def get_logger(name: typing.Optional[str] = None) -> CustomLogger:
+def get_logger(name: str | None = None) -> CustomLogger:
     """
     Utility to make mypy recognise that logger is of type :obj:`CustomLogger`.
 
     Args:
         name: The name given to the logger.
 
     Returns:
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/members.py` & `pydis_core-9.7.0/pydis_core/utils/members.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import discord
 
 from pydis_core.utils import logging
 
 log = logging.get_logger(__name__)
 
 
-async def get_or_fetch_member(guild: discord.Guild, member_id: int) -> typing.Optional[discord.Member]:
+async def get_or_fetch_member(guild: discord.Guild, member_id: int) -> discord.Member | None:
     """
     Attempt to get a member from cache; on failure fetch from the API.
 
     Returns:
         The :obj:`discord.Member` or :obj:`None` to indicate the member could not be found.
     """
     if member := guild.get_member(member_id):
```

### Comparing `pydis_core-9.6.0/pydis_core/utils/regex.py` & `pydis_core-9.7.0/pydis_core/utils/regex.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.6.0/pydis_core/utils/scheduling.py` & `pydis_core-9.7.0/pydis_core/utils/scheduling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Generic python scheduler."""
 
 import asyncio
 import contextlib
 import inspect
 import typing
 from collections import abc
-from datetime import datetime
+from datetime import datetime, timezone
 from functools import partial
 
+from discord.errors import Forbidden
+
 from pydis_core.utils import logging
+from pydis_core.utils.error_handling import handle_forbidden_from_block
 
 _background_tasks: set[asyncio.Task] = set()
 
 
 class Scheduler:
     """
     Schedule the execution of coroutines and keep track of them.
@@ -65,22 +68,23 @@
         Args:
             task_id: A unique ID to create the task with.
             coroutine: The function to be called.
         """
         self._log.trace(f"Scheduling task #{task_id}...")
 
         msg = f"Cannot schedule an already started coroutine for #{task_id}"
-        assert inspect.getcoroutinestate(coroutine) == "CORO_CREATED", msg
+        if inspect.getcoroutinestate(coroutine) != "CORO_CREATED":
+            raise ValueError(msg)
 
         if task_id in self._scheduled_tasks:
             self._log.debug(f"Did not schedule task #{task_id}; task was already scheduled.")
             coroutine.close()
             return
 
-        task = asyncio.create_task(coroutine, name=f"{self.name}_{task_id}")
+        task = asyncio.create_task(_coro_wrapper(coroutine), name=f"{self.name}_{task_id}")
         task.add_done_callback(partial(self._task_done_callback, task_id))
 
         self._scheduled_tasks[task_id] = task
         self._log.debug(f"Scheduled task #{task_id} {id(task)}.")
 
     def schedule_at(self, time: datetime, task_id: abc.Hashable, coroutine: abc.Coroutine) -> None:
         """
@@ -95,24 +99,24 @@
         prevents unawaited coroutine warnings. Don't pass a coroutine that'll be re-used elsewhere.
 
         Args:
             time: The time to start the task.
             task_id: A unique ID to create the task with.
             coroutine: The function to be called.
         """
-        now_datetime = datetime.now(time.tzinfo) if time.tzinfo else datetime.utcnow()
+        now_datetime = datetime.now(time.tzinfo) if time.tzinfo else datetime.now(tz=timezone.utc)
         delay = (time - now_datetime).total_seconds()
         if delay > 0:
             coroutine = self._await_later(delay, task_id, coroutine)
 
         self.schedule(task_id, coroutine)
 
     def schedule_later(
         self,
-        delay: typing.Union[int, float],
+        delay: int | float,
         task_id: abc.Hashable,
         coroutine: abc.Coroutine
     ) -> None:
         """
         Schedule ``coroutine`` to be executed after ``delay`` seconds.
 
         If a task with ``task_id`` already exists, close ``coroutine`` instead of scheduling it. This
@@ -148,15 +152,15 @@
         self._log.debug("Unscheduling all tasks")
 
         for task_id in self._scheduled_tasks.copy():
             self.cancel(task_id)
 
     async def _await_later(
         self,
-        delay: typing.Union[int, float],
+        delay: int | float,
         task_id: abc.Hashable,
         coroutine: abc.Coroutine
     ) -> None:
         """Await ``coroutine`` after ``delay`` seconds."""
         try:
             self._log.trace(f"Waiting {delay} seconds before awaiting coroutine for #{task_id}.")
             await asyncio.sleep(delay)
@@ -214,15 +218,15 @@
 TASK_RETURN = typing.TypeVar("TASK_RETURN")
 
 
 def create_task(
     coro: abc.Coroutine[typing.Any, typing.Any, TASK_RETURN],
     *,
     suppressed_exceptions: tuple[type[Exception], ...] = (),
-    event_loop: typing.Optional[asyncio.AbstractEventLoop] = None,
+    event_loop: asyncio.AbstractEventLoop | None = None,
     **kwargs,
 ) -> asyncio.Task[TASK_RETURN]:
     """
     Wrapper for creating an :obj:`asyncio.Task` which logs exceptions raised in the task.
 
     If the ``event_loop`` kwarg is provided, the task is created from that event loop,
     otherwise the running loop is used.
@@ -233,25 +237,33 @@
         event_loop (:obj:`asyncio.AbstractEventLoop`): The loop to create the task from.
         kwargs: Passed to :py:func:`asyncio.create_task`.
 
     Returns:
         asyncio.Task: The wrapped task.
     """
     if event_loop is not None:
-        task = event_loop.create_task(coro, **kwargs)
+        task = event_loop.create_task(_coro_wrapper(coro), **kwargs)
     else:
-        task = asyncio.create_task(coro, **kwargs)
+        task = asyncio.create_task(_coro_wrapper(coro), **kwargs)
 
     _background_tasks.add(task)
     task.add_done_callback(_background_tasks.discard)
     task.add_done_callback(partial(_log_task_exception, suppressed_exceptions=suppressed_exceptions))
     return task
 
 
+async def _coro_wrapper(coro: abc.Coroutine[typing.Any, typing.Any, TASK_RETURN]) -> None:
+    """Wraps `coro` in a try/except block that will handle 90001 Forbidden errors."""
+    try:
+        await coro
+    except Forbidden as e:
+        await handle_forbidden_from_block(e)
+
+
 def _log_task_exception(task: asyncio.Task, *, suppressed_exceptions: tuple[type[Exception], ...]) -> None:
-    """Retrieve and log the exception raised in ``task`` if one exists."""
+    """Retrieve and log the exception raised in ``task``, if one exists and it's not suppressed."""
     with contextlib.suppress(asyncio.CancelledError):
         exception = task.exception()
-        # Log the exception if one exists.
+        # Log the exception if one exists and it's not suppressed/handled.
         if exception and not isinstance(exception, suppressed_exceptions):
             log = logging.get_logger(__name__)
             log.error(f"Error in task {task.get_name()} {id(task)}!", exc_info=exception)
```

### Comparing `pydis_core-9.6.0/pyproject.toml` & `pydis_core-9.7.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydis_core"
-version = "9.6.0"
+version = "9.7.0"
 description = "PyDis core provides core functionality and utility to the bots of the Python Discord community."
 authors = ["Python Discord <info@pythondiscord.com>"]
 license = "MIT"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -30,45 +30,38 @@
 statsd  = "4.0.1"
 aiodns = "3.0.0"
 
 [tool.poetry.extras]
 async-rediscache = ["async-rediscache"]
 
 [tool.poetry.group.dev.dependencies]
-taskipy = "1.10.3"
+taskipy = "1.11.0"
 python-dotenv = "1.0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.2.1"
-pytest-cov = "4.0.0"
-pytest-xdist = "3.2.0"
+pytest = "7.3.1"
+pytest-cov = "4.1.0"
+pytest-xdist = "3.3.1"
 
 [tool.poetry.group.lint.dependencies]
-flake8 = "6.0.0"
-flake8-annotations = "3.0.0"
-flake8-bugbear = "23.2.13"
-flake8-docstrings = "1.7.0"
-flake8-import-order = "0.18.2"
-flake8-string-format = "0.3.0"
-flake8-tidy-imports = "4.8.0"
-flake8-todo = "0.7"
-pep8-naming = "0.13.3"
-pre-commit = "3.1.1"
-typing-extensions = "4.5.0"
+isort = "5.12.0"
+ruff = "0.0.270"
+pre-commit = "3.3.2"
+typing-extensions = "4.6.2"
 
 [tool.poetry.group.doc.dependencies]
-Sphinx = "6.1.3"
+Sphinx = "7.0.1"
 GitPython = "3.1.31"
-sphinx-autodoc-typehints = "1.22"
-furo = "2022.12.7"
+sphinx-autodoc-typehints = "1.23.0"
+furo = "2023.5.20"
 six = "1.16.0"
-releases = "2.1.0"
+releases = "2.1.1"
 sphinx-multiversion = "0.2.4"
 docstring-parser = "0.15"
-typing-extensions = "4.5.0"
+typing-extensions = "4.6.2"
 tomli = "2.0.1"
 
 [tool.taskipy.tasks]
 lint = "pre-commit run --all-files"
 precommit = "pre-commit install"
 docs = "sphinx-build -nW -j auto -b html docs docs/build"
 test = "pytest -n 8 --ff"
@@ -78,7 +71,37 @@
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 branch = true
 source_pkgs = ["pydis_core"]
 source = ["tests"]
+
+[tool.isort]
+multi_line_output = 6
+order_by_type = false
+case_sensitive = true
+combine_as_imports = true
+line_length = 120
+atomic = true
+known_first_party = ["dev", "pydis_core", "docs"]
+
+[tool.ruff]
+target-version = "py310"
+extend-exclude = [".cache"]
+ignore = [
+    "ANN002", "ANN003", "ANN101", "ANN102", "ANN204", "ANN206", "ANN401",
+    "B904",
+    "C401", "C408",
+    "D100", "D104", "D105", "D107", "D203", "D212", "D214", "D215", "D301",
+    "D400", "D401", "D402", "D404", "D405", "D406", "D407", "D408", "D409", "D410", "D411", "D412", "D413", "D414", "D416", "D417",
+    "E731",
+    "RET504",
+    "RUF005",
+    "S311",
+    "SIM102", "SIM108",
+]
+line-length = 120
+select = ["ANN", "B", "C4", "D", "DTZ", "E", "F", "ISC", "INT", "N", "PGH", "PIE", "Q", "RET", "RSE", "RUF", "S", "SIM", "T20", "TID", "UP", "W"]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["ANN", "D"]
```

### Comparing `pydis_core-9.6.0/PKG-INFO` & `pydis_core-9.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pydis-core
-Version: 9.6.0
+Version: 9.7.0
 Summary: PyDis core provides core functionality and utility to the bots of the Python Discord community.
 Home-page: https://pythondiscord.com/
 License: MIT
 Keywords: bot,discord,discord.py
 Author: Python Discord
 Author-email: info@pythondiscord.com
-Requires-Python: >=3.10.0,<3.12.0
+Requires-Python: >=3.10.dev0,<3.12.dev0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: async-rediscache
 Requires-Dist: aiodns (==3.0.0)
 Requires-Dist: async-rediscache[fakeredis] (==1.0.0rc2) ; extra == "async-rediscache"
 Requires-Dist: discord.py (==2.2.3)
 Requires-Dist: statsd (==4.0.1)
 Project-URL: Documentation, https://bot-core.pythondiscord.com/
 Project-URL: Repository, https://github.com/python-discord/bot-core
```

