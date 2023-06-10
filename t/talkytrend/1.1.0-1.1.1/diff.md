# Comparing `tmp/talkytrend-1.1.0.tar.gz` & `tmp/talkytrend-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.1.0.tar", max compression
+gzip compressed data, was "talkytrend-1.1.1.tar", max compression
```

## Comparing `talkytrend-1.1.0.tar` & `talkytrend-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-10 15:02:55.563721 talkytrend-1.1.0/LICENSE
--rw-r--r--   0        0        0     1456 2023-06-10 15:02:55.563721 talkytrend-1.1.0/README.md
--rw-r--r--   0        0        0     1669 2023-06-10 15:03:15.520003 talkytrend-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      116 2023-06-10 15:03:15.520003 talkytrend-1.1.0/talkytrend/__init__.py
--rw-r--r--   0        0        0      630 2023-06-10 15:02:55.563721 talkytrend-1.1.0/talkytrend/config.py
--rw-r--r--   0        0        0      489 2023-06-10 15:02:55.563721 talkytrend-1.1.0/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     2922 2023-06-10 15:02:55.563721 talkytrend-1.1.0/talkytrend/main.py
--rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 talkytrend-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-10 16:32:01.061954 talkytrend-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-10 16:32:01.061954 talkytrend-1.1.1/README.md
+-rw-r--r--   0        0        0     1669 2023-06-10 16:32:15.189895 talkytrend-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-10 16:32:15.189895 talkytrend-1.1.1/talkytrend/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-10 16:32:01.061954 talkytrend-1.1.1/talkytrend/config.py
+-rw-r--r--   0        0        0      612 2023-06-10 16:32:01.061954 talkytrend-1.1.1/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     3442 2023-06-10 16:32:01.061954 talkytrend-1.1.1/talkytrend/main.py
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 talkytrend-1.1.1/PKG-INFO
```

### Comparing `talkytrend-1.1.0/LICENSE` & `talkytrend-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.0/README.md` & `talkytrend-1.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,19 +11,27 @@
 ## Install
 
 `pip install talkytrend`
 
 ## How to use it
 
 ```
-    trend = TalkyTrend()
-    result = await trend.fetch_analysis()
-    print(result) #BUY
-    monitor = await trend.monitor_assets() #monitor change of trend
-
+    talky = TalkyTrend()
+    result = await talky.check_signal()
+    <!-- BUY -->
+
+    result = await talky.fetch_key_events()
+    print(result)
+    <!-- Title:  FDA advisers say new Alzheimer’s drug lecanemab slows cognitive decline -->
+    <!-- Description:  Panel’s opinion could pave way for full regulatory approval next month for treatment of disease that affects 6.5m Americans -->
+
+    monitor = await talky.scanner() #ongoing monitoring
+    <!-- New signal for BTCUSD (4h): STRONG_SELL -->
+    <!-- Key event: {'title': 'OPEC-JMMC Meetings', 'country': 'ALL', 'date': '2023-06-04T06:15:00-04:00', 'impact': 'High', 'forecast': '', 'previous': ''} -->
+    <!-- Key news: FDA advisers say new Alzheimer’s drug lecanemab slows cognitive decline -->
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/talkytrend/blob/main/examples/example.py)
 
 ### Real use case
```

### Comparing `talkytrend-1.1.0/pyproject.toml` & `talkytrend-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.1.0"
+version = "1.1.1"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.1.0/talkytrend/config.py` & `talkytrend-1.1.1/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.0/talkytrend/main.py` & `talkytrend-1.1.1/talkytrend/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,60 +8,63 @@
 
 from tradingview_ta import TA_Handler, Interval
 
 from talkytrend import __version__
 from .config import settings
 
 class TalkyTrend:
-    def __init__(self,
-                 asset=None,
-                 exchange="FX_IDC",
-                 screener="forex",
-                 interval=Interval.INTERVAL_4_HOURS):
-        self.logger = logging.getLogger(name="TalkyTrend")
-        if asset is None:
-            asset = settings.asset
+    def __init__(self):
+        self.economic_calendar = settings.economic_calendar
+        self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
         self.enabled = settings.talkytrend_status
-        self.asset = asset
-        self.exchange = exchange
-        self.screener = screener
-        self.interval = interval
-        self.asset_signals = {'4h': None} 
-
-    async def fetch_analysis(self):
-        
-        # Initialize the TA_Handler
-        handler = TA_Handler(
-        symbol=self.asset,
-        exchange=self.exchange,
-        screener=self.screener,
-        interval=self.interval)
-
-        analysis = handler.get_analysis()
-        print(analysis)
-        return analysis.summary['RECOMMENDATION']
+        self.assets = settings.assets
+        self.asset_signals = {"15m": None, "1h": None, "4h": None}
+
+    async def fetch_analysis(
+        self,
+        asset_id,
+        exchange,
+        screener,
+        interval):
+        try:
+            handler = TA_Handler(
+                symbol=asset_id,
+                exchange=exchange,
+                screener=screener,
+                interval=interval
+            )
+            analysis = handler.get_analysis()
+            return analysis.summary["RECOMMENDATION"]
+        except Exception as e:
+            print(e)
+
 
     async def check_signal(self):
-        current_signal = await self.fetch_analysis()
-        if self.asset_signals[self.interval] and current_signal != self.asset_signals[self.interval]:
-            message = f'New signal for {self.asset} ({self.interval}): {current_signal}'
-            print(message)
-            self.asset_signals[self.interval] = current_signal
-            return message
-            
-    async def monitor_assets(self):
-        while True:
-            await asyncio.gather(*[self.check_signal()])
-            await asyncio.sleep(settings.scanner_frequency)
+        messages = []
+        for asset in self.assets:
+            current_signal = await self.fetch_analysis(
+                asset["id"],
+                asset["exchange"],
+                asset["screener"],
+                asset["interval"])
+            if self.asset_signals.get(asset["id"]) and self.asset_signals[asset["id"]].get(asset["interval"]) and current_signal != self.asset_signals[asset["id"]][asset["interval"]]:
+                message = f'New signal for {asset["id"]} ({asset["interval"]}): {current_signal}'
+                print(message)
+                self.asset_signals[asset["id"]][asset["interval"]] = current_signal
+                messages.append(message)
+            elif not self.asset_signals.get(asset["id"]):
+                self.asset_signals[asset["id"]] = {asset["interval"]: current_signal}
+            else:
+                self.asset_signals[asset["id"]][asset["interval"]] = current_signal
+        return messages
 
-class TalkyBreaking:
-    def __init__(self):
-        self.logger = logging.getLogger(name="TalkyBreaking")
-        self.economic_calendar = settings.economic_calendar
-        self.news_url = f"{settings.news_url}{settings.news_api_key}"
+
+
+    def get_asset_signals(self):
+        return self.asset_signals
 
     async def fetch_key_events(self):
         response = requests.get(self.economic_calendar, timeout=10)  
         if response.status_code == 200:
             event_list = response.json()
             for event in event_list:
                 impact = event.get('impact')
@@ -73,14 +76,22 @@
                     return event
 
     async def fetch_key_news(self):
         response = requests.get(self.news_url,timeout=10)
         data = response.json()
         articles = data['articles']
         for article in articles:
-            print("Title: ", article['title'])
-            print("Description: ", article['description'])
+            # print("Title: ", article['title'])
+            # print("Description: ", article['description'])
+            return article
 
-    async def monitor_events(self):
+    async def scanner(self):
         while True:
-            await asyncio.gather(*[self.fetch_key_events()])
+            tasks = [self.check_signal()]
+            tasks.append(self.fetch_key_events())
+            tasks.append(self.fetch_key_news())
+            results = await asyncio.gather(*tasks)
+            if results[1] is not None:
+                print("Key event:", results[1])
+            if results[2] is not None:
+                print("Key news:", results[2]["title"])
             await asyncio.sleep(settings.scanner_frequency)
```

### Comparing `talkytrend-1.1.0/PKG-INFO` & `talkytrend-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,19 +32,27 @@
 ## Install
 
 `pip install talkytrend`
 
 ## How to use it
 
 ```
-    trend = TalkyTrend()
-    result = await trend.fetch_analysis()
-    print(result) #BUY
-    monitor = await trend.monitor_assets() #monitor change of trend
-
+    talky = TalkyTrend()
+    result = await talky.check_signal()
+    <!-- BUY -->
+
+    result = await talky.fetch_key_events()
+    print(result)
+    <!-- Title:  FDA advisers say new Alzheimer’s drug lecanemab slows cognitive decline -->
+    <!-- Description:  Panel’s opinion could pave way for full regulatory approval next month for treatment of disease that affects 6.5m Americans -->
+
+    monitor = await talky.scanner() #ongoing monitoring
+    <!-- New signal for BTCUSD (4h): STRONG_SELL -->
+    <!-- Key event: {'title': 'OPEC-JMMC Meetings', 'country': 'ALL', 'date': '2023-06-04T06:15:00-04:00', 'impact': 'High', 'forecast': '', 'previous': ''} -->
+    <!-- Key news: FDA advisers say new Alzheimer’s drug lecanemab slows cognitive decline -->
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/talkytrend/blob/main/examples/example.py)
 
 ### Real use case
```

