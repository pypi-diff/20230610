# Comparing `tmp/dcrx-api-0.2.0.tar.gz` & `tmp/dcrx-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.2.0.tar", last modified: Sat Jun 10 17:11:03 2023, max compression
+gzip compressed data, was "dcrx-api-0.2.2.tar", last modified: Sat Jun 10 18:07:58 2023, max compression
```

## Comparing `dcrx-api-0.2.0.tar` & `dcrx-api-0.2.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.018736 dcrx-api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/image_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/remote_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/models/server_memory_limit_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/jobs/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/base/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/cpu/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.014736 dcrx-api-0.2.0/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:11:03.010736 dcrx-api-0.2.0/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-10 17:11:03.000000 dcrx-api-0.2.0/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 17:11:02.000000 dcrx-api-0.2.0/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:11:03.018736 dcrx-api-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-10 17:10:56.000000 dcrx-api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/server_memory_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/setup.py
```

### Comparing `dcrx-api-0.2.0/LICENSE` & `dcrx-api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/PKG-INFO` & `dcrx-api-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.2.0
+Version: 0.2.2
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,22 +18,22 @@
 
 # dcrx-api
 [![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
 [![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
 
-Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
+DCRX-API is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! DCRX-API extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
-Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
+DCRX-API also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
-Dcrx-api is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
+DCRX-API is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
 
 ```bash
 python -m venv ~/.dcrx && \
 source ~/.dcrx/bin/activate && \
 pip install dcrx-api
 ```
 
@@ -42,22 +42,28 @@
 ```
 docker pull adalundhe/dcrx-api:latest
 ```
 
 
 # Getting Started
 
-Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
+DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
+DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
+
+DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
+
+DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
+
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
 
 DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
-DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
+DCRX_API_TOKEN_EXPIRATION='15m' # Time for JWT authorization token to expire. Default is 15 minutes.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
 DCRX_API_DATABASE_TYPE=sqlite # Type of database to use. Default is sqlite and options are mysql, asyncpg, and sqlite.
```

### Comparing `dcrx-api-0.2.0/README.md` & `dcrx-api-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # dcrx-api
 [![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
 [![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
 
-Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
+DCRX-API is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! DCRX-API extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
-Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
+DCRX-API also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
-Dcrx-api is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
+DCRX-API is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
 
 ```bash
 python -m venv ~/.dcrx && \
 source ~/.dcrx/bin/activate && \
 pip install dcrx-api
 ```
 
@@ -24,22 +24,28 @@
 ```
 docker pull adalundhe/dcrx-api:latest
 ```
 
 
 # Getting Started
 
-Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
+DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
+DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
+
+DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
+
+DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
+
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
 
 DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
-DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
+DCRX_API_TOKEN_EXPIRATION='15m' # Time for JWT authorization token to expire. Default is 15 minutes.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
 DCRX_API_DATABASE_TYPE=sqlite # Type of database to use. Default is sqlite and options are mysql, asyncpg, and sqlite.
```

### Comparing `dcrx-api-0.2.0/dcrx_api/cli/base.py` & `dcrx-api-0.2.2/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/cli/database.py` & `dcrx-api-0.2.2/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/cli/server.py` & `dcrx-api-0.2.2/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/context/manager.py` & `dcrx-api-0.2.2/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/database/connection.py` & `dcrx-api-0.2.2/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/env/env.py` & `dcrx-api-0.2.2/dcrx_api/env/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     DCRX_API_MAX_MEMORY_PERCENT_USAGE: StrictFloat=50
     DCRX_API_JOB_PRUNE_INTERVAL: StrictStr='1s'
     DCRX_API_JOB_MAX_AGE: StrictStr='1m'
     DCRX_API_JOB_WORKERS: StrictInt=psutil.cpu_count()
     DCRX_API_JOB_POOL_SIZE: StrictInt=10
     DCRX_API_SECRET_KEY: StrictStr
     DCRX_API_AUTH_ALGORITHM: StrictStr='HS256'
-    DCRX_API_TOKEN_EXPIRATION_MINUTES: StrictInt=30
+    DCRX_API_TOKEN_EXPIRATION: StrictStr='15m'
     DCRX_API_DATABASE_TYPE: Optional[StrictStr]='sqlite'
     DCRX_API_DATABASE_USER: Optional[StrictStr]
     DCRX_API_DATABASE_URI: Optional[StrictStr]
     DCRX_API_DATABASE_PORT: Optional[StrictInt]
     DCRX_API_DATABASE_PASSWORD: Optional[StrictStr]
     DCRX_API_DATABASE_NAME: StrictStr='dcrx'
     DOCKER_REGISTRY_URI: StrictStr
@@ -41,15 +41,15 @@
             'DCRX_API_MAX_MEMORY_PERCENT_USAGE': float,
             'DCRX_API_JOB_PRUNE_INTERVAL': str,
             'DCRX_API_JOB_MAX_AGE': str,
             'DCRX_API_JOB_WORKERS': int,
             'DCRX_API_JOB_POOL_SIZE': int,
             'DCRX_API_SECRET_KEY': str,
             'DCRX_API_AUTH_ALGORITHM': str,
-            'DCRX_API_TOKEN_EXPIRATION_MINUTES': int,
+            'DCRX_API_TOKEN_EXPIRATION': str,
             'DCRX_API_DATABASE_TYPE': str,
             'DCRX_API_DATABASE_USER': str,
             'DCRX_API_DATABASE_PASSWORD': str,
             'DCRX_API_DATABASE_NAME': str,
             'DCRX_API_DATABASE_URI': str,
             'DCRX_API_DATABASE_PORT': int,
             'DOCKER_REGISTRY_URI': str,
```

### Comparing `dcrx-api-0.2.0/dcrx_api/env/load_env.py` & `dcrx-api-0.2.2/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/lifespan.py` & `dcrx-api-0.2.2/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.2.2/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/auth/manager.py` & `dcrx-api-0.2.2/dcrx_api/services/auth/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import (
     Optional,
     Dict,
     Any,
     List,
     Union
 )
+from dcrx_api.env.time_parser import TimeParser
 from dcrx_api.services.users.connection import UsersConnection
 from dcrx_api.services.users.models import (
     DBUser,
     LoginUser
 )
 from .models import (
     AuthResponse,
@@ -35,15 +36,15 @@
             schemes=["bcrypt"], 
             deprecated="auto"
         )
 
         self.scheme = OAuth2PasswordBearer(tokenUrl="token")
         self.secret_key = env.DCRX_API_SECRET_KEY
         self.auth_algorithm = env.DCRX_API_AUTH_ALGORITHM
-        self.token_expiration_minutes = env.DCRX_API_TOKEN_EXPIRATION_MINUTES
+        self.token_expiration_time = TimeParser(env.DCRX_API_TOKEN_EXPIRATION).time
 
         self._executor: Union[ThreadPoolExecutor, None] = None
         self._loop: Union[asyncio.AbstractEventLoop, None] = None
 
     async def connect(self):
         self._loop = asyncio.get_event_loop()
         self._executor = ThreadPoolExecutor(max_workers=self.pool_size)
@@ -131,15 +132,15 @@
             login_user.password
         )
 
         if isinstance(user, AuthResponse):
             return user
 
         access_token_expires = datetime.timedelta(
-            minutes=self.token_expiration_minutes
+            seconds=self.token_expiration_time
         )
         
         auth_token = self.create_access_token(
             data={
                 "sub": user.username
             }, 
             expires_delta=access_token_expires
```

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,22 +68,22 @@
                     name: self.table.selected.types_map.get(
                         name
                     )(value) for name, value in filters.items()
                 }
             )
         )
     
-    async def delete(
+    async def remove(
         self,
         filters: Dict[str, Any]
     ):
-        return await self.delete(
+        return await self.delete([
             self.table.delete({
                 name: self.table.selected.types_map.get(
                     name
                 )(value) for name, value in filters.items()
             })
-        )
+        ])
     
     async def drop(self):
         return await self.drop_table(self.table)
```

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/context.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/job.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
             value=str(self.job_id)
         )
 
         self.image.layers.insert(1, dcrx_api_label)
         self.job_image_label = f'{dcrx_api_label.name}={dcrx_api_label.value}'
         self.job_start_time = time.monotonic()
         self.image_stats = ImageStats()
+        self.client_closed = False
 
     async def list(self) -> List[DockerImage]:
         return await self.loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.client.images.list,
                 self.image.name
@@ -217,29 +218,38 @@
             )
         )
 
     async def clear(self):
 
         for layer in self.image.layers:
             if layer.layer_type == 'stage':
-                await self.loop.run_in_executor(
-                    self._executor,
-                    functools.partial(
-                        self.client.images.remove,
-                        f'{layer.base}:{layer.tag}'
+
+                try:
+                    await self.loop.run_in_executor(
+                        self._executor,
+                        functools.partial(
+                            self.client.images.remove,
+                            f'{layer.base}:{layer.tag}'
+                        )
                     )
-                )
+                
+                except Exception:
+                    pass
 
-        await self.loop.run_in_executor(
-            self._executor,
-            functools.partial(
-                self.client.images.remove,
-                self.image.full_name
+        try:
+            await self.loop.run_in_executor(
+                self._executor,
+                functools.partial(
+                    self.client.images.remove,
+                    self.image.full_name
+                )
             )
-        )
+
+        except Exception:
+            pass
 
         await self.loop.run_in_executor(
             self._executor,
             self.image.clear
         )
 
 
@@ -274,15 +284,18 @@
         await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
         self._executor.shutdown(cancel_futures=True)
-        self.client.close()
+
+        if self.client_closed is False:
+            self.client.close()
+            self.client_closed = True
 
         if self.context:
             self.context.close()
```

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/queue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import uuid
 import time
-from dcrx.image import Image
 from dcrx_api.env import Env
+from dcrx_api.env.time_parser import TimeParser
+from dcrx.image import Image
 from docker.models.images import Image as DockerImage
 from .models import BuildOptions
 from .models import Registry
 from typing import (
     Optional, 
     Dict, 
     Union,
@@ -14,15 +15,15 @@
 )
 from .job import Job
 from .connection import JobsConnection
 from .models import (
     JobMetadata,
     JobNotFoundException
 )
-from .time_parser import TimeParser
+from .status import JobStatus
 
 
 class JobQueue:
 
     def __init__(self, env: Env) -> None:
 
         self.pool_size = env.DCRX_API_JOB_WORKERS
@@ -38,14 +39,15 @@
         )
 
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._job_max_age = TimeParser(env.DCRX_API_JOB_MAX_AGE).time
         self._job_prune_interval = TimeParser(env.DCRX_API_JOB_PRUNE_INTERVAL).time
         self._run_cleanup = True
         self.active_images: List[DockerImage] = []
+        self.cancelling: List[asyncio.Task] = []
 
     async def get_active_images(self) -> List[DockerImage]:
 
         active_statuses = [
             'AUTHORIZING',
             'CREATED',
             'GENERATING',
@@ -84,19 +86,40 @@
             queue_jobs = dict(self._jobs)
             
             for job_id, job in queue_jobs.items():
                 
                 job_elapsed = time.monotonic() - job.job_start_time
                 job_is_pruneable = job.metadata.status in ['DONE', 'CANCELLED', 'FAILED']
 
+                if job.metadata.status == 'CANCELLED':
+                    self.cancelling.append(
+                        asyncio.create_task(
+                            self._cancel_task(job)
+                        )
+                    )
+
                 if job_is_pruneable and job_elapsed > self._job_max_age:
                     del self._jobs[job_id]
+
+            
+            cancelling_tasks = list(self.cancelling)
+            for cancel_task in cancelling_tasks:
+                if cancel_task.done():
+                    self.cancelling.remove(cancel_task)
             
             await asyncio.sleep(self._job_prune_interval)
 
+    async def _cancel_task(self, job: Job):
+        
+        job.client.close()
+        job.client_closed = True
+
+        await job.clear()
+        await job.close(cancelled=True)
+
     def submit(
         self,
         connection: JobsConnection,
         image: Image, 
         build_options: Optional[BuildOptions]=None
     ) -> JobMetadata:
 
@@ -127,31 +150,58 @@
             return JobNotFoundException(
                 job_id=job_id,
                 message=f'Job - {job_id} - not found.'
             )
 
         return job.metadata
     
-    def cancel(self, job_id: uuid.UUID) -> Union[JobMetadata, JobNotFoundException]:
-        job = self._active.get(job_id)
-        if job is None or job.done():
+    def cancel(self, job_id: uuid.UUID) -> Union[Job, JobNotFoundException]:
+
+        active_task = self._active.get(job_id)
+        if active_task and active_task.done() is False:
+            active_task.cancel()
+
+        cancellable_states = [
+            'CREATED',
+            'AUTHORIZING', 
+            'BUILDING',
+            'GENERATING',
+            'PUSHING'
+        ]
+
+
+        cancelled_job = self._jobs.get(job_id)
+
+        if cancelled_job is None:
             return JobNotFoundException(
                 job_id=job_id,
                 message=f'Job - {job_id} - not found or is not active.'
             )
-        
-        job.cancel()
 
-        cancelled_job = self._jobs.get(job_id)
+        job_is_cancellable = cancelled_job.metadata.status in cancellable_states
 
-        self._jobs[job_id].close(
-            cancelled=True
+        if job_is_cancellable is False:
+            return JobNotFoundException(
+                job_id=job_id,
+                message=f'Job - {job_id} - not found or is not active.'
+            )
+        
+        cancelled_job.metadata = JobMetadata(
+            id=cancelled_job.job_id,
+            name=cancelled_job.job_name,
+            image=cancelled_job.image.name,
+            tag=cancelled_job.image.tag,
+            status=JobStatus.CANCELLED.value,
+            context=f'Job {cancelled_job.job_id} cancelled.',
+            size=cancelled_job.metadata.size
         )
+        
+        self._jobs[job_id] = cancelled_job
 
-        return cancelled_job.metadata
+        return cancelled_job
     
     async def close(self):
 
         self._run_cleanup = False
         await self._cleanup_task
 
         for job in self._active.values():
```

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/service.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,13 +168,13 @@
 
     cancelled_job = job_service_context.queue.cancel(
         uuid.UUID(job_id)
     )
 
     if isinstance(cancelled_job, JobNotFoundException):
         raise HTTPException(404, detail=cancelled_job.message)
-
-    return cancelled_job
+    
+    return cancelled_job.metadata
```

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/jobs/time_parser.py` & `dcrx-api-0.2.2/dcrx_api/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/monitoring/base/monitor.py` & `dcrx-api-0.2.2/dcrx_api/services/monitoring/base/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/monitoring/context.py` & `dcrx-api-0.2.2/dcrx_api/services/monitoring/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/docker_memory_monitor.py` & `dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/docker_memory_monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/monitoring/memory/monitor.py` & `dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/users/connection.py` & `dcrx-api-0.2.2/dcrx_api/services/users/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,22 +68,22 @@
                     name: self.table.selected.types_map.get(
                         name
                     )(value) for name, value in filters.items()
                 }
             )
         )
     
-    async def delete(
+    async def remove(
         self,
         filters: Dict[str, Any]
     ):
-        return await self.delete(
+        return await self.delete([
             self.table.delete({
                 name: self.table.selected.types_map.get(
                     name
                 )(value) for name, value in filters.items()
             })
-        )
+        ])
     
     async def drop(self):
         return await self.drop_table(self.table)
```

### Comparing `dcrx-api-0.2.0/dcrx_api/services/users/context.py` & `dcrx-api-0.2.2/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/users/service.py` & `dcrx-api-0.2.2/dcrx_api/services/users/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         }
     }
 )
 async def delete_user(user_id: str) -> UserTransactionSuccessResponse:
 
     users_service_context = context.get(ContextType.USERS_SERVICE)
 
-    await users_service_context.connection.delete(
+    await users_service_context.connection.remove(
         filters={
             'id': user_id
         }
     )
 
     return UserTransactionSuccessResponse(
         message='Deleted user.'
```

### Comparing `dcrx-api-0.2.0/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.2.2/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.2.2/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.2.2/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.2.2/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.0/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.2.2/dcrx_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.2.0
+Version: 0.2.2
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,22 +18,22 @@
 
 # dcrx-api
 [![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
 [![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
 
-Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
+DCRX-API is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! DCRX-API extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
-Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
+DCRX-API also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
-Dcrx-api is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
+DCRX-API is available both as a Docker image and as a PyPi package. For local use, we recommend using PyPi, Python 3.10+, and a virtual environment. To install, run:
 
 ```bash
 python -m venv ~/.dcrx && \
 source ~/.dcrx/bin/activate && \
 pip install dcrx-api
 ```
 
@@ -42,22 +42,28 @@
 ```
 docker pull adalundhe/dcrx-api:latest
 ```
 
 
 # Getting Started
 
-Dcrx-api requires a slew of environmental variables in order to run correctly. These include:
+DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
+DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
+
+DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
+
+DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
+
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
 
 DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
-DCRX_API_TOKEN_EXPIRATION_MINUTES=10 # Time in minutes for JWT authorization token to expire. Default is 30.
+DCRX_API_TOKEN_EXPIRATION='15m' # Time for JWT authorization token to expire. Default is 15 minutes.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
 DCRX_API_DATABASE_TYPE=sqlite # Type of database to use. Default is sqlite and options are mysql, asyncpg, and sqlite.
```

### Comparing `dcrx-api-0.2.0/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.2.2/dcrx_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 dcrx_api/database/__init__.py
 dcrx_api/database/connection.py
 dcrx_api/database/connection_config.py
 dcrx_api/database/table_types.py
 dcrx_api/env/__init__.py
 dcrx_api/env/env.py
 dcrx_api/env/load_env.py
+dcrx_api/env/time_parser.py
 dcrx_api/middleware/__init__.py
 dcrx_api/middleware/auth_middleware.py
 dcrx_api/services/__init__.py
 dcrx_api/services/auth/__init__.py
 dcrx_api/services/auth/context.py
 dcrx_api/services/auth/manager.py
 dcrx_api/services/auth/models/__init__.py
@@ -38,15 +39,14 @@
 dcrx_api/services/jobs/__init__.py
 dcrx_api/services/jobs/connection.py
 dcrx_api/services/jobs/context.py
 dcrx_api/services/jobs/job.py
 dcrx_api/services/jobs/queue.py
 dcrx_api/services/jobs/service.py
 dcrx_api/services/jobs/status.py
-dcrx_api/services/jobs/time_parser.py
 dcrx_api/services/jobs/models/__init__.py
 dcrx_api/services/jobs/models/build_options.py
 dcrx_api/services/jobs/models/image_stats.py
 dcrx_api/services/jobs/models/job_metadata.py
 dcrx_api/services/jobs/models/job_not_found_exception.py
 dcrx_api/services/jobs/models/new_image.py
 dcrx_api/services/jobs/models/registry.py
```

### Comparing `dcrx-api-0.2.0/setup.py` & `dcrx-api-0.2.2/setup.py`

 * *Files identical despite different names*

