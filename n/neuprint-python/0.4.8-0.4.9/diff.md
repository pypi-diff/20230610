# Comparing `tmp/neuprint-python-0.4.8.tar.gz` & `tmp/neuprint-python-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neuprint-python-0.4.8.tar", last modified: Sun Feb 23 20:44:29 2020, max compression
+gzip compressed data, was "dist/neuprint-python-0.4.9.tar", last modified: Thu Apr 30 04:03:08 2020, max compression
```

## Comparing `neuprint-python-0.4.8.tar` & `neuprint-python-0.4.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/
--rw-r--r--   0 bergs      (503) staff       (20)       51 2020-02-12 01:06:28.000000 neuprint-python-0.4.8/MANIFEST.in
--rw-r--r--   0 bergs      (503) staff       (20)     1599 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/PKG-INFO
--rw-r--r--   0 bergs      (503) staff       (20)      810 2020-02-12 01:06:28.000000 neuprint-python-0.4.8/README.md
-drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint/
--rw-r--r--   0 bergs      (503) staff       (20)     1497 2020-02-14 21:16:30.000000 neuprint-python-0.4.8/neuprint/__init__.py
--rw-r--r--   0 bergs      (503) staff       (20)      497 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint/_version.py
--rw-r--r--   0 bergs      (503) staff       (20)     3545 2020-02-12 01:06:28.000000 neuprint-python-0.4.8/neuprint/admin.py
--rw-r--r--   0 bergs      (503) staff       (20)    25622 2020-02-23 03:46:08.000000 neuprint-python-0.4.8/neuprint/client.py
--rw-r--r--   0 bergs      (503) staff       (20)    31004 2020-02-19 22:52:03.000000 neuprint-python-0.4.8/neuprint/neuroncriteria.py
--rw-r--r--   0 bergs      (503) staff       (20)     7791 2020-02-23 01:45:26.000000 neuprint-python-0.4.8/neuprint/plotting.py
--rw-r--r--   0 bergs      (503) staff       (20)    79678 2020-02-20 04:14:04.000000 neuprint-python-0.4.8/neuprint/queries.py
--rw-r--r--   0 bergs      (503) staff       (20)     4524 2020-02-12 01:06:28.000000 neuprint-python-0.4.8/neuprint/synapsecriteria.py
-drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint/tests/
--rw-r--r--   0 bergs      (503) staff       (20)      279 2020-02-12 01:06:28.000000 neuprint-python-0.4.8/neuprint/tests/__init__.py
--rw-r--r--   0 bergs      (503) staff       (20)     2723 2020-02-23 20:38:27.000000 neuprint-python-0.4.8/neuprint/tests/test_client.py
--rw-r--r--   0 bergs      (503) staff       (20)     3920 2020-02-20 02:46:17.000000 neuprint-python-0.4.8/neuprint/tests/test_neuroncriteria.py
--rw-r--r--   0 bergs      (503) staff       (20)     7046 2020-02-16 05:07:38.000000 neuprint-python-0.4.8/neuprint/tests/test_queries.py
--rw-r--r--   0 bergs      (503) staff       (20)      826 2020-02-12 01:06:28.000000 neuprint-python-0.4.8/neuprint/tests/test_utils.py
--rw-r--r--   0 bergs      (503) staff       (20)    16648 2020-02-23 20:35:17.000000 neuprint-python-0.4.8/neuprint/utils.py
-drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint_python.egg-info/
--rw-r--r--   0 bergs      (503) staff       (20)     1599 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint_python.egg-info/PKG-INFO
--rw-r--r--   0 bergs      (503) staff       (20)      596 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint_python.egg-info/SOURCES.txt
--rw-r--r--   0 bergs      (503) staff       (20)        1 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint_python.egg-info/dependency_links.txt
--rw-r--r--   0 bergs      (503) staff       (20)       58 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint_python.egg-info/requires.txt
--rw-r--r--   0 bergs      (503) staff       (20)        9 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/neuprint_python.egg-info/top_level.txt
--rw-r--r--   0 bergs      (503) staff       (20)      641 2020-02-23 20:44:29.000000 neuprint-python-0.4.8/setup.cfg
--rw-r--r--   0 bergs      (503) staff       (20)     1033 2020-02-18 19:26:43.000000 neuprint-python-0.4.8/setup.py
--rw-r--r--   0 bergs      (503) staff       (20)    68611 2020-02-12 01:06:28.000000 neuprint-python-0.4.8/versioneer.py
+drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/
+-rw-r--r--   0 bergs      (503) staff       (20)       51 2020-02-12 01:06:28.000000 neuprint-python-0.4.9/MANIFEST.in
+-rw-r--r--   0 bergs      (503) staff       (20)     1599 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/PKG-INFO
+-rw-r--r--   0 bergs      (503) staff       (20)      810 2020-02-12 01:06:28.000000 neuprint-python-0.4.9/README.md
+drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint/
+-rw-r--r--   0 bergs      (503) staff       (20)     2035 2020-04-30 03:23:07.000000 neuprint-python-0.4.9/neuprint/__init__.py
+-rw-r--r--   0 bergs      (503) staff       (20)      497 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint/_version.py
+-rw-r--r--   0 bergs      (503) staff       (20)     3481 2020-04-30 02:24:18.000000 neuprint-python-0.4.9/neuprint/admin.py
+-rw-r--r--   0 bergs      (503) staff       (20)    25315 2020-04-30 02:24:33.000000 neuprint-python-0.4.9/neuprint/client.py
+-rw-r--r--   0 bergs      (503) staff       (20)    30539 2020-04-30 02:24:16.000000 neuprint-python-0.4.9/neuprint/neuroncriteria.py
+-rw-r--r--   0 bergs      (503) staff       (20)     7654 2020-04-30 02:24:35.000000 neuprint-python-0.4.9/neuprint/plotting.py
+-rw-r--r--   0 bergs      (503) staff       (20)    79220 2020-04-30 02:24:07.000000 neuprint-python-0.4.9/neuprint/queries.py
+-rw-r--r--   0 bergs      (503) staff       (20)    30820 2020-04-30 03:57:08.000000 neuprint-python-0.4.9/neuprint/simulation.py
+-rw-r--r--   0 bergs      (503) staff       (20)     4400 2020-04-30 02:24:10.000000 neuprint-python-0.4.9/neuprint/synapsecriteria.py
+drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint/tests/
+-rw-r--r--   0 bergs      (503) staff       (20)      279 2020-04-30 02:24:28.000000 neuprint-python-0.4.9/neuprint/tests/__init__.py
+-rw-r--r--   0 bergs      (503) staff       (20)     2888 2020-04-30 03:57:08.000000 neuprint-python-0.4.9/neuprint/tests/test_client.py
+-rw-r--r--   0 bergs      (503) staff       (20)     3912 2020-04-30 02:24:30.000000 neuprint-python-0.4.9/neuprint/tests/test_neuroncriteria.py
+-rw-r--r--   0 bergs      (503) staff       (20)     7021 2020-04-30 02:24:26.000000 neuprint-python-0.4.9/neuprint/tests/test_queries.py
+-rw-r--r--   0 bergs      (503) staff       (20)      814 2020-04-30 02:24:32.000000 neuprint-python-0.4.9/neuprint/tests/test_utils.py
+-rw-r--r--   0 bergs      (503) staff       (20)    18102 2020-04-30 02:24:12.000000 neuprint-python-0.4.9/neuprint/utils.py
+drwxr-xr-x   0 bergs      (503) staff       (20)        0 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint_python.egg-info/
+-rw-r--r--   0 bergs      (503) staff       (20)     1599 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint_python.egg-info/PKG-INFO
+-rw-r--r--   0 bergs      (503) staff       (20)      619 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint_python.egg-info/SOURCES.txt
+-rw-r--r--   0 bergs      (503) staff       (20)        1 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint_python.egg-info/dependency_links.txt
+-rw-r--r--   0 bergs      (503) staff       (20)       58 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint_python.egg-info/requires.txt
+-rw-r--r--   0 bergs      (503) staff       (20)        9 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/neuprint_python.egg-info/top_level.txt
+-rw-r--r--   0 bergs      (503) staff       (20)      641 2020-04-30 04:03:08.000000 neuprint-python-0.4.9/setup.cfg
+-rw-r--r--   0 bergs      (503) staff       (20)     1033 2020-02-18 19:26:43.000000 neuprint-python-0.4.9/setup.py
+-rw-r--r--   0 bergs      (503) staff       (20)    68611 2020-02-12 01:06:28.000000 neuprint-python-0.4.9/versioneer.py
```

### Comparing `neuprint-python-0.4.8/PKG-INFO` & `neuprint-python-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuprint-python
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python client utilties for interacting with the neuPrint connectome analysis service
 Home-page: https://github.com/connectome-neuprint/neuprint-python
 Author: Stuart Berg
 Author-email: bergs@hhmi.janelia.org
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.com/connectome-neuprint/neuprint-python.svg?branch=master)](https://travis-ci.com/connectome-neuprint/neuprint-python)
         [![docs-badge](docs/source/_static/docs-badge.svg)][docs]
```

### Comparing `neuprint-python-0.4.8/README.md` & `neuprint-python-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `neuprint-python-0.4.8/neuprint/__init__.py` & `neuprint-python-0.4.9/neuprint/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 from .client import Client, default_client, set_default_client
 from .neuroncriteria import NeuronCriteria
 
 #: Same as ``NeuronCriteria``.  This name is deprecated, but kept for backwards compatibility.
 SegmentCriteria = NeuronCriteria
 
 from .synapsecriteria import SynapseCriteria
-from .queries import *
+from .queries import ( fetch_custom, fetch_meta, fetch_all_rois, fetch_primary_rois, fetch_roi_hierarchy,
+                       fetch_neurons, fetch_custom_neurons, fetch_simple_connections, fetch_adjacencies,
+                       fetch_traced_adjacencies, fetch_common_connectivity, fetch_shortest_paths,
+                       fetch_synapses, fetch_synapse_connections, fetch_output_completeness,
+                       fetch_downstream_orphan_tasks )
 from .utils import merge_neuron_properties, connection_table_to_matrix
+from .simulation import ( NeuronModel, TimingResult, Ra_LOW, Ra_MED, Ra_HIGH, Rm_LOW, Rm_MED, Rm_HIGH )
 
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 
 # On Mac, requests uses a system library which is not fork-safe,
 # so using multiprocessing results in segfaults such as the following:
```

### Comparing `neuprint-python-0.4.8/neuprint/admin.py` & `neuprint-python-0.4.9/neuprint/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,63 +5,63 @@
 from requests import HTTPError
 from .client import inject_client
 
 class Transaction:
     """
     For admins only.
     Used to batch a set of operations into a single database transaction.
-    
+
     This class is implemented as a context manager.
-    
+
     Example:
-    
+
         .. code-block:: python
-        
+
             with Transaction('hemibrain') as t:
                 t.query("MATCH (n :Neuron {bodyId: 1047426385}) SET m.type=TuBu4)")
-    """    
+    """
     @inject_client
     def __init__(self, dataset, *, client=None):
         """
         Transaction constructor.
-        
+
         Args:
             dataset:
                 Name of the dataset to use.  Required.
-            
+
             client:
                 Client object to use.
         """
         # This requirement isn't technically necessary,
         # but hopefully it avoids some confusing mistakes.
         if client.dataset and client.dataset != dataset:
             msg = ("The dataset you provided does not match the client's dataset.\n"
                    "To avoid confusion, provide a client whose dataset matches the transaction dataset.")
             raise RuntimeError(msg)
-        
+
         assert dataset, \
             "Transactions require an an explicit dataset."
         self.dataset = dataset
         self.client = client
         self.transaction_id = None
         self.killed = False
-    
+
 
     def query(self, cypher, format='pandas'):
         """
         Make a custom cypher query within the context
         of this transaction (allows writes).
         """
         if self.transaction_id is None:
             raise RuntimeError("no transaction was created")
 
         url = f"{self.client.server}/api/raw/cypher/transaction/{self.transaction_id}/cypher"
         return self.client._fetch_cypher(url, cypher, self.dataset, format)
 
-    
+
     def kill(self):
         """
         Kills (rolls back) transaction.
         """
         if self.transaction_id is None:
             raise RuntimeError("no transaction was created")
 
@@ -70,15 +70,15 @@
         self.killed = True
         self.transaction_id = None
 
 
     def __enter__(self):
         self._start()
         return self
-    
+
 
     def __exit__(self, exc_type, exc_value, traceback):
         if exc_type is None:
             if not self.killed:
                 self._commit()
         elif not self.killed and self.transaction_id is not None:
             self.kill()
```

### Comparing `neuprint-python-0.4.8/neuprint/client.py` & `neuprint-python-0.4.9/neuprint/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 For commonly used queries, see :ref:`queries`.
 Or you can implement your own cypher queries using :py:func:`.fetch_custom()`.
 
 Example:
 
     .. code-block:: ipython
-    
+
         In [1]: from neuprint import Client, fetch_custom, fetch_neurons
 
         In [2]: # Create a default client. Will be implicitly used for all subsequent queries.
            ...: c = Client('neuprint.janelia.org', dataset='hemibrain:v1.0')
 
         In [3]: fetch_custom("""\\
            ...:     MATCH (n: Neuron)
@@ -32,19 +32,19 @@
         4      1290563000  ADL01b_pct  ADL01b_pct(ADL01)_R
         ...           ...         ...                  ...
         21658  2346523421        None                 None
         21659  2397377415        None                 None
         21660  2429314661        None                 None
         21661  2464541644        None                 None
         21662  2404203061        None                 None
-        
+
         [21663 rows x 3 columns]
 
 Tip:
-    
+
     All cypher queries are logged, but the messages are not
     shown in the console by default.  To display them, see
     :py:func:`setup_debug_logging()`.
 '''
 import os
 import sys
 import copy
@@ -77,37 +77,37 @@
 class NeuprintTimeoutError(HTTPError):
     pass
 
 def setup_debug_logging():
     """
     Simple debug logging configuration.
     Useful for interactive terminal sessions.
-    
+
     Warning:
         Replaces your current logging setup.
         If you've already set up logging for your app,
         don't call this function.
         Enable neuprint debug logging via:
-        
+
         .. code-block:: python
-        
+
             import logging
             logging.getLogger('neuprint.client').setLevel(logging.DEBUG)
 
     To disable cypher logging again, increase the logging severity threshold:
-    
+
         .. code-block:: python
-        
+
             import logging
             logging.getLogger('neuprint.client').setLevel(logging.INFO)
 
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: from neuprint.client import setup_debug_logging
                ...: from neuprint import fetch_neurons, NeuronCriteria as NC
                ...:
                ...: setup_debug_logging()
                ...: neuron_df, roi_df = fetch_neurons(NC(type='MBON.*', rois=['MB(R)'], regex=True))
             [2020-01-30 08:48:20,367] DEBUG Performing cypher query against dataset 'hemibrain:v1.0':
                 MATCH (n :Neuron)
@@ -122,15 +122,15 @@
     handler = logging.StreamHandler(sys.stdout)
     handler.setFormatter(formatter)
 
     root_logger = logging.getLogger()
     root_logger.handlers = []
     root_logger.addHandler(handler)
     root_logger.setLevel(logging.INFO)
-    
+
     enable_debug_logging()
 
 
 def enable_debug_logging():
     logger.setLevel(logging.DEBUG)
 
 
@@ -139,15 +139,15 @@
 
 
 def default_client():
     """
     Obtain the default Client object to use.
     This function returns a separate copy of the
     default client for each thread (and process).
-    
+
     There's usually no need to call this function.
     It is automatically called by all query functions if
     you haven't passed in an explict `client` argument.
     """
     global DEFAULT_NEUPRINT_CLIENT
 
     thread_id = threading.current_thread().ident
@@ -166,15 +166,15 @@
 
     return c
 
 
 def set_default_client(client):
     """
     Set (or overwrite) the default Client.
-    
+
     There's usually no need to call this function.
     It's is automatically called when your first
     ``Client`` is created, but you can call it again
     to replace the default.
     """
     global NEUPRINT_CLIENTS
     global DEFAULT_NEUPRINT_CLIENT
@@ -199,15 +199,15 @@
     Rather than requiring the user to pass the the client
     to every neuprint call, this decorator automatically
     passes the default (global) Client.
     """
     argspec = inspect.getfullargspec(f)
     assert 'client' in argspec.kwonlyargs, \
         f"Cannot wrap {f.__name__}: neuprint API wrappers must accept 'client' as a keyword-only argument."
-    
+
     @functools.wraps(f)
     def wrapper(*args, client=None, **kwargs):
         if client is None:
             client = default_client()
         return f(*args, **kwargs, client=client)
 
     wrapper.__signature__ = inspect.signature(f)
@@ -252,33 +252,33 @@
                     msg += f" ({ex.response.status_code})"
                 if ex.response.content:
                     try:
                         err = ex.response.json()['error']
                         msg += f":\n\n{err}"
                     except Exception:
                         pass
-            
+
             if ex.response and 'timeout' in ex.response.content.decode('utf-8').lower():
                 new_ex = NeuprintTimeoutError(msg, *ex.args[1:], response=ex.response, request=ex.request)
             else:
                 new_ex = copy.copy(ex)
                 new_ex.args = (msg, *ex.args[1:])
-            
+
             # In case this decorator is used twice in a nested call,
             # mark it as already modified it doesn't get modified twice.
             new_ex.response_content_appended = True
             raise new_ex from ex
     return wrapper
 
 
 class Client:
     def __init__(self, server, dataset=None, token=None, verify=True):
         """
         Client constructor.
-        
+
         The first ``Client`` you create will be stored as the default
         ``Client`` to be used with all ``neuprint-python`` functions
         if you don't explicitly specify one.
 
         Args:
             server:
                 URL of neuprintHttp server
@@ -395,57 +395,57 @@
     ## CUSTOM QUERIES
     ##
     ## Note: Transaction queries are not implemented here.  See admin.py
 
     def fetch_custom(self, cypher, dataset="", format='pandas'):
         """
         Query the neuprint server with a custom Cypher query.
-        
+
         Args:
             cypher:
                 A cypher query string
 
             dataset:
                 *Deprecated. Please provide your dataset as a Client constructor argument.*
-                
+
                 Which neuprint dataset to query against.
                 If None provided, the client's default dataset is used.
 
             format:
                 Either ``'pandas'`` or ``'json'``.
                 Whether to load the results into a ``pandas.DataFrame``,
                 or return the server's raw JSON response as a Python ``dict``.
-        
+
         Returns:
             Either json or DataFrame, depending on ``format``.
         """
         url = f"{self.server}/api/custom/custom"
         return self._fetch_cypher(url, cypher, dataset, format)
-    
+
 
     def _fetch_cypher(self, url, cypher, dataset, format='pandas'):
         """
         Fetch cypher from an endpoint.
         Called by fetch_custom and by Transaction queries.
         """
         assert format in ('json', 'pandas')
-        
+
         if set("‘’“”").intersection(cypher):
             msg = ("Your cypher query contains 'smart quotes' (e.g. ‘foo’ or “foo”),"
                    " which are not valid characters in cypher."
                    " Please replace them with ordinary quotes (e.g. 'foo' or \"foo\").\n"
                    "Your query was:\n"
                    + cypher)
             raise RuntimeError(msg)
-        
+
         dataset = dataset or self.dataset
-        
+
         cypher = indent(dedent(cypher), '    ')
         logger.debug(f"Performing cypher query against dataset '{dataset}':\n{cypher}")
-        
+
         result = self._fetch_json(url,
                                   json={"cypher": cypher, "dataset": dataset},
                                   ispost=True)
 
         if format == 'json':
             return result
 
@@ -505,15 +505,15 @@
 
     def fetch_instances(self):
         """
         Fetch secondary data instances avaiable through neupint http
         """
         return self._fetch_json(f"{self.server}/api/dbmeta/instances")
 
-    
+
     def fetch_db_version(self):
         """
         Fetch the database version
         """
         return self._fetch_json(f"{self.server}/api/dbmeta/version")['Version']
 
 
@@ -528,32 +528,32 @@
         """
         return self._fetch_json(f"{self.server}/profile")
 
 
     def fetch_token(self):
         """
         Fetch your user authentication token.
-        
+
         Note:
             This method just echoes the token back to you for debug purposes.
             To obtain your token for the first time, use the neuprint explorer
             web UI to login and obtain your token as explained elsewhere in
             this documentation.
         """
         return self._fetch_json(f"{self.server}/token")['token']
 
-    
+
     ##
     ## Cached
     ##
-    
+
     def fetch_daily_type(self, format='pandas'):
         """
         Return information about today's cell type of the day.
-        
+
         The server updates the completeness numbers each day. A different
         cell type is randomly picked and an exemplar is chosen
         from this type.
 
         Returns:
             If ``format='json'``, a dictionary is returned with keys
             ``['info', 'connectivity', 'skeleton']``.
@@ -562,139 +562,139 @@
             and ``skeleton`` are DataFrames.
         """
         assert format in ('json', 'pandas')
         url = f"{self.server}/api/cached/dailytype?dataset={self.dataset}"
         result = self._fetch_json(url, ispost=False)
         if format == 'json':
             return result
-        
+
         conn_df = pd.DataFrame(result['connectivity']['data'],
-                               columns=result['connectivity']['columns']) 
+                               columns=result['connectivity']['columns'])
         skel_df = pd.DataFrame(result['skeleton']['data'],
                                columns=result['skeleton']['columns'])
 
         return result['info'], conn_df, skel_df
 
-    
+
     def fetch_roi_completeness(self, format='pandas'):
         """
         Fetch the pre-computed traced "completeness" statistics
         for each primary ROI in the dataset.
-        
+
         The completeness statistics indicate how many synapses
         belong to Traced neurons.
-        
+
         Note:
             These results are not computed on-the-fly.
             They are computed periodically and cached.
         """
         assert format in ('json', 'pandas')
         url = f"{self.server}/api/cached/roicompleteness?dataset={self.dataset}"
         result = self._fetch_json(url, ispost=False)
         if format == 'json':
             return result
-        
+
         df = pd.DataFrame(result['data'], columns=result['columns'])
         return df
 
 
     def fetch_roi_connectivity(self, format='pandas'):
         """
         Fetch the pre-computed connectivity statistics
         between primary ROIs in the dataset.
-        
+
         Note:
             These results are not computed on-the-fly.
             They are computed periodically and cached.
         """
         assert format in ('json', 'pandas')
         url = f"{self.server}/api/cached/roiconnectivity?dataset={self.dataset}"
         result = self._fetch_json(url, ispost=False)
         if format == 'json':
             return result
-        
+
         # Example result:
         # {
         #    "roi_names": [['ME(R)', "a'L(L)", 'aL(L)', ...]],
         #    "weights": {
         #       'EPA(R)=>gL(L)': {'count': 7, 'weight': 1.253483174941712},
         #       'EPA(R)=>gL(R)': {'count': 29, 'weight': 2.112117795621343},
         #       'FB=>AB(L)': {'count': 62, 'weight': 230.11732347331355},
         #       'FB=>AB(R)': {'count': 110, 'weight': 496.733276906109},
         #       ...
         #    }
         # }
-        
+
         weights = [(*k.split('=>'), v['count'], v['weight']) for k,v in result["weights"].items()]
         df = pd.DataFrame(weights, columns=['from_roi', 'to_roi', 'count', 'weight'])
         return df
 
 
     ##
     ## ROI MESHES
     ##
     def fetch_roi_mesh(self, roi, export_path=None):
         """
         Fetch a mesh for the given ROI, in ``.obj`` format.
-        
+
         Args:
             roi:
                 Name of an ROI
             export_path:
                 Optional. Writes the ``.obj`` file to the given path.
-            
+
         Returns:
             bytes
             The contents of the fetched ``.obj`` mesh file.
 
         Note:
             ROI meshes are intended for visualization only.
             (They are not suitable for quantitative analysis.)
         """
         url = f"{self.server}/api/roimeshes/mesh/{self.dataset}/{roi}"
         data = self._fetch_raw(url, ispost=False)
-        
+
         if export_path:
             with open(export_path, 'wb') as f:
                 f.write(data)
         return data
-        
-    
+
+
     ##
     ## SKELETONS
     ##
     def fetch_skeleton(self, body, heal=False, export_path=None, format='pandas'):
         """
         Fetch the skeleton for a neuron or segment.
-        
+
         Args:
 
             body (int):
                 A neuron or segment ID
 
             heal (bool):
-                If ``True`` and the skeleton is fragmented, 'heal' it by connecting 
+                If ``True`` and the skeleton is fragmented, 'heal' it by connecting
                 its fragments into a single tree. The fragments are joined by
                 selecting the minimum spanning tree after joining all fragments
                 via their pairwise nearest neighbors. See :py:func:`.heal_skeleton()`
                 for more details.
 
             format (str):
                 Either 'pandas', 'swc' (similar to CSV), or 'nx' (``networkx.DiGraph``).
 
             export_path (str):
                 Optional. Writes the ``.swc`` file to disk.
                 (SWC format is written, regardless of the returned ``format``.)
-        
+
         Returns:
 
             Either a string (swc), a DataFrame (pandas), or ``networkx.DiGraph`` (nx).
-        
+
         See also:
-        
+
             - :py:func:`.heal_skeleton()`
             - :py:func:`.skeleton_df_to_nx()`
             - :py:func:`.skeleton_df_to_swc()`
         """
         try:
             body = int(body)
         except ValueError:
@@ -702,33 +702,34 @@
 
         assert isinstance(heal, bool), "Bad argument: 'heal' should be a bool."
         assert format in ('swc', 'pandas', 'nx'), f'Invalid format: {format}'
 
         url = f"{self.server}/api/skeletons/skeleton/{self.dataset}/{body}?format=swc"
         swc = self._fetch_raw(url, ispost=False).decode('utf-8')
 
-        swc_csv = '\n'.join(filter(lambda line: '#' not in line, swc.split('\n')))
-        
         if heal or format != 'swc':
             cols = ['rowId', 'node_type', 'x', 'y', 'z', 'radius', 'link']
+            lines = swc.split('\n')
+            lines = filter(lambda line: '#' not in line, lines)
+            swc_csv = '\n'.join(lines)
             df = pd.read_csv(StringIO(swc_csv), delimiter=' ', engine='c', names=cols, header=None)
             df = df.drop(columns=['node_type'])
 
         if heal:
             df = heal_skeleton(df)
             if export_path or format == 'swc':
                 swc = skeleton_df_to_swc(df)
 
         if export_path:
             with open(export_path, 'w') as f:
                 f.write(swc)
 
         if format == 'swc':
             return swc
-        
+
         if format == 'pandas':
             return df
 
         if format == 'nx':
             return skeleton_df_to_nx(df)
 
         raise AssertionError('Should not get here.')
@@ -741,15 +742,15 @@
         """
         Fetch a value from the ``neuprintHTTP`` server.
         The data address is given by both the instance name and key.
         (For admins and experts only.)
         """
         url = f"{self.server}/api/raw/keyvalue/key/{instance}/{key}"
         return self._fetch_raw(url, ispost=False)
-        
+
 
     def post_raw_keyvalue(self, instance, key, value):
         """
         Post a value from the ``neuprintHTTP`` server.
         The data address is given by both the instance name and key.
         (For admins and experts only.)
         """
```

### Comparing `neuprint-python-0.4.8/neuprint/neuroncriteria.py` & `neuprint-python-0.4.9/neuprint/neuroncriteria.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .client import inject_client
 
 def neuroncriteria_args(*argnames):
     """
     Returns a decorator.
     For the given argument names, the decorator converts the
     arguments into NeuronCriteria objects via ``copy_as_neuroncriteria()``.
-    
+
     If the decorated function also accepts a 'client' argument,
     that argument is used to initialize the NeuronCriteria.
     """
     def decorator(f):
 
         @functools.wraps(f)
         def wrapper(*args, **kwargs):
@@ -48,77 +48,77 @@
         NC -> copy(NC)
 
         None -> NC()
 
         int -> NC(bodyId)
         [str,...] -> NC(bodyId)
         DataFrame['bodyId'] -> NC(bodyId)
-        
+
         str -> NC(type, instance)
         [str, ...] -> NC(type, instance)
 
         [] -> Error
         [None] -> Error
         Anything else -> Error
-        
+
     """
     if isinstance(obj, pd.DataFrame):
         assert 'bodyId' in obj.columns, \
             'If passing a DataFrame as NeuronCriteria, it must have "bodyId" column'
         return NeuronCriteria(bodyId=obj['bodyId'].values, client=client)
 
     if not isinstance(obj, Collection) or isinstance(obj, str):
         if obj is None:
             return NeuronCriteria(client=client)
-        
+
         if isinstance(obj, NeuronCriteria):
             return copy.copy(obj)
-    
+
         if isinstance(obj, str):
             return NeuronCriteria(type=obj, instance=obj, client=client)
-        
+
         if np.issubdtype(type(obj), np.integer):
             return NeuronCriteria(bodyId=obj, client=client)
 
         raise RuntimeError(f"Can't auto-construct a NeuronCriteria from {obj}.  Please explicitly create one.")
     else:
         if len(obj) == 0:
             raise RuntimeError(f"Can't auto-construct a NeuronCriteria from {obj}.  Please explicitly create one.")
-    
+
         if len(obj) == 1 and obj[0] is None:
             raise RuntimeError(f"Can't auto-construct a NeuronCriteria from {obj}.  Please explicitly create one.")
-    
+
         if isinstance(obj, np.ndarray) and np.issubdtype(obj.dtype, np.integer):
             return NeuronCriteria(bodyId=obj, client=client)
-        
+
         item = [*filter(lambda item: item is not None, obj)][0]
         if np.issubdtype(type(item), np.integer):
             return NeuronCriteria(bodyId=obj, client=client)
-    
+
         if isinstance(item, str):
             return NeuronCriteria(type=obj, instance=obj, client=client)
-    
+
         raise RuntimeError(f"Can't auto-construct a NeuronCriteria from {obj}.  Please explicitly create one.")
 
 
 class NeuronCriteria:
     """
     Specifies which fields to filter by when searching for a Neuron (or Segment).
     This class does not send queries itself, but you use it to specify search
     criteria for various query functions.
-    
+
     Note:
         For simple queries involving only particular bodyId(s) or type(s)/instance(s),
         you can usually just pass the ``bodyId`` or ``type`` to the query function,
         without constructing a full ``NeuronCriteria``.
-        
+
         .. code-block:: python
-        
+
             from neuprint import fetch_neurons, NeuronCriteria as NC
-        
+
             # Equivalent
             neuron_df, conn_df = fetch_neurons(NC(bodyId=329566174))
             neuron_df, conn_df = fetch_neurons(329566174)
 
             # Equivalent
             # (Criteria is satisfied if either type or instance matches.)
             neuron_df, conn_df = fetch_neurons(NC(type="OA-VPM3", instance="OA-VPM3"))
@@ -237,15 +237,15 @@
         assert matchvar, "matchvar cannot be an empty string"
         assert re.match('^[a-z].*$', matchvar), \
             (f"matchvar must begin with a lowercase letter, not '{matchvar}'. "
              "Did you mean to pass this as a type or instance name?")
         assert re.match('^[a-zA-Z0-9]+$', matchvar), \
             (f"matchvar contains invalid characters: '{matchvar}'. "
              "Did you mean to pass this as a type or instance?")
-        
+
         assert label in ('Neuron', 'Segment'), f"Invalid label: {label}"
         assert len(bodyId) == 0 or np.issubdtype(np.asarray(bodyId).dtype, np.integer), \
             "bodyId should be an integer or list of integers"
 
         assert not regex or len(instance) <= 1, \
             "Please provide only one regex pattern for instance"
         assert not regex or len(type) <= 1, \
@@ -346,36 +346,36 @@
         # If all comparisons have passed, return True
         return True
 
 
     def __repr__(self):
         # Show all non-default constructor args
         s = f'NeuronCriteria("{self.matchvar}"'
-        
+
         if len(self.bodyId):
             s += f", bodyId={list(self.bodyId)}"
-        
+
         if len(self.instance) == 1:
             s += f', instance="{self.instance[0]}"'
         elif len(self.instance) > 1:
             s += f", instance={list(self.instance)}"
-            
+
         if len(self.type) == 1:
             s += f', type="{self.type[0]}"'
         elif len(self.instance) > 1:
             s += f", type={list(self.type)}"
-        
+
         if self.regex:
             s += ", regex=True"
 
         if len(self.status) == 1:
             s += f', status="{self.status[0]}"'
         elif len(self.instance) > 1:
             s += f", status={list(self.status)}"
-        
+
         if self.cropped is not None:
             s += f", cropped={self.cropped}"
 
         if self.min_pre != 0:
             s += f", min_pre={self.min_pre}"
 
         if self.min_post != 0:
@@ -385,46 +385,46 @@
             s += f", rois={list(self.rois)}"
 
         if self.inputRois:
             s += f", inputRois={list(self.inputRois)}"
 
         if self.outputRois:
             s += f", outputRois={list(self.outputRois)}"
-        
+
         if self.min_roi_inputs != 1:
             s += f", min_roi_inputs={self.min_roi_inputs}"
-                    
+
         if self.min_roi_outputs != 1:
             s += f", min_roi_outputs={self.min_roi_outputs}"
 
         if self.label != 'Neuron':
             s += f', label="{self.label}"'
 
         if self.roi_req != 'all':
             s += f', roi_req="{self.roi_req}"'
 
         s += ')'
-        
+
         return s
-    
+
 
     MAX_LITERAL_LENGTH = 3
     assert MAX_LITERAL_LENGTH >= 3, \
         ("The logic in where_expr() assumes valuevars "
          "have length 3 (assuming one could be None).")
 
 
     def global_vars(self):
         exprs = {}
 
         if len(self.bodyId) > self.MAX_LITERAL_LENGTH:
             values = [*filter(lambda s: s is not None, self.bodyId)]
             var = f"{self.matchvar}_search_bodyIds"
             exprs[var] = (f"{[*values]} as {var}")
-        
+
         if len(self.type) > self.MAX_LITERAL_LENGTH:
             values = [*filter(lambda s: s is not None, self.type)]
             var = f"{self.matchvar}_search_types"
             exprs[var] = f"{[*values]} as {var}"
 
         if len(self.instance) > self.MAX_LITERAL_LENGTH:
             values = [*filter(lambda s: s is not None, self.instance)]
@@ -438,15 +438,15 @@
 
         return exprs
 
 
     def global_with(self, *vars, prefix=0):
         if isinstance(prefix, int):
             prefix = ' '*prefix
-        
+
         if vars:
             carry_forward = [', '.join(vars)]
         else:
             carry_forward = []
 
         full_list = ',\n     '.join([*carry_forward, *self.global_vars().values()])
         if full_list:
@@ -476,15 +476,15 @@
     def typeinst_expr(self):
         """
         Unlike all other fields, type and instance OR'd together.
         Either match satisfies the criteria.
         """
         t = self.type_expr()
         i = self.instance_expr()
-        
+
         if t and i:
             return f"({t} OR {i})"
         if t:
             return t
         if i:
             return i
         return ""
@@ -518,15 +518,15 @@
             # so simply checking for False values isn't enough.
             # Must check exists().
             return f"(NOT {self.matchvar}.cropped OR NOT exists({self.matchvar}.cropped))"
 
     def rois_expr(self):
         if len(self.rois) == 0:
             return ""
-        
+
         rois = sorted(self.rois)
         roi_logic = {'any': 'OR', 'all': 'AND'}[self.roi_req]
         return "(" + f" {roi_logic} ".join(f"{self.matchvar}.`{roi}`" for roi in rois) + ")"
 
 
     def pre_expr(self):
         if self.min_pre:
@@ -543,43 +543,43 @@
 
     def all_conditions(self, *vars, prefix=0, comments=True):
         if isinstance(prefix, int):
             prefix = ' '*prefix
 
         vars = {*vars} | {self.matchvar, *self.global_vars().keys()}
         vars = (*vars,)
-        
+
         basic_cond = self.basic_conditions(0, comments)
         if basic_cond:
             basic_cond = f"WHERE \n{basic_cond}"
             basic_cond = indent(basic_cond, '  ')[2:]
-        
+
         roi_cond = self.directed_rois_condition(*vars, comments=comments)
-        
+
         if roi_cond:
             combined = basic_cond + "\n\n" + roi_cond
         else:
             combined = basic_cond
 
         return indent(combined, prefix)[len(prefix):]
-        
+
 
     @classmethod
     def combined_global_with(cls, neuron_conditions, vars=[], prefix=0):
         if isinstance(prefix, int):
             prefix = ' '*prefix
-        
+
         if vars:
             carry_forward = [', '.join(vars)]
         else:
             carry_forward = []
 
         all_globals = chain(*(nc.global_vars().values() for nc in neuron_conditions))
         full_list = ',\n     '.join([*carry_forward, *all_globals])
-        
+
         if full_list:
             return indent('WITH ' + full_list, prefix)[len(prefix):]
         return ""
 
     @classmethod
     def combined_conditions(cls, neuron_conditions, vars=[], prefix=0, comments=True):
         """
@@ -602,36 +602,36 @@
 
         if basic_cond:
             basic_cond = '\nAND\n'.join(basic_cond)
             basic_cond = indent(basic_cond, ' '*2)
             basic_cond = f"WHERE \n{basic_cond}"
 
         combined = basic_cond
-        
+
         roi_conds = [nc.directed_rois_condition(*vars, comments=comments) for nc in neuron_conditions]
         roi_conds = [*filter(None, roi_conds)]
         if roi_conds:
             roi_conds = '\n\n'.join(roi_conds)
             combined = basic_cond + "\n\n" + roi_conds
-        
+
         return indent(combined, prefix)[len(prefix):]
-        
+
 
     def basic_conditions(self, prefix=0, comments=True):
         """
         Construct a WHERE clause based on the basic conditions
         in this criteria (i.e. everything except for the "directed ROI" conditions.)
         """
         exprs = self.basic_exprs()
         if not exprs:
             return ""
 
         if isinstance(prefix, int):
             prefix = prefix*' '
-            
+
         # Build WHERE clause by combining exprs for each field
         clauses = ""
         if comments:
             clauses += f"// -- Basic conditions for segment '{self.matchvar}' --\n"
 
         clauses += f"\nAND ".join(exprs)
 
@@ -639,15 +639,15 @@
 
 
     def directed_rois_condition(self, *vars, prefix=0, comments=True):
         """
         Construct the ```WITH...WHERE``` statements that apply the "directed ROI"
         conditions specified by this criteria's ``inputRois`` and ``outputRois``
         members.
-        
+
         These conditions are expensive to evaluate, so it's usually a good
         idea to position them LAST in your cypher query, once the result set
         has already been narrowed down by eariler filters.
         """
         if not self.inputRois and not self.outputRois:
             return ""
 
@@ -673,31 +673,31 @@
             assert False
 
         if vars:
             assert self.matchvar in vars, "Pass all match vars, including the one that belongs to this criteria"
             vars = ', '.join(vars)
         else:
             vars = self.matchvar
-         
+
         conditions = dedent(f"""\
             // -- Directed ROI conditions for segment '{self.matchvar}' --
             WITH {vars},
                  {[*self.inputRois]} as inputRois,
                  {[*self.outputRois]} as outputRois,
                  apoc.convert.fromJsonMap({self.matchvar}.roiInfo) as roiInfo
-    
+
             // Check input ROIs (segment '{self.matchvar}')
             UNWIND keys(roiInfo) as roi
             WITH {vars}, roi, roiInfo, inputRois, outputRois, roiInfo[roi]['post'] as roi_post
             ORDER BY roi
             // No filter if no input ROIs were specified, otherwise select the ones that meet the reqs
             WHERE {min_input_matches} = 0 OR (roi in inputRois AND roi_post >= {self.min_roi_inputs})
             WITH {vars}, roiInfo, inputRois, outputRois, collect(roi) as matchingInputRois, size(collect(roi)) as numMatchingInputRois
             WHERE numMatchingInputRois >= {min_input_matches}
-    
+
             // Check output ROIs (segment '{self.matchvar}')
             UNWIND keys(roiInfo) as roi
             WITH {vars}, roi, roiInfo, inputRois, outputRois, matchingInputRois, roiInfo[roi]['pre'] as roi_pre
             ORDER BY roi
             // No filter if no output ROIs were specified, otherwise select the ones that meet the reqs
             WHERE {min_output_matches} = 0 OR (roi in outputRois AND roi_pre >= {self.min_roi_outputs})
             WITH {vars}, inputRois, outputRois, matchingInputRois, collect(roi) as matchingOutputRois, size(collect(roi)) as numMatchingOutputRois
@@ -722,76 +722,76 @@
     within the WHERE clause.
 
     'values' must be a list, and the generated cypher depends on:
         - the length of the list
         - whether or not it contains 'None'
         - whether or not 'regex' is True
         - whether or not 'valuevar' was given
-    
+
     If 'valuevar' is given, then the generated cypher will refer to the variable
     instead of the literal values, BUT if the literal values contain None,
     then an additional 'exists()' condition will be added.
-    
+
     Examples:
-    
+
         .. code-block: ipython
 
             In [1]: from neuprint.neuroncriteria import where_expr
-        
+
             In [2]: where_expr('status', [])
             Out[2]: ''
-            
+
             In [3]: where_expr('status', [None])
             Out[3]: 'NOT exists(n.status)'
-            
+
             In [4]: where_expr('status', ['Orphan'])
             Out[4]: "n.status = 'Orphan'"
-            
+
             In [5]: where_expr('status', ['Orphan', 'Assign'])
             Out[5]: "n.status in ['Orphan', 'Assign']"
-            
+
             In [6]: where_expr('status', ['Orphan', 'Assign', None])
             Out[6]: "n.status in ['Orphan', 'Assign'] OR NOT exists(n.status)"
-            
+
             In [7]: where_expr('status', ['Orph.*'], regex=True)
             Out[7]: "n.status =~ 'Orph.*'"
-            
+
             In [8]: where_expr('bodyId', [123])
             Out[8]: 'n.bodyId = 123'
-            
+
             In [9]: where_expr('bodyId', [123, 456])
             Out[9]: 'n.bodyId in [123, 456]'
 
             In [10]: where_expr('bodyId', [123, 456, 789], valuevar='bodies')
             Out[10]: 'n.bodyId in bodies'
-            
+
             In [11]: where_expr('bodyId', [123, None, 456], valuevar='bodies')
             Out[11]: 'n.bodyId in bodies OR NOT exists(n.bodyId)'
     """
     assert isinstance(values, collections.abc.Iterable), \
         f"Please pass a list or a variable name, not {values}"
 
     assert valuevar is None or isinstance(valuevar, str)
-    
+
     assert not regex or len(values) <= 1, \
         f"Can't use regex mode with more than one value: {values}"
 
     if len(values) == 0:
         return ""
 
     if len(values) == 1:
         if values[0] is None:
             return f"NOT exists({matchvar}.{field})"
-    
+
         if regex:
             return f"{matchvar}.{field} =~ '{values[0]}'"
-    
+
         if isinstance(values[0], str):
             return f"{matchvar}.{field} = '{values[0]}'"
-    
+
         return f"{matchvar}.{field} = {values[0]}"
 
     # list of values
     if None not in values:
         if valuevar:
             return f"{matchvar}.{field} in {valuevar}"
         else:
@@ -805,10 +805,10 @@
         else:
             return f"{matchvar}.{field} = {values[0]} OR NOT exists({matchvar}.{field})"
     else:
         if valuevar:
             return f"{matchvar}.{field} in {valuevar} OR NOT exists({matchvar}.{field})"
         else:
             return f"{matchvar}.{field} in {[*values]} OR NOT exists({matchvar}.{field})"
-        
+
```

### Comparing `neuprint-python-0.4.8/neuprint/plotting.py` & `neuprint-python-0.4.9/neuprint/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 
 def plot_soma_projections(neurons_df, color_by='cellBodyFiber'):
     """
     Plot the soma locations as XY, XZ, and ZY 2D projections,
     colored by the given column.
 
     Requires ``bokeh``.
-    
+
     Returns a layout which can be displayed
     with ``bokeh.plotting.show()``.
 
     Example:
-    
+
     .. code-block: python
-    
+
         from neuprint import fetch_neurons, NeuronCriteria as NC
         from bokeh.plotting import output_notebook
         output_notebook()
-        
+
         criteria = NC(status='Traced', cropped=False)
         neurons_df, _roi_counts_df = fetch_neurons(criteria)
         p = plot_soma_projections(neurons_df, 'cellBodyFiber')
         show(p)
 
     """
     import bokeh
@@ -72,85 +72,85 @@
     return layout
 
 
 def plot_soma_3d(neurons_df, color_by='cellBodyFiber', point_size=1.0):
     """
     Plot the soma locations in 3D, colored randomly according
     to the column given in ``color_by``.
-    
+
     Requires ``ipyvolume``.
     If using Jupyterlab, install it like this:
-    
+
     .. code-block: bash
-    
+
         conda install -c conda-forge ipyvolume
         jupyter labextension install ipyvolume
-    
+
     Example:
-    
+
         .. code-block: python
-        
+
             from neuprint import fetch_neurons, NeuronCriteria as NC
-            
+
             criteria = NC(status='Traced', cropped=False)
             neurons_df, _roi_counts_df = fetch_neurons(criteria)
             plot_soma_3d(neurons_df, 'cellBodyFiber')
     """
     import ipyvolume.pylab as ipv
     neurons_df = neurons_df[['somaLocation', color_by]].copy()
 
     extract_soma_coords(neurons_df)
     assign_colors(neurons_df, color_by)
-    
+
     neurons_with_soma_df = neurons_df.query('not somaLocation.isnull()')
     assert neurons_with_soma_df.eval('color.isnull()').sum() == 0
-    
+
     soma_x = neurons_with_soma_df['soma_x'].values
     soma_y = neurons_with_soma_df['soma_y'].values
     soma_z = neurons_with_soma_df['soma_z'].values
-    
+
     def color_to_vals(color_string):
         # Convert bokeh color string into float tuples,
         # e.g. '#00ff00' -> (0.0, 1.0, 0.0)
         s = color_string
         return (int(s[1:3], 16) / 255,
                 int(s[3:5], 16) / 255,
                 int(s[5:7], 16) / 255 )
-        
+
     color_vals = neurons_with_soma_df['color'].apply(color_to_vals).tolist()
 
     # DVID coordinate system assumes (0,0,0) is in the upper-left.
     # For consistency with DVID and neuroglancer conventions,
     # we invert the Y and X coordinates.
     ipv.figure()
     ipv.scatter(soma_x, -soma_y, -soma_z, color=color_vals, marker="circle_2d", size=point_size)
     ipv.show()
 
 
 @inject_client
 def plot_skeleton_3d(skeleton, color='blue', *, client=None):
     """
     Plot the given skeleton in 3D.
-    
+
     Args:
         skeleton:
             Either a bodyId or a pre-fetched pandas DataFrame
-        
+
         color:
             See ``ipyvolume`` docs.
             Examples: ``'blue'``, ``'#0000ff'``
             If the skeleton is fragmented, you can give a list
             of colors and each fragment will be shown in a
             different color.
 
     Requires ``ipyvolume``.
     If using Jupyterlab, install it like this:
-    
+
     .. code-block: bash
-    
+
         conda install -c conda-forge ipyvolume
         jupyter labextension install ipyvolume
     """
     import ipyvolume.pylab as ipv
 
     if np.issubdtype(type(skeleton), np.integer):
         skeleton = client.fetch_skeleton(skeleton, format='pandas')
@@ -166,26 +166,26 @@
         This means that the line will be drawn on top of itself,
         and we'll have 2x as many line segments in the plot,
         but that's not a big deal.
         """
         def accumulate_points(n):
             p = (g.nodes[n]['x'], g.nodes[n]['y'], g.nodes[n]['z'])
             points.append(p)
-    
+
             children = [*g.successors(n)]
             if not children:
                 return
             for c in children:
                 accumulate_points(c)
                 points.append(p)
-    
+
         points = []
         accumulate_points(root)
         return np.asarray(points)
-    
+
     # Skeleton may contain multiple fragments,
     # so compute the path for each one.
     def skel_paths(df):
         paths = []
         for root in df.query('link == -1')['rowId']:
             paths.append(skel_path(root))
         return paths
@@ -202,17 +202,17 @@
     ipv.show()
 
 
 def extract_soma_coords(neurons_df):
     """
     Expand the ``somaLocation`` column into three separate
     columns for ``soma_x``, ``soma_y``, and ``soma_z``.
-    
-    If ``somaLocation is None``, then the soma coords will be ``NaN``. 
-    
+
+    If ``somaLocation is None``, then the soma coords will be ``NaN``.
+
     Works in-place.
     """
     neurons_df['soma_x'] = neurons_df['soma_y'] = neurons_df['soma_z'] = np.nan
 
     somaloc = neurons_df.query('not somaLocation.isnull()')['somaLocation']
     somaloc_array = np.asarray(somaloc.tolist())
 
@@ -221,28 +221,28 @@
     neurons_df.loc[somaloc.index, 'soma_z'] = somaloc_array[:, 2]
 
 
 def assign_colors(neurons_df, color_by='cellBodyFiber'):
     """
     Use a random colortable to assign a color to each row,
     according to the column given in ``color_by``.
-    
+
     NaN values are always black.
-    
-    Works in-place.    
+
+    Works in-place.
     """
     from bokeh.palettes import Turbo256
     colors = list(Turbo256)
     colors[0] = '#000000'
     color_categories = np.sort(neurons_df[color_by].fillna('').unique())
     assert color_categories[0] == ''
 
     np.random.seed(0)
     np.random.shuffle(color_categories[1:])
     assert color_categories[0] == ''
 
     while len(colors) < len(color_categories):
         colors.extend(colors[1:])
-    
+
     color_mapping = dict(zip(color_categories, colors))
     neurons_df['color'] = neurons_df[color_by].fillna('').map(color_mapping)
```

### Comparing `neuprint-python-0.4.8/neuprint/queries.py` & `neuprint-python-0.4.9/neuprint/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,60 +24,60 @@
                'inputRois', 'outputRois', 'roiInfo']
 
 
 @inject_client
 def fetch_custom(cypher, dataset="", format='pandas', *, client=None):
     """
     Make a custom cypher query.
-    
+
     Alternative form of :py:meth:`.Client.fetch_custom()`, as a free function.
     That is, ``fetch_custom(..., client=c)`` is equivalent to ``c.fetch_custom(...)``.
 
     If ``client=None``, the default ``Client`` is used
     (assuming you have created at least one ``Client``.)
-    
+
     Args:
         cypher:
             A cypher query string
 
         dataset:
             *Deprecated. Please provide your dataset as a Client constructor argument.*
-            
+
             Which neuprint dataset to query against.
             If None provided, the client's default dataset is used.
 
         format:
             Either 'pandas' or 'json'.
             Whether to load the results into a pandas DataFrame,
             or return the server's raw json response as a Python dict.
 
         client:
             If not provided, the global default :py:class:`.Client` will be used.
-    
+
     Returns:
         Either json or DataFrame, depending on ``format``.
     """
     return client.fetch_custom(cypher, dataset, format)
 
 
 @inject_client
 def fetch_meta(*, client=None):
     """
     Fetch the dataset metadata.
     Parses json fields as needed.
-    
+
     Returns:
         dict
-    
+
     Example
-    
+
     .. code-block:: ipython
-    
+
         In [1]: meta = fetch_meta()
-    
+
         In [2]: list(meta.keys())
         Out[2]:
         ['dataset',
          'info',
          'lastDatabaseEdit',
          'latestMutationId',
          'logo',
@@ -143,45 +143,45 @@
     rois = client.fetch_custom(q)['rois'].iloc[0]
     return sorted(rois)
 
 
 def fetch_roi_hierarchy(include_subprimary=True, mark_primary=True, format='dict', *, client=None):
     """
     Fetch the ROI hierarchy nesting relationships.
-    
+
     Most ROIs in neuprint are part of a hierarchy of nested regions.
     The structure of the hierarchy is stored in the dataset metadata,
     and can be retrieved with this function.
-    
+
     Args:
         include_subprimary:
             If True, all hierarchy levels are included in the output.
             Otherwise, the hierarchy will only go as deep as necessary to
             cover all "primary" ROIs, but not any sub-primary ROIs that
             are contained within them.
-        
+
         mark_primary:
             If True, append an asterisk (``*``) to the names of
             "primary" ROIs in the hierarchy.
             Primary ROIs do not overlap with each other.
-            
+
         format:
             Either ``"dict"``, ``"text"``, or ``nx``.
             Specifies whether to return the hierarchy as a `dict`, or as
             a printable text-based tree, or as a ``networkx.DiGraph``
             (requires ``networkx``).
-    
+
     Returns:
         Either ``dict``, ``str``, or ``nx.DiGraph``,
         depending on your chosen ``format``.
 
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: from neuprint.queries import fetch_roi_hierarchy
                ...:
                ...: # Print the first few nodes of the tree -- you get the idea
                ...: roi_tree_text = fetch_roi_hierarchy(False, True, 'text')
                ...: print(roi_tree_text[:180])
             hemibrain
              +-- AL(L)*
@@ -206,119 +206,119 @@
     primary_rois = {*meta['primaryRois']}
 
     def insert(h, d):
         name = h['name']
         is_primary = (name in primary_rois)
         if mark_primary and is_primary:
             name += "*"
-        
+
         d[name] = {}
-        
+
         if 'children' not in h:
             return
 
         if is_primary and not include_subprimary:
             return
-        
+
         for c in sorted(h['children'], key=lambda c: c['name']):
             insert(c, d[name])
 
     d = {}
     insert(hierarchy, d)
-    
+
     if format == 'dict':
         return d
-    
+
     if format == "text":
         return LeftAligned()(d)
-    
+
     if format == 'nx':
         import networkx as nx
         g = nx.DiGraph()
         def add_nodes(parent, d):
             for k in d.keys():
                 g.add_edge(parent, k)
                 add_nodes(k, d[k])
         add_nodes('hemibrain', d['hemibrain'])
         return g
-        
+
 
 @inject_client
 @neuroncriteria_args('criteria')
 def fetch_neurons(criteria, *, client=None):
     """
     Return properties and per-ROI synapse counts for a set of neurons.
-    
+
     Searches for a set of Neurons (or Segments) that match the given :py:class:`.NeuronCriteria`.
     Returns their properties, including the distibution of their synapses in all brain regions.
-    
+
     This implements a superset of the features on the Neuprint Explorer `Find Neurons`_ page.
 
     Returns data in the the same format as :py:func:`fetch_custom_neurons()`,
     but doesn't require you to write cypher.
-    
+
     .. _Find Neurons: https://neuprint.janelia.org/?dataset=hemibrain%3Av1.0&qt=findneurons&q=1
-    
+
     Args:
         criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             Only Neurons which satisfy all components of the given criteria are returned.
 
         client:
             If not provided, the global default :py:class:`.Client` will be used.
-    
+
     Returns:
         Two DataFrames.
         ``(neurons_df, roi_counts_df)``
-        
+
         In ``neurons_df``, all available ``:Neuron`` columns are returned, with the following changes:
-        
+
             - ROI boolean columns are removed
             - ``roiInfo`` is parsed as json data
             - ``somaLocation`` is provided as a list ``[x, y, z]``
             - New columns ``input_rois`` and ``output_rois`` contain lists of each neuron's ROIs.
-        
+
         In ``roi_counts_df``, the ``roiInfo`` has been loadded into a table
         of per-neuron-per-ROI synapse counts, with separate columns
         for ``pre`` (outputs) and ``post`` (inputs).
 
     See also:
 
         :py:func:`.fetch_custom_neurons()` produces similar output,
         but permits you to supply your own cypher query directly.
 
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: from neuprint import fetch_neurons, NeuronCriteria as NC
 
             In [2]: neurons_df, roi_counts_df = fetch_neurons(
                ...:     NC(inputRois=['SIP(R)', 'aL(R)'],
                ...:        status='Traced',
                ...:        type='MBON.*',
                ...:        regex=True))
-            
+
             In [3]: neurons_df.iloc[:5, :11]
             Out[3]:
                   bodyId                     instance    type cellBodyFiber   pre   post        size  status  cropped     statusLabel  somaRadius
             0  300972942                 MBON14(a3)_R  MBON14           NaN   543  13634  1563154937  Traced    False  Roughly traced         NaN
             1  422725634        MBON06(B1>a)(AVM07)_L  MBON06           NaN  1356  20978  3118269136  Traced    False  Roughly traced         NaN
             2  423382015        MBON23(a2sp)(PDL05)_R  MBON23          SFS1   733   4466   857093893  Traced    False  Roughly traced       291.0
             3  423774471       MBON19(a2p3p)(PDL05)_R  MBON19          SFS1   299   1484   628019179  Traced    False  Roughly traced       286.0
             4  424767514  MBON11(y1pedc>a/B)(ADM05)_R  MBON11        mAOTU2  1643  27641  5249327644  Traced    False          Traced       694.5
-            
+
             In [4]: neurons_df['inputRois'].head()
             Out[4]:
             0    [MB(+ACA)(R), MB(R), None, SIP(R), SLP(R), SMP...
             1    [CRE(-ROB,-RUB)(R), CRE(R), INP, MB(+ACA)(R), ...
             2    [MB(+ACA)(R), MB(R), None, SIP(R), SLP(R), SMP...
             3    [MB(+ACA)(R), MB(R), SIP(R), SMP(R), SNP(R), a...
             4    [CRE(-ROB,-RUB)(R), CRE(L), CRE(R), INP, MB(+A...
             Name: inputRois, dtype: object
-            
+
             In [5]: roi_counts_df.head()
             Out[5]:
                   bodyId          roi  pre   post
             0  300972942        MB(R)   17  13295
             1  300972942        aL(R)   17  13271
             2  300972942        a3(R)   17  13224
             3  300972942  MB(+ACA)(R)   17  13295
@@ -329,15 +329,15 @@
     # Unlike in fetch_custom_neurons() below, here we specify the
     # return properties individually to avoid a large JSON payload.
     # (Returning a map on every row is ~2x more costly than returning a table of rows/columns.)
     props = list(NEURON_COLS)
     props.remove('somaLocation')
     return_exprs = ',\n'.join(f'n.{prop} as {prop}' for prop in props)
     return_exprs = indent(return_exprs, ' '*15)[15:]
-    
+
     q = f"""\
         {criteria.global_with(prefix=8)}
         MATCH (n :{criteria.label})
         {criteria.all_conditions(prefix=8)}
         RETURN {return_exprs},
                CASE
                  WHEN n.somaLocation IS NULL
@@ -351,69 +351,64 @@
 
 
 @inject_client
 def fetch_custom_neurons(q, *, client=None):
     """
     Return properties and per-ROI synapse counts for a set of neurons,
     using your own cypher query.
-    
+
     Use a custom query to fetch a neuron table, with nicer output
     than you would get from a call to :py:func:`.fetch_custom()`.
-    
+
     Returns data in the the same format as :py:func:`.fetch_neurons()`.
     but allows you to provide your own cypher query logic
     (subject to certain requirements; see below).
 
     This function includes all Neuron fields in the results,
     and also sends back ROI counts as a separate table.
-    
+
     Args:
 
         q:
             Custom query. Must match a neuron named ``n``,
             and must ``RETURN n``.
-            
+
             .. code-block::
-            
+
                 ...
                 MATCH (n :Neuron)
                 ...
                 RETURN n
                 ...
 
-        neuprint_rois:
-            Optional.  The list of ROI names from neuprint.
-            If not provided, they will be fetched
-            (so that ROI boolean columns can be dropped from the results).
-
         client:
             If not provided, the global default ``Client`` will be used.
-        
+
     Returns:
         Two DataFrames.
         ``(neurons_df, roi_counts_df)``
-        
+
         In ``neurons_df``, all available columns ``:Neuron`` columns are returned, with the following changes:
-        
+
             - ROI boolean columns are removed
             - ``roiInfo`` is parsed as json data
             - ``somaLocation`` is provided as a list ``[x, y, z]``
             - New columns ``inputRoi`` and ``outputRoi`` contain lists of each neuron's ROIs.
-        
+
         In ``roi_counts_df``, the ``roiInfo`` has been loadded into a table
         of per-neuron-per-ROI synapse counts, with separate columns
         for ``pre`` (outputs) and ``post`` (inputs).
     """
     results = client.fetch_custom(q)
-    
+
     if len(results) == 0:
         neuron_df = pd.DataFrame([], columns=NEURON_COLS, dtype=object)
         roi_counts_df = pd.DataFrame([], columns=['bodyId', 'roi', 'pre', 'post'])
         return neuron_df, roi_counts_df
-    
+
     neuron_df = pd.DataFrame(results['n'].tolist())
 
     # If somaLocation is already provided as a top-level column in the query results,
     # we assume the user's cypher query already converted it to [x,y,z] form.
     if 'somaLocation' in results:
         neuron_df['somaLocation'] = results['somaLocation']
     elif 'somaLocation' in neuron_df:
@@ -426,18 +421,18 @@
 
 
 def _process_neuron_df(neuron_df, client):
     """
     Given a DataFrame of neuron properties, parse the roiInfo into
     inputRois and outputRois, and a secondary DataFrame for per-ROI
     synapse counts.
-    
+
     Returns:
         neuron_df, roi_counts_df
-    
+
     Warning: destructively modifies the input DataFrame.
     """
     # Drop roi columns
     columns = {*neuron_df.columns} - {*client.all_rois}
     neuron_df = neuron_df[[*columns]]
 
     # Specify column order:
@@ -468,49 +463,51 @@
 @make_args_iterable(['rois'])
 @neuroncriteria_args('upstream_criteria', 'downstream_criteria')
 def fetch_simple_connections(upstream_criteria=None, downstream_criteria=None, rois=None, min_weight=1,
                              properties=['type', 'instance'],
                              *, client=None):
     """
     Find connections to/from small set(s) of neurons.
-    
+
     Finds all connections from a set of "upstream" neurons,
     or to a set of "downstream" neurons,
     or all connections from a set of upstream neurons to a set of downstream neurons.
 
     Note:
         This function is not intended to be used with very large sets of neurons.
+        Furthermore, it does not return ROI information in a convenient format.
+        But the simple output table it returns is sometimes convenient for small,
+        interactive queries.
+
         To fetch all adjacencies between a large set of neurons,
         see :py:func:`fetch_adjacencies()`, which also has additional
-        ROI-filtering options.
-        
-        However, may be more convenient for small interactive queries.
+        ROI-filtering options, and also returns ROI info in a separate table.
 
     Args:
         upstream_criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             How to filter for neurons on the presynaptic side of connections.
         downstream_criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             How to filter for neurons on the postsynaptic side of connections.
         rois:
             Limit results to neuron pairs that connect in at least one of the given ROIs.
         min_weight:
             Exclude connections whose total weight (across all ROIs) falls below this threshold.
         properties:
             Additional columns to include in the results, for both the upstream and downstream body.
         client:
             If not provided, the global default :py:class:`.Client` will be used.
-    
+
     Returns:
         DataFrame
         One row per connection, with columns for upstream (pre-synaptic) and downstream (post-synaptic) properties.
-    
+
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: from neuprint import fetch_simple_connections
                ...: sources = [329566174, 425790257, 424379864, 329599710]
                ...: targets = [425790257, 424379864, 329566174, 329599710, 420274150]
                ...: fetch_simple_connections(sources, targets)
             Out[1]:
                bodyId_pre  bodyId_post  weight                   type_pre                  type_post         instance_pre        instance_post                                       conn_roiInfo
             0   329566174    425790257      43                    OA-VPM3                        APL   OA-VPM3(NO2/NO3)_R                APL_R  {'MB(R)': {'pre': 39, 'post': 39}, 'b'L(R)': {...
@@ -528,45 +525,45 @@
     if up_crit is None:
         up_crit = NC(label='Neuron')
     if down_crit is None:
         down_crit = NC(label='Neuron')
 
     up_crit.matchvar = 'n'
     down_crit.matchvar = 'm'
-    
+
     assert up_crit is not None or down_crit is not None, "No criteria specified"
 
     if min_weight > 1:
         weight_expr = dedent(f"""\
             WITH n, m, e
             WHERE e.weight >= {min_weight}
             """)
-        weight_expr = indent(weight_expr, ' '*8)[8:] 
+        weight_expr = indent(weight_expr, ' '*8)[8:]
     else:
         weight_expr = ""
 
     rois = {*rois}
     if rois:
         invalid_rois = {*rois} - {*client.all_rois}
         assert not invalid_rois, f"Unrecognized ROIs: {invalid_rois}"
 
     return_props = ['n.bodyId as bodyId_pre',
                     'm.bodyId as bodyId_post',
                     'e.weight as weight']
-    
+
     for p in properties:
         if p == 'roiInfo':
             return_props.append('apoc.convert.fromJsonMap(n.roiInfo) as roiInfo_pre')
             return_props.append('apoc.convert.fromJsonMap(m.roiInfo) as roiInfo_post')
         else:
             return_props.append(f'n.{p} as {p}_pre')
             return_props.append(f'm.{p} as {p}_post')
-    
+
     return_props += ['e.roiInfo as conn_roiInfo']
-    
+
     return_props_str = indent(',\n'.join(return_props), prefix=' '*15)[15:]
 
     combined_global_with = NC.combined_global_with([up_crit, down_crit], prefix=8)
     combined_conditions = NC.combined_conditions([up_crit, down_crit], ('n', 'm', 'e'), prefix=8)
     q = f"""\
         {combined_global_with}
         MATCH (n:{up_crit.label})-[e:ConnectsTo]->(m:{down_crit.label})
@@ -575,18 +572,18 @@
         {weight_expr}
         RETURN {return_props_str}
         ORDER BY e.weight DESC,
                  n.bodyId,
                  m.bodyId
     """
     edges_df = client.fetch_custom(q)
-    
+
     # Load connection roiInfo with ujson
     edges_df['conn_roiInfo'] = edges_df['conn_roiInfo'].apply(ujson.loads)
-    
+
     if rois:
         keep = edges_df['conn_roiInfo'].apply(lambda roiInfo: bool(rois & {*roiInfo.keys()}))
         edges_df = edges_df.loc[keep].reset_index(drop=True)
 
     return edges_df
 
 
@@ -594,15 +591,15 @@
 @make_args_iterable(['rois'])
 @neuroncriteria_args('sources', 'targets')
 def fetch_adjacencies(sources=None, targets=None, rois=None, min_roi_weight=1, min_total_weight=1,
                       include_nonprimary=False, export_dir=None, batch_size=200,
                       properties=['type', 'instance'], *, client=None):
     """
     Find connections to/from large sets of neurons, with per-ROI connection strengths.
-    
+
     Fetches the adjacency table for connections between sets of neurons, broken down by ROI.
     Unless ``include_nonprimary=True``, only primary ROIs are included in the per-ROI connection table.
     Connections outside of the primary ROIs are labeled with the special name
     ``"NotPrimary"`` (which is not currently an ROI name in neuprint itself).
 
     Note:
         :py:func:`.fetch_simple_connections()` has similar functionality,
@@ -619,18 +616,18 @@
             If ``None``, all neurons downstream of ``sources`` will be fetched.
 
         rois:
             Limit results to connections within the listed ROIs.
 
         min_roi_weight:
             Limit results to connections of at least this strength within at least one of the returned ROIs.
-        
+
         min_total_weight:
             Limit results to connections that are at least this strong when totaled across all ROIs.
-            
+
             Note:
                 Even if ``min_roi_weight`` is also specified, all connections are counted towards satisfying
                 the total weight threshold, even though some ROI entries are filtered out.
                 Therefore, some connections in the results may appear not to satisfy ``min_total_weight``
                 when their per-ROI weights are totaled.  That's just because you filtered out the weak
                 per-ROI entries.
 
@@ -665,34 +662,34 @@
         See caveat above concerning non-primary ROIs.
 
     See also:
         :py:func:`.fetch_simple_connections()`
         :py:func:`.fetch_traced_adjacencies()`
 
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: from neuprint import Client
                ...: c = Client('neuprint.janelia.org', dataset='hemibrain:v1.0.1')
-            
+
             In [2]: from neuprint import fetch_adjacencies
                ...: sources = [329566174, 425790257, 424379864, 329599710]
                ...: targets = [425790257, 424379864, 329566174, 329599710, 420274150]
                ...: neuron_df, connection_df = fetch_adjacencies(sources, targets)
-            
+
             In [3]: neuron_df
             Out[3]:
                   bodyId             instance                       type
             0  329566174   OA-VPM3(NO2/NO3)_R                    OA-VPM3
             1  329599710        mPNX(AVM06)_R  olfactory multi lvPN mALT
             2  424379864  AVM03e_pct(AVM03)_R                 AVM03e_pct
             3  425790257                APL_R                        APL
             4  420274150  AVM03m_pct(AVM03)_R                 AVM03m_pct
-            
+
             In [4]: connection_df
             Out[4]:
                 bodyId_pre  bodyId_post     roi  weight
             0    329566174    329599710  SLP(R)       1
             1    329566174    420274150  SLP(R)       1
             2    329566174    424379864  SLP(R)      31
             3    329566174    424379864  SCL(R)       3
@@ -713,15 +710,15 @@
             18   425790257    329566174   gL(R)       8
             19   425790257    329566174   CA(R)       3
             20   425790257    329566174   aL(R)       1
 
     **Total Connection Strength**
 
     To aggregate the per-ROI connection weights into total connection weights, use ``groupby(...)['weight'].sum()``
-    
+
     .. code-block:: ipython
 
         In [5]: connection_df.groupby(['bodyId_pre', 'bodyId_post'], as_index=False)['weight'].sum()
         Out[5]:
            bodyId_pre  bodyId_post  weight
         0   329566174    329599710       1
         1   329566174    420274150       1
@@ -739,15 +736,15 @@
     ##    source (or target) bodies.
     ##
     ## 2. To achieve (1), it has to pre-fetch either the source body list or the
     ##    target body list.
     ##
     ## 3. To achieve (2), it first fetches the *counts* of the source/body lists,
     ##    and determines which is shorter, or at least which one can be fetched
-    ##    withina short timeout.
+    ##    within a short timeout.
     ##
     ## 4. It 'reshapes' roi info into a column, with special care given to the
     ##    `include_nonprimary` option, and also invents a special ROI `NotPrimary`.
     ##
     ## 5. It updates the neuron list if necessary to include all sources and targets.
     ##
     ## 6. It writes to CSV.
@@ -755,28 +752,28 @@
     ##
     ## Preprocess arguments
     ##
 
     rois = {*rois}
     invalid_rois = rois - {*client.all_rois}
     assert not invalid_rois, f"Unrecognized ROIs: {invalid_rois}"
-    
+
     nonprimary_rois = rois - {*client.primary_rois}
     assert include_nonprimary or not nonprimary_rois, \
         f"Since you listed nonprimary rois ({nonprimary_rois}), please specify include_nonprimary=True"
 
     min_roi_weight = max(min_roi_weight, 1)
     min_total_weight = max(min_total_weight, min_roi_weight)
 
     if 'bodyId' not in properties:
         properties = ['bodyId'] + properties
 
     def _prepare_criteria(criteria, matchvar):
         criteria.matchvar = matchvar
-        
+
         # If the user wants to filter for specific rois,
         # we can speed up the query by adding them to the NeuronCriteria
         if rois and not criteria.rois:
             criteria.rois = rois
             criteria.roi_req = 'any'
 
         return criteria
@@ -790,15 +787,15 @@
         matchvar = criteria.matchvar
 
         return_props = [f'{matchvar}.{prop} as {prop}' for prop in properties]
         return_props = indent(',\n'.join(return_props), ' '*23)[23:]
 
         value_props = [f'value.{prop} as {prop}' for prop in properties]
         value_props = indent(',\n'.join(value_props), ' '*19)[19:]
-        
+
         q = f"""\
             {criteria.global_with(prefix=12)}
             MATCH ({matchvar}:{criteria.label})
             {criteria.all_conditions(prefix=12)}
             WITH {matchvar}
             RETURN {return_props}
             ORDER BY bodyId
@@ -826,48 +823,48 @@
                 ", {{}}, {timeout*1000}) YIELD value
                 RETURN value.c as count
             """
             try:
                 result = client.fetch_custom(q)['count']
             except NeuprintTimeoutError:
                 return None
-    
+
             if len(result) == 0:
                 return None
-    
+
             return result.iloc[0]
-    
+
         num_sources = _fetch_count(sources, 5)
         num_targets = _fetch_count(targets, 5)
-    
+
         if num_sources is None and num_targets is None:
             num_sources = _fetch_count(sources, 120)
             num_targets = _fetch_count(targets, 120)
-    
+
         if num_sources is None and num_targets is None:
             raise RuntimeError("Both source and target list are too large to pre-fetch without timing out. "
                                "This query is too big to process.")
-    
+
         if num_sources == 0:
             raise RuntimeError("No neurons match your source criteria")
-    
+
         if num_targets == 0:
             raise RuntimeError("No neurons match your target criteria")
-    
+
         sources_df = targets_df = None
         if (num_sources is not None) and (num_targets is not None):
             if num_sources <= num_targets:
                 sources_df = _fetch_neurons(sources)
             else:
                 targets_df = _fetch_neurons(targets)
         elif num_sources is not None:
             sources_df = _fetch_neurons(sources)
         elif num_targets is not None:
             targets_df = _fetch_neurons(targets)
-    
+
         assert (sources_df is None) != (targets_df is None)
         return sources_df, targets_df
 
     sources_df, targets_df = _prefetch_batchlist()
 
     ##
     ## Fetch connections in batches
@@ -882,62 +879,62 @@
         else:
             weight_condition = dedent(f"""\
                 // -- Filter by total connection weight --
                 WITH n,m,e
                 WHERE e.weight >= {min_total_weight}
             """)
             weight_condition = indent(weight_condition, prefix=20*' ')[20:]
-        
+
         # Fetch connections by batching either the source list
         # or the target list, not both.
         # (It turns out that batching across BOTH sources and
         # targets is much slower than batching across only one.)
         conn_tables = []
-        
+
         if sources_df is not None:
             # Break sources into batches
             for batch_start in trange(0, len(sources_df), batch_size):
                 batch_stop = batch_start + batch_size
                 source_bodies = sources_df['bodyId'].iloc[batch_start:batch_stop].tolist()
-                
+
                 batch_criteria = copy.copy(sources)
                 batch_criteria.bodyId = source_bodies
-                
+
                 criteria_globals = [*batch_criteria.global_vars().keys(), *targets.global_vars().keys()]
-                
+
                 q = f"""\
                     {NeuronCriteria.combined_global_with((batch_criteria, targets), prefix=20)}
                     MATCH (n:{sources.label})-[e:ConnectsTo]->(m:{targets.label})
                     {batch_criteria.all_conditions(*'nme', *criteria_globals, prefix=20)}
 
                     // Artificial break in the query flow to fool the query
                     // planner into avoiding a Cartesian product.
                     // This improves performance considerably in some cases.
                     WITH {','.join([*'nme', *criteria_globals])}, true as _
- 
+
                     {targets.all_conditions(*'nme', prefix=20)}
                     {weight_condition}
 
                     RETURN n.bodyId as bodyId_pre,
                            m.bodyId as bodyId_post,
                            e.weight as weight,
                            e.roiInfo as roiInfo
                 """
                 conn_tables.append(client.fetch_custom(q))
         else:
             # Break targets into batches
             for batch_start in trange(0, len(targets_df), batch_size):
                 batch_stop = batch_start + batch_size
                 target_bodies = targets_df['bodyId'].iloc[batch_start:batch_stop].tolist()
-                
+
                 batch_criteria = copy.copy(targets)
                 batch_criteria.bodyId = target_bodies
-                
+
                 criteria_globals = [*batch_criteria.global_vars().keys(), *sources.global_vars().keys()]
-                
+
                 q = f"""\
                     {NeuronCriteria.combined_global_with((sources, batch_criteria), prefix=20)}
                     MATCH (n:{sources.label})-[e:ConnectsTo]->(m:{targets.label})
                     {batch_criteria.all_conditions(*'nme', *criteria_globals, prefix=20)}
 
                     // Artificial break in the query flow to fool the query
                     // planner into avoiding a Cartesian product.
@@ -948,15 +945,15 @@
                     {weight_condition}
                     RETURN n.bodyId as bodyId_pre,
                            m.bodyId as bodyId_post,
                            e.weight as weight,
                            e.roiInfo as roiInfo
                 """
                 conn_tables.append(client.fetch_custom(q))
-    
+
         # Combine batches
         connections_df = pd.concat(conn_tables, ignore_index=True)
         return connections_df
 
     connections_df = _fetch_connections()
 
     ##
@@ -969,43 +966,43 @@
     # Extract per-ROI counts from the roiInfo column
     # to construct one big table of per-ROI counts
     roi_connections = []
     for row in connections_df.itertuples(index=False):
         # We use the 'post' count as the weight (ignore pre)
         roi_connections += [(row.bodyId_pre, row.bodyId_post, roi, weights.get('post', 0))
                             for roi, weights in row.roiInfo.items()]
-    
+
     roi_conn_df = pd.DataFrame(roi_connections,
                                columns=['bodyId_pre', 'bodyId_post', 'roi', 'weight'])
-    
+
     # Filter out non-primary ROIs
     primary_roi_conn_df = roi_conn_df.query('roi in @client.primary_rois')
-    
+
     # Add a special roi name "NotPrimary" to account for the
     # difference between total weights and primary-only weights.
     primary_totals = primary_roi_conn_df.groupby(['bodyId_pre', 'bodyId_post'], as_index=False)['weight'].sum()
 
     totals_df = connections_df.merge(primary_totals, 'left', on=['bodyId_pre', 'bodyId_post'], suffixes=['_all', '_primary'])
     totals_df.fillna(0, inplace=True)
     totals_df['weight_notprimary'] = totals_df.eval('weight_all - weight_primary').astype(int)
     totals_df['roi'] = 'NotPrimary'
-    
+
     # Drop weights other than NotPrimary
     totals_df = totals_df[['bodyId_pre', 'bodyId_post', 'roi', 'weight_notprimary']]
     notprimary_totals_df = totals_df.query('weight_notprimary > 0')
     notprimary_totals_df = notprimary_totals_df.rename(columns={'weight_notprimary': 'weight'})
-    
+
     if not include_nonprimary:
         roi_conn_df = primary_roi_conn_df
-    
+
     # Append NotPrimary rows to the connection table.
     roi_conn_df = pd.concat((roi_conn_df, notprimary_totals_df), ignore_index=True)
     roi_conn_df.sort_values(['bodyId_pre', 'bodyId_post', 'weight'], ascending=[True, True, False], inplace=True)
     roi_conn_df.reset_index(drop=True, inplace=True)
-    
+
     # Consistency check: Double-check our math against the original totals
     summed_roi_weights = (roi_conn_df
                             .query('roi in @client.primary_rois or roi == "NotPrimary"')
                             .groupby(['bodyId_pre', 'bodyId_post'], as_index=False)['weight']
                             .sum())
     compare_df = connections_df.merge(summed_roi_weights, 'left', on=['bodyId_pre', 'bodyId_post'], suffixes=['_orig', '_summed'])
     assert compare_df.fillna(0).eval('weight_orig == weight_summed').all()
@@ -1055,15 +1052,15 @@
     ##
     if export_dir:
         os.makedirs(export_dir, exist_ok=True)
 
         # Export Nodes
         p = f"{export_dir}/neurons.csv"
         neurons_df.to_csv(p, index=False, header=True)
-        
+
         # Export Edges (per ROI)
         p = f"{export_dir}/roi-connections.csv"
         roi_conn_df.to_csv(p, index=False, header=True)
 
         # Export Edges (total weight)
         p = f"{export_dir}/total-connections.csv"
         connections_df[['bodyId_pre', 'bodyId_post', 'weight']].to_csv(p, index=False, header=True)
@@ -1071,24 +1068,24 @@
     return neurons_df, roi_conn_df
 
 
 @inject_client
 def fetch_traced_adjacencies(export_dir=None, batch_size=200, *, client=None):
     """
     Convenience function that calls :py:func:`.fetch_adjacencies()`
-    for all ``Traced``, non-``cropped`` neurons. 
- 
+    for all ``Traced``, non-``cropped`` neurons.
+
     Note:
         On the hemibrain dataset, this function takes a few minutes to run,
         and the results are somewhat large (~300 MB).
-    
+
     Example:
-        
+
         .. code-block:: ipython
-        
+
             In [1]: neurons_df, roi_conn_df = fetch_traced_adjacencies('exported-connections')
 
             In [2]: roi_conn_df.head()
             Out[2]:
                    bodyId_pre  bodyId_post        roi  weight
             0      5813009352    516098538     SNP(R)       2
             1      5813009352    516098538     SLP(R)       2
@@ -1102,75 +1099,75 @@
                ...: total_conn_df.head()
             Out[3]:
                bodyId_pre  bodyId_post  weight
             0   202916528    203253253       2
             1   202916528    203257652       2
             2   202916528    203598557       2
             3   202916528    234292899       4
-            4   202916528    264986706       2        
+            4   202916528    264986706       2
      """
     criteria = NeuronCriteria(status="Traced", cropped=False, client=client)
     return fetch_adjacencies(criteria, criteria, include_nonprimary=False, export_dir=export_dir, batch_size=batch_size, client=client)
 
 
 @inject_client
 @neuroncriteria_args('criteria')
 def fetch_common_connectivity(criteria, search_direction='upstream', min_weight=1, properties=['type', 'instance'], *, client=None):
     """
     Find shared connections among a set of neurons.
-    
+
     Given a set of neurons that match the given criteria, find neurons
     that connect to ALL of the neurons in the set, i.e. connections
     that are common to all neurons in the matched set.
-    
+
     This is the Python equivalent to the Neuprint Explorer `Common Connectivity`_ page.
 
     .. _Common Connectivity: https://neuprint.janelia.org/?dataset=hemibrain%3Av1.0&qt=commonconnectivity&q=1
-    
-    
+
+
     Args:
         criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             Used to determine the match set, for which common connections will be found.
 
         search_direction (``"upstream"`` or ``"downstream"``):
             Whether or not to search for common connections upstream of
-            the matched neurons or downstream of the matched neurons. 
-        
+            the matched neurons or downstream of the matched neurons.
+
         min_weight:
             Connections below the given strength will not be included in the results.
 
         properties:
             Additional columns to include in the results, for both the upstream and downstream body.
 
         client:
             If not provided, the global default :py:class:`.Client` will be used.
-    
+
     Returns:
         DataFrame.
         (Same format as returned by :py:func:`fetch_simple_connections()`.)
         One row per connection, with columns for upstream and downstream properties.
         For instance, if ``search_direction="upstream"``, then the matched neurons will appear
         in the ``_post`` columns, and the common connections will appear in the ``_pre``
         columns.
     """
     assert search_direction in ('upstream', 'downstream')
     if search_direction == "upstream":
         edges_df = fetch_simple_connections(None, criteria, min_weight, properties, client=client)
-        
+
         # How bodies many met main search criteria?
         num_primary = edges_df['bodyId_post'].nunique()
 
         # upstream bodies that connect to ALL of the main bodies are the 'common' bodies.
         upstream_counts = edges_df['bodyId_pre'].value_counts()
         _keep = upstream_counts[upstream_counts == num_primary].index
         return edges_df.query('bodyId_pre in @_keep')
 
     if search_direction == "downstream":
         edges_df = fetch_simple_connections(criteria, None, min_weight, properties, client=client)
-        
+
         # How bodies many met main search criteria?
         num_primary = edges_df['bodyId_pre'].nunique()
 
         # upstream bodies that connect to ALL of the main are the 'common' bodies.
         upstream_counts = edges_df['bodyId_post'].value_counts()
         _keep = upstream_counts[upstream_counts == num_primary].index
         return edges_df.query('bodyId_post in @_keep')
@@ -1178,107 +1175,107 @@
 
 @inject_client
 def fetch_shortest_paths(upstream_bodyId, downstream_bodyId, min_weight=1,
                          intermediate_criteria=None,
                          timeout=5.0, *, client=None):
     """
     Find all neurons along the shortest path between two neurons.
-    
+
     Args:
         upstream_bodyId:
             The starting neuron
-        
+
         downstream_bodyId:
             The destination neuron
-        
+
         min_weight:
             Minimum connection strength for each step in the path.
-        
+
         intermediate_criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             Filtering criteria for neurons on path.
             All intermediate neurons in the path must satisfy this criteria.
             By default, ``NeuronCriteria(status="Traced")`` is used.
-        
+
         timeout:
             Give up after this many seconds, in which case an **empty DataFrame is returned.**
             No exception is raised!
-        
+
         client:
             If not provided, the global default :py:class:`.Client` will be used.
-    
+
     Returns:
         All paths are concatenated into a single DataFrame.
         The `path` column indicates which path that row belongs to.
         The `weight` column indicates the connection strength to that
         body from the previous body in the path.
-        
+
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: fetch_shortest_paths(329566174, 294792184, min_weight=10)
             Out[1]:
                   path     bodyId                       type  weight
             0        0  329566174                    OA-VPM3       0
             1        0  517169460                 PDL05h_pct      11
             2        0  297251714                ADM01om_pct      15
             3        0  294424196                PDL13ob_pct      11
             4        0  295133927               PDM18a_d_pct      10
             ...    ...        ...                        ...     ...
             5773   962  511271574                 ADL24h_pct      43
             5774   962  480923210                PDL10od_pct      18
             5775   962  294424196                PDL13ob_pct      21
             5776   962  295133927               PDM18a_d_pct      10
             5777   962  294792184  olfactory multi vPN mlALT      10
-            
+
             [5778 rows x 4 columns]
     """
     if intermediate_criteria is None:
         intermediate_criteria = NeuronCriteria(status="Traced", client=client)
     else:
         intermediate_criteria = copy_as_neuroncriteria(intermediate_criteria)
-    
+
     assert len(intermediate_criteria.inputRois) == 0 and len(intermediate_criteria.outputRois) == 0, \
         "This function doesn't support search criteria that specifies inputRois or outputRois. "\
         "You can specify generic (intersecting) rois, though."
 
     intermediate_criteria.matchvar = 'n'
 
     timeout_ms = int(1000*timeout)
 
     nodes_where = intermediate_criteria.all_conditions(comments=False)
     nodes_where += f"\n OR n.bodyId in [{upstream_bodyId}, {downstream_bodyId}]"
     nodes_where = nodes_where.replace('\n', '')
-    
+
     q = f"""\
         call apoc.cypher.runTimeboxed(
             "MATCH (src :Neuron {{ bodyId: {upstream_bodyId} }}),
                    (dest:Neuron {{ bodyId: {downstream_bodyId} }}),
                    p = allShortestPaths((src)-[:ConnectsTo*]->(dest))
 
             WHERE     ALL (x in relationships(p) WHERE x.weight >= {min_weight})
                   AND ALL (n in nodes(p) {nodes_where})
 
             RETURN [n in nodes(p) | [n.bodyId, n.type]] AS path,
                    [x in relationships(p) | x.weight] AS weights",
-            
+
             {{}},{timeout_ms}) YIELD value
             RETURN value.path as path, value.weights AS weights
     """
     results_df = client.fetch_custom(q)
-    
+
     table_indexes = []
     table_bodies = []
     table_types = []
     table_weights = []
 
     for path_index, (path, weights) in enumerate(results_df.itertuples(index=False)):
         bodies, types = zip(*path)
         weights = [0, *weights]
-        
+
         table_indexes += len(bodies)*[path_index]
         table_bodies += bodies
         table_types += types
         table_weights += weights
 
     paths_df = pd.DataFrame({'path': table_indexes,
                              'bodyId': table_bodies,
@@ -1290,15 +1287,15 @@
 @inject_client
 @neuroncriteria_args('neuron_criteria')
 def fetch_synapses(neuron_criteria, synapse_criteria=None, batch_size=10, *, client=None):
     """
     Fetch synapses from a neuron or selection of neurons.
 
     Args:
-    
+
         neuron_criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             Determines which bodies to fetch synapses for.
 
             Note:
                 Any ROI criteria specified in this argument does not affect
                 which synapses are returned, only which bodies are inspected.
 
@@ -1308,33 +1305,33 @@
 
             If the criteria specifies ``primary_only=True`` only primary ROIs will be returned in the results.
             If a synapse does not intersect any primary ROI, it will be listed with an roi of ``None``.
             (Since 'primary' ROIs do not overlap, each synapse will be listed only once.)
             Otherwise, all ROI names will be included in the results.
             In that case, some synapses will be listed multiple times -- once per intersecting ROI.
             If a synapse does not intersect any ROI, it will be listed with an roi of ``None``.
-        
+
         batch_size:
             To improve performance and avoid timeouts, the synapses for multiple bodies
             will be fetched in batches, where each batch corresponds to N bodies.
             This argument sets the batch size N.
 
         client:
             If not provided, the global default :py:class:`.Client` will be used.
 
     Returns:
-    
+
         DataFrame in which each row represent a single synapse.
         Unless ``primary_only`` was specified, some synapses may be listed more than once,
         if they reside in more than one overlapping ROI.
-    
+
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: from neuprint import NeuronCriteria as NC, SynapseCriteria as SC, fetch_synapses
                ...: fetch_synapses(NC(type='ADL.*', regex=True, rois=['FB']),
                ...:                SC(rois=['LH(R)', 'SIP(R)'], primary_only=True))
             Out[1]:
                     bodyId  type     roi      x      y      z  confidence
             0   5812983094   pre  SIP(R)  15300  25268  14043    0.992000
             1   5812983094   pre  SIP(R)  15300  25268  14043    0.992000
@@ -1378,28 +1375,28 @@
     q = f"""
         {neuron_criteria.global_with(prefix=8)}
         MATCH (n:{neuron_criteria.label})
         {neuron_criteria.all_conditions(prefix=8)}
         RETURN n.bodyId as bodyId
     """
     bodies = client.fetch_custom(q)['bodyId'].values
-    
+
     batch_dfs = []
     for batch_bodies in tqdm(iter_batches(bodies, batch_size)):
         batch_criteria = copy.copy(neuron_criteria)
         batch_criteria.bodyId = batch_bodies
         batch_df = _fetch_synapses(batch_criteria, synapse_criteria, client)
         batch_dfs.append( batch_df )
-    
+
     return pd.concat( batch_dfs, ignore_index=True )
 
 
 def _fetch_synapses(neuron_criteria, synapse_criteria, client):
     neuron_criteria.matchvar = 'n'
-    
+
     if synapse_criteria is None:
         synapse_criteria = SynapseCriteria()
 
     if synapse_criteria.primary_only:
         return_rois = {*client.primary_rois}
     else:
         return_rois = {*client.all_rois}
@@ -1418,15 +1415,15 @@
 
         MATCH (n)-[:Contains]->(ss:SynapseSet),
               (ss)-[:Contains]->(s:Synapse)
 
         {synapse_criteria.condition('n', 's', prefix=8)}
         // De-duplicate 's' because 'pre' synapses can appear in more than one SynapseSet
         WITH DISTINCT n, s
-        
+
         RETURN n.bodyId as bodyId,
                s.type as type,
                s.confidence as confidence,
                s.location.x as x,
                s.location.y as y,
                s.location.z as z,
                apoc.map.removeKeys(s, ['location', 'confidence', 'type']) as syn_info
@@ -1434,14 +1431,15 @@
     data = client.fetch_custom(cypher, format='json')['data']
 
     # Assemble DataFrame
     syn_table = []
     for body, syn_type, conf, x, y, z, syn_info in data:
         # Exclude non-primary ROIs if necessary
         syn_rois = return_rois & {*syn_info.keys()}
+        # Fixme: Filter for the user's ROIs (drop duplicates)
         for roi in syn_rois:
             syn_table.append((body, syn_type, roi, x, y, z, conf))
 
         if not syn_rois:
             syn_table.append((body, syn_type, None, x, y, z, conf))
 
     syn_df = pd.DataFrame(syn_table, columns=['bodyId', 'type', 'roi', 'x', 'y', 'z', 'confidence'])
@@ -1458,25 +1456,25 @@
 
 
 @inject_client
 @neuroncriteria_args('source_criteria', 'target_criteria')
 def fetch_synapse_connections(source_criteria=None, target_criteria=None, synapse_criteria=None, min_total_weight=1, batch_size=10, *, client=None):
     """
     Fetch synaptic-level connections between source and target neurons.
-    
+
     Note:
         Use this function if you need information about individual synapse connections,
         such as their exact positions or confidence scores.
         If you're just interested in aggregate neuron-to-neuron connection info
         (including connection strengths and ROI intersections), see
         :py:func:`fetch_simple_connections()` and :py:func:`fetch_adjacencies()`,
         which are faster and have more condensed outputs than this function.
-    
+
     Args:
-    
+
         source_criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             Criteria to by which to filter source (pre-synaptic) neurons.
             If omitted, all Neurons will be considered as possible sources.
 
             Note:
                 Any ROI criteria specified in this argument does not affect
                 which synapses are returned, only which bodies are inspected.
@@ -1490,28 +1488,28 @@
                 which synapses are returned, only which bodies are inspected.
 
         synapse_criteria (SynapseCriteria):
             Optional. Allows you to filter synapses by roi, type, confidence.
             The same criteria is used to filter both ``pre`` and ``post`` sides
             of the connection.
             By default, ``SynapseCriteria(primary_only=True)`` is used.
-            
+
             If ``primary_only`` is specified in the criteria, then the resulting
             ``roi_pre`` and ``roi_post`` columns will contain a single
             string (or ``None``) in every row.
-            
+
             Otherwise, the roi columns will contain a list of ROIs for every row.
             (Primary ROIs do not overlap, so every synapse resides in only one
             (or zero) primary ROI.)
             See :py:class:`.SynapseCriteria` for details.
 
         min_total_weight:
             If the total weight of the connection between two bodies is not at least
             this strong, don't include the synapses for that connection in the results.
-            
+
             Note:
                 This filters for total connection weight, regardless of the weight
                 within any particular ROI.  So, if your ``SynapseCriteria`` limits
                 results to a particular ROI, but two bodies connect in multiple ROIs,
                 then the number of synapses returned for the two bodies may appear to
                 be less than ``min_total_weight``. That's because you filtered out
                 the synapses in other ROIs.
@@ -1521,26 +1519,26 @@
             will be fetched in batches, split across N pre-synaptic bodies.
             This argument sets the batch size N.
 
         client:
             If not provided, the global default :py:class:`.Client` will be used.
 
     Returns:
-    
+
         DataFrame in which each row represents a single synaptic connection
         between an upstream (pre-synaptic) body and downstream (post-synaptic) body.
 
         Synapse locations are listed in columns ``[x_pre, y_pre, z_pre]`` and
         ``[x_post, y_post, z_post]`` for the upstream and downstream synapses,
         respectively.
 
         The ``roi_pre`` and ``roi_post`` columns will contain either strings
         or lists-of-strings, depending on the ``primary_only`` synapse criteria as
         described above.
-    
+
     Example:
 
         .. code-block:: ipython
 
             In [1]: from neuprint import fetch_synapse_connections, SynapseCriteria as SC
                ...: fetch_synapse_connections(792368888, None, SC(rois=['PED(R)', 'SMP(R)'], primary_only=True))
             Out[1]:
@@ -1563,48 +1561,60 @@
             15   792368888   1131831702  SMP(R)   SMP(R)  23630  29443  16297   23651   29434   16316           0.984         0.362952
     """
     assert source_criteria is not None or target_criteria is not None, \
         "Please specify either source or target search criteria (or both)."
 
     if synapse_criteria is None:
         synapse_criteria = SynapseCriteria(primary_only=True)
-    
+
     def prepare_nc(nc, matchvar):
         nc.matchvar = matchvar
-        
+
         # If the user specified rois to filter synapses by, but hasn't specified rois
         # in the NeuronCriteria, add them to the NeuronCriteria to speed up the query.
         if synapse_criteria.rois and not nc.rois:
             nc.rois = {*synapse_criteria.rois}
             nc.roi_req = 'any'
-    
+
         return nc
 
     source_criteria = prepare_nc(source_criteria, 'n')
     target_criteria = prepare_nc(target_criteria, 'm')
 
-    _neuron_df, roi_conn_df = fetch_adjacencies(source_criteria, target_criteria, synapse_criteria.rois, 1, min_total_weight, properties=[])
-    conn_df = roi_conn_df.drop_duplicates(['bodyId_pre', 'bodyId_post']).sort_values(['bodyId_pre', 'bodyId_post'])
-    
+    # Fetch the list of neuron-neuron pairs in advance so we can break into batches.
+    _neuron_df, roi_conn_df = fetch_adjacencies( source_criteria,
+                                                 target_criteria,
+                                                 synapse_criteria.rois,
+                                                 1,
+                                                 min_total_weight,
+                                                 properties=[] )
+
+    conn_df = (roi_conn_df.drop_duplicates(['bodyId_pre', 'bodyId_post'])
+                          .sort_values(['bodyId_pre', 'bodyId_post']))
+
+    # Fetch in batches
     syn_dfs = []
-    
     conn_groups = [*conn_df.groupby('bodyId_pre')]
     for group in iter_batches(conn_groups, batch_size):
         _, group_dfs = zip(*group)
         batch_conn_df = pd.concat(group_dfs, ignore_index=True)
         source_criteria.bodyId = batch_conn_df['bodyId_pre'].unique()
         target_criteria.bodyId = batch_conn_df['bodyId_post'].unique()
-        
-        batch_syn_df = _fetch_synapse_connections(source_criteria, target_criteria, synapse_criteria, min_total_weight, client)
+
+        batch_syn_df = _fetch_synapse_connections( source_criteria,
+                                                   target_criteria,
+                                                   synapse_criteria,
+                                                   min_total_weight,
+                                                   client )
         syn_dfs.append(batch_syn_df)
-    
+
     syn_df = pd.concat(syn_dfs, ignore_index=True)
     assert syn_df.duplicated(syn_df.columns).sum() == 0
     return syn_df
-        
+
 
 def _fetch_synapse_connections(source_criteria, target_criteria, synapse_criteria, min_total_weight, client):
     if synapse_criteria.primary_only:
         return_rois = {*client.primary_rois}
     else:
         return_rois = {*client.all_rois}
 
@@ -1614,15 +1624,15 @@
     source_syn_crit.matchvar = 'ns'
     target_syn_crit.matchvar = 'ms'
 
     source_syn_crit.type = 'pre'
     target_syn_crit.type = 'post'
 
     criteria_globals = [*source_criteria.global_vars().keys(), *target_criteria.global_vars().keys()]
-    
+
     # Fetch results
     cypher = dedent(f"""\
         {NeuronCriteria.combined_global_with((source_criteria, target_criteria), prefix=8)}
         MATCH (n:{source_criteria.label})-[e:ConnectsTo]->(m:{target_criteria.label}),
               (n)-[:Contains]->(nss:SynapseSet),
               (m)-[:Contains]->(mss:SynapseSet),
               (nss)-[:ConnectsTo]->(mss),
@@ -1634,21 +1644,21 @@
 
         // Artificial break in the query flow to fool the query
         // planner into avoiding a Cartesian product.
         // This improves performance considerably in some cases.
         WITH {','.join(['n', 'e', 'm', 'ns', 'ms', *criteria_globals])}, true as _
 
         {target_criteria.all_conditions('n', 'e', 'm', 'ns', 'ms', prefix=8)}
-        
+
         WITH n, m, ns, ms, e
         WHERE e.weight >= {min_total_weight}
 
         {source_syn_crit.condition('n', 'm', 'ns', 'ms', prefix=8)}
         {target_syn_crit.condition('n', 'm', 'ns', 'ms', prefix=8)}
-        
+
         RETURN n.bodyId as bodyId_pre,
                m.bodyId as bodyId_post,
                ns.location.x as ux,
                ns.location.y as uy,
                ns.location.z as uz,
                ms.location.x as dx,
                ms.location.y as dy,
@@ -1675,15 +1685,15 @@
         post_rois = post_rois or [None]
 
         # Should be (at most) one ROI when primary_only=True,
         # so only show that one (not a list)
         if synapse_criteria.primary_only:
             pre_rois = pre_rois[0]
             post_rois = post_rois[0]
-        
+
         syn_table.append((bodyId_pre, bodyId_post, pre_rois, post_rois, ux, uy, uz, dx, dy, dz, up_conf, dn_conf))
 
     syn_df = pd.DataFrame(syn_table, columns=['bodyId_pre', 'bodyId_post',
                                               'roi_pre', 'roi_post',
                                               'x_pre', 'y_pre', 'z_pre', 'x_post', 'y_post', 'z_post',
                                               'confidence_pre', 'confidence_post'])
 
@@ -1703,35 +1713,35 @@
 @inject_client
 @neuroncriteria_args('criteria')
 def fetch_output_completeness(criteria, batch_size=1000, *, client=None):
     """
     Compute an estimate of "output completeness" for a set of neurons.
     Output completeness is defined as the fraction of post-synaptic
     connections which belong to Traced neurons.
-    
+
     Args:
         criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             Defines the set of neurons for which output completeness should be computed.
     Returns:
         DataFrame with columns ``['bodyId', 'completeness', 'traced_weight', 'untraced_weight', 'total_weight']``
     """
     assert isinstance(criteria, NeuronCriteria)
     criteria.matchvar = 'n'
 
     if batch_size is None:
         return _fetch_output_completeness(criteria, client)
-    
+
     q = f"""\
         {criteria.global_with(prefix=8)}
         MATCH (n:{criteria.label})
         {criteria.all_conditions(prefix=8)}
         RETURN n.bodyId as bodyId
     """
     bodies = fetch_custom(q)['bodyId']
-    
+
     batch_results = []
     for start in trange(0, len(bodies), batch_size):
         criteria.bodyId = bodies[start:start+batch_size]
         batch_results.append( _fetch_output_completeness(criteria, client) )
     return pd.concat( batch_results, ignore_index=True )
 
 
@@ -1752,46 +1762,46 @@
         RETURN n.bodyId as bodyId,
                total_weight,
                sum(e2.weight) as traced_weight
     """
     completion_stats_df = client.fetch_custom(q)
     completion_stats_df['untraced_weight'] = completion_stats_df.eval('total_weight - traced_weight')
     completion_stats_df['completeness'] = completion_stats_df.eval('traced_weight / total_weight')
-    
+
     return completion_stats_df[['bodyId', 'total_weight', 'traced_weight', 'untraced_weight', 'completeness']]
 
 
 @inject_client
 @neuroncriteria_args('criteria')
 def fetch_downstream_orphan_tasks(criteria, *, client=None):
     """
     Fetch the set of "downstream orphans" for a given set of neurons.
-    
+
     Returns a single DataFrame, where the downstream orphans have
     been sorted by the weight of the connection, and their cumulative
     contributions to the overall output-completeness of the upstream
     neuron is also given.
-    
+
     That is, if you started tracing orphans from this DataFrame in
     order, then the ``cum_completeness`` column indicates how complete
     the upstream body is after each orphan becomes traced.
-    
+
     Args:
         criteria (bodyId(s), type/instance, or :py:class:`.NeuronCriteria`):
             Determines the set of "upstream" bodies for which
             downstream orphans should be identified.
-    
+
     Returns:
         DataFrame, where ``bodyId_pre`` contains the upstream bodies you specified
         via ``criteria``, and ``bodyId_post`` contains the list of downstream orphans.
-    
+
     Example:
-    
+
         .. code-block:: ipython
-        
+
             In [1]: orphan_tasks = fetch_downstream_orphan_tasks(NC(status='Traced', cropped=False, rois=['PB']))
 
             In [1]: orphan_tasks.query('cum_completeness < 0.2').head(10)
             Out[1]:
                    bodyId_pre  bodyId_post  orphan_weight status_post  total_weight  orig_traced_weight  orig_untraced_weight  orig_completeness  cum_orphan_weight  cum_completeness
             6478    759685279    759676733              2      Assign          7757                1427                  6330           0.183963                  2          0.184221
             8932    759685279    913193340              1        None          7757                1427                  6330           0.183963                  3          0.184350
```

### Comparing `neuprint-python-0.4.8/neuprint/synapsecriteria.py` & `neuprint-python-0.4.9/neuprint/synapsecriteria.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,34 @@
         """
         Except for ``matchvar``, all parameters must be passed as keyword arguments.
 
         Args:
             matchvar (str):
                 An arbitrary cypher variable name to use when this
                 ``SynapseCriteria`` is used to construct cypher queries.
-        
+
             rois (str or list):
                 Optional.
                 If provided, limit the results to synapses that reside within the given roi(s).
-    
+
             type:
                 If provided, limit results to either 'pre' or 'post' synapses.
-    
+
             confidence (float, 0.0-1.0):
                 Limit results to synapses of at least this confidence rating.
-    
+
             primary_only (boolean):
                 If True, only include primary ROI names in the results.
 
                 Note:
                     This parameter does NOT filter by ROI. (See the ``rois`` argument for that.)
                     It merely determines whether or each synapse should be associated with exactly
                     one ROI in the query output, or with multiple ROIs (one for every non-primary
                     ROI the synapse intersects).
-    
+
             client:
                 Used to validate ROI names.
                 If not provided, the global default :py:class:`.Client` will be used.
         """
         unknown_rois = {*rois} - {*client.all_rois}
         assert not unknown_rois, f"Unrecognized synapse rois: {unknown_rois}"
 
@@ -51,33 +51,33 @@
             f"Invalid synapse type: {type}.  Choices are 'pre' and 'post'."
 
         self.matchvar = matchvar
         self.rois = rois
         self.type = type
         self.confidence = confidence
         self.primary_only = primary_only
-        
-    
+
+
     def condition(self, *vars, prefix='', comments=True):
         """
         Construct a cypher WITH..WHERE clause to filter for synapse criteria.
-        
+
         Any match variables you wish to "carry through" for subsequent clauses
         in your query must be named in the ``vars`` arguments.
         """
         if not vars:
             vars = [self.matchvar]
-        
+
         assert self.matchvar in vars, \
             ("Please pass all match vars, including the one that "
              f"belongs to this criteria ('{self.matchvar}').")
-        
+
         if isinstance(prefix, int):
             prefix = ' '*prefix
-        
+
         roi_expr = conf_expr = type_expr = ""
         if self.rois:
             roi_expr = '(' + ' OR '.join([f'{self.matchvar}.`{roi}`' for roi in self.rois]) + ')'
 
         if self.confidence:
             conf_expr = f'({self.matchvar}.confidence > {self.confidence})'
 
@@ -107,27 +107,27 @@
                 and (self.type == other.type)
                 and (self.confidence == other.confidence)
                 and (self.primary_only == other.primary_only))
 
 
     def __repr__(self):
         s = f"SynapseCriteria('{self.matchvar}'"
-        
+
         args = []
-        
+
         if self.rois:
             args.append("rois=[" + ", ".join(f"'{roi}'" for roi in self.rois) + "]")
-        
+
         if self.type:
             args.append(f"type='{self.type}'")
-        
+
         if self.confidence:
             args.append(f"confidence={self.confidence}")
-        
+
         if self.primary_only:
             args.append("primary_only=True")
-        
+
         if args:
             s += ', ' + ', '.join(args)
-        
+
         s += ")"
         return s
```

### Comparing `neuprint-python-0.4.8/neuprint/tests/test_client.py` & `neuprint-python-0.4.9/neuprint/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import pytest
 import pandas as pd
-from neuprint import Client, default_client, set_default_client, inject_client
+from neuprint import Client, default_client, set_default_client
+from neuprint.client import inject_client
 from neuprint.tests import NEUPRINT_SERVER, DATASET
 
 EXAMPLE_BODY = 5813037876 # Delta6G, Delta6G_04, Traced, non-cropped
 
 
 def test_members():
     set_default_client(None)
     assert default_client() is None
     c = Client(NEUPRINT_SERVER, DATASET)
     assert c.server == f'https://{NEUPRINT_SERVER}'
     assert c.dataset == DATASET
-    
+
     assert default_client() is c
-    
+
     df = c.fetch_custom("MATCH (m:Meta) RETURN m.primaryRois as rois")
     assert isinstance(df, pd.DataFrame)
     assert df.columns == ['rois']
     assert len(df) == 1
     assert isinstance(df['rois'].iloc[0], list)
-    
-    
+
+
     assert isinstance(c.fetch_available(), list)
     assert isinstance(c.fetch_help(), str)
     assert c.fetch_server_info() is True
     assert isinstance(c.fetch_version(), str)
     assert isinstance(c.fetch_database(), dict)
     assert isinstance(c.fetch_datasets(), dict)
     assert isinstance(c.fetch_db_version(), str)
@@ -49,19 +50,19 @@
 
 
 @pytest.mark.xfail
 def test_broken_members():
     """
     These endpoints are listed in the neuprintHTTP API,
     but don't seem to work.
-    """    
+    """
     c = Client(NEUPRINT_SERVER, DATASET)
 
     # Broken. neuprint returns error 500
-    assert isinstance(c.fetch_instances(), list) 
+    assert isinstance(c.fetch_instances(), list)
 
 
 @pytest.mark.skip
 def test_keyvalue():
     # TODO:
     # What is an appropriate key/value to test with?
     c = Client(NEUPRINT_SERVER, DATASET)
@@ -74,17 +75,22 @@
     c2 = Client(NEUPRINT_SERVER, DATASET)
 
     set_default_client(c)
 
     @inject_client
     def f(*, client):
         return client
-    
+
     # Uses default client unless client was specified
     assert f() is c
     assert f(client=c2) is c2
 
     with pytest.raises(AssertionError):
         # Wrong signature -- asserts
         @inject_client
         def f2(client):
             pass
+
+if __name__ == "__main__":
+    args = ['-s', '--tb=native', '--pyargs', 'neuprint.tests.test_client']
+    #args += ['-k', 'fetch_skeleton']
+    pytest.main(args)
```

### Comparing `neuprint-python-0.4.8/neuprint/tests/test_neuroncriteria.py` & `neuprint-python-0.4.9/neuprint/tests/test_neuroncriteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def test_NeuronCriteria(client):
     ##
     ## basic_exprs()
     ##
     assert NC(bodyId=123).basic_exprs() == ["n.bodyId = 123"]
     assert NC('m', bodyId=123).basic_exprs() == ["m.bodyId = 123"]
     assert NC(bodyId=[123, 456]).basic_exprs() == ["n.bodyId in [123, 456]"]
-    
+
     assert NC(instance="foo").basic_exprs() == ["n.instance = 'foo'"]
     assert NC(instance="foo", regex=True).basic_exprs() == ["n.instance =~ 'foo'"]
     assert NC(instance=["foo", "bar"]).basic_exprs() == ["n.instance in ['foo', 'bar']"]
     with pytest.raises(AssertionError):
         NC(instance=["foo", "bar"], regex=True).basic_exprs()
 
     assert NC(type="foo").basic_exprs() == ["n.type = 'foo'"]
@@ -52,15 +52,15 @@
 
     ##
     ## basic_conditions()
     ##
     assert NC().basic_conditions() == ""
     assert NC().all_conditions() == ""
     assert NC.combined_conditions([NC(), NC(), NC()]) == ""
-    
+
 
     bodies = [1,2,3]
     assert NC(bodyId=bodies).basic_conditions(comments=False) == "n.bodyId in [1, 2, 3]"
 
     bodies = [1,2,3,4,5]
     nc = NC(bodyId=bodies)
     assert nc.global_with() == dedent(f"""\
```

### Comparing `neuprint-python-0.4.8/neuprint/tests/test_queries.py` & `neuprint-python-0.4.9/neuprint/tests/test_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # This works but takes a long time.
     #neurons, roi_counts = fetch_neurons(NC())
 
     neurons, roi_counts = fetch_neurons(NC(bodyId=bodyId))
     assert len(neurons) == len(bodyId)
     assert set(roi_counts['bodyId']) == set(bodyId)
-    
+
     neurons, roi_counts = fetch_neurons(NC(instance='APL_R'))
     assert len(neurons) == 1, "There's only one APL neuron in the hemibrain"
     assert neurons.loc[0, 'type'] == "APL"
     assert neurons.loc[0, 'instance'] == "APL_R"
 
     neurons, roi_counts = fetch_neurons(NC(instance='APL[^ ]*', regex=True))
     assert len(neurons) == 1, "There's only one APL neuron in the hemibrain"
@@ -51,16 +51,16 @@
     neurons, roi_counts = fetch_neurons(NC(type='APL.*', regex=True))
     assert len(neurons) == 1, "There's only one APL neuron in the hemibrain"
     assert neurons.loc[0, 'type'] == "APL"
     assert neurons.loc[0, 'instance'] == "APL_R"
 
     neurons, roi_counts = fetch_neurons(NC(status=['Traced', 'Orphan'], cropped=False))
     assert neurons.eval('status == "Traced" or status == "Orphan"').all()
-    assert not neurons['cropped'].any() 
-    
+    assert not neurons['cropped'].any()
+
     neurons, roi_counts = fetch_neurons(NC(inputRois='AL(R)', outputRois='SNP(R)'))
     assert all(['AL(R)' in rois for rois in neurons['inputRois']])
     assert all(['SNP(R)' in rois for rois in neurons['outputRois']])
     assert sorted(roi_counts.query('roi == "AL(R)" and post > 0')['bodyId']) == sorted(neurons['bodyId'])
     assert sorted(roi_counts.query('roi == "SNP(R)" and pre > 0')['bodyId']) == sorted(neurons['bodyId'])
 
     neurons, roi_counts = fetch_neurons(NC(min_pre=1000, min_post=2000))
@@ -72,15 +72,15 @@
               424379864, 425790257, 451982486, 480927537, 481268653]
 
     conn_df = fetch_simple_connections(NC(bodyId=bodyId))
     assert set(conn_df['bodyId_pre'].unique()) == set(bodyId)
 
     conn_df = fetch_simple_connections(None, NC(bodyId=bodyId))
     assert set(conn_df['bodyId_post'].unique()) == set(bodyId)
-    
+
     APL_R = 425790257
 
     conn_df = fetch_simple_connections(NC(instance='APL_R'))
     assert (conn_df['bodyId_pre'] == APL_R).all()
 
     conn_df = fetch_simple_connections(NC(type='APL'))
     assert (conn_df['bodyId_pre'] == APL_R).all()
@@ -90,15 +90,15 @@
 
     conn_df = fetch_simple_connections(None, NC(type='APL'))
     assert (conn_df['bodyId_post'] == APL_R).all()
 
     conn_df = fetch_simple_connections(NC(bodyId=APL_R), min_weight=10)
     assert (conn_df['bodyId_pre'] == APL_R).all()
     assert (conn_df['weight'] >= 10).all()
-    
+
     conn_df = fetch_simple_connections(NC(bodyId=APL_R), min_weight=10, properties=['somaLocation'])
     assert 'somaLocation_pre' in conn_df
     assert 'somaLocation_post' in conn_df
 
     conn_df = fetch_simple_connections(NC(bodyId=APL_R), min_weight=10, properties=['roiInfo'])
     assert 'roiInfo_pre' in conn_df
     assert 'roiInfo_post' in conn_df
@@ -158,20 +158,20 @@
 
 
 def test_fetch_synapses(client):
     nc = NC(type='ADL.*', regex=True, rois=['FB'])
     sc = SC(rois=['LH(R)', 'SIP(R)'], primary_only=True)
     syn_df = fetch_synapses(nc, sc)
     assert set(syn_df['roi']) == {'LH(R)', 'SIP(R)'}
-    
+
     neuron_df, _count_df = fetch_neurons(nc)
     syn_df = syn_df.merge(neuron_df[['bodyId', 'type']], 'left', on='bodyId', suffixes=['_syn', '_body'])
     assert syn_df['type_body'].isnull().sum() == 0
     assert syn_df['type_body'].apply(lambda s: s.startswith('ADL')).all()
-    
+
 
 def test_fetch_synapse_connections(client):
     rois = ['PED(R)', 'SMP(R)']
     syn_df = fetch_synapse_connections(792368888, None, SC(rois=rois, primary_only=True))
     assert syn_df.eval('roi_pre in @rois and roi_post in @rois').all()
```

### Comparing `neuprint-python-0.4.8/neuprint/tests/test_utils.py` & `neuprint-python-0.4.9/neuprint/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     assert make_iterable(1) == [1]
     assert make_iterable([1]) == [1]
 
     assert isinstance(make_iterable(np.array([1,2,3])), np.ndarray)
 
 
 def test_make_args_iterable():
-    
+
     @make_args_iterable(['a', 'c', 'd'])
     def f(a, b, c, d='d', *, e=None):
         return (a,b,c,d,e)
 
-    # Must preserve function signature    
+    # Must preserve function signature
     spec = inspect.getfullargspec(f)
     assert spec.args == ['a', 'b', 'c', 'd']
     assert spec.defaults == ('d',)
     assert spec.kwonlyargs == ['e']
     assert spec.kwonlydefaults == {'e': None}
-    
+
     # Check results
     assert f('a', 'b', 'c', 'd') == (['a'], 'b', ['c'], ['d'], None)
```

### Comparing `neuprint-python-0.4.8/neuprint/utils.py` & `neuprint-python-0.4.9/neuprint/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Utility functions for manipulating neuprint-python output.
 """
 import sys
 import inspect
 import functools
+import warnings
+from textwrap import dedent
 from itertools import combinations
 from collections import namedtuple
 from collections.abc import Iterable, Iterator, Collection
 
 import numpy as np
 import pandas as pd
 import networkx as nx
@@ -17,53 +19,90 @@
 # Import the notebook-aware version of tqdm if
 # we appear to be running within a notebook context.
 #
 try:
     import ipykernel.iostream
     if isinstance(sys.stdout, ipykernel.iostream.OutStream):
         from tqdm.notebook import tqdm
+
+        try:
+            import ipywidgets
+            ipywidgets
+        except ImportError:
+            msg = dedent("""\
+
+                Progress bar will not work well in the notebook without ipywidgets.
+                Run the following commands (for notebook and jupyterlab users):
+
+                    conda install -c conda-forge ipywidgets
+                    jupyter nbextension enable --py widgetsnbextension
+                    jupyter labextension install @jupyter-widgets/jupyterlab-manager
+
+                ...and then reload your jupyter session, and restart your kernel.
+            """)
+            warnings.warn(msg)
     else:
         from tqdm import tqdm
+
 except ImportError:
     from tqdm import tqdm
 
 
 class tqdm(tqdm):
     """
     Same as tqdm, but auto-disable the progress bar if there's only one item.
     """
     def __init__(self, iterable=None, *args, disable=None, **kwargs):
         if disable is None:
             disable = (iterable is not None
                        and hasattr(iterable, '__len__')
                        and len(iterable) <= 1)
-        
+
         super().__init__(iterable, *args, disable=disable, **kwargs)
 
 
 def trange(*args, **kwargs):
     return tqdm(range(*args), **kwargs)
 
 
+def UMAP(*args, **kwargs):
+    """
+    UMAP is an optional dependency, so this wrapper emits
+    a nicer error message if it's not available.
+    """
+    try:
+        from umap import UMAP
+    except ImportError as ex:
+        msg = (
+            "The 'umap' dimensionality reduction package is required for some "
+            "plotting functionality, but it isn't currently installed.\n\n"
+            "Please install it:\n\n"
+            "  conda install -c conda-forge umap-learn\n\n"
+        )
+        raise RuntimeError(msg) from ex
+
+    return UMAP(*args, **kwargs)
+
+
 def make_iterable(x):
     """
     If ``x`` is already a list or array, return it unchanged.
     If ``x`` is Series, return its values.
     If ``x`` is ``None``, return an empty list ``[]``.
     Otherwise, wrap it in a list.
     """
     if x is None:
         return []
-    
+
     if isinstance(x, np.ndarray):
         return x
-    
+
     if isinstance(x, pd.Series):
         return x.values
-    
+
     if isinstance(x, Collection) and not isinstance(x, str):
         return x
     else:
         return [x]
 
 
 def make_args_iterable(argnames):
@@ -87,51 +126,51 @@
     return decorator
 
 
 @make_args_iterable(['properties'])
 def merge_neuron_properties(neuron_df, conn_df, properties=['type', 'instance']):
     """
     Merge neuron properties to a connection table.
-    
+
     Given a table of neuron properties and a connection table, append
     ``_pre`` and ``_post`` columns to the connection table for each of
     the given properties via the appropriate merge operations.
-    
+
     Args:
         neuron_df:
             DataFrame with columns for 'bodyId' and any properties you want to merge
-        
+
         conn_df:
             DataFrame with columns ``bodyId_pre`` and ``bodyId_post``
-        
+
         properties:
             Column names from ``neuron_df`` to merge onto ``conn_df``.
-    
+
     Returns:
         Updated ``conn_df`` with new columns.
-    
+
     Example:
-    
+
         .. code-block:: ipython
-    
+
             In [1]: from neuprint import fetch_adjacencies, NeuronCriteria as NC, merge_neuron_properties
                ...: neuron_df, conn_df = fetch_adjacencies(rois='PB', min_roi_weight=120)
                ...: print(conn_df)
                bodyId_pre  bodyId_post roi  weight
             0   880875736   1631450739  PB     123
             1   880880259    849421763  PB     141
             2   910442723    849421763  PB     139
             3   910783961   5813070465  PB     184
             4   911129204    724280817  PB     127
             5   911134009    849421763  PB     125
             6   911565419   5813070465  PB     141
             7   911911004   1062526223  PB     125
             8   911919044    973566036  PB     122
             9  5813080838    974239375  PB     136
-            
+
             In [2]: merge_neuron_properties(neuron_df, conn_df, 'type')
             Out[2]:
                bodyId_pre  bodyId_post roi  weight  type_pre    type_post
             0   880875736   1631450739  PB     123  Delta7_a  PEN_b(PEN2)
             1   880880259    849421763  PB     141  Delta7_a  PEN_b(PEN2)
             2   910442723    849421763  PB     139  Delta7_a  PEN_b(PEN2)
             3   910783961   5813070465  PB     184  Delta7_a  PEN_b(PEN2)
@@ -139,17 +178,17 @@
             5   911134009    849421763  PB     125  Delta7_a  PEN_b(PEN2)
             6   911565419   5813070465  PB     141  Delta7_a  PEN_b(PEN2)
             7   911911004   1062526223  PB     125  Delta7_b  PEN_b(PEN2)
             8   911919044    973566036  PB     122  Delta7_a  PEN_b(PEN2)
             9  5813080838    974239375  PB     136       EPG          PEG
     """
     neuron_df = neuron_df[['bodyId', *properties]]
-    
+
     newcols  = [f'{prop}_pre'  for prop in properties]
-    newcols += [f'{prop}_post' for prop in properties]    
+    newcols += [f'{prop}_post' for prop in properties]
     conn_df = conn_df.drop(columns=newcols, errors='ignore')
 
     conn_df = conn_df.merge(neuron_df, 'left', left_on='bodyId_pre', right_on='bodyId')
     del conn_df['bodyId']
 
     conn_df = conn_df.merge(neuron_df, 'left', left_on='bodyId_post', right_on='bodyId',
                             suffixes=['_pre', '_post'])
@@ -157,102 +196,102 @@
 
     return conn_df
 
 
 def connection_table_to_matrix(conn_df, group_cols='bodyId', weight_col='weight', sort_by=None):
     """
     Given a weighted connection table, produce a weighted adjacency matrix.
-    
+
     Args:
         conn_df:
             A DataFrame with columns for pre- and post- identifiers
             (e.g. bodyId, type or instance), and a column for the
             weight of the connection.
-        
+
         group_cols:
             Which two columns to use as the row index and column index
             of the returned matrix, respetively.
             Or give a single string (e.g. ``"body"``, in which case the
             two column names are chosen by appending the suffixes
             ``_pre`` and ``_post`` to your string.
 
             If a pair of pre/post values occurs more than once in the
             connection table, all of its weights will be summed in the
             output matrix.
-        
+
         weight_col:
             Which column holds the connection weight, to be aggregated for each unique pre/post pair.
-            
+
         sort_by:
             How to sort the rows and columns of the result.
             Can be two strings, e.g. ``("type_pre", "type_post")``,
             or a single string, e.g. ``"type"`` in which case the suffixes are assumed.
-            
+
     Returns:
         DataFrame, shape NxM, where N is the number of unique values in
         the 'pre' group column, and M is the number of unique values in
         the 'post' group column.
-    
+
     Example:
-    
+
         .. code-block:: ipython
-        
-            In [1]: from neuprint import fetch_simple_connections, NeuronCriteria as NC  
+
+            In [1]: from neuprint import fetch_simple_connections, NeuronCriteria as NC
                ...: kc_criteria = NC(type='KC.*', regex=True)
                ...: conn_df = fetch_simple_connections(kc_criteria, kc_criteria)
             In [1]: conn_df.head()
             Out[1]:
                bodyId_pre  bodyId_post  weight type_pre type_post instance_pre instance_post                                       conn_roiInfo
             0  1224137495   5813032771      29      KCg       KCg          KCg    KCg(super)  {'MB(R)': {'pre': 26, 'post': 26}, 'gL(R)': {'...
             1  1172713521   5813067826      27      KCg       KCg   KCg(super)         KCg-d  {'MB(R)': {'pre': 26, 'post': 26}, 'PED(R)': {...
             2   517858947   5813032943      26   KCab-p    KCab-p       KCab-p        KCab-p  {'MB(R)': {'pre': 25, 'post': 25}, 'PED(R)': {...
             3   642680826   5812980940      25   KCab-p    KCab-p       KCab-p        KCab-p  {'MB(R)': {'pre': 25, 'post': 25}, 'PED(R)': {...
             4  5813067826   1172713521      24      KCg       KCg        KCg-d    KCg(super)  {'MB(R)': {'pre': 23, 'post': 23}, 'gL(R)': {'...
-    
+
             In [2]: from neuprint.utils import connection_table_to_matrix
                ...: connection_table_to_matrix(conn_df, 'type')
             Out[2]:
             type_post   KC  KCa'b'  KCab-p  KCab-sc     KCg
             type_pre
             KC           3     139       6        5     365
             KCa'b'     154  102337     245      997    1977
             KCab-p       7     310   17899     3029     127
             KCab-sc      4    2591    3975   247038    3419
             KCg        380    1969      79     1526  250351
     """
     if isinstance(group_cols, str):
-        group_cols = (f"{group_cols}_pre", f"{group_cols}_post") 
-    
+        group_cols = (f"{group_cols}_pre", f"{group_cols}_post")
+
     assert len(group_cols) == 2, \
         "Please provide two group_cols (e.g. 'bodyId_pre', 'bodyId_post')"
-    
+
     assert group_cols[0] in conn_df, \
         f"Column missing: {group_cols[0]}"
 
     assert group_cols[1] in conn_df, \
         f"Column missing: {group_cols[1]}"
-        
+
     assert weight_col in conn_df, \
         f"Column missing: {weight_col}"
-    
+
     col_pre, col_post = group_cols
     dtype = conn_df[weight_col].dtype
 
     grouped = conn_df.groupby([col_pre, col_post], as_index=False, sort=False)
     agg_weights_df = grouped[weight_col].sum()
     matrix = agg_weights_df.pivot(col_pre, col_post, weight_col)
     matrix = matrix.fillna(0).astype(dtype)
-    
+
     if sort_by:
         if isinstance(sort_by, str):
-            sort_by = (f"{sort_by}_pre", f"{sort_by}_post") 
+            sort_by = (f"{sort_by}_pre", f"{sort_by}_post")
 
         assert len(sort_by) == 2, \
             "Please provide two sort_by column names (e.g. 'type_pre', 'type_post')"
-        
+
         pre_order = conn_df.sort_values(sort_by[0])[col_pre].unique()
         post_order = conn_df.sort_values(sort_by[1])[col_post].unique()
         matrix = matrix.reindex(index=pre_order, columns=post_order)
     else:
         # No sort: Keep the order as close to the input order as possible.
         pre_order = conn_df[col_pre].unique()
         post_order = conn_df[col_post].unique()
@@ -260,54 +299,54 @@
 
     return matrix
 
 
 def iter_batches(it, batch_size):
     """
     Iterator.
-    
+
     Consume the given iterator/iterable in batches and
     yield each batch as a list of items.
-    
+
     The last batch might be smaller than the others,
     if there aren't enough items to fill it.
-    
+
     If the given iterator supports the __len__ method,
     the returned batch iterator will, too.
     """
     if hasattr(it, '__len__'):
         return _iter_batches_with_len(it, batch_size)
     else:
         return _iter_batches(it, batch_size)
 
 
 class _iter_batches:
     def __init__(self, it, batch_size):
         self.base_iterator = it
         self.batch_size = batch_size
-                
+
 
     def __iter__(self):
         return self._iter_batches(self.base_iterator, self.batch_size)
-    
+
 
     def _iter_batches(self, it, batch_size):
         if isinstance(it, (pd.DataFrame, pd.Series)):
             for batch_start in range(0, len(it), batch_size):
                 yield it.iloc[batch_start:batch_start+batch_size]
             return
         elif isinstance(it, (list, np.ndarray)):
             for batch_start in range(0, len(it), batch_size):
                 yield it[batch_start:batch_start+batch_size]
             return
         else:
             if not isinstance(it, Iterator):
                 assert isinstance(it, Iterable)
                 it = iter(it)
-    
+
             while True:
                 batch = []
                 try:
                     for _ in range(batch_size):
                         batch.append(next(it))
                 except StopIteration:
                     return
@@ -320,135 +359,146 @@
     def __len__(self):
         return int(np.ceil(len(self.base_iterator) / self.batch_size))
 
 
 def skeleton_df_to_nx(df, with_attributes=True, directed=True):
     """
     Convert a skeleton DataFrame into a ``networkx`` graph.
-    
+
     Args:
         df:
             DataFrame as returned by :py:meth:`.Client.fetch_skeleton()`
-        
+
         with_attributes:
             If True, store node attributes for x, y, z, radius
-        
+
         directed:
             If True, return ``nx.DiGraph``, otherwise ``nx.Graph``.
-    
+
     Returns:
         ``nx.DiGraph`` or ``nx.Graph``
     """
     if directed:
         g = nx.DiGraph()
     else:
         g = nx.Graph()
-    
+
     if with_attributes:
         for row in df.itertuples(index=False):
             g.add_node(row.rowId, x=row.x, y=row.y, z=row.z, radius=row.radius)
             if row.link != -1:
                 g.add_edge(row.link, row.rowId)
     else:
         df = df[['rowId', 'link']].sort_values(['rowId', 'link'])
         g.add_nodes_from(df['rowId'].sort_values())
         g.add_edges_from(df.query('link != -1').values)
+
     return g
 
 
 def skeleton_df_to_swc(df, export_path=None):
     """
     Convert a skeleton DataFrame into a the text of an SWC file.
-    
+
     Args:
         df:
             DataFrame, as returned by :py:meth:`.Client.fetch_skeleton()`
-        
+
         export_path:
             Optional. Write the SWC file to disk a the given location.
-    
+
     Returns:
         string
     """
     df['node_type'] = 0
     df = df[['rowId', 'node_type', 'x', 'y', 'z', 'radius', 'link']]
     swc = "# "
     swc += df.to_csv(sep=' ', header=True, index=False)
-    
+
     if export_path:
         with open(export_path, 'w') as f:
             f.write(swc)
 
     return swc
 
-    
+
 def heal_skeleton(skeleton_df):
     """
+    Ensure a skeleton consists of a single connected component.
+
     Rather than a single tree, skeletons from neuprint sometimes
     consist of multiple fragments, i.e. multiple connected
     components.  That's due to artifacts in the underlying
     segmentation from which the skeletons were generated.
     In such skeletons, there will be multiple 'root' nodes
     (SWC rows where ``link == -1``).
-    
-    This function 'heals' a fragmented skeleton by joining its 
-    fragments into a single tree. The fragments are joined by
-    selecting the minimum spanning tree after joining all fragments
-    via their pairwise nearest neighbors.
-    
+
+    This function 'heals' a fragmented skeleton by joining its
+    fragments into a single tree.
+
+    First, each fragment is joined to every other fragment at
+    their nearest points. The resulting graph has unnecessary
+    edges, which are then removed by extracting the minimum
+    spanning tree.  The MST is returned as the healed skeleton.
+
     Args:
         skeleton_df:
             DataFrame as returned by :py:meth:`.Client.fetch_skeleton()`
-    
+
     Returns:
         DataFrame, with ``link`` column updated with updated edges.
     """
-    skeleton_df = (skeleton_df.sort_values('rowId').reset_index(drop=True))
+    skeleton_df = skeleton_df.sort_values('rowId').reset_index(drop=True)
     g = skeleton_df_to_nx(skeleton_df, False, False)
 
     # Extract each fragment's rows and construct a KD-Tree
-    CC = namedtuple('CC', ['i', 'df', 'kd'])
-    ccs = []
-    for i, cc in enumerate(nx.connected_components(g)):
+    Fragment = namedtuple('Fragment', ['frag_id', 'df', 'kd'])
+    fragments = []
+    for frag_id, cc in enumerate(nx.connected_components(g)):
         if len(cc) == len(skeleton_df):
             # There's only one component -- no healing necessary
             return skeleton_df
-        
+
         df = skeleton_df.query('rowId in @cc')
         kd = cKDTree(df[[*'xyz']].values)
-        ccs.append( CC(i, df, kd) )
+        fragments.append( Fragment(frag_id, df, kd) )
 
     # Sort from big-to-small, so the calculations below use a
     # KD tree for the larger point set in every fragment pair.
-    ccs = sorted(ccs, key=lambda cc: -len(cc.df))
-    
+    fragments = sorted(fragments, key=lambda frag: -len(frag.df))
+
     # We could use the full graph and connect all
     # fragment pairs at their nearest neighbors,
     # but it's faster to treat each fragment as a
     # single node and run MST on that quotient graph,
     # which is tiny.
     frag_graph = nx.Graph()
-    for cc_a, cc_b in combinations(ccs, 2):
-        coords_b = cc_b.df[[*'xyz']].values
-        distances, indexes = cc_a.kd.query(coords_b)
+    for frag_a, frag_b in combinations(fragments, 2):
+        coords_b = frag_b.df[[*'xyz']].values
+        distances, indexes = frag_a.kd.query(coords_b)
 
         index_b = np.argmin(distances)
         index_a = indexes[index_b]
-        
-        node_a = cc_a.df['rowId'].iloc[index_a]
-        node_b = cc_b.df['rowId'].iloc[index_b]
+
+        node_a = frag_a.df['rowId'].iloc[index_a]
+        node_b = frag_b.df['rowId'].iloc[index_b]
         dist_ab = distances[index_b]
-        
-        frag_graph.add_edge(cc_a.i, cc_b.i, node_a=node_a, node_b=node_b, distance=dist_ab)
+
+        # Add edge from one fragment to another,
+        # but keep track of which fine-grained skeleton
+        # nodes were used to calculate distance.
+        frag_graph.add_edge( frag_a.frag_id, frag_b.frag_id,
+                             node_a=node_a, node_b=node_b,
+                             distance=dist_ab )
 
     # Compute inter-fragment MST edges
     frag_edges = nx.minimum_spanning_edges(frag_graph, weight='distance', data=True)
-    
+
     # For each inter-fragment edge, add the corresponding
-    # fine-grained edge between skeleton nodes
+    # fine-grained edge between skeleton nodes in the original graph.
     for _u, _v, d in frag_edges:
         g.add_edge(d['node_a'], d['node_b'])
 
     # Traverse in depth-first order to compute final tree
     root = skeleton_df['rowId'].iloc[0]
     edges = list(nx.dfs_edges(g, source=root))
     edges = pd.DataFrame(edges, columns=['link', 'rowId']) # parent, child
```

### Comparing `neuprint-python-0.4.8/neuprint_python.egg-info/PKG-INFO` & `neuprint-python-0.4.9/neuprint_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuprint-python
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python client utilties for interacting with the neuPrint connectome analysis service
 Home-page: https://github.com/connectome-neuprint/neuprint-python
 Author: Stuart Berg
 Author-email: bergs@hhmi.janelia.org
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.com/connectome-neuprint/neuprint-python.svg?branch=master)](https://travis-ci.com/connectome-neuprint/neuprint-python)
         [![docs-badge](docs/source/_static/docs-badge.svg)][docs]
```

### Comparing `neuprint-python-0.4.8/neuprint_python.egg-info/SOURCES.txt` & `neuprint-python-0.4.9/neuprint_python.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 neuprint/__init__.py
 neuprint/_version.py
 neuprint/admin.py
 neuprint/client.py
 neuprint/neuroncriteria.py
 neuprint/plotting.py
 neuprint/queries.py
+neuprint/simulation.py
 neuprint/synapsecriteria.py
 neuprint/utils.py
 neuprint/tests/__init__.py
 neuprint/tests/test_client.py
 neuprint/tests/test_neuroncriteria.py
 neuprint/tests/test_queries.py
 neuprint/tests/test_utils.py
```

### Comparing `neuprint-python-0.4.8/setup.cfg` & `neuprint-python-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `neuprint-python-0.4.8/setup.py` & `neuprint-python-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `neuprint-python-0.4.8/versioneer.py` & `neuprint-python-0.4.9/versioneer.py`

 * *Files identical despite different names*

