# Comparing `tmp/PlanaPY-0.2.2.tar.gz` & `tmp/PlanaPY-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.2.2.tar", last modified: Fri Jun  9 20:45:36 2023, max compression
+gzip compressed data, was "PlanaPY-0.2.3.tar", last modified: Fri Jun  9 23:18:22 2023, max compression
```

## Comparing `PlanaPY-0.2.2.tar` & `PlanaPY-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:45:36.690951 PlanaPY-0.2.2/
--rw-rw-rw-   0        0        0      286 2023-06-09 20:45:36.689955 PlanaPY-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 20:45:36.677603 PlanaPY-0.2.2/PlanaPY/
--rw-rw-rw-   0        0        0    13466 2023-06-09 20:21:58.000000 PlanaPY-0.2.2/PlanaPY/PlanaPY.py
--rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.2/PlanaPY/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:45:36.687846 PlanaPY-0.2.2/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-09 20:45:36.000000 PlanaPY-0.2.2/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-09 20:45:36.000000 PlanaPY-0.2.2/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:45:36.000000 PlanaPY-0.2.2/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 20:45:36.000000 PlanaPY-0.2.2/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 20:45:36.000000 PlanaPY-0.2.2/PlanaPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 20:45:36.691948 PlanaPY-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-06-09 20:45:10.000000 PlanaPY-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 23:18:22.278275 PlanaPY-0.2.3/
+-rw-rw-rw-   0        0        0      286 2023-06-09 23:18:22.278275 PlanaPY-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 23:18:22.257346 PlanaPY-0.2.3/PlanaPY/
+-rw-rw-rw-   0        0        0    13477 2023-06-09 23:09:30.000000 PlanaPY-0.2.3/PlanaPY/PlanaPY.py
+-rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.3/PlanaPY/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 23:18:22.275285 PlanaPY-0.2.3/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-06-09 23:18:22.000000 PlanaPY-0.2.3/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-09 23:18:22.000000 PlanaPY-0.2.3/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 23:18:22.000000 PlanaPY-0.2.3/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 23:18:22.000000 PlanaPY-0.2.3/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 23:18:22.000000 PlanaPY-0.2.3/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 23:18:22.279272 PlanaPY-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-06-09 23:18:17.000000 PlanaPY-0.2.3/setup.py
```

### Comparing `PlanaPY-0.2.2/PlanaPY/PlanaPY.py` & `PlanaPY-0.2.3/PlanaPY/PlanaPY.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     
     def all_revisions(self, model, workspace):
         model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
         URL = self.api.api_url + "models/{0}/alm/revisions".format(model_id)
         
         return self.get_request(URL)
     
-    def sync_models(self, source_model, target_model):
+    def sync_models(self, source_model, target_model, workspace):
         s_model_id = self.models[(self.models.name == source_model) 
                                             & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
         t_model_id = self.models[(self.models.name == source_model) 
                                  & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
 
         URL = self.api.api_url + "models/{0}/alm/syncTasks".format(t_model_id)
```

