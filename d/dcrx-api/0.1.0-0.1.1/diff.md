# Comparing `tmp/dcrx-api-0.1.0.tar.gz` & `tmp/dcrx-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.1.0.tar", last modified: Fri Jun  9 16:22:32 2023, max compression
+gzip compressed data, was "dcrx-api-0.1.1.tar", last modified: Sat Jun 10 00:29:19 2023, max compression
```

## Comparing `dcrx-api-0.1.0.tar` & `dcrx-api-0.1.1.tar`

### file list

```diff
@@ -1,76 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/auth/auth_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/database/connection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/env/load_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/docker_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/dcrx_api/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/dcrx_api/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/dcrx_api/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/dcrx_api/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/table/table_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/table/users_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/dcrx_api/users/users_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:32.886089 dcrx-api-0.1.0/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-09 16:22:32.000000 dcrx-api-0.1.0/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 16:22:32.000000 dcrx-api-0.1.0/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:22:32.000000 dcrx-api-0.1.0/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 16:22:32.000000 dcrx-api-0.1.0/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 16:22:32.000000 dcrx-api-0.1.0/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 16:22:32.000000 dcrx-api-0.1.0/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:22:32.890089 dcrx-api-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 16:22:29.000000 dcrx-api-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/setup.py
```

### Comparing `dcrx-api-0.1.0/LICENSE` & `dcrx-api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.0/PKG-INFO` & `dcrx-api-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -109,15 +109,15 @@
 {
   "name": "hello-world",
   "tag": "latest",
   "layers": [
     {
       "layer_type": "stage",
       "base": "python",
-      "tag": "3.11-slim",
+      "tag": "3.11-slim"
     },
     {
         "layer_type": "entrypoint",
         "command": [
             "echo",
             "Hello world!"
         ]
@@ -152,13 +152,30 @@
 
 To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
 
 ```bash
 docker run -p 2277:2277 --env-file .env --privileged dcrx-api:latest
 ```
 
+# Deploying via Helm
+
+DCRX-API has a minimal helm chart to help you scale up when ready. To begin, first create a Kuberenetes secret as below:
+
+```
+kubectl create secret generic dcrx-api-secrets --from-literal="DCRX_API_SECRET_KEY=$DCRX_API_SECRET_KEY" --from-literal="DOCKER_REGISTRY_USERNAME=$DOCKER_REGISTRY_USERNAME" --from-literal="DOCKER_REGISTRY_PASSWORD=$DOCKER_REGISTRY_PASSWORD"
+
+```
+
+Then install the provided helm chart:
+
+```
+helm install dcrx-api helm/dcrx-api/ --values helm/dcrx-api/values.yml
+```
+
+The chart creates three replica dcrx-api pods, a LoadBalancer service, and Nginx ingress to get you up and running in your Kubernetes cluster!
+
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.1.0/README.md` & `dcrx-api-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 {
   "name": "hello-world",
   "tag": "latest",
   "layers": [
     {
       "layer_type": "stage",
       "base": "python",
-      "tag": "3.11-slim",
+      "tag": "3.11-slim"
     },
     {
         "layer_type": "entrypoint",
         "command": [
             "echo",
             "Hello world!"
         ]
@@ -134,13 +134,30 @@
 
 To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
 
 ```bash
 docker run -p 2277:2277 --env-file .env --privileged dcrx-api:latest
 ```
 
+# Deploying via Helm
+
+DCRX-API has a minimal helm chart to help you scale up when ready. To begin, first create a Kuberenetes secret as below:
+
+```
+kubectl create secret generic dcrx-api-secrets --from-literal="DCRX_API_SECRET_KEY=$DCRX_API_SECRET_KEY" --from-literal="DOCKER_REGISTRY_USERNAME=$DOCKER_REGISTRY_USERNAME" --from-literal="DOCKER_REGISTRY_PASSWORD=$DOCKER_REGISTRY_PASSWORD"
+
+```
+
+Then install the provided helm chart:
+
+```
+helm install dcrx-api helm/dcrx-api/ --values helm/dcrx-api/values.yml
+```
+
+The chart creates three replica dcrx-api pods, a LoadBalancer service, and Nginx ingress to get you up and running in your Kubernetes cluster!
+
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.1.0/dcrx_api/auth/auth_context.py` & `dcrx-api-0.1.1/dcrx_api/services/auth/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 from typing import (
     Optional,
     Dict,
     Any,
     List,
     Union
 )
-from dcrx_api.users.users_connection import UsersConnection
-from dcrx_api.users.models import (
+from dcrx_api.services.users.connection import UsersConnection
+from dcrx_api.services.users.models import (
     DBUser,
     LoginUser
 )
 from .models import (
     AuthResponse,
     AuthClaims,
     GeneratedToken
 )
 
 
-class AuthContext:
+class AuthorizationSessionManager:
 
     def __init__(self, env: Env) -> None:
 
         self.pool_size = env.DCRX_API_WORKERS
         self.context = CryptContext(
             schemes=["bcrypt"], 
             deprecated="auto"
@@ -66,15 +66,15 @@
             filters={
                 'username': username
             }
         )
 
         if len(users) < 1:
             return AuthResponse(
-                error='User not found',
+                error='User authorization failed',
                 message='Authentication failed'
             )
         
         user = users.pop()
         
         password_verified = await self._loop.run_in_executor(
             self._executor,
@@ -82,15 +82,19 @@
                 self.context.verify,
                 password, 
                 user.hashed_password
             )
         )
 
         if password_verified is False:
-            return None
+            return AuthResponse(
+                error='User authorization failed',
+                message='Authentication failed'
+            )
+        
         
         return user
     
     def create_access_token(
         self, 
         data: Dict[str, Any], 
         expires_delta: Optional[datetime.datetime]=None
@@ -122,19 +126,16 @@
     ) -> AuthResponse:
         user = await self.authenticate_user(
             db_connection, 
             login_user.username, 
             login_user.password
         )
 
-        if user is None:
-            return AuthResponse(
-                error='Login failed - invalid username or password',
-                message='Authorization failed'
-            )
+        if isinstance(user, AuthResponse):
+            return user
 
         access_token_expires = datetime.timedelta(
             minutes=self.token_expiration_minutes
         )
         
         auth_token = self.create_access_token(
             data={
@@ -201,11 +202,8 @@
             )
         
         return AuthResponse(
             message='OK'
         )
     
     async def close(self):
-        self._executor.shutdown(cancel_futures=True)
-
-
-active_auth_contexts: Dict[str, AuthContext] = {}
+        self._executor.shutdown(cancel_futures=True)
```

### Comparing `dcrx-api-0.1.0/dcrx_api/cli/base.py` & `dcrx-api-0.1.1/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.0/dcrx_api/cli/database.py` & `dcrx-api-0.1.1/dcrx_api/cli/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import uuid
 import asyncio
 import click
 from dcrx_api.env import load_env, Env
-from dcrx_api.auth.auth_context import AuthContext
-from dcrx_api.users.users_connection import UsersConnection, ConnectionConfig
-from dcrx_api.users.models import DBUser, NewUser
+from dcrx_api.services.auth.manager import AuthorizationSessionManager
+from dcrx_api.services.users.connection import UsersConnection
+from dcrx_api.services.users.models import DBUser, NewUser
 from typing import Dict, Any
 
 
 
 async def create_user(
     user: Dict[str, Any],
     env: Env,
 ):
     
-    connection = UsersConnection(
-        ConnectionConfig(
-            database_username=env.DCRX_API_DATABASE_USER,
-            database_password=env.DCRX_API_DATABASE_PASSWORD,
-            database_type=env.DCRX_API_DATABASE_TYPE,
-            database_uri=env.DCRX_API_DATABASE_URI,
-            database_name=env.DCRX_API_DATABASE_NAME
-        )
-    )
+    connection = UsersConnection(env)
 
-    auth = AuthContext(env)
+    auth = AuthorizationSessionManager(env)
     await auth.connect()
 
     new_user = NewUser(
         username=user.get('username'),
         first_name=user.get('first_name'),
         last_name=user.get('last_name'),
         email=user.get('email'),
@@ -46,15 +38,15 @@
         last_name=new_user.last_name,
         email=new_user.email,
         disabled=new_user.disabled,
         hashed_password=hashed_password
     )
 
     await connection.connect()
-    await connection.create_table()
+    await connection.init()
 
     users = await connection.select()
 
     if len(users) < 1:
         await connection.create([
             user
         ])
```

### Comparing `dcrx-api-0.1.0/dcrx_api/database/connection.py` & `dcrx-api-0.1.1/dcrx_api/database/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from sqlalchemy.ext.asyncio import (
     create_async_engine,
     AsyncEngine as PostgresEngine,
     AsyncConnection
 )
 from typing import (
     Union, 
-    Any, 
     Generic,
     TypeVar,
     List
 )
 from .connection_config import ConnectionConfig
 
 
@@ -60,17 +59,17 @@
                 host=self.config.database_uri,
                 database=self.config.database_name,
                 loop=self.loop
             )
 
         elif self.engine is None and self.config.database_type == 'asyncpg':
             self.engine = create_async_engine(
+                self.config.database_uri,
                 user=self.config.database_username,
                 password=self.config.database_password,
-                host=self.config.database_uri,
                 database=self.config.database_name
             )
 
         elif self.engine is None and self.config.database_type == 'sqlite':
             self.engine = create_async_engine(self.config.database_uri)
 
         self.connection = await self.engine.connect()
@@ -99,15 +98,15 @@
     
     async def insert_or_update(
         self,
         statements: List[
             Union[Insert, Update]
         ]
     ):
-
+        
         for statement in statements:
             await self.connection.execute(statement)
         
         await self.connection.commit()
 
     async def delete(
         self,
```

### Comparing `dcrx-api-0.1.0/dcrx_api/env/env.py` & `dcrx-api-0.1.1/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.0/dcrx_api/env/load_env.py` & `dcrx-api-0.1.1/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.0/dcrx_api/jobs/docker_job.py` & `dcrx-api-0.1.1/dcrx_api/services/jobs/queue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,94 @@
 import asyncio
-import docker
-import functools
-import traceback
-import os
-import psutil
 import uuid
-from concurrent.futures import ThreadPoolExecutor
 from dcrx.image import Image
-from dcrx.memory_file import MemoryFile
+from dcrx_api.env import Env
 from .models import BuildOptions
 from .models import Registry
-from typing import (
-    Union, 
-    Optional, 
-    Dict, 
-    Any
+from typing import Optional, Dict, Union
+from .job import Job
+from .connection import JobsConnection
+from .status import JobStatus
+from .models import (
+    JobMetadata,
+    JobNotFoundException
 )
-from .job_status import JobStatus
 
 
-class DockerJob:
+class JobQueue:
 
-    def __init__(
-        self, 
-        image: Image, 
-        registry: Registry,
-        build_options: Optional[BuildOptions]=None,
-        pool_size: int=psutil.cpu_count()
-    ) -> None:
-        
-        self.job_id = uuid.uuid4()
-        self.job_name = image.full_name
-
-        self.image = image
-        self.registry = registry
-        self.build_options = build_options
-
-        self.client = docker.DockerClient(
-            max_pool_size=pool_size,
-        )
-
-        self.context: Union[MemoryFile, None] = None
-        self._executor = ThreadPoolExecutor(max_workers=pool_size)
-        self.loop = asyncio.get_event_loop()
-        self.status = JobStatus.CREATED
-        self.error: Union[Exception, None] = None
-
-    async def run(self):
-
-        try:
-            await self.login_to_registry()
-            await self.assemble_context()
-            await self.build_image()
-            await self.push_image()
-
-        except Exception as job_exception:
-            self.error = job_exception
-
-        await self.clear()
-        await self.close()
-
-    async def login_to_registry(self):
-
-        self.status = JobStatus.AUTHORIZING
-
-        await self.loop.run_in_executor(
-            self._executor,
-            functools.partial(
-                self.client.api.login,
-                self.registry.registry_user,
-                password=self.registry.registry_password,
-                registry=self.registry.registry_uri,
-                reauth=True
-            )
-        )
-
-    async def assemble_context(self):
-
-        self.status = JobStatus.GENERATING
-
-        self.context = await self.loop.run_in_executor(
-            self._executor,
-            self.image.to_context
-        )
-
-
-    async def build_image(self):
+    def __init__(self, env: Env) -> None:
 
-        self.status = JobStatus.BUILDING
+        self.pool_size = env.DCRX_API_WORKERS
+        self.push_timeout_minutes = env.DCRX_API_PUSH_TIMEOUT_MINUTES
 
-        build_options: Dict[str, Any] = {}
+        self.registry_uri = env.DOCKER_REGISTRY_URI
+        self.registry_username = env.DOCKER_REGISTRY_USERNAME
+        self.registry_password = env.DOCKER_REGISTRY_PASSWORD
 
-        if self.build_options:
-            build_options = self.build_options.dict()
+        self._jobs: Dict[uuid.UUID, Job] = {}
+        self._active: Dict[uuid.UUID, asyncio.Task] = {}
 
-        await self.loop.run_in_executor(
-            self._executor,
-            functools.partial(
-                self.client.api.build,
-                dockerfile=self.image.filename,
-                fileobj=self.context,
-                tag=self.image.full_name,
-                custom_context=True,
-                **build_options
-            )   
-        )
-
-    async def push_image(self):
-
-        self.status = JobStatus.PUSHING
+    def submit(
+        self,
+        connection: JobsConnection,
+        image: Image, 
+        build_options: Optional[BuildOptions]=None
+    ) -> JobMetadata:
 
-        await self.loop.run_in_executor(
-            self._executor,
-            functools.partial(
-                self.client.api.push,
-                self.image.name,
-                tag=self.image.tag
+        job = Job(
+            connection,
+            image,
+            Registry(
+                registry_uri=self.registry_uri,
+                registry_user=self.registry_username,
+                registry_password=self.registry_password
+                
+            ),
+            build_options=build_options,
+            pool_size=self.pool_size
+        )
+
+        self._jobs[job.job_id] = job
+
+        self._active[job.job_id] = asyncio.create_task(
+            job.run(self.push_timeout_minutes)
+        )
+
+        return job.metadata
+
+    def get(self, job_id: uuid.UUID) -> Union[JobMetadata, JobNotFoundException]:
+        job = self._jobs.get(job_id)
+        if job is None:
+            return JobNotFoundException(
+                job_id=job_id,
+                message=f'Job - {job_id} - not found.'
             )
-        )
-
-    async def clear(self):
-        await self.loop.run_in_executor(
-            self._executor,
-            self.image.clear
-        )
-            
 
-    async def close(self):
-
-        self._executor.shutdown(cancel_futures=True)
-        self.client.close()
-        self.context.close()
-
-        if self.error is None:
-            self.status = JobStatus.DONE
-
-        else:
-            self.status = JobStatus.FAILED
+        return job.metadata
+    
+    def cancel(self, job_id: uuid.UUID) -> Union[JobMetadata, JobNotFoundException]:
+        job = self._active.get(job_id)
+        if job is None or job.done():
+            return JobNotFoundException(
+                job_id=job_id,
+                message=f'Job - {job_id} - not found or is not active.'
+            )
         
+        job.cancel()
 
+        cancelled_job = self._jobs.get(job_id)
 
+        self._jobs[job_id].close(
+            cancelled=True
+        )
 
-    
+        return cancelled_job.metadata
+    
+    async def close(self):
+        for job in self._active.values():
+            if not job.done():
+                job.cancel()
+
+        for job in self._jobs.values():
+            await job.close()
+
```

### Comparing `dcrx-api-0.1.0/dcrx_api/jobs/models/new_image.py` & `dcrx-api-0.1.1/dcrx_api/services/jobs/models/new_image.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,24 +18,23 @@
     Stage,
     User,
     Volume,
     Workdir
 )
 
 
-from typing import List, Union
+from typing import List, Union, Optional
 from .build_options import BuildOptions
-from .registry import Registry
 
 
 class NewImage(BaseModel):
     name: StrictStr
     tag: StrictStr='latest'
-    files: List[StrictStr]=[]
-    build_options: BuildOptions
+    files: Optional[List[StrictStr]]
+    build_options: Optional[BuildOptions]
     layers: conlist(Union[
         Add,
         Arg,
         Cmd,
         Copy,
         Entrypoint,
         Env,
```

### Comparing `dcrx-api-0.1.0/dcrx_api/users/service.py` & `dcrx-api-0.1.1/dcrx_api/services/users/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,41 @@
 import uuid
-import datetime
-from dcrx_api.env import Env
+from dcrx_api.services.auth.models import AuthenticationFailureException
+from dcrx_api.context.manager import context, ContextType
 from fastapi import APIRouter, HTTPException
 from fastapi.responses import JSONResponse
-from dcrx_api.auth.auth_context import active_auth_contexts
-from dcrx_api.auth.models import AuthenticationFailureException
-from typing import (
-    Dict,
-    Literal, 
-    Union
-)
+from typing import Literal
 from .models import (
     AuthorizedUser,
     DBUser,
     LoginUser,
     NewUser,
     UpdatedUser,
     UserNotFoundException,
     UserTransactionSuccessResponse,
 )
-from .users_connection import UsersConnection
-
-
-users_context: Dict[str,Union[Env, UsersConnection]] = {}
-
 
 users_router = APIRouter()
 
 
 @users_router.post(
     '/users/login',
     responses={
         401: {
             "model": AuthenticationFailureException
         }
     }
 )
 async def login_user(user: LoginUser) -> UserTransactionSuccessResponse:
-    users_connection = users_context.get('connection')
-    auth = active_auth_contexts.get('session')
 
-    authorization = await auth.generate_token(
-        users_connection,
+    users_service_context = context.get(ContextType.USERS_SERVICE)
+    auth_service_context = context.get(ContextType.AUTH_SERVICE)
+
+    authorization = await auth_service_context.manager.generate_token(
+        users_service_context.connection,
         user
     )
 
     if authorization.error:
         raise HTTPException(401, detail=authorization.error)
     
     success_response = UserTransactionSuccessResponse(
@@ -77,26 +67,27 @@
         }
     }
 )
 async def get_user(
     user_id_or_name: str, 
     match_by: Literal["id", "username"]="id"
 ) -> AuthorizedUser:
-    users_connection = users_context.get('connection')
+
+    users_service_context = context.get(ContextType.USERS_SERVICE)
 
     filters = {
         'id': user_id_or_name
     }
 
     if match_by == 'username':
         filters = {
             'username': user_id_or_name
         }
 
-    users = await users_connection.select(
+    users = await users_service_context.connection.select(
         filters=filters
     )
 
     if len(users) < 1:
         raise HTTPException(404, detail=f'User {user_id_or_name} not found.')
     
     user = users.pop()
@@ -113,20 +104,21 @@
     responses={
         401: {
             "model": AuthenticationFailureException
         }
     }
 )
 async def create_user(user: NewUser) -> UserTransactionSuccessResponse:
-    users_connection = users_context.get('connection')
-    auth = active_auth_contexts.get('session')
 
-    hashed_password = await auth.encrypt(user.password)
+    users_service_context = context.get(ContextType.USERS_SERVICE)
+    auth_service_context = context.get(ContextType.AUTH_SERVICE)
+
+    hashed_password = await auth_service_context.manager.encrypt(user.password)
 
-    await users_connection.create([
+    await users_service_context.connection.create([
         DBUser(
             id=uuid.uuid4(),
             hashed_password=hashed_password,
             **user.dict(exclude={"password"})
         )
     ])
 
@@ -141,17 +133,18 @@
     responses={
         401: {
             "model": AuthenticationFailureException
         }
     }
 )
 async def update_user(user: UpdatedUser) -> UserTransactionSuccessResponse:
-    users_connection = users_context.get('connection')
 
-    await users_connection.create([
+    users_service_context = context.get(ContextType.USERS_SERVICE)
+
+    await users_service_context.connection.update([
         user
     ])
 
     return UserTransactionSuccessResponse(
         message='Updated user.'
     )
 
@@ -162,17 +155,18 @@
     responses={
         401: {
             "model": AuthenticationFailureException
         }
     }
 )
 async def delete_user(user_id: str) -> UserTransactionSuccessResponse:
-    users_connection = users_context.get('connection')
 
-    await users_connection.delete(
+    users_service_context = context.get(ContextType.USERS_SERVICE)
+
+    await users_service_context.connection.delete(
         filters={
             'id': user_id
         }
     )
 
     return UserTransactionSuccessResponse(
         message='Deleted user.'
```

### Comparing `dcrx-api-0.1.0/dcrx_api/users/table/users_mysql_table.py` & `dcrx-api-0.1.1/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sqlalchemy
 import uuid
-from .table_types import TableTypes
+from dcrx_api.database.table_types import TableTypes
 
 
 class UsersMySQLTable:
 
     def __init__(
         self, 
         users_table_name: str
```

### Comparing `dcrx-api-0.1.0/dcrx_api/users/table/users_postgres_table.py` & `dcrx-api-0.1.1/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import sqlalchemy
 import uuid
-from sqlalchemy.dialects.postgresql import UUID
-from .table_types import TableTypes
+from dcrx_api.database.table_types import TableTypes
 
 
-class UsersPostgresTable:
+class UsersSQLiteTable:
 
     def __init__(
         self, 
         users_table_name: str
     ) -> None:
         self.table = sqlalchemy.Table(
             users_table_name,
             sqlalchemy.MetaData(),
             sqlalchemy.Column(
                 'id', 
-                UUID(as_uuid=True),
+                sqlalchemy.BLOB,
                 primary_key=True,
                 default=uuid.uuid4
             ),
             sqlalchemy.Column(
                 'username',
                 sqlalchemy.TEXT
             ),
@@ -52,18 +51,17 @@
             'last_name': self.table.c.last_name,
             'email': self.table.c.email,
             'disable': self.table.c.disabled,
             'hashed_password': self.table.c.hashed_password
         }
 
         self.types_map = {
-            'id': lambda value: uuid.UUID(value),
+            'id': lambda value: str(value).encode(),
             'username': lambda value: str(value),
             'first_name': lambda value: str(value),
             'last_name': lambda value: str(value),
             'email': lambda value: str(value),
             'disabled': lambda value: bool(value),
             'hashed_password': lambda value: str(value)
         }
 
-        self.table_type = TableTypes.POSTGRES
-
+        self.table_type = TableTypes.SQLITE
```

### Comparing `dcrx-api-0.1.0/dcrx_api/users/table/users_sqllite_table.py` & `dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 import sqlalchemy
 import uuid
-from .table_types import TableTypes
+from dcrx_api.database.table_types import TableTypes
 
 
-class UsersSQLLiteTable:
+class JobsSQLiteTable:
 
     def __init__(
         self, 
-        users_table_name: str
+        jobs_table_name: str
     ) -> None:
         self.table = sqlalchemy.Table(
-            users_table_name,
+            jobs_table_name,
             sqlalchemy.MetaData(),
             sqlalchemy.Column(
                 'id', 
                 sqlalchemy.BLOB,
                 primary_key=True,
                 default=uuid.uuid4
             ),
             sqlalchemy.Column(
-                'username',
+                'name',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
-                'first_name',
+                'image',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
-                'last_name',
+                'tag',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
-                'email',
+                'status',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
-                'disabled',
-                sqlalchemy.BOOLEAN
-            ),
-            sqlalchemy.Column(
-                'hashed_password',
+                'context',
                 sqlalchemy.TEXT
             )
         )
 
         self.columns = {
             'id': self.table.c.id,
-            'username': self.table.c.username,
-            'first_name': self.table.c.first_name,
-            'last_name': self.table.c.last_name,
-            'email': self.table.c.email,
-            'disable': self.table.c.disabled,
-            'hashed_password': self.table.c.hashed_password
+            'name': self.table.c.name,
+            'image': self.table.c.image,
+            'tag': self.table.c.tag,
+            'status': self.table.c.status,
+            'context': self.table.c.context,
         }
 
         self.types_map = {
             'id': lambda value: str(value).encode(),
-            'username': lambda value: str(value),
-            'first_name': lambda value: str(value),
-            'last_name': lambda value: str(value),
-            'email': lambda value: str(value),
-            'disabled': lambda value: bool(value),
-            'hashed_password': lambda value: str(value)
+            'name': lambda value: str(value),
+            'image': lambda value: str(value),
+            'tag': lambda value: str(value),
+            'status': lambda value: str(value),
+            'context': lambda value: str(value)
         }
 
-        self.table_type = TableTypes.SQLITE
+        self.table_type = TableTypes.MYSQL
+
```

### Comparing `dcrx-api-0.1.0/dcrx_api/users/table/users_table.py` & `dcrx-api-0.1.1/dcrx_api/services/users/table/users_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,45 +14,45 @@
     Callable,
     Optional,
     TypeVar,
     Generic
 )
 from .users_mysql_table import UsersMySQLTable
 from .users_postgres_table import UsersPostgresTable
-from .users_sqllite_table import UsersSQLLiteTable
+from .users_sqllite_table import UsersSQLiteTable
 
 M = TypeVar('M', bound=BaseModel)
 
 class UsersTable(Generic[M]):
 
     def __init__(
         self,
         users_table_name: str,
         database_type: Literal["mysql", "postgres", "sqlite"]="sqlite"
     ) -> None:
         self._table_types: Dict[
-            Literal["mysql", "postgres", "Sqlite"],
+            Literal["mysql", "postgres", "sqlite"],
             Callable[
                 [str],
                 Union[
                     UsersMySQLTable,
                     UsersPostgresTable,
-                    UsersSQLLiteTable
+                    UsersSQLiteTable
                 ]
             ]
         ] = {
             'mysql': lambda table_name: UsersMySQLTable(table_name),
             'postgres': lambda table_name: UsersPostgresTable(table_name),
-            'sqlite': lambda table_name: UsersSQLLiteTable(table_name)
+            'sqlite': lambda table_name: UsersSQLiteTable(table_name)
         }
 
         self.selected: Union[
             UsersMySQLTable,
             UsersPostgresTable,
-            UsersSQLLiteTable
+            UsersSQLiteTable
         ] = self._table_types.get(
             database_type,
             UsersMySQLTable
         )(users_table_name)
 
     def select(
         self, 
@@ -60,15 +60,17 @@
     ) -> Select:
 
         select_clause: Select = self.selected.table.select()
 
         if filters:
             for field_name, value in filters.items():
                 select_clause = select_clause.where(
-                    self.selected.columns.get(field_name) == value
+                    self.selected.columns.get(field_name) == self.selected.types_map.get(
+                        field_name
+                    )(value)
                 )
 
         return select_clause
     
     def insert(
         self,
         users: List[M]
@@ -87,41 +89,46 @@
         filters: Optional[Dict[str, Any]]={}
     ) -> List[Update]:
         
         updates: List[Update] = []
 
         for user in users:
 
-            update_columns = user.dict(
-                exclude_none=True,
-                exclude_unset=True
-            )
-
-
             update_clause: Update = self.selected.table.update()
 
 
             for field_name, value in filters.items():
                 update_clause = update_clause.where(
-                    self.selected.columns.get(field_name) == value
+                    self.selected.columns.get(field_name) == self.selected.types_map.get(
+                        field_name
+                    )(value)
                 )
 
-            update_clause = update_clause.values(**update_columns)
+            update_clause = update_clause.values({
+                name: self.selected.types_map.get(
+                    name
+                )(value) for name, value in user.dict(  
+                    exclude_none=True,
+                    exclude_unset=True
+                ).items()
+            })
             updates.append(update_clause)
 
         return updates
     
     def delete(
         self,
         filters: Dict[str, Any]
     ) -> List[Delete]:
         
         delete_clause: Delete = self.selected.table.delete()
 
         if filters:
             for field_name, value in filters.items():
                 delete_clause = delete_clause.where(
-                    self.selected.columns.get(field_name) == value
+                    self.selected.columns.get(field_name) == self.selected.types_map.get(
+                        field_name
+                    )(value)
                 )
 
         return delete_clause
```

### Comparing `dcrx-api-0.1.0/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.1.1/dcrx_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -109,15 +109,15 @@
 {
   "name": "hello-world",
   "tag": "latest",
   "layers": [
     {
       "layer_type": "stage",
       "base": "python",
-      "tag": "3.11-slim",
+      "tag": "3.11-slim"
     },
     {
         "layer_type": "entrypoint",
         "command": [
             "echo",
             "Hello world!"
         ]
@@ -152,13 +152,30 @@
 
 To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
 
 ```bash
 docker run -p 2277:2277 --env-file .env --privileged dcrx-api:latest
 ```
 
+# Deploying via Helm
+
+DCRX-API has a minimal helm chart to help you scale up when ready. To begin, first create a Kuberenetes secret as below:
+
+```
+kubectl create secret generic dcrx-api-secrets --from-literal="DCRX_API_SECRET_KEY=$DCRX_API_SECRET_KEY" --from-literal="DOCKER_REGISTRY_USERNAME=$DOCKER_REGISTRY_USERNAME" --from-literal="DOCKER_REGISTRY_PASSWORD=$DOCKER_REGISTRY_PASSWORD"
+
+```
+
+Then install the provided helm chart:
+
+```
+helm install dcrx-api helm/dcrx-api/ --values helm/dcrx-api/values.yml
+```
+
+The chart creates three replica dcrx-api pods, a LoadBalancer service, and Nginx ingress to get you up and running in your Kubernetes cluster!
+
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.1.0/setup.py` & `dcrx-api-0.1.1/setup.py`

 * *Files identical despite different names*

