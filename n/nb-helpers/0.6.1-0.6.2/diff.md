# Comparing `tmp/nb_helpers-0.6.1.tar.gz` & `tmp/nb_helpers-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_helpers-0.6.1.tar", last modified: Fri Jun  9 21:58:42 2023, max compression
+gzip compressed data, was "nb_helpers-0.6.2.tar", last modified: Fri Jun  9 22:17:54 2023, max compression
```

## Comparing `nb_helpers-0.6.1.tar` & `nb_helpers-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:58:42.734192 nb_helpers-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:58:42.734192 nb_helpers-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:58:42.730192 nb_helpers-0.6.1/nb_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:58:42.730192 nb_helpers-0.6.1/nb_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:58:42.734192 nb_helpers-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:17:54.783981 nb_helpers-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 22:17:54.783981 nb_helpers-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:17:54.779981 nb_helpers-0.6.2/nb_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/nb_helpers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:17:54.783981 nb_helpers-0.6.2/nb_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 22:17:54.000000 nb_helpers-0.6.2/nb_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 22:17:54.000000 nb_helpers-0.6.2/nb_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:17:54.000000 nb_helpers-0.6.2/nb_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 22:17:54.000000 nb_helpers-0.6.2/nb_helpers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:17:54.000000 nb_helpers-0.6.2/nb_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 22:17:54.000000 nb_helpers-0.6.2/nb_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 22:17:54.000000 nb_helpers-0.6.2/nb_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 22:17:54.783981 nb_helpers-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-09 22:17:44.000000 nb_helpers-0.6.2/setup.py
```

### Comparing `nb_helpers-0.6.1/LICENSE` & `nb_helpers-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/PKG-INFO` & `nb_helpers-0.6.2/nb_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nb_helpers
-Version: 0.6.1
+Name: nb-helpers
+Version: 0.6.2
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.6.1/README.md` & `nb_helpers-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/_modidx.py` & `nb_helpers-0.6.2/nb_helpers/_modidx.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/actions.py` & `nb_helpers-0.6.2/nb_helpers/actions.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/clean.py` & `nb_helpers-0.6.2/nb_helpers/clean.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/colab.py` & `nb_helpers-0.6.2/nb_helpers/colab.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/docker.py` & `nb_helpers-0.6.2/nb_helpers/docker.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/export.py` & `nb_helpers-0.6.2/nb_helpers/export.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/run.py` & `nb_helpers-0.6.2/nb_helpers/run.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers/utils.py` & `nb_helpers-0.6.2/nb_helpers/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,14 +315,16 @@
 
 # %% ../nbs/02_utils.ipynb 62
 def _get_github_repo_remote(repo_url):
     if "git@" in repo_url:
         github_repo = re.search(r".com:(.*).git", repo_url).group(1)
     else:
         github_repo = re.search(r".com/(.*)", repo_url).group(1)
+        if github_repo.endswith(".git"):
+            github_repo = github_repo[:-4]
     return github_repo
 
 # %% ../nbs/02_utils.ipynb 64
 def git_origin_repo(fname):
     "Get github repo name from `fname`"
     repo = get_repo(fname)
     repo_url = repo.remote().url
```

### Comparing `nb_helpers-0.6.1/nb_helpers/wandb.py` & `nb_helpers-0.6.2/nb_helpers/wandb.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.1/nb_helpers.egg-info/PKG-INFO` & `nb_helpers-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nb-helpers
-Version: 0.6.1
+Name: nb_helpers
+Version: 0.6.2
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.6.1/setup.py` & `nb_helpers-0.6.2/setup.py`

 * *Files identical despite different names*

