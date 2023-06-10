# Comparing `tmp/braintrust-0.0.3.tar.gz` & `tmp/braintrust-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.3.tar", last modified: Wed Jun  7 15:57:32 2023, max compression
+gzip compressed data, was "braintrust-0.0.4.tar", last modified: Sat Jun 10 17:46:57 2023, max compression
```

## Comparing `braintrust-0.0.3.tar` & `braintrust-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.813499 braintrust-0.0.3/
--rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-07 15:57:32.813379 braintrust-0.0.3/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.3/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-07 15:57:32.813537 braintrust-0.0.3/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1582 2023-06-06 15:10:19.000000 braintrust-0.0.3/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.811734 braintrust-0.0.3/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.812438 braintrust-0.0.3/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    12709 2023-06-06 15:10:19.000000 braintrust-0.0.3/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.3/src/braintrust/cache.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.3/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-07 15:56:14.000000 braintrust-0.0.3/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.813205 braintrust-0.0.3/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      347 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      251 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.559114 braintrust-0.0.4/
+-rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-10 17:46:57.558983 braintrust-0.0.4/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.4/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-10 17:46:57.559152 braintrust-0.0.4/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1582 2023-06-06 15:10:19.000000 braintrust-0.0.4/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.557287 braintrust-0.0.4/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.558103 braintrust-0.0.4/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    16049 2023-06-10 17:46:14.000000 braintrust-0.0.4/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.4/src/braintrust/cache.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.4/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-10 17:46:14.000000 braintrust-0.0.4/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.558813 braintrust-0.0.4/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      347 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      251 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.3/setup.py` & `braintrust-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.3/src/braintrust/__init__.py` & `braintrust-0.0.4/src/braintrust/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class BrainTrustState:
     def __init__(self):
         self.current_project = None
         self.current_experiment = None
 
 
 _state = BrainTrustState()
-
+_logger = logging.getLogger("braintrust")
 
 API_URL = None
 ORG_ID = None
 LOG_URL = None
 
 
 class HTTPConnection:
@@ -289,15 +289,28 @@
             if len(items) < batch_size:
                 break
 
             items.clear()
 
 
 class Experiment(ModelWrapper):
-    def __init__(self, project, name=None, description=None):
+    """
+    An experiment is a collection of logged events, such as model inputs and outputs, which represent
+    a snapshot of your application at a particular point in time. An experiment is meant to capture more
+    than just the model you use, and includes the data you use to test, pre- and post- processing code,
+    comparison metrics (scores), and any other metadata you want to include.
+
+    Experiments are associated with a project, and two experiments are meant to be easily comparable via
+    their `inputs`. You can change the attributes of the experiments in a project (e.g. scoring functions)
+    over time, simply by changing what you log.
+
+    You should not create `Experiment` objects directly. Instead, use the `braintrust.init()` method.
+    """
+
+    def __init__(self, project: Project, name: str = None, description: str = None):
         self.project = project
         args = {"project_id": project.id}
 
         if not name:
             name = guess_experiment_name()
 
         if name:
@@ -305,33 +318,31 @@
 
         if description:
             args["description"] = description
 
         self.data = api_insert("register-experiment", args)[0]
         self.logger = _LogThread(name=name)
 
-    def log(self, inputs, output, expected=None, scores=None, metadata=None):
+    def log(self, inputs, output, expected, scores, metadata=None):
         user_id = _user_info()["id"]
         args = {
             "id": str(uuid.uuid4()),
             "inputs": inputs,
-            "output": json.dumps(output),
+            "output": output,
+            "expected": expected,
+            "scores": scores,
             "project_id": self.project.id,
             "experiment_id": self.id,
             "user_id": user_id,
             "created": datetime.datetime.now(datetime.timezone.utc).isoformat(),
         }
-        if expected:
-            args["expected"] = json.dumps(expected)
-        if scores:
-            args["scores"] = scores
+
         if metadata:
             args["metadata"] = metadata
 
-        # TODO: We should queue this up in the background
         self.logger.log(args)
         return args["id"]
 
     def summarize(self):
         # TODO: Show results so far here as well
         org_name = _user_info()["organizations"][0]["name"]
 
@@ -362,19 +373,35 @@
     return _state.current_experiment
 
 
 def log(inputs, output, expected, scores, metadata=None):
     """
     Log a single event to the current experiment. The event will be batched and uploaded behind the scenes.
 
-    :param inputs: The inputs to the model (an arbitrary, JSON serializable object).
-    :param output: The output of the model (an arbitrary, JSON serializable object).
-    :param expected: The expected output of the model (an arbitrary, JSON serializable object).
-    :param scores: A dictionary of scores to log.
-    :param metadata: (Optional) Additional metadata about the event (that you can later use to slice/dice your results).
+    :param inputs: The arguments that uniquely define a test case (an arbitrary, JSON serializable object). Later on,
+    BrainTrust will use the `inputs` to know whether two test casess are the same between experiments, so they should
+    not contain experiment-specific state. A simple rule of thumb is that if you run the same experiment twice, the
+    `inputs` should be identical.
+    :param output: The output of your application, including post-processing (an arbitrary, JSON serializable object),
+    that allows you to determine whether the result is correct or not. For example, in an app that generates SQL queries,
+    the `output` should be the _result_ of the SQL query generated by the model, not the query itself, because there may
+    be multiple valid queries that answer a single question.
+    :param expected: The ground truth value (an arbitrary, JSON serializable object) that you'd compare to `output` to
+    determine if your `output` value is correct or not. BrainTrust currently does not compare `output` to `expected` for
+    you, since there are so many different ways to do that correctly. Instead, these values are just used to help you
+    navigate your experiments while digging into analyses. However, we may later use these values to re-score outputs or
+    fine-tune your models.
+    :param scores: A dictionary of numeric values (between 0 and 1) to log. The scores should give you a variety of signals
+    that help you determine how accurate the outputs are compared to what you expect and diagnose failures. For example, a
+    summarization app might have one score that tells you how accurate the summary is, and another that measures the word similarity
+    between the generated and grouth truth summary. The word similarity score could help you determine whether the summarization was
+    covering similar concepts or not. You can use these scores to help you sort, filter, and compare experiments.
+    :param metadata: (Optional) a JSON-serializable object with additional data about the test example, model outputs, or just
+    about anything else that's relevant, that you can use to help find and analyze examples later. For example, you could log the
+    `prompt`, example's `id`, or anything else that would be useful to slice/dice later.
     :returns: The `id` of the logged event.
     """
 
     if not _state.current_experiment:
         raise Exception("Not initialized. Please call init() or login() first")
 
     return _state.current_experiment.log(
@@ -409,32 +436,54 @@
         token = api_info.get("token")
         if token is not None:
             conn.set_token(token)
 
         ping_resp = conn.get("ping")
         ping_ok = ping_resp.ok
 
+    if not ping_ok and api_info and api_info.get("refresh_token"):
+        resp = requests.post(
+            _urljoin(API_URL, "/api/token/refresh"), json={"refresh_token": api_info.get("refresh_token")}
+        )
+        if resp.ok:
+            resp_data = resp.json()
+            token = resp_data["id_token"]
+            refresh_token = resp_data.get("refresh_token")
+            _save_api_info({**api_info, "token": token, "refresh_token": refresh_token})
+
+            conn.set_token(token)
+            ping_resp = conn.get("ping")
+            ping_ok = ping_resp.ok
+        else:
+            _logger.warning(f"Failed to refresh token: [{resp.status_code}] {resp.text}")
+
     if not ping_ok:
         print(f"Please copy your API token from {API_URL}/app/token")
         temp_token = getpass("Token: ")
 
         resp = requests.post(_urljoin(API_URL, "/api/id-token"), json={"token": temp_token})
         assert resp.ok, f"Failed to acquire token: {resp.text}"
         info = resp.json()
         token, ORG_ID, LOG_URL = info["token"], info["org_info"][0]["id"], info["org_info"][0]["api_url"]
 
-        with open(API_INFO_PATH, "w") as f:
-            json.dump({"token": token, "org_id": ORG_ID, "log_url": LOG_URL}, f)
+        _save_api_info(
+            {"token": token, "org_id": ORG_ID, "log_url": LOG_URL, "refresh_token": info.get("refresh_token")}
+        )
 
         conn = api_conn()
         conn.set_token(token)
 
     assert conn, "Conn should be set at this point (a bug)"
     resp = conn.get("ping")
     assert resp.ok, "Invalid token: " + resp.text
 
 
+def _save_api_info(api_info):
+    with open(API_INFO_PATH, "w") as f:
+        json.dump(api_info, f)
+
+
 def _urljoin(*parts):
     return "/".join([x.lstrip("/") for x in parts])
 
 
 __all__ = ["init", "log", "login"]
```

### Comparing `braintrust-0.0.3/src/braintrust/oai.py` & `braintrust-0.0.4/src/braintrust/oai.py`

 * *Files identical despite different names*

