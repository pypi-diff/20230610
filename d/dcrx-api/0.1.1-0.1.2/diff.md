# Comparing `tmp/dcrx-api-0.1.1.tar.gz` & `tmp/dcrx-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.1.1.tar", last modified: Sat Jun 10 00:29:19 2023, max compression
+gzip compressed data, was "dcrx-api-0.1.2.tar", last modified: Sat Jun 10 00:45:38 2023, max compression
```

## Comparing `dcrx-api-0.1.1.tar` & `dcrx-api-0.1.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:29:19.802524 dcrx-api-0.1.1/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 00:29:19.000000 dcrx-api-0.1.1/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:29:19.806524 dcrx-api-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-10 00:29:13.000000 dcrx-api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.729386 dcrx-api-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 00:45:38.729386 dcrx-api-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.717386 dcrx-api-0.1.2/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.721386 dcrx-api-0.1.2/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.725386 dcrx-api-0.1.2/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.725386 dcrx-api-0.1.2/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.725386 dcrx-api-0.1.2/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.725386 dcrx-api-0.1.2/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.729386 dcrx-api-0.1.2/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:45:38.717386 dcrx-api-0.1.2/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 00:45:38.000000 dcrx-api-0.1.2/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 00:45:38.000000 dcrx-api-0.1.2/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:45:38.000000 dcrx-api-0.1.2/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 00:45:38.000000 dcrx-api-0.1.2/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 00:45:38.000000 dcrx-api-0.1.2/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 00:45:38.000000 dcrx-api-0.1.2/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:45:38.729386 dcrx-api-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-10 00:45:33.000000 dcrx-api-0.1.2/setup.py
```

### Comparing `dcrx-api-0.1.1/LICENSE` & `dcrx-api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/PKG-INFO` & `dcrx-api-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,15 +25,15 @@
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
-DCRX is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
+Dcrx-api is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
 
 ```bash
 python -m venv ~/.dcrx && \
 source ~/.dcrx/bin/activate && \
 pip install dcrx-api
 ```
 
@@ -42,15 +42,15 @@
 ```
 docker pull adalundhe/dcrx-api:latest
 ```
 
 
 # Getting Started
 
-Dcrx requires a slew of environmental variables in order to run correctly. These include:
+Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
 
 ```
 DCRX_API_WORKERS=10 # Number of workers to use for Job executor. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
```

### Comparing `dcrx-api-0.1.1/README.md` & `dcrx-api-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
-DCRX is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
+Dcrx-api is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
 
 ```bash
 python -m venv ~/.dcrx && \
 source ~/.dcrx/bin/activate && \
 pip install dcrx-api
 ```
 
@@ -24,15 +24,15 @@
 ```
 docker pull adalundhe/dcrx-api:latest
 ```
 
 
 # Getting Started
 
-Dcrx requires a slew of environmental variables in order to run correctly. These include:
+Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
 
 ```
 DCRX_API_WORKERS=10 # Number of workers to use for Job executor. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
```

### Comparing `dcrx-api-0.1.1/dcrx_api/cli/base.py` & `dcrx-api-0.1.2/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/cli/database.py` & `dcrx-api-0.1.2/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/cli/server.py` & `dcrx-api-0.1.2/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/context/manager.py` & `dcrx-api-0.1.2/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/database/connection.py` & `dcrx-api-0.1.2/dcrx_api/database/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import os
 from sqlalchemy import Table
 from sqlalchemy.sql import (
     Select,
     Insert,
     Update,
     Delete
 )
@@ -58,20 +57,30 @@
                 password=self.config.database_password,
                 host=self.config.database_uri,
                 database=self.config.database_name,
                 loop=self.loop
             )
 
         elif self.engine is None and self.config.database_type == 'asyncpg':
-            self.engine = create_async_engine(
-                self.config.database_uri,
-                user=self.config.database_username,
-                password=self.config.database_password,
-                database=self.config.database_name
-            )
+            
+            connection_string = ['postgresql+asyncpg://']
+            
+            if self.config.database_username and self.config.database_password:
+                connection_string.append(
+                    f'{self.config.database_username}:{self.config.database_password}@'
+                )
+
+            connection_string.append(self.config.database_uri)
+
+            if self.config.database_name:
+                connection_string.append(self.config.database_name)
+
+            connection_string = ''.join(connection_string)
+
+            self.engine = create_async_engine(connection_string)
 
         elif self.engine is None and self.config.database_type == 'sqlite':
             self.engine = create_async_engine(self.config.database_uri)
 
         self.connection = await self.engine.connect()
 
     async def create_table(
```

### Comparing `dcrx-api-0.1.1/dcrx_api/env/env.py` & `dcrx-api-0.1.2/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/env/load_env.py` & `dcrx-api-0.1.2/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/lifespan.py` & `dcrx-api-0.1.2/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.1.2/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/auth/manager.py` & `dcrx-api-0.1.2/dcrx_api/services/auth/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/context.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/job.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/job.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/queue.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/service.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.1.2/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/users/connection.py` & `dcrx-api-0.1.2/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/users/context.py` & `dcrx-api-0.1.2/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/users/service.py` & `dcrx-api-0.1.2/dcrx_api/services/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.1.2/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.1.2/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.1.2/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.1.2/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.1.2/dcrx_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,15 +25,15 @@
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
-DCRX is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
+Dcrx-api is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
 
 ```bash
 python -m venv ~/.dcrx && \
 source ~/.dcrx/bin/activate && \
 pip install dcrx-api
 ```
 
@@ -42,15 +42,15 @@
 ```
 docker pull adalundhe/dcrx-api:latest
 ```
 
 
 # Getting Started
 
-Dcrx requires a slew of environmental variables in order to run correctly. These include:
+Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
 
 ```
 DCRX_API_WORKERS=10 # Number of workers to use for Job executor. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
```

### Comparing `dcrx-api-0.1.1/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.1.2/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.1/setup.py` & `dcrx-api-0.1.2/setup.py`

 * *Files identical despite different names*

