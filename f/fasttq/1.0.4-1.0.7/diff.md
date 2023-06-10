# Comparing `tmp/fasttq-1.0.4.tar.gz` & `tmp/fasttq-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttq-1.0.4.tar", last modified: Tue Jun  6 17:02:27 2023, max compression
+gzip compressed data, was "fasttq-1.0.7.tar", last modified: Sat Jun 10 05:51:38 2023, max compression
```

## Comparing `fasttq-1.0.4.tar` & `fasttq-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:02:27.872712 fasttq-1.0.4/
--rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1848 2023-06-06 17:02:27.872712 fasttq-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 17:02:27.823841 fasttq-1.0.4/fasttq/
--rw-rw-rw-   0        0        0      133 2023-06-06 16:53:36.000000 fasttq-1.0.4/fasttq/__init__.py
--rw-rw-rw-   0        0        0     6025 2023-06-06 13:39:37.000000 fasttq-1.0.4/fasttq/client.py
--rw-rw-rw-   0        0        0     9610 2023-06-06 16:50:43.000000 fasttq-1.0.4/fasttq/queue.py
--rw-rw-rw-   0        0        0     6034 2023-06-06 14:47:22.000000 fasttq-1.0.4/fasttq/worker.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:02:27.869720 fasttq-1.0.4/fasttq.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.4/fasttq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 17:02:27.889822 fasttq-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:51:38.532118 fasttq-1.0.7/
+-rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1848 2023-06-10 05:51:38.531587 fasttq-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 05:51:38.515607 fasttq-1.0.7/fasttq/
+-rw-rw-rw-   0        0        0      133 2023-06-10 05:50:00.000000 fasttq-1.0.7/fasttq/__init__.py
+-rw-rw-rw-   0        0        0     6025 2023-06-06 13:39:37.000000 fasttq-1.0.7/fasttq/client.py
+-rw-rw-rw-   0        0        0     9709 2023-06-10 05:21:59.000000 fasttq-1.0.7/fasttq/queue.py
+-rw-rw-rw-   0        0        0     6034 2023-06-06 14:47:22.000000 fasttq-1.0.7/fasttq/worker.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:51:38.530589 fasttq-1.0.7/fasttq.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.7/fasttq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 05:51:38.532118 fasttq-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.7/setup.py
```

### Comparing `fasttq-1.0.4/LICENSE` & `fasttq-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.4/PKG-INFO` & `fasttq-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.4
+Version: 1.0.7
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.4/README.md` & `fasttq-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.4/fasttq/client.py` & `fasttq-1.0.7/fasttq/client.py`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.4/fasttq/queue.py` & `fasttq-1.0.7/fasttq/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,36 +64,36 @@
 
     def jobs(self, topic:str = None):
         def decorator(func:Callable):
             self.getJobs.append(partial(func, topic))
             return self.getJobs
         return decorator        
 
-    def pending(self, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100):
+    def pending(self, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100, **kwargs):
         for getJob in self.getJobs:
             topic = getJob.args[0]
             if topic is None:
-                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in getJob().items()}
+                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in getJob(**kwargs).items()}
                 for chunk in dict2chunk(jobs, chunksize):
                     self.client.push_topics(chunk)
             else:
-                jobs = [serialize(data, retrys, retry_delay) for data in getJob()]
+                jobs = [serialize(data, retrys, retry_delay) for data in getJob(**kwargs)]
                 for chunk in items2chunk(jobs, chunksize):
                     self.client.push_topic(topic, chunk)
 
     #########################################################################################
     # 方案3.0，替换成Pool模式
-    def pending_mp(self, client_str:str, conn_url:str, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100):
+    def pending_mp(self, client_str:str, conn_url:str, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100, **kwargs):
         for getJob in self.getJobs:
             topic = getJob.args[0]
             if topic is None:
-                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in getJob().items()}
+                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in getJob(**kwargs).items()}
                 chunks = dict2chunk(jobs, chunksize)
             else:
-                jobs = [serialize(data, retrys, retry_delay) for data in getJob()]
+                jobs = [serialize(data, retrys, retry_delay) for data in getJob(**kwargs)]
                 chunks = items2chunk(jobs, chunksize)
             with Pool(processes=cpu_count()) as pool:
                 for chunk in chunks:
                     pool.apply_async(
                         start_pusher,
                         (client_str, conn_url, topic, chunk)
                     )
@@ -193,16 +193,16 @@
                 self._workers[process.pid] = process
                 # print(f"Workser({process.pid}): 创建成功({workers}/{len(self._workers)})！", "#"*40)
             workers = self.clear_worker()
         # for pid, process in self._workers.items():
         #     process.close()
         #     process.join()
 
-    def start(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1):
+    def start(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1, **kwargs):
         client_str = func2str(self.client)
-        self.pending(retrys, retry_delay)
+        self.pending(*args, retrys, retry_delay, **kwargs)
         self.start_workers(client_str, self.client.conn_url, workers, assignor, chunksize, retrys, retry_delay)
         
-    def start_mp(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1):
+    def start_mp(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1, **kwargs):
         client_str = func2str(self.client)
-        self.pending_mp(client_str, self.client.conn_url, retrys, retry_delay, chunksize)
+        self.pending_mp(client_str, self.client.conn_url, retrys, retry_delay, chunksize, **kwargs)
         self.start_workers(client_str, self.client.conn_url, workers, assignor, chunksize, retrys, retry_delay)
```

### Comparing `fasttq-1.0.4/fasttq/worker.py` & `fasttq-1.0.7/fasttq/worker.py`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.4/fasttq.egg-info/PKG-INFO` & `fasttq-1.0.7/fasttq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.4
+Version: 1.0.7
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.4/setup.py` & `fasttq-1.0.7/setup.py`

 * *Files identical despite different names*

