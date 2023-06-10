# Comparing `tmp/dcrx-api-0.1.7.tar.gz` & `tmp/dcrx-api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.1.7.tar", last modified: Sat Jun 10 01:38:17 2023, max compression
+gzip compressed data, was "dcrx-api-0.1.8.tar", last modified: Sat Jun 10 02:14:05 2023, max compression
```

## Comparing `dcrx-api-0.1.7.tar` & `dcrx-api-0.1.8.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.472270 dcrx-api-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 01:38:17.472270 dcrx-api-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.460270 dcrx-api-0.1.7/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.464270 dcrx-api-0.1.7/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.464270 dcrx-api-0.1.7/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.464270 dcrx-api-0.1.7/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.464270 dcrx-api-0.1.7/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.464270 dcrx-api-0.1.7/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.464270 dcrx-api-0.1.7/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.468270 dcrx-api-0.1.7/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.468270 dcrx-api-0.1.7/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.468270 dcrx-api-0.1.7/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.468270 dcrx-api-0.1.7/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.468270 dcrx-api-0.1.7/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.472270 dcrx-api-0.1.7/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.472270 dcrx-api-0.1.7/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.472270 dcrx-api-0.1.7/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:38:17.464270 dcrx-api-0.1.7/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 01:38:17.000000 dcrx-api-0.1.7/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 01:38:17.000000 dcrx-api-0.1.7/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:38:17.000000 dcrx-api-0.1.7/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 01:38:17.000000 dcrx-api-0.1.7/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 01:38:17.000000 dcrx-api-0.1.7/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 01:38:17.000000 dcrx-api-0.1.7/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 01:38:17.472270 dcrx-api-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-10 01:38:14.000000 dcrx-api-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.365606 dcrx-api-0.1.8/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:05.369606 dcrx-api-0.1.8/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 02:14:05.000000 dcrx-api-0.1.8/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:14:05.373606 dcrx-api-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-10 02:14:01.000000 dcrx-api-0.1.8/setup.py
```

### Comparing `dcrx-api-0.1.7/LICENSE` & `dcrx-api-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/PKG-INFO` & `dcrx-api-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.7
+Version: 0.1.8
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.1.7/README.md` & `dcrx-api-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/cli/base.py` & `dcrx-api-0.1.8/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/cli/database.py` & `dcrx-api-0.1.8/dcrx_api/cli/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,44 @@
 ):
 
     loop = asyncio.get_event_loop()
 
     connection = UsersConnection(env)
     connection.setup()
 
-    engine_url = connection.engine.url
+    if connection.config.database_type == 'mysql':
+        engine_url = ['mysql://']
+        
+    elif connection.config.database_type == 'asyncpg':
+        engine_url = ['postgresql://']
+
+    else:
+        engine_url = ['sqlite://']
+
+    if connection.config.database_username and connection.config.database_password:
+        engine_url.append(
+            f'{connection.config.database_username}:{connection.config.database_password}@'
+        )
+
+    if connection.config.database_port:
+        engine_url.append(
+            f'{connection.config.database_uri}:{connection.config.database_port}/{connection.config.database_name}'
+        )
+
+    elif connection.config.database_uri:
+        engine_url.append(
+            f'{connection.config.database_uri}/{connection.config.database_name}'
+        )
+
+    else:
+        engine_url.append(
+            f'/{connection.config.database_name}'
+        )
+
+    engine_url = ''.join(engine_url)
 
     api_database_exists = await loop.run_in_executor(
         None,
         functools.partial(
             database_exists,
             engine_url
         )
```

### Comparing `dcrx-api-0.1.7/dcrx_api/cli/server.py` & `dcrx-api-0.1.8/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/context/manager.py` & `dcrx-api-0.1.8/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/database/connection.py` & `dcrx-api-0.1.8/dcrx_api/database/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,46 +45,59 @@
             AsyncConnection,
             None
         ] = None
 
         self.loop: Union[asyncio.AbstractEventLoop, None] = None
 
     def setup(self):
+
+        if self.config.database_type == 'asyncpg':
+            engine_url = ['postgresql+asyncpg://']
+
+        elif self.config.database_type == 'sqlite':
+            engine_url = ['sqlite+aiosqlite://']
+
+        if self.config.database_username and self.config.database_password:
+            engine_url.append(
+                f'{self.config.database_username}:{self.config.database_password}@'
+            )
+
+        if self.config.database_port:
+            engine_url.append(
+                f'{self.config.database_uri}:{self.config.database_port}/{self.config.database_name}'
+            )
+
+        elif self.config.database_uri:
+            engine_url.append(
+                f'{self.config.database_uri}/{self.config.database_name}'
+            )
+
+        else:
+            engine_url.append(
+                f'/{self.config.database_name}'
+            )
+
+
+        engine_url = ''.join(engine_url)
+
         if self.engine is None and self.config.database_type == 'mysql':
             self.engine = create_engine(
                 user=self.config.database_username,
                 password=self.config.database_password,
                 host=self.config.database_uri,
                 database=self.config.database_name,
                 loop=self.loop
             )
 
         elif self.engine is None and self.config.database_type == 'asyncpg':
             
-            connection_string = ['postgresql+asyncpg://']
-            
-            if self.config.database_username and self.config.database_password:
-                connection_string.append(
-                    f'{self.config.database_username}:{self.config.database_password}@'
-                )
-
-            database_port = self.config.database_port
-            if database_port is None:
-                database_port = 5432
-
-            connection_string.append(
-                f'{self.config.database_uri}:{database_port}/{self.config.database_name}'
-            )
-
-            connection_string = ''.join(connection_string)
-
-            self.engine = create_async_engine(connection_string)
+            self.engine = create_async_engine(engine_url)
 
         elif self.engine is None and self.config.database_type == 'sqlite':
-            self.engine = create_async_engine(self.config.database_uri)
+            self.engine = create_async_engine(engine_url)
 
     async def connect(self):
         self.loop = asyncio.get_event_loop()    
 
         if self.engine is None:
             self.setup()
```

### Comparing `dcrx-api-0.1.7/dcrx_api/env/env.py` & `dcrx-api-0.1.8/dcrx_api/env/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class Env(BaseModel):
     DCRX_API_WORKERS: StrictInt=psutil.cpu_count()
     DCRX_API_SECRET_KEY: StrictStr
     DCRX_API_AUTH_ALGORITHM: StrictStr='HS256'
     DCRX_API_TOKEN_EXPIRATION_MINUTES: StrictInt=30
     DCRX_API_DATABASE_TYPE: Optional[StrictStr]='sqlite'
     DCRX_API_DATABASE_USER: Optional[StrictStr]
-    DCRX_API_DATABASE_URI: StrictStr
+    DCRX_API_DATABASE_URI: Optional[StrictStr]
     DCRX_API_DATABASE_PORT: Optional[StrictInt]
     DCRX_API_DATABASE_PASSWORD: Optional[StrictStr]
     DCRX_API_DATABASE_NAME: StrictStr='dcrx'
     DOCKER_REGISTRY_URI: StrictStr
     DOCKER_REGISTRY_USERNAME: StrictStr
     DOCKER_REGISTRY_PASSWORD: StrictStr
```

### Comparing `dcrx-api-0.1.7/dcrx_api/env/load_env.py` & `dcrx-api-0.1.8/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/lifespan.py` & `dcrx-api-0.1.8/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.1.8/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/auth/manager.py` & `dcrx-api-0.1.8/dcrx_api/services/auth/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/context.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/job.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,22 +63,15 @@
             name='dcrx.api.id',
             value=str(self.job_id)
         )
 
         self.image.layers.insert(1, dcrx_api_label)
         self.job_image_label = f'{dcrx_api_label.name}={dcrx_api_label.value}'
     
-        self.push_timeout_minutes: Union[int, None] = None
-
-    async def run(
-        self,
-        timeout: int
-    ):
-
-        self.push_timeout_minutes = timeout
+    async def run(self):
         
         await self.connection.create([
             self.metadata
         ])
 
         try:
             await self.login_to_registry()
```

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 
 class JobQueue:
 
     def __init__(self, env: Env) -> None:
 
         self.pool_size = env.DCRX_API_WORKERS
-        self.push_timeout_minutes = env.DCRX_API_PUSH_TIMEOUT_MINUTES
 
         self.registry_uri = env.DOCKER_REGISTRY_URI
         self.registry_username = env.DOCKER_REGISTRY_USERNAME
         self.registry_password = env.DOCKER_REGISTRY_PASSWORD
 
         self._jobs: Dict[uuid.UUID, Job] = {}
         self._active: Dict[uuid.UUID, asyncio.Task] = {}
@@ -47,15 +46,15 @@
             build_options=build_options,
             pool_size=self.pool_size
         )
 
         self._jobs[job.job_id] = job
 
         self._active[job.job_id] = asyncio.create_task(
-            job.run(self.push_timeout_minutes)
+            job.run()
         )
 
         return job.metadata
 
     def get(self, job_id: uuid.UUID) -> Union[JobMetadata, JobNotFoundException]:
         job = self._jobs.get(job_id)
         if job is None:
```

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/service.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.1.8/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/users/connection.py` & `dcrx-api-0.1.8/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/users/context.py` & `dcrx-api-0.1.8/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/users/service.py` & `dcrx-api-0.1.8/dcrx_api/services/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.1.8/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.1.8/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.1.8/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.1.8/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.1.8/dcrx_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.7
+Version: 0.1.8
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.1.7/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.1.8/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.7/setup.py` & `dcrx-api-0.1.8/setup.py`

 * *Files identical despite different names*

