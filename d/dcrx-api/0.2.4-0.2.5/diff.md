# Comparing `tmp/dcrx-api-0.2.4.tar.gz` & `tmp/dcrx-api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.2.4.tar", last modified: Sat Jun 10 19:31:19 2023, max compression
+gzip compressed data, was "dcrx-api-0.2.5.tar", last modified: Sat Jun 10 19:39:46 2023, max compression
```

## Comparing `dcrx-api-0.2.4.tar` & `dcrx-api-0.2.5.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.203931 dcrx-api-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-10 19:31:19.203931 dcrx-api-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.187930 dcrx-api-0.2.4/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.191930 dcrx-api-0.2.4/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.191930 dcrx-api-0.2.4/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.191930 dcrx-api-0.2.4/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.191930 dcrx-api-0.2.4/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/env/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.191930 dcrx-api-0.2.4/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.195931 dcrx-api-0.2.4/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.195931 dcrx-api-0.2.4/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.195931 dcrx-api-0.2.4/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.195931 dcrx-api-0.2.4/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.199931 dcrx-api-0.2.4/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/image_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/remote_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/models/server_memory_limit_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.199931 dcrx-api-0.2.4/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.199931 dcrx-api-0.2.4/dcrx_api/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.199931 dcrx-api-0.2.4/dcrx_api/services/monitoring/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/base/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.199931 dcrx-api-0.2.4/dcrx_api/services/monitoring/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/cpu/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.199931 dcrx-api-0.2.4/dcrx_api/services/monitoring/memory/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/monitoring/memory/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.203931 dcrx-api-0.2.4/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.203931 dcrx-api-0.2.4/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.203931 dcrx-api-0.2.4/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:31:19.191930 dcrx-api-0.2.4/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-10 19:31:19.000000 dcrx-api-0.2.4/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-10 19:31:19.000000 dcrx-api-0.2.4/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:31:19.000000 dcrx-api-0.2.4/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 19:31:19.000000 dcrx-api-0.2.4/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 19:31:19.000000 dcrx-api-0.2.4/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 19:31:19.000000 dcrx-api-0.2.4/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:31:19.203931 dcrx-api-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-10 19:31:16.000000 dcrx-api-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.841794 dcrx-api-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-10 19:39:46.841794 dcrx-api-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.833794 dcrx-api-0.2.5/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.833794 dcrx-api-0.2.5/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/env/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/models/server_memory_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.837794 dcrx-api-0.2.5/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.841794 dcrx-api-0.2.5/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.841794 dcrx-api-0.2.5/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.841794 dcrx-api-0.2.5/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.841794 dcrx-api-0.2.5/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:46.833794 dcrx-api-0.2.5/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-10 19:39:46.000000 dcrx-api-0.2.5/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-10 19:39:46.000000 dcrx-api-0.2.5/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:39:46.000000 dcrx-api-0.2.5/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-10 19:39:46.000000 dcrx-api-0.2.5/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 19:39:46.000000 dcrx-api-0.2.5/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 19:39:46.000000 dcrx-api-0.2.5/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:39:46.841794 dcrx-api-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-10 19:39:43.000000 dcrx-api-0.2.5/setup.py
```

### Comparing `dcrx-api-0.2.4/LICENSE` & `dcrx-api-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/PKG-INFO` & `dcrx-api-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.2.4/README.md` & `dcrx-api-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/cli/base.py` & `dcrx-api-0.2.5/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/cli/database.py` & `dcrx-api-0.2.5/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/cli/server.py` & `dcrx-api-0.2.5/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/context/manager.py` & `dcrx-api-0.2.5/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/database/connection.py` & `dcrx-api-0.2.5/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/env/env.py` & `dcrx-api-0.2.5/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/env/load_env.py` & `dcrx-api-0.2.5/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/env/time_parser.py` & `dcrx-api-0.2.5/dcrx_api/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/lifespan.py` & `dcrx-api-0.2.5/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.2.5/dcrx_api/middleware/auth_middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,17 +38,13 @@
                 status_code=401,
                 content=json.dumps({
                     'detail': authorization.error
                 })
             )
 
             if token:
-                response.delete_cookie(
-                    'X-Auth-Token',
-                    httponly=True,
-                    secure=True
-                )
+                response.delete_cookie('X-Auth-Token')
 
             return response
 
         response = await call_next(request)
         return response
```

### Comparing `dcrx-api-0.2.4/dcrx_api/services/auth/manager.py` & `dcrx-api-0.2.5/dcrx_api/services/auth/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/context.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/job.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/job.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/queue.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/service.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.2.5/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/monitoring/base/monitor.py` & `dcrx-api-0.2.5/dcrx_api/services/monitoring/base/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/monitoring/context.py` & `dcrx-api-0.2.5/dcrx_api/services/monitoring/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/monitoring/memory/docker_memory_monitor.py` & `dcrx-api-0.2.5/dcrx_api/services/monitoring/memory/docker_memory_monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/monitoring/memory/monitor.py` & `dcrx-api-0.2.5/dcrx_api/services/monitoring/memory/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/users/connection.py` & `dcrx-api-0.2.5/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/users/context.py` & `dcrx-api-0.2.5/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/users/service.py` & `dcrx-api-0.2.5/dcrx_api/services/users/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,15 @@
     response = JSONResponse(
         content=success_response.dict()
     )
 
     response.set_cookie(
         key='X-Auth-Token',
         value=f'Bearer {authorization.token}',
-        expires=authorization.token_expires,
-        httponly=True,
-        secure=True
+        expires=authorization.token_expires
     )
 
 
     return response
 
 
 @users_router.get(
```

### Comparing `dcrx-api-0.2.4/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.2.5/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.2.5/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.2.5/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.2.5/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.2.5/dcrx_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.2.4/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.2.5/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.4/setup.py` & `dcrx-api-0.2.5/setup.py`

 * *Files identical despite different names*

