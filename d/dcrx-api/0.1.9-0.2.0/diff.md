# Comparing `tmp/dcrx-api-0.1.9.tar.gz` & `tmp/dcrx-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.1.9.tar", last modified: Sat Jun 10 02:22:31 2023, max compression
+gzip compressed data, was "dcrx-api-0.2.0.tar", last modified: Sat Jun 10 17:11:03 2023, max compression
```

## Comparing `dcrx-api-0.1.9.tar` & `dcrx-api-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:22:31.683076 dcrx-api-0.1.9/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 02:22:31.000000 dcrx-api-0.1.9/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:22:31.687076 dcrx-api-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-10 02:22:28.000000 dcrx-api-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.018736 dcrx-api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/server_memory_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-10 17:11:03.000000 dcrx-api-0.2.0/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:11:03.018736 dcrx-api-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/setup.py
```

### Comparing `dcrx-api-0.1.9/LICENSE` & `dcrx-api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/PKG-INFO` & `dcrx-api-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.9
+Version: 0.2.0
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,15 +45,17 @@
 
 
 # Getting Started
 
 Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
 
 ```
-DCRX_API_WORKERS=10 # Number of workers to use for Job executor. Default is the number os OS threads.
+DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
+
+DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
@@ -61,15 +63,17 @@
 
 DCRX_API_DATABASE_USER=admin # Username used for database connection authentication
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
-DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users
+DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
+
+DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
 DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
 
 DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
 
 DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
 ```
```

### Comparing `dcrx-api-0.1.9/README.md` & `dcrx-api-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 
 
 # Getting Started
 
 Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
 
 ```
-DCRX_API_WORKERS=10 # Number of workers to use for Job executor. Default is the number os OS threads.
+DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
+
+DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
@@ -43,15 +45,17 @@
 
 DCRX_API_DATABASE_USER=admin # Username used for database connection authentication
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
-DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users
+DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
+
+DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
 DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
 
 DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
 
 DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
 ```
```

### Comparing `dcrx-api-0.1.9/dcrx_api/cli/base.py` & `dcrx-api-0.2.0/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/cli/database.py` & `dcrx-api-0.2.0/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/cli/server.py` & `dcrx-api-0.2.0/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/context/manager.py` & `dcrx-api-0.2.0/dcrx_api/context/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from dcrx_api.services.auth.context import AuthServiceContext
 from dcrx_api.services.jobs.context import JobServiceContext
+from dcrx_api.services.monitoring.context import MonitoringServiceContext
 from dcrx_api.services.users.context import UsersServiceContext
 from typing import Dict, Union, List
 from .types import ContextType
 
 
 class ContextManager:
 
     def __init__(self) -> None:
         self.contexts: Dict[
             ContextType, 
             Union[
                 AuthServiceContext,
                 JobServiceContext, 
+                MonitoringServiceContext,
                 UsersServiceContext
             ]
         ] = {}
 
     
     def get(self, context_type: ContextType) -> Union[
         AuthServiceContext,
         JobServiceContext,
+        MonitoringServiceContext,
         UsersServiceContext,
         None
     ]:
         return self.contexts.get(context_type)
 
     async def initialize(
         self,
         contexts: List[
             Union[
                 AuthServiceContext,
                 JobServiceContext,
+                MonitoringServiceContext,
                 UsersServiceContext
             ]
         ]
     ):
         
         for context in contexts:
             await context.initialize()
```

### Comparing `dcrx-api-0.1.9/dcrx_api/database/connection.py` & `dcrx-api-0.2.0/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/env/env.py` & `dcrx-api-0.2.0/dcrx_api/env/env.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import psutil
 from pydantic import (
     BaseModel,
     StrictStr,
-    StrictInt
+    StrictInt,
+    StrictFloat
 )
 from typing import (
     Optional, 
     Dict, 
     Union,
     Callable
 )
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
-    DCRX_API_WORKERS: StrictInt=psutil.cpu_count()
+    DCRX_API_MAX_MEMORY_PERCENT_USAGE: StrictFloat=50
+    DCRX_API_JOB_PRUNE_INTERVAL: StrictStr='1s'
+    DCRX_API_JOB_MAX_AGE: StrictStr='1m'
+    DCRX_API_JOB_WORKERS: StrictInt=psutil.cpu_count()
+    DCRX_API_JOB_POOL_SIZE: StrictInt=10
     DCRX_API_SECRET_KEY: StrictStr
     DCRX_API_AUTH_ALGORITHM: StrictStr='HS256'
     DCRX_API_TOKEN_EXPIRATION_MINUTES: StrictInt=30
     DCRX_API_DATABASE_TYPE: Optional[StrictStr]='sqlite'
     DCRX_API_DATABASE_USER: Optional[StrictStr]
     DCRX_API_DATABASE_URI: Optional[StrictStr]
     DCRX_API_DATABASE_PORT: Optional[StrictInt]
@@ -29,15 +34,19 @@
     DOCKER_REGISTRY_URI: StrictStr
     DOCKER_REGISTRY_USERNAME: StrictStr
     DOCKER_REGISTRY_PASSWORD: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
-            'DCRX_API_WORKERS': int,
+            'DCRX_API_MAX_MEMORY_PERCENT_USAGE': float,
+            'DCRX_API_JOB_PRUNE_INTERVAL': str,
+            'DCRX_API_JOB_MAX_AGE': str,
+            'DCRX_API_JOB_WORKERS': int,
+            'DCRX_API_JOB_POOL_SIZE': int,
             'DCRX_API_SECRET_KEY': str,
             'DCRX_API_AUTH_ALGORITHM': str,
             'DCRX_API_TOKEN_EXPIRATION_MINUTES': int,
             'DCRX_API_DATABASE_TYPE': str,
             'DCRX_API_DATABASE_USER': str,
             'DCRX_API_DATABASE_PASSWORD': str,
             'DCRX_API_DATABASE_NAME': str,
```

### Comparing `dcrx-api-0.1.9/dcrx_api/env/load_env.py` & `dcrx-api-0.2.0/dcrx_api/env/load_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         if envar_value:
             values[envar_name] = envar_type(envar_value)
 
     if env_file and os.path.exists(env_file):
         env_file_values = dotenv_values(dotenv_path=env_file)
 
         for envar_name, envar_value in env_file_values.items():
-            env_file_values[envar_name] = envars.get(
-                envar_name
-            )(envar_value)
+            envar_type = envars.get(envar_name)
+            if envar_type:
+                env_file_values[envar_name] = envar_type(envar_value)
 
         values.update(env_file_values)
 
     return Env(**{
         name: value for name, value in values.items() if value is not None
     })
```

### Comparing `dcrx-api-0.1.9/dcrx_api/lifespan.py` & `dcrx-api-0.2.0/dcrx_api/lifespan.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,35 +9,60 @@
     JobsConnection,
     JobServiceContext
 )
 from dcrx_api.services.users.context import (
     UsersConnection,
     UsersServiceContext
 )
+from dcrx_api.services.monitoring.context import (
+    CPUMonitor,
+    DockerMemoryMonitor,
+    MemoryMonitor,
+    MonitoringServiceContext
+)
+
 from dcrx_api.context.manager import context
 from .env import load_env, Env
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
 
     env = load_env(Env.types_map())
 
-    await context.initialize([
-        AuthServiceContext(
-            env=env,
-            manager=AuthorizationSessionManager(env)
-        ),
-        JobServiceContext(
-            env=env,
-            queue=JobQueue(env),
-            connection=JobsConnection(env)
+    auth_service_context = AuthServiceContext(
+        env=env,
+        manager=AuthorizationSessionManager(env)
+    )
+
+    job_service_context = JobServiceContext(
+        env=env,
+        queue=JobQueue(env),
+        connection=JobsConnection(env)
+    )
+
+    monitoring_service_context = MonitoringServiceContext(
+        env=env,
+        monitor_name='dcrx.main',
+        cpu=CPUMonitor(),
+        docker_memory=DockerMemoryMonitor(
+            env,
+            job_service_context.queue
         ),
-        UsersServiceContext(
-            env=env,
-            connection=UsersConnection(env)
-        )
+        memory=MemoryMonitor()
+    )
+
+    users_service_context = UsersServiceContext(
+        env=env,
+        connection=UsersConnection(env)
+    )
+
+    await context.initialize([
+        auth_service_context,
+        job_service_context,
+        monitoring_service_context,
+        users_service_context
     ])
 
     yield
 
     await context.close()
```

### Comparing `dcrx-api-0.1.9/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.2.0/dcrx_api/middleware/auth_middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,16 +30,26 @@
 
         authorization = await auth_service_context.manager.verify_token(
             users_service_context.connection,
             token
         )
 
         if authorization.error:
-            return Response(
+            response = Response(
                 status_code=401,
                 content=json.dumps({
                     'detail': authorization.error
                 })
             )
 
+            if token:
+                response.delete_cookie(
+                    'X-Auth-Token',
+                    httponly=True,
+                    secure=True,
+                    samesite='strict'
+                )
+
+            return response
+
         response = await call_next(request)
         return response
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/auth/manager.py` & `dcrx-api-0.2.0/dcrx_api/services/auth/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import datetime
 import functools
 from concurrent.futures import ThreadPoolExecutor
 from dcrx_api.env import Env
 from jose import JWTError, jwt
 from fastapi.security import OAuth2PasswordBearer
+from fastapi.security.utils import get_authorization_scheme_param
 from passlib.context import CryptContext
 from typing import (
     Optional,
     Dict,
     Any,
     List,
     Union
@@ -25,15 +26,15 @@
 )
 
 
 class AuthorizationSessionManager:
 
     def __init__(self, env: Env) -> None:
 
-        self.pool_size = env.DCRX_API_WORKERS
+        self.pool_size = env.DCRX_API_JOB_WORKERS
         self.context = CryptContext(
             schemes=["bcrypt"], 
             deprecated="auto"
         )
 
         self.scheme = OAuth2PasswordBearer(tokenUrl="token")
         self.secret_key = env.DCRX_API_SECRET_KEY
@@ -159,29 +160,36 @@
         try:
 
             if token is None:
                 return AuthResponse(
                     error='No token provided',
                     message='Authentication failed'
                 )
+            
+            scheme, value = get_authorization_scheme_param(token)
+            if scheme.lower() != 'bearer':
+                return AuthResponse(
+                    error='User authorization failed',
+                    message='Authentication failed'
+                )
 
             payload = await self._loop.run_in_executor(
                 self._executor,
                 functools.partial(
                     jwt.decode,
-                    token, 
+                    value, 
                     self.secret_key, 
                     algorithms=[self.auth_algorithm]
                 )
             )
 
             username: str = payload.get("sub")
             if username is None:
                 return AuthResponse(
-                    error='User not found',
+                    error='User authorization failed',
                     message='Authentication failed'
                 )
             
             token_data = AuthClaims(username=username)
 
         except JWTError as validation_error:
             return AuthResponse(
@@ -193,15 +201,15 @@
             filters={
                 'username': token_data.username
             }
         )
 
         if len(users) < 1:
             return AuthResponse(
-                error='User not found',
+                error='User authorization failed',
                 message='Authentication failed'
             )
         
         return AuthResponse(
             message='OK'
         )
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/context.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,13 +13,14 @@
     context_type: ContextType=ContextType.JOB_SERVICE
 
 
     class Config:
         arbitrary_types_allowed = True
 
     async def initialize(self):
+        await self.queue.start()
         await self.connection.connect()
         await self.connection.init()
 
     async def close(self):
         await self.queue.close()
         await self.connection.close()
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/job.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/job.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import asyncio
 import docker
 import functools
 import psutil
 import time
 import uuid
 from concurrent.futures import ThreadPoolExecutor
+from docker.models.images import Image as DockerImage
 from dcrx.image import Image, Label
 from dcrx.memory_file import MemoryFile
 from .models import (
     BuildOptions,
+    ImageStats,
     JobMetadata,
     Registry
 )
 from typing import (
     Union, 
     Optional, 
     Dict, 
-    Any
+    Any,
+    List
 )
 from .status import JobStatus
 from .connection import JobsConnection
 
 
 class Job:
 
@@ -62,14 +65,25 @@
         dcrx_api_label = Label(
             name='dcrx.api.id',
             value=str(self.job_id)
         )
 
         self.image.layers.insert(1, dcrx_api_label)
         self.job_image_label = f'{dcrx_api_label.name}={dcrx_api_label.value}'
+        self.job_start_time = time.monotonic()
+        self.image_stats = ImageStats()
+
+    async def list(self) -> List[DockerImage]:
+        return await self.loop.run_in_executor(
+            self._executor,
+            functools.partial(
+                self.client.images.list,
+                self.image.name
+            )
+        )
     
     async def run(self):
         
         await self.connection.create([
             self.metadata
         ])
 
@@ -154,37 +168,42 @@
         })
 
         build_options: Dict[str, Any] = {}
 
         if self.build_options:
             build_options = self.build_options.dict()
 
-        await self.loop.run_in_executor(
+        image_result = await self.loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.client.images.build,
                 dockerfile=self.image.filename,
                 fileobj=self.context,
                 tag=self.image.full_name,
                 custom_context=True,
                 forcerm=True,
                 **build_options
             )   
         )
 
-
+        image, _ = image_result 
+        self.image_stats = ImageStats(
+            size=int(image.attrs.get('Size', 0)/10**6)
+        )
+        
     async def push_image(self):
 
         self.metadata = JobMetadata(
             id=self.job_id,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.PUSHING.value,
-            context=f'Job {self.job_id} pushing image {self.image.full_name} to registry {self.registry.registry_uri}'
+            context=f'Job {self.job_id} pushing image {self.image.full_name} to registry {self.registry.registry_uri}',
+            size=self.image_stats.size
         )
 
         await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
@@ -243,25 +262,28 @@
 
         self.metadata = JobMetadata(
             id=self.job_id,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=status.value,
-            context=context
+            context=context,
+            size=self.image_stats.size
         )
         
 
         await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
         self._executor.shutdown(cancel_futures=True)
         self.client.close()
-        self.context.close()
+
+        if self.context:
+            self.context.close()
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/models/new_image.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,34 +16,35 @@
     Label,
     Run,
     Stage,
     User,
     Volume,
     Workdir
 )
-
-
 from typing import List, Union, Optional
 from .build_options import BuildOptions
 
 
+Layer = Union[
+    Add,
+    Arg,
+    Cmd,
+    Copy,
+    Entrypoint,
+    Env,
+    Expose,
+    Healthcheck,
+    Label,
+    Run,
+    Stage,
+    User,
+    Volume,
+    Workdir
+]
+
+
 class NewImage(BaseModel):
     name: StrictStr
     tag: StrictStr='latest'
     files: Optional[List[StrictStr]]
     build_options: Optional[BuildOptions]
-    layers: conlist(Union[
-        Add,
-        Arg,
-        Cmd,
-        Copy,
-        Entrypoint,
-        Env,
-        Expose,
-        Healthcheck,
-        Label,
-        Run,
-        Stage,
-        User,
-        Volume,
-        Workdir
-    ], min_items=1)
+    layers: conlist(Layer, min_items=1)
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,30 +33,36 @@
             sqlalchemy.Column(
                 'status',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'context',
                 sqlalchemy.TEXT
+            ),
+            sqlalchemy.Column(
+                'size',
+                sqlalchemy.INTEGER
             )
         )
 
         self.columns = {
             'id': self.table.c.id,
             'name': self.table.c.name,
             'image': self.table.c.image,
             'tag': self.table.c.tag,
             'status': self.table.c.status,
             'context': self.table.c.context,
+            'size': self.table.c.size
         }
 
         self.types_map = {
             'id': lambda value: str(value),
             'name': lambda value: str(value),
             'image': lambda value: str(value),
             'tag': lambda value: str(value),
             'status': lambda value: str(value),
-            'context': lambda value: str(value)
+            'context': lambda value: str(value),
+            'size': lambda value: int(value)
         }
 
         self.table_type = TableTypes.MYSQL
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,30 +34,36 @@
             sqlalchemy.Column(
                 'status',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'context',
                 sqlalchemy.TEXT
+            ),
+            sqlalchemy.Column(
+                'size',
+                sqlalchemy.BIGINT
             )
         )
 
         self.columns = {
             'id': self.table.c.id,
             'name': self.table.c.name,
             'image': self.table.c.image,
             'tag': self.table.c.tag,
             'status': self.table.c.status,
             'context': self.table.c.context,
+            'size': self.table.c.size
         }
 
         self.types_map = {
             'id': lambda value: uuid.UUID(value),
             'name': lambda value: str(value),
             'image': lambda value: str(value),
             'tag': lambda value: str(value),
             'status': lambda value: str(value),
-            'context': lambda value: str(value)
+            'context': lambda value: str(value),
+            'size': lambda value: int(value)
         }
 
         self.table_type = TableTypes.POSTGRES
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,30 +33,36 @@
             sqlalchemy.Column(
                 'status',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'context',
                 sqlalchemy.TEXT
+            ),
+            sqlalchemy.Column(
+                'size',
+                sqlalchemy.INTEGER
             )
         )
 
         self.columns = {
             'id': self.table.c.id,
             'name': self.table.c.name,
             'image': self.table.c.image,
             'tag': self.table.c.tag,
             'status': self.table.c.status,
             'context': self.table.c.context,
+            'size': self.table.c.size
         }
 
         self.types_map = {
             'id': lambda value: str(value).encode(),
             'name': lambda value: str(value),
             'image': lambda value: str(value),
             'tag': lambda value: str(value),
             'status': lambda value: str(value),
-            'context': lambda value: str(value)
+            'context': lambda value: str(value),
+            'size': lambda value: int(value)
         }
 
         self.table_type = TableTypes.MYSQL
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,15 @@
                     )(value)
                 )
 
             update_clause = update_clause.values({
                 name: self.selected.types_map.get(
                     name
                 )(value) for name, value in job.dict(  
-                    exclude_none=True,
-                    exclude_unset=True
+                    exclude_none=True
                 ).items()
             })
 
             updates.append(update_clause)
 
         return updates
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/users/connection.py` & `dcrx-api-0.2.0/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/services/users/context.py` & `dcrx-api-0.2.0/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/services/users/service.py` & `dcrx-api-0.2.0/dcrx_api/services/users/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,19 @@
 
     response = JSONResponse(
         content=success_response.dict()
     )
 
     response.set_cookie(
         key='X-Auth-Token',
-        value=authorization.token,
-        expires=authorization.token_expires
+        value=f'Bearer {authorization.token}',
+        expires=authorization.token_expires,
+        httponly=True,
+        secure=True,
+        samesite='strict'
     )
 
 
     return response
 
 
 @users_router.get(
```

### Comparing `dcrx-api-0.1.9/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.2.0/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.2.0/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.2.0/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.2.0/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.1.9/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.2.0/dcrx_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.1.9
+Version: 0.2.0
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,15 +45,17 @@
 
 
 # Getting Started
 
 Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
 
 ```
-DCRX_API_WORKERS=10 # Number of workers to use for Job executor. Default is the number os OS threads.
+DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
+
+DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
@@ -61,15 +63,17 @@
 
 DCRX_API_DATABASE_USER=admin # Username used for database connection authentication
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
-DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users
+DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
+
+DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
 DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
 
 DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
 
 DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
 ```
```

### Comparing `dcrx-api-0.1.9/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.2.0/dcrx_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,39 @@
 dcrx_api/services/jobs/__init__.py
 dcrx_api/services/jobs/connection.py
 dcrx_api/services/jobs/context.py
 dcrx_api/services/jobs/job.py
 dcrx_api/services/jobs/queue.py
 dcrx_api/services/jobs/service.py
 dcrx_api/services/jobs/status.py
+dcrx_api/services/jobs/time_parser.py
 dcrx_api/services/jobs/models/__init__.py
 dcrx_api/services/jobs/models/build_options.py
+dcrx_api/services/jobs/models/image_stats.py
 dcrx_api/services/jobs/models/job_metadata.py
 dcrx_api/services/jobs/models/job_not_found_exception.py
 dcrx_api/services/jobs/models/new_image.py
 dcrx_api/services/jobs/models/registry.py
+dcrx_api/services/jobs/models/remote_add.py
+dcrx_api/services/jobs/models/server_memory_limit_exception.py
 dcrx_api/services/jobs/table/__init__.py
 dcrx_api/services/jobs/table/jobs_mysql_table.py
 dcrx_api/services/jobs/table/jobs_postgres_table.py
 dcrx_api/services/jobs/table/jobs_sqlite_table.py
 dcrx_api/services/jobs/table/jobs_table.py
+dcrx_api/services/monitoring/__init__.py
+dcrx_api/services/monitoring/context.py
+dcrx_api/services/monitoring/base/__init__.py
+dcrx_api/services/monitoring/base/exceptions.py
+dcrx_api/services/monitoring/base/monitor.py
+dcrx_api/services/monitoring/cpu/__init__.py
+dcrx_api/services/monitoring/cpu/monitor.py
+dcrx_api/services/monitoring/memory/__init__.py
+dcrx_api/services/monitoring/memory/docker_memory_monitor.py
+dcrx_api/services/monitoring/memory/monitor.py
 dcrx_api/services/users/__init__.py
 dcrx_api/services/users/connection.py
 dcrx_api/services/users/context.py
 dcrx_api/services/users/service.py
 dcrx_api/services/users/models/__init__.py
 dcrx_api/services/users/models/authorized_user.py
 dcrx_api/services/users/models/base_user.py
```

### Comparing `dcrx-api-0.1.9/setup.py` & `dcrx-api-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,26 +61,26 @@
     extras_requires={
         'all': [
             'aiomysql',
             'asyncpg',
             'sqlalchemy',
             'aiosqlite',
             'sqlalchemy-utils',
-            'psycopg2'
+            'psycopg2-binary'
         ],
         'mysql': [
             'aiomysql',
             'sqlalchemy',
             'sqlalchemy-utils'
         ],
         'postgres': [
             'asyncpg',
             'sqlalchemy',
             'sqlalchemy-utils',
-            'psycopg2'
+            'psycopg2-binary'
         ],
         'sqlite': [
             'aiosqlite',
             'sqlalchemy',
             'sqlalchemy-utils'
         ]
     },
```

