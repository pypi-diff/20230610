# Comparing `tmp/permit-2.0.2.tar.gz` & `tmp/permit-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.0.2.tar", last modified: Sun May 28 07:14:16 2023, max compression
+gzip compressed data, was "permit-2.0.3.tar", last modified: Sat Jun 10 13:56:11 2023, max compression
```

## Comparing `permit-2.0.2.tar` & `permit-2.0.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.343609 permit-2.0.2/
--rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.2/LICENSE
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.2/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-28 07:14:16.343488 permit-2.0.2/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.2/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.339239 permit-2.0.2/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.2/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.342006 permit-2.0.2/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     9730 2023-05-28 06:52:45.000000 permit-2.0.2/permit/api/base.py
--rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/condition_set_rules.py
--rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/condition_sets.py
--rw-r--r--   0 asafc      (501) staff       (20)     3534 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/context.py
--rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.2/permit/api/deprecated.py
--rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.2/permit/api/elements.py
--rw-r--r--   0 asafc      (501) staff       (20)     8821 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/environments.py
--rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-05-28 07:14:10.000000 permit-2.0.2/permit/api/models.py
--rw-r--r--   0 asafc      (501) staff       (20)     5098 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resource_action_groups.py
--rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/sync_api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.2/permit/api/users.py
--rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.2/permit/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.342310 permit-2.0.2/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.2/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.2/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.2/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     2865 2023-05-22 12:10:06.000000 permit-2.0.2/permit/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.2/permit/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.2/permit/permit.py
--rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.2/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.342662 permit-2.0.2/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.2/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.2/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.2/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.2/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.339751 permit-2.0.2/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.2/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-28 07:14:16.343645 permit-2.0.2/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      793 2023-05-28 07:14:10.000000 permit-2.0.2/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.343343 permit-2.0.2/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.2/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.2/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.2/tests/test_abac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-28 06:54:39.000000 permit-2.0.2/tests/test_rbac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.2/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.2/tests/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.709554 permit-2.0.3/
+-rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.3/LICENSE
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.3/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-10 13:56:11.709440 permit-2.0.3/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.3/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.702908 permit-2.0.3/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.3/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.707265 permit-2.0.3/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9966 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/base.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/condition_set_rules.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/condition_sets.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3686 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.3/permit/api/deprecated.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.3/permit/api/elements.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8771 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/models.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5063 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/resource_action_groups.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/sync_api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.3/permit/api/users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.3/permit/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.707596 permit-2.0.3/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.3/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.3/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.3/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2865 2023-05-22 12:10:06.000000 permit-2.0.3/permit/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.3/permit/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.3/permit/permit.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.3/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.708197 permit-2.0.3/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.3/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.3/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.3/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.3/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.703501 permit-2.0.3/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.3/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-06-10 13:56:11.709587 permit-2.0.3/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      793 2023-06-10 13:49:09.000000 permit-2.0.3/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.709282 permit-2.0.3/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.3/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.3/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.3/tests/test_abac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-28 06:54:39.000000 permit-2.0.3/tests/test_rbac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.3/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.3/tests/utils.py
```

### Comparing `permit-2.0.2/LICENSE` & `permit-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/api_client.py` & `permit-2.0.3/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/base.py` & `permit-2.0.3/permit/api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import aiohttp
 from loguru import logger
 from pydantic import BaseModel, Extra, Field, parse_obj_as
 
 from ..config import PermitConfig
 from ..exceptions import PermitContextError, handle_api_error, handle_client_error
-from .context import ApiKeyLevel
+from .context import API_ACCESS_LEVELS, ApiKeyLevel
 from .models import APIKeyScopeRead
 
 
 class ClientConfig(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -243,34 +243,38 @@
         Raises:
             PermitContextError: If the API context does not match the required endpoint context.
         """
         if self.config.api_context.level == ApiKeyLevel.WAIT_FOR_INIT:
             await self._set_context_from_api_key()
 
         if call_level != self.config.api_context.level:
-            raise PermitContextError(
-                f"You're trying to use an SDK method that requires an API Key with level: {call_level}, "
-                + f"however the SDK is running with an API key with level {self.config.api_context.level}."
-            )
+            if API_ACCESS_LEVELS.index(call_level) < API_ACCESS_LEVELS.index(
+                self.config.api_context.level
+            ):
+                raise PermitContextError(
+                    f"You're trying to use an SDK method that requires an API Key with level: {call_level}, "
+                    + f"however the SDK is running with an API key with level {self.config.api_context.level}."
+                )
+            return
 
         if (
             call_level == ApiKeyLevel.PROJECT_LEVEL_API_KEY
             and self.config.api_context.project is None
         ):
             raise PermitContextError(
                 "You're trying to use an SDK method that's specific to a project, "
                 + "but you haven't set the current project in your client's context yet, "
                 + "or you are using an organization level API key. "
                 + "Please set the context to a specific "
                 + "project using `permit.set_context()` method."
             )
 
-        if (
-            call_level == ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY
-            and self.config.api_context.environment is None
+        if call_level == ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY and (
+            self.config.api_context.project is None
+            or self.config.api_context.environment is None
         ):
             raise PermitContextError(
                 "You're trying to use an SDK method that's specific to an environment, "
                 + "but you haven't set the current environment in your client's context yet, "
                 + "or you are using an organization/project level API key. "
                 + "Please set the context to a specific "
                 + "environment using `permit.set_context()` method."
```

### Comparing `permit-2.0.2/permit/api/condition_set_rules.py` & `permit-2.0.3/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/condition_sets.py` & `permit-2.0.3/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/context.py` & `permit-2.0.3/permit/api/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,21 @@
     """
     Environment level API key authorization.
     Using an API key of this scope will allow the SDK user to modify
     a single Permit environment.
     """
 
 
+API_ACCESS_LEVELS = [
+    ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY,
+    ApiKeyLevel.PROJECT_LEVEL_API_KEY,
+    ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY,
+]
+
+
 class ApiContext:
     """
     The `ApiContext` class represents the context for API key authorization in Permit.
     It allows setting and retrieving the API Key context to be either:
     organization-level context, project-level context, or environment-level context.
     """
```

### Comparing `permit-2.0.2/permit/api/deprecated.py` & `permit-2.0.3/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/elements.py` & `permit-2.0.3/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/environments.py` & `permit-2.0.3/permit/api/environments.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class EnvironmentsApi(BasePermitApi):
     def __init__(self, config: PermitConfig):
         super().__init__(config)
         self.__environments = self._build_http_client("")
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def list(
         self, project_key: str, page: int = 1, per_page: int = 100
     ) -> List[EnvironmentRead]:
         """
         Retrieves a list of environments.
 
@@ -40,15 +40,15 @@
         """
         return await self.__environments.get(
             f"/v2/projects/{project_key}/envs",
             model=List[EnvironmentRead],
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get(self, project_key: str, environment_key: str) -> EnvironmentRead:
         """
         Gets an environment by project key and environment key.
 
         Args:
             project_key: The project key.
@@ -61,15 +61,15 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__environments.get(
             f"/v2/projects/{project_key}/envs/{environment_key}", model=EnvironmentRead
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get_by_key(
         self, project_key: str, environment_key: str
     ) -> EnvironmentRead:
         """
         Gets an environment by project key and environment key.
         Alias for the get method.
@@ -83,15 +83,15 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.get(project_key, environment_key)
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get_by_id(self, project_id: str, environment_id: str) -> EnvironmentRead:
         """
         Gets an environment by project ID and environment ID.
         Alias for the get method.
 
         Args:
@@ -103,15 +103,15 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.get(project_id, environment_id)
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get_stats(
         self, project_key: str, environment_key: str
     ) -> EnvironmentStats:
         """
         Retrieves statistics and metadata for an environment.
 
@@ -127,15 +127,15 @@
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__environments.get(
             f"/v2/projects/{project_key}/envs/{environment_key}/stats",
             model=EnvironmentStats,
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get_api_key(self, project_key: str, environment_key: str) -> APIKeyRead:
         """
         Retrieves the API key that grants access for an environment.
 
         Args:
             project_key: The project key.
@@ -149,15 +149,15 @@
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__environments.get(
             f"/v2/api-key/{project_key}/{environment_key}",
             model=APIKeyRead,
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def create(
         self, project_key: str, environment_data: EnvironmentCreate
     ) -> EnvironmentRead:
         """
         Creates a new environment.
 
@@ -174,15 +174,15 @@
         """
         return await self.__environments.post(
             f"/v2/projects/{project_key}/envs",
             model=EnvironmentRead,
             json=environment_data,
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def update(
         self,
         project_key: str,
         environment_key: str,
         environment_data: EnvironmentUpdate,
     ) -> EnvironmentRead:
@@ -203,15 +203,15 @@
         """
         return await self.__environments.patch(
             f"/v2/projects/{project_key}/envs/{environment_key}",
             model=EnvironmentRead,
             json=environment_data,
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def copy(
         self, project_key: str, environment_key: str, copy_params: EnvironmentCopy
     ) -> EnvironmentRead:
         """
         Clones data from a source specified environment into a different target environment in the same project.
 
@@ -229,15 +229,15 @@
         """
         return await self.__environments.post(
             f"/v2/projects/{project_key}/envs/{environment_key}/copy",
             model=EnvironmentRead,
             json=copy_params,
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def delete(self, project_key: str, environment_key: str) -> None:
         """
         Deletes an environment.
 
         Args:
             project_key: The project key.
```

### Comparing `permit-2.0.2/permit/api/models.py` & `permit-2.0.3/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/projects.py` & `permit-2.0.3/permit/api/projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class ProjectsApi(BasePermitApi):
     def __init__(self, config: PermitConfig):
         super().__init__(config)
         self.__projects = self._build_http_client("/v2/projects")
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def list(self, page: int = 1, per_page: int = 100) -> List[ProjectRead]:
         """
         Retrieves a list of projects.
 
         Args:
             page: The page number to fetch (default: 1).
@@ -30,15 +30,15 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__projects.get(
             "", model=List[ProjectRead], params=pagination_params(page, per_page)
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get(self, project_key: str) -> ProjectRead:
         """
         Retrieves a project by its key.
 
         Args:
             project_key: The key of the project.
@@ -48,15 +48,15 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__projects.get(f"/{project_key}", model=ProjectRead)
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get_by_key(self, project_key: str) -> ProjectRead:
         """
         Retrieves a project by its key.
         Alias for the get method.
 
         Args:
@@ -67,15 +67,15 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.get(project_key)
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def get_by_id(self, project_id: str) -> ProjectRead:
         """
         Retrieves a project by its ID.
         Alias for the get method.
 
         Args:
@@ -86,15 +86,15 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.get(project_id)
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def create(self, project_data: ProjectCreate) -> ProjectRead:
         """
         Creates a new project.
 
         Args:
             project_data: The data for the new project.
@@ -104,15 +104,15 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__projects.post("", model=ProjectRead, json=project_data)
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def update(
         self, project_key: str, project_data: ProjectUpdate
     ) -> ProjectRead:
         """
         Updates a project.
 
@@ -127,15 +127,15 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__projects.patch(
             f"/{project_key}", model=ProjectRead, json=project_data
         )
 
-    @ensure_context(ApiKeyLevel.ORGANIZATION_LEVEL_API_KEY)
+    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
     @validate_arguments
     async def delete(self, project_key: str) -> None:
         """
         Deletes a project.
 
         Args:
             project_key: The key of the project to delete.
```

### Comparing `permit-2.0.2/permit/api/resource_action_groups.py` & `permit-2.0.3/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/resource_actions.py` & `permit-2.0.3/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/resource_attributes.py` & `permit-2.0.3/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/resources.py` & `permit-2.0.3/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/role_assignments.py` & `permit-2.0.3/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/roles.py` & `permit-2.0.3/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/sync_api_client.py` & `permit-2.0.3/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/tenants.py` & `permit-2.0.3/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/api/users.py` & `permit-2.0.3/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/config.py` & `permit-2.0.3/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/enforcement/enforcer.py` & `permit-2.0.3/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/enforcement/interfaces.py` & `permit-2.0.3/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/exceptions.py` & `permit-2.0.3/permit/exceptions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/permit.py` & `permit-2.0.3/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/sync.py` & `permit-2.0.3/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/utils/context.py` & `permit-2.0.3/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit/utils/sync.py` & `permit-2.0.3/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/permit.egg-info/SOURCES.txt` & `permit-2.0.3/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/setup.py` & `permit-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="2.0.2",
+    version="2.0.3",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.0.2/tests/conftest.py` & `permit-2.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/tests/test_abac_e2e.py` & `permit-2.0.3/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/tests/test_rbac_e2e.py` & `permit-2.0.3/tests/test_rbac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.2/tests/test_rbac_e2e_sync.py` & `permit-2.0.3/tests/test_rbac_e2e_sync.py`

 * *Files identical despite different names*

