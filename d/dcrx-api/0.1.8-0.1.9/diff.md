# Comparing `tmp/dcrx-api-0.1.8.tar.gz` & `tmp/dcrx-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.1.8.tar", last modified: Sat Jun 10 02:14:05 2023, max compression
+gzip compressed data, was "dcrx-api-0.1.9.tar", last modified: Sat Jun 10 02:22:31 2023, max compression
```

## Comparing `dcrx-api-0.1.8.tar` & `dcrx-api-0.1.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.365606 dcrx-api-0.1.8/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/setup.py
```

### Comparing `dcrx-api-0.1.8/LICENSE` & `dcrx-api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/PKG-INFO` & `dcrx-api-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.1.8/README.md` & `dcrx-api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/cli/base.py` & `dcrx-api-0.1.9/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/cli/database.py` & `dcrx-api-0.1.9/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/cli/server.py` & `dcrx-api-0.1.9/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/context/manager.py` & `dcrx-api-0.1.9/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/database/connection.py` & `dcrx-api-0.1.9/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/env/env.py` & `dcrx-api-0.1.9/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/env/load_env.py` & `dcrx-api-0.1.9/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/lifespan.py` & `dcrx-api-0.1.9/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.1.9/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/auth/manager.py` & `dcrx-api-0.1.9/dcrx_api/services/auth/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/context.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/job.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/job.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/queue.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/service.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/users/connection.py` & `dcrx-api-0.1.9/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/users/context.py` & `dcrx-api-0.1.9/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/users/service.py` & `dcrx-api-0.1.9/dcrx_api/services/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.1.9/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.1.9/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.1.9/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.1.9/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.1.9/dcrx_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.1.8/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.1.9/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.8/setup.py` & `dcrx-api-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,25 +60,27 @@
     ],
     extras_requires={
         'all': [
             'aiomysql',
             'asyncpg',
             'sqlalchemy',
             'aiosqlite',
-            'sqlalchemy-utils'
+            'sqlalchemy-utils',
+            'psycopg2'
         ],
         'mysql': [
             'aiomysql',
             'sqlalchemy',
             'sqlalchemy-utils'
         ],
         'postgres': [
             'asyncpg',
             'sqlalchemy',
-            'sqlalchemy-utils'
+            'sqlalchemy-utils',
+            'psycopg2'
         ],
         'sqlite': [
             'aiosqlite',
             'sqlalchemy',
             'sqlalchemy-utils'
         ]
     },
```

