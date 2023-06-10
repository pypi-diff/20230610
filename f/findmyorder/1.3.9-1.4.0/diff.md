# Comparing `tmp/findmyorder-1.3.9.tar.gz` & `tmp/findmyorder-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.3.9.tar", max compression
+gzip compressed data, was "findmyorder-1.4.0.tar", max compression
```

## Comparing `findmyorder-1.3.9.tar` & `findmyorder-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-22 19:47:29.499663 findmyorder-1.3.9/LICENSE
--rw-r--r--   0        0        0     2090 2023-05-22 19:47:29.499663 findmyorder-1.3.9/README.md
--rw-r--r--   0        0        0      113 2023-05-22 19:47:30.359736 findmyorder-1.3.9/findmyorder/__init__.py
--rw-r--r--   0        0        0      630 2023-05-22 19:47:29.503663 findmyorder-1.3.9/findmyorder/config.py
--rw-r--r--   0        0        0      615 2023-05-22 19:47:29.503663 findmyorder-1.3.9/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     6383 2023-05-22 19:47:29.503663 findmyorder-1.3.9/findmyorder/main.py
--rw-r--r--   0        0        0     2042 2023-05-22 19:47:30.359736 findmyorder-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 findmyorder-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-10 08:36:39.679722 findmyorder-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1995 2023-06-10 08:36:39.679722 findmyorder-1.4.0/README.md
+-rw-r--r--   0        0        0      113 2023-06-10 08:36:55.536697 findmyorder-1.4.0/findmyorder/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-10 08:36:39.679722 findmyorder-1.4.0/findmyorder/config.py
+-rw-r--r--   0        0        0      686 2023-06-10 08:36:39.679722 findmyorder-1.4.0/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5703 2023-06-10 08:36:39.679722 findmyorder-1.4.0/findmyorder/main.py
+-rw-r--r--   0        0        0     1745 2023-06-10 08:36:55.532697 findmyorder-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.0/PKG-INFO
```

### Comparing `findmyorder-1.3.9/LICENSE` & `findmyorder-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.9/README.md` & `findmyorder-1.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Find my order
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
 
@@ -29,15 +29,9 @@
 
 ### Real use case
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 ## Documentation
 
-[Wiki](https://github.com/mraniki/findmyorder/wiki)
-
-
-## Questions? Want to help?
-
-[![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
-[![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
 
+[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `findmyorder-1.3.9/findmyorder/config.py` & `findmyorder-1.4.0/findmyorder/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dynaconf import Dynaconf
 
 # Define the root path of the project
 ROOT = os.path.dirname(__file__)
 
 # Load the default settings file
 settings = Dynaconf(
-    envvar_prefix="FMO",
+    envvar_prefix="TT",
     # Set the root path of the project
     root_path=os.path.dirname(ROOT),
     # Load the default settings file
     settings_files=[
         os.path.join(ROOT, "default_settings.toml"),
         'settings.toml',
         '.secrets.toml'
```

### Comparing `findmyorder-1.3.9/findmyorder/default_settings.toml` & `findmyorder-1.4.0/findmyorder/default_settings.toml`

 * *Files 22% similar despite different names*

```diff
@@ -13,11 +13,13 @@
 quantity_identifier = 'q='
 order_type_identifier = "spot future margin"
 leverage_type_identifier = "cross isolated"
 comment_identifier = "comment="
 stop_loss = 1000
 take_profit = 1000
 quantity = 1
+instrument_mapping = false
+mapping = {"BTC"="BTCUSDT","ETH"="ETHUSDT"}
 VALUE = "On Default"
 
 [testing]
 VALUE = "On Testing"
```

### Comparing `findmyorder-1.3.9/findmyorder/main.py` & `findmyorder-1.4.0/findmyorder/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 """
  FindMyOrder Main
 """
 import logging
 from datetime import datetime
 
-import emoji
+from emoji import is_emoji
 from pyparsing import (
     Combine, Optional, Word, alphas,
-    nums, one_of, ParseBaseException,
-    pyparsing_common, Suppress)
+    nums, one_of, pyparsing_common, Suppress)
 
 from .config import settings
 
 
 class FindMyOrder:
     """find an order class """
 
     def __init__(
         self,
     ):
         self.logger = logging.getLogger(name="FMO")
 
     async def search(
         self,
-        mystring: str,
+        my_string: str,
     ) -> bool:
         """Search an order."""
         try:
-            if mystring:
-                string_check = mystring.split()[0]
-                logging.debug("action identifier %s",
-                              settings.action_identifier)
-                if string_check.lower() in settings.action_identifier.lower():
-                    logging.debug("found order in %s ", mystring)
+            if my_string:
+                string_check = my_string.split()[0].lower()
+                if string_check in settings.action_identifier.lower():
                     return True
-            logging.debug("no order found")
-            return False
-        except Exception:
             return False
+        except Exception as e:
+            return e
 
-    async def contains_emoji(self, s: str) -> bool:
+    async def contains_emoji(self, input_string: str) -> bool:
         """Check if the input string contains an emoji."""
-        return any(character in emoji.UNICODE_EMOJI_ENGLISH for character in s)
+        print(input_string)
+        return is_emoji(input_string)
 
-    async def is_match(self, grammar, s: str) -> bool:
-        """Check if the input string matches the given grammar."""
-        try:
-            grammar.parseString(s, parseAll=True)
-            return True
-        except ParseBaseException:
-            return False
 
     async def identify_order(
             self,
-            mystring: str,
+            my_string: str,
             ) -> dict:
         """Identify an order."""
-        logging.debug("identify_order: %s", mystring)
         try:
             action = one_of(
                 settings.action_identifier, caseless=True
                 ).set_results_name("action").set_parse_action(
                     pyparsing_common.upcase_tokens)
             instrument = Word(
                 alphas
@@ -85,62 +73,62 @@
                 settings.leverage_type_identifier, caseless=True
                 ).set_results_name("leverage_type")
             comment = Combine(
                     Suppress(settings.comment_identifier)
                     + Word(alphas)
                 ).set_results_name("comment")
 
-            # for action in settings.actions:
-            # print(f"{action.identifier} ({action.type})")
             order_grammar = (
                 action("action")
                 + Optional(instrument, default=None)
                 + Optional(stop_loss, default=settings.stop_loss)
                 + Optional(take_profit, default=settings.take_profit)
                 + Optional(quantity, default=settings.quantity)
                 + Optional(order_type, default=None)
                 + Optional(leverage_type, default=None)
                 + Optional(comment, default=None)
               )
 
             order = order_grammar.parse_string(
-                    instring=mystring,
+                    instring=my_string,
                     parse_all=False
                     )
-            logging.debug("identify_order %s", order)
-            # logging.info("identify_order:  %s", order.asDict())
             return order.asDict()
 
         except Exception as e:
-            logging.exception("IdentifyError: %s", e)
-            return None
+            return e
 
     async def get_order(
         self,
         msg: str,
     ):
         """get an order."""
         try:
             logging.debug("get_order %s", msg)
 
             if await self.search(msg):
-                logging.debug("get_order found in %s", msg)
                 order = await self.identify_order(msg)
-                logging.debug("order: %s", order)
                 if isinstance(order, dict):
                     order["timestamp"] = datetime.utcnow().strftime(
                         "%Y-%m-%dT%H:%M:%SZ")
+                if settings.instrument_mapping:
+                    self.replace_symbol(order)
                 return order
             return None
 
         except Exception as e:
-            logging.exception("GetOrderError: %s", e)
-            return None
-
+            return e
 
+    async def replace_symbol(
+        self, 
+        order: dict,):
+        symbol = order["instrument"]
+        if symbol in settings.mapping:
+            order["instrument"] = settings.mapping[symbol]
+            return order
 # Grammar
 # class TradingGrammar:
 #     def __init__(self):
 #         self.action = self._action()
 #         self.instrument = self._instrument()
 #         self.exchange = self._exchange()
```

### Comparing `findmyorder-1.3.9/PKG-INFO` & `findmyorder-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.3.9
+Version: 1.4.0
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio
-Requires-Dist: dynaconf
-Requires-Dist: emoji
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: emoji (>=2.4.0,<3.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 # Find my order
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
 
@@ -51,16 +50,10 @@
 
 ### Real use case
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 ## Documentation
 
-[Wiki](https://github.com/mraniki/findmyorder/wiki)
-
-
-## Questions? Want to help?
-
-[![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
-[![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
 
+[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

