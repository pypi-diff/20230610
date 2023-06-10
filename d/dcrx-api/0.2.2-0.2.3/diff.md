# Comparing `tmp/dcrx-api-0.2.2.tar.gz` & `tmp/dcrx-api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.2.2.tar", last modified: Sat Jun 10 18:07:58 2023, max compression
+gzip compressed data, was "dcrx-api-0.2.3.tar", last modified: Sat Jun 10 18:15:55 2023, max compression
```

## Comparing `dcrx-api-0.2.2.tar` & `dcrx-api-0.2.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/env/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/image_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/remote_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/models/server_memory_limit_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/base/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/cpu/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.400473 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:07:58.396473 dcrx-api-0.2.2/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 18:07:58.000000 dcrx-api-0.2.2/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 18:07:58.404473 dcrx-api-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-10 18:07:50.000000 dcrx-api-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.069707 dcrx-api-0.2.3/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/env/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/models/server_memory_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.073707 dcrx-api-0.2.3/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:15:55.069707 dcrx-api-0.2.3/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-10 18:15:55.000000 dcrx-api-0.2.3/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-10 18:15:55.000000 dcrx-api-0.2.3/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:15:55.000000 dcrx-api-0.2.3/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 18:15:55.000000 dcrx-api-0.2.3/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 18:15:55.000000 dcrx-api-0.2.3/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 18:15:55.000000 dcrx-api-0.2.3/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 18:15:55.077707 dcrx-api-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-10 18:15:46.000000 dcrx-api-0.2.3/setup.py
```

### Comparing `dcrx-api-0.2.2/LICENSE` & `dcrx-api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/PKG-INFO` & `dcrx-api-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -73,19 +73,19 @@
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
 
 DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
-DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
+DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Default Docker image registry to push images to.
 
-DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_USERNAME=test # Default Username to authenticate Docker pushes to the provided registry.
 
-DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_PASSWORD=test-repo-password # Default Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -185,7 +185,35 @@
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+
+3. Can I push to a registry besides the default? - Yes. New image job requests can be submitted with optional Registry configuration. For example:
+
+```
+{
+  "name": "hello-world",
+  "tag": "latest",
+  "registry": {
+    "registry_url": "https://docker.io/v1/mytest/registry",
+    "registry_user": "DockerUser100",
+    "registry_password": "MyDockerHubToken999*"
+  },
+  "layers": [
+    {
+      "layer_type": "stage",
+      "base": "python",
+      "tag": "3.11-slim"
+    },
+    {
+        "layer_type": "entrypoint",
+        "command": [
+            "echo",
+            "Hello world!"
+        ]
+    }
+  ]
+}
+```
```

### Comparing `dcrx-api-0.2.2/README.md` & `dcrx-api-0.2.3/dcrx_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: dcrx-api
+Version: 0.2.3
+Summary: A RESTful implementation of the DCRX Docker library.
+Home-page: https://github.com/scorbettUM/dcrx-api
+Author: Sean Corbett
+Author-email: sean.corbett@umontana.edu
+Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dcrx-api
 [![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
 [![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
 
 DCRX-API is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! DCRX-API extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
@@ -55,19 +73,19 @@
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
 
 DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
-DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
+DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Default Docker image registry to push images to.
 
-DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_USERNAME=test # Default Username to authenticate Docker pushes to the provided registry.
 
-DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_PASSWORD=test-repo-password # Default Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -166,8 +184,36 @@
 The chart creates three replica dcrx-api pods, a LoadBalancer service, and Nginx ingress to get you up and running in your Kubernetes cluster!
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
-2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+
+3. Can I push to a registry besides the default? - Yes. New image job requests can be submitted with optional Registry configuration. For example:
+
+```
+{
+  "name": "hello-world",
+  "tag": "latest",
+  "registry": {
+    "registry_url": "https://docker.io/v1/mytest/registry",
+    "registry_user": "DockerUser100",
+    "registry_password": "MyDockerHubToken999*"
+  },
+  "layers": [
+    {
+      "layer_type": "stage",
+      "base": "python",
+      "tag": "3.11-slim"
+    },
+    {
+        "layer_type": "entrypoint",
+        "command": [
+            "echo",
+            "Hello world!"
+        ]
+    }
+  ]
+}
+```
```

### Comparing `dcrx-api-0.2.2/dcrx_api/cli/base.py` & `dcrx-api-0.2.3/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/cli/database.py` & `dcrx-api-0.2.3/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/cli/server.py` & `dcrx-api-0.2.3/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/context/manager.py` & `dcrx-api-0.2.3/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/database/connection.py` & `dcrx-api-0.2.3/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/env/env.py` & `dcrx-api-0.2.3/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/env/load_env.py` & `dcrx-api-0.2.3/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/env/time_parser.py` & `dcrx-api-0.2.3/dcrx_api/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/lifespan.py` & `dcrx-api-0.2.3/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.2.3/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/auth/manager.py` & `dcrx-api-0.2.3/dcrx_api/services/auth/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/context.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/job.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/job.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,26 +116,30 @@
         await job.clear()
         await job.close(cancelled=True)
 
     def submit(
         self,
         connection: JobsConnection,
         image: Image, 
+        registry: Optional[Registry]=None,
         build_options: Optional[BuildOptions]=None
     ) -> JobMetadata:
-
-        job = Job(
-            connection,
-            image,
-            Registry(
+        
+        if registry is None:
+            registry = Registry(
                 registry_uri=self.registry_uri,
                 registry_user=self.registry_username,
                 registry_password=self.registry_password
                 
-            ),
+            )
+
+        job = Job(
+            connection,
+            image,
+            registry,
             build_options=build_options,
             pool_size=self.pool_size
         )
 
         self._jobs[job.job_id] = job
 
         self._active[job.job_id] = asyncio.create_task(
```

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/service.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     "/jobs/images/create",
     responses={
         400: {
             'model': ServerMemoryLimitException
         }
     }
 )
-async def start_job(new_image: NewImage) -> JobMetadata:
+async def create_job(new_image: NewImage) -> JobMetadata:
 
     job_service_context = context.get(ContextType.JOB_SERVICE)
     monitoring_service_context = context.get(ContextType.MONITORING_SERVICE)
     
 
     if monitoring_service_context.exceeded_memory_limit:
         raise HTTPException(400, detail={
@@ -104,14 +104,15 @@
                 )
 
             dcrx_image.layers.append(layer)
 
         return job_service_context.queue.submit(
             job_service_context.connection,
             dcrx_image,
+            registry=new_image.registry,
             build_options=new_image.build_options
         )
 
 
 @jobs_router.get(
     "/jobs/images/{job_id}/get",
     responses={
```

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.2.3/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/monitoring/base/monitor.py` & `dcrx-api-0.2.3/dcrx_api/services/monitoring/base/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/monitoring/context.py` & `dcrx-api-0.2.3/dcrx_api/services/monitoring/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/docker_memory_monitor.py` & `dcrx-api-0.2.3/dcrx_api/services/monitoring/memory/docker_memory_monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/monitoring/memory/monitor.py` & `dcrx-api-0.2.3/dcrx_api/services/monitoring/memory/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/users/connection.py` & `dcrx-api-0.2.3/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/users/context.py` & `dcrx-api-0.2.3/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/users/service.py` & `dcrx-api-0.2.3/dcrx_api/services/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.2.3/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.2.3/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.2.3/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.2.3/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.2.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: dcrx-api
-Version: 0.2.2
-Summary: A RESTful implementation of the DCRX Docker library.
-Home-page: https://github.com/scorbettUM/dcrx-api
-Author: Sean Corbett
-Author-email: sean.corbett@umontana.edu
-Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dcrx-api
 [![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
 [![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
 
 DCRX-API is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! DCRX-API extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
@@ -73,19 +55,19 @@
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
 
 DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
-DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
+DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Default Docker image registry to push images to.
 
-DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_USERNAME=test # Default Username to authenticate Docker pushes to the provided registry.
 
-DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_PASSWORD=test-repo-password # Default Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -185,7 +167,35 @@
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+
+3. Can I push to a registry besides the default? - Yes. New image job requests can be submitted with optional Registry configuration. For example:
+
+```
+{
+  "name": "hello-world",
+  "tag": "latest",
+  "registry": {
+    "registry_url": "https://docker.io/v1/mytest/registry",
+    "registry_user": "DockerUser100",
+    "registry_password": "MyDockerHubToken999*"
+  },
+  "layers": [
+    {
+      "layer_type": "stage",
+      "base": "python",
+      "tag": "3.11-slim"
+    },
+    {
+        "layer_type": "entrypoint",
+        "command": [
+            "echo",
+            "Hello world!"
+        ]
+    }
+  ]
+}
+```
```

### Comparing `dcrx-api-0.2.2/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.2.3/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.2/setup.py` & `dcrx-api-0.2.3/setup.py`

 * *Files identical despite different names*

