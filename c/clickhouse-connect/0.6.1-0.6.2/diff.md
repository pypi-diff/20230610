# Comparing `tmp/clickhouse-connect-0.6.1.tar.gz` & `tmp/clickhouse-connect-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.6.1.tar", last modified: Tue Jun  6 14:00:08 2023, max compression
+gzip compressed data, was "clickhouse-connect-0.6.2.tar", last modified: Sat Jun 10 05:55:26 2023, max compression
```

## Comparing `clickhouse-connect-0.6.1.tar` & `clickhouse-connect-0.6.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/clickhouse_connect/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/clickhouse_connect/driverc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/json_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/clickhouse_connect/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.177868 clickhouse-connect-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-10 05:55:26.177868 clickhouse-connect-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.169869 clickhouse-connect-0.6.2/clickhouse_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.169869 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.169869 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.169869 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.169869 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.173869 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.173869 clickhouse-connect-0.6.2/clickhouse_connect/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.177868 clickhouse-connect-0.6.2/clickhouse_connect/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.177868 clickhouse-connect-0.6.2/clickhouse_connect/driverc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/json_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.177868 clickhouse-connect-0.6.2/clickhouse_connect/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:55:26.169869 clickhouse-connect-0.6.2/clickhouse_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-10 05:55:26.000000 clickhouse-connect-0.6.2/clickhouse_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-10 05:55:26.000000 clickhouse-connect-0.6.2/clickhouse_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 05:55:26.000000 clickhouse-connect-0.6.2/clickhouse_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-10 05:55:26.000000 clickhouse-connect-0.6.2/clickhouse_connect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 05:55:26.000000 clickhouse-connect-0.6.2/clickhouse_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 05:55:26.000000 clickhouse-connect-0.6.2/clickhouse_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 05:55:26.177868 clickhouse-connect-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-10 05:55:25.000000 clickhouse-connect-0.6.2/setup.py
```

### Comparing `clickhouse-connect-0.6.1/LICENSE` & `clickhouse-connect-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/PKG-INFO` & `clickhouse-connect-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.1
+Version: 0.6.2
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.1/README.md` & `clickhouse-connect-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse-connect-0.6.2/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/common.py` & `clickhouse-connect-0.6.2/clickhouse_connect/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/base.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/container.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/format.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/network.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/numeric.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/registry.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/special.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/string.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/string.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Sequence, MutableSequence, Union, Collection
 
+from clickhouse_connect.driver.ctypes import data_conv
+
 from clickhouse_connect.datatypes.base import ClickHouseType, TypeDef
 from clickhouse_connect.driver.insert import InsertContext
 from clickhouse_connect.driver.query import QueryContext
 from clickhouse_connect.driver.types import ByteSource
 from clickhouse_connect.driver.options import np, pd
 
 
@@ -37,71 +39,18 @@
             return pd.array(column, dtype=pd.StringDtype())
         if ctx.use_numpy and ctx.max_str_len:
             return np.array(column, dtype=f'<U{ctx.max_str_len}')
         return column
 
     # pylint: disable=duplicate-code,too-many-nested-blocks,too-many-branches
     def _write_column_binary(self, column: Union[Sequence, MutableSequence], dest: bytearray, ctx: InsertContext):
-        encoding = ctx.encoding or self.encoding
-        app = dest.append
-        first = self._first_value(column)
-        if isinstance(first, str):
-            if self.nullable:
-                for x in column:
-                    if x is None:
-                        app(0)
-                    else:
-                        y = x.encode(encoding)
-                        sz = len(y)
-                        while True:
-                            b = sz & 0x7f
-                            sz >>= 7
-                            if sz == 0:
-                                app(b)
-                                break
-                            app(0x80 | b)
-                        dest += y
-            else:
-                for x in column:
-                    y = x.encode(encoding)
-                    sz = len(y)
-                    while True:
-                        b = sz & 0x7f
-                        sz >>= 7
-                        if sz == 0:
-                            app(b)
-                            break
-                        app(0x80 | b)
-                    dest += y
-        else:
-            if self.nullable:
-                for x in column:
-                    if x is None:
-                        app(0)
-                    else:
-                        sz = len(x)
-                        while True:
-                            b = sz & 0x7f
-                            sz >>= 7
-                            if sz == 0:
-                                app(b)
-                                break
-                            app(0x80 | b)
-                        dest += x
-            else:
-                for x in column:
-                    sz = len(x)
-                    while True:
-                        b = sz & 0x7f
-                        sz >>= 7
-                        if sz == 0:
-                            app(b)
-                            break
-                        app(0x80 | b)
-                    dest += x
+        encoding = None
+        if isinstance(self._first_value(column), str):
+            encoding = ctx.encoding or self.encoding
+        data_conv.write_str_col(column, encoding, dest)
 
     def _active_null(self, ctx):
         if ctx.use_none:
             return None
         if self.read_format(ctx) == 'bytes':
             return bytes()
         return ''
```

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/temporal.py` & `clickhouse-connect-0.6.2/clickhouse_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/dbapi/__init__.py` & `clickhouse-connect-0.6.2/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/dbapi/connection.py` & `clickhouse-connect-0.6.2/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/dbapi/cursor.py` & `clickhouse-connect-0.6.2/clickhouse_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/__init__.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/buffer.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/client.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/client.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/common.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import array
+import struct
 import sys
 
 from typing import Sequence, MutableSequence, Dict, Optional, Union, Generator
 
 from clickhouse_connect.driver.exceptions import ProgrammingError, StreamClosedError
 from clickhouse_connect.driver.types import Closable
 
@@ -46,21 +47,19 @@
     """
     if len(column) and not isinstance(column[0], (int, float)):
         if code in ('f', 'F', 'd', 'D'):
             column = [float(x) for x in column]
         else:
             column = [int(x) for x in column]
     try:
-        buff = array.array(code, column)
-    except (TypeError, OverflowError) as ex:
+        buff = struct.Struct(f'<{len(column)}{code}')
+        dest += buff.pack(*column)
+    except (TypeError, OverflowError, struct.error) as ex:
         raise ProgrammingError('Unable to create Python array.  This is usually caused by trying to insert None ' +
                                'values into a ClickHouse column that is not Nullable') from ex
-    if must_swap:
-        buff.byteswap()
-    dest += buff.tobytes()
 
 
 def write_uint64(value: int, dest: MutableSequence):
     """
     Write a single UInt64 value to a binary write buffer
     :param value: UInt64 value to write
     :param dest: Destination byte buffer
```

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/compression.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/context.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/ctypes.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/dataconv.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/dataconv.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,7 +104,26 @@
     arr = np.empty((len(column),), dtype=np.object)
     arr[:] = column
     return arr
 
 
 def pivot(data: Sequence[Sequence], start_row: int, end_row: int) -> Sequence[Sequence]:
     return tuple(zip(*data[start_row: end_row]))
+
+
+def write_str_col(column: Sequence, encoding: Optional[str], dest: bytearray):
+    app = dest.append
+    for x in column:
+        if not x:
+            app(0)
+        else:
+            if encoding:
+                x = x.encode(encoding)
+            sz = len(x)
+            while True:
+                b = sz & 0x7f
+                sz >>= 7
+                if sz == 0:
+                    app(b)
+                    break
+                app(0x80 | b)
+            dest += x
```

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/ddl.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/exceptions.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/external.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/external.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/httpclient.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/httpclient.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/httputil.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/httputil.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 logger = logging.getLogger(__name__)
 
 # We disable this warning.  Verify must explicitly set to false, so we assume the user knows what they're doing
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 # Increase this number just to be safe when ClickHouse is returning progress headers
-http._MAXHEADERS = 10000  # pylint: disable=protected-access
+http.client._MAXHEADERS = 10000  # pylint: disable=protected-access
 
 DEFAULT_KEEP_INTERVAL = 30
 DEFAULT_KEEP_COUNT = 3
 DEFAULT_KEEP_IDLE = 30
 
 SOCKET_TCP = socket.IPPROTO_TCP
```

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/insert.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/models.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/npquery.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/options.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/parser.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/query.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/query.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/tools.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/transform.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/transform.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/driver/types.py` & `clickhouse-connect-0.6.2/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/entry_points.py` & `clickhouse-connect-0.6.2/clickhouse_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/json_impl.py` & `clickhouse-connect-0.6.2/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/tools/datagen.py` & `clickhouse-connect-0.6.2/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect/tools/testing.py` & `clickhouse-connect-0.6.2/clickhouse_connect/tools/testing.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect.egg-info/PKG-INFO` & `clickhouse-connect-0.6.2/clickhouse_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.1
+Version: 0.6.2
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.1/clickhouse_connect.egg-info/SOURCES.txt` & `clickhouse-connect-0.6.2/clickhouse_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.1/setup.py` & `clickhouse-connect-0.6.2/setup.py`

 * *Files identical despite different names*

