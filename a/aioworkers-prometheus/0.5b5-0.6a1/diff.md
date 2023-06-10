# Comparing `tmp/aioworkers-prometheus-0.5b5.tar.gz` & `tmp/aioworkers_prometheus-0.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioworkers-prometheus-0.5b5.tar", last modified: Sun Dec 25 23:06:16 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aioworkers-prometheus-0.5b5.tar` & `aioworkers_prometheus-0.6a1.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 23:06:16.308710 aioworkers-prometheus-0.5b5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2022-12-25 23:06:16.308710 aioworkers-prometheus-0.5b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 23:06:16.308710 aioworkers-prometheus-0.5b5/aioworkers_prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus/service.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-25 23:06:15.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 23:06:16.308710 aioworkers-prometheus-0.5b5/aioworkers_prometheus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2022-12-25 23:06:16.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-25 23:06:16.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-25 23:06:16.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-25 23:06:16.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-25 23:06:16.000000 aioworkers-prometheus-0.5b5/aioworkers_prometheus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-25 23:06:16.308710 aioworkers-prometheus-0.5b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2022-12-25 23:06:07.000000 aioworkers-prometheus-0.5b5/setup.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/aioworkers_prometheus/__init__.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/aioworkers_prometheus/config.ini
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/aioworkers_prometheus/metric.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/aioworkers_prometheus/registry.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/aioworkers_prometheus/service.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/LICENSE
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/README.rst
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/pyproject.toml
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 aioworkers_prometheus-0.6a1/PKG-INFO
```

### Comparing `aioworkers-prometheus-0.5b5/LICENSE` & `aioworkers_prometheus-0.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioworkers-prometheus-0.5b5/aioworkers_prometheus/config.ini` & `aioworkers_prometheus-0.6a1/aioworkers_prometheus/config.ini`

 * *Files identical despite different names*

### Comparing `aioworkers-prometheus-0.5b5/aioworkers_prometheus/metric.py` & `aioworkers_prometheus-0.6a1/aioworkers_prometheus/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         histogram=metrics.Histogram,
         info=metrics.Info,
         summary=metrics.Summary,
     )
     _cache: Dict[Tuple, metrics.MetricWrapperBase] = {}
 
     def set_config(self, config: ValueExtractor) -> None:
-        cfg = config.new_parent(
+        cfg: ValueExtractor = config.new_parent(
             logger=__package__,
             autorun=bool(MULTIPROC_DIR),
             persist=True,
         )
         super().set_config(cfg)
         registry: str = self.config.get("registry", REGISTRY)
         namespace: Optional[str] = self.config.get("namespace")
```

### Comparing `aioworkers-prometheus-0.5b5/aioworkers_prometheus/registry.py` & `aioworkers_prometheus-0.6a1/aioworkers_prometheus/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-import logging
 from functools import lru_cache
 from typing import Iterable, Mapping
 
-from prometheus_client import Metric
 from prometheus_client import registry as r
 
 REGISTRY = "REGISTRY"
 
-logger = logging.getLogger(__package__)
-
 
 @lru_cache(None)
 def get_registry(name: str = REGISTRY) -> r.CollectorRegistry:
     if name == REGISTRY:
         return r.REGISTRY
     else:
         return r.CollectorRegistry(auto_describe=True)
 
 
-class LabelsRegistry(r.Collector):
+class CollectorWithLabels(r.Collector):
     def __init__(self, registry: r.Collector, labels: Mapping[str, str]):
         self._registry = registry
         self._labels = labels
 
-    def collect(self) -> Iterable[Metric]:
+    def collect(self) -> Iterable[r.Metric]:
         for mf in self._registry.collect():
             for sample in mf.samples:
                 sample.labels.update(self._labels)
             yield mf
```

### Comparing `aioworkers-prometheus-0.5b5/aioworkers_prometheus/service.py` & `aioworkers_prometheus-0.6a1/aioworkers_prometheus/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 from aioworkers.core.config import ValueExtractor
 from prometheus_client import CollectorRegistry
 from prometheus_client.bridge.graphite import GraphiteBridge
 from prometheus_client.exposition import generate_latest, start_http_server
 from prometheus_client.multiprocess import MultiProcessCollector
 
 from aioworkers_prometheus import MULTIPROC_DIR
-from aioworkers_prometheus.registry import REGISTRY, LabelsRegistry, get_registry
+from aioworkers_prometheus.registry import REGISTRY, CollectorWithLabels, get_registry
 
 
 class Service(ExecutorEntity):
     _registry: CollectorRegistry
 
     def set_config(self, config: ValueExtractor) -> None:
         super().set_config(config)
-        registry = get_registry(self.config.get("registry", REGISTRY))
         if MULTIPROC_DIR:
+            registry = CollectorRegistry()
             MultiProcessCollector(registry)
+        else:
+            registry = get_registry(self.config.get("registry", REGISTRY))
         labels = self.config.get("labels")
         if labels:
             registry = cast(
                 CollectorRegistry,
-                LabelsRegistry(
+                CollectorWithLabels(
                     registry=registry,
                     labels=labels,
                 ),
             )
         self._registry = registry
 
         port: int = self.config.get_int("port", default=0)
```

