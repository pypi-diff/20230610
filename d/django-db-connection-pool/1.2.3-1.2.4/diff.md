# Comparing `tmp/django-db-connection-pool-1.2.3.tar.gz` & `tmp/django-db-connection-pool-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-db-connection-pool-1.2.3.tar", last modified: Thu May 25 08:06:07 2023, max compression
+gzip compressed data, was "django-db-connection-pool-1.2.4.tar", last modified: Sat Jun 10 01:58:53 2023, max compression
```

## Comparing `django-db-connection-pool-1.2.3.tar` & `django-db-connection-pool-1.2.4.tar`

### file list

```diff
@@ -1,68 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.156866 django-db-connection-pool-1.2.3/
--rw-rw-rw-   0        0        0     1067 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/LICENSE
--rw-rw-rw-   0        0        0       80 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6082 2023-05-25 08:06:07.156866 django-db-connection-pool-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4913 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/README.md
--rw-rw-rw-   0        0        0     6665 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/README_cn.md
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.131354 django-db-connection-pool-1.2.3/dj_db_conn_pool/
--rw-rw-rw-   0        0        0      391 2023-04-21 08:48:04.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.132354 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.132354 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/
--rw-rw-rw-   0        0        0     2096 2023-04-21 06:54:28.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.133354 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/
--rw-rw-rw-   0        0        0        0 2022-03-28 02:57:23.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
--rw-rw-rw-   0        0        0      281 2022-11-10 08:02:57.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mixins.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.135353 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/
--rw-rw-rw-   0        0        0        0 2022-11-10 07:45:39.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/__init__.py
--rw-rw-rw-   0        0        0      574 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.135353 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/
--rw-rw-rw-   0        0        0        0 2022-11-10 07:45:39.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/__init__.py
--rw-rw-rw-   0        0        0      703 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.136858 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-04-21 07:24:27.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.137864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/mysql/
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/mysql/__init__.py
--rw-rw-rw-   0        0        0      516 2023-04-21 02:41:00.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/mysql/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.138864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/
--rw-rw-rw-   0        0        0        0 2022-11-10 07:54:21.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/__init__.py
--rw-rw-rw-   0        0        0      682 2023-04-21 02:00:57.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/mixins.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.139866 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/
--rw-rw-rw-   0        0        0        1 2022-11-10 07:54:21.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.140864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/oracle/
--rw-rw-rw-   0        0        0        0 2022-11-10 07:54:21.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/oracle/__init__.py
--rw-rw-rw-   0        0        0      365 2023-04-21 02:42:53.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/oracle/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.141864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/oracle/
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/oracle/__init__.py
--rw-rw-rw-   0        0        0      488 2023-04-21 06:08:53.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/oracle/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.143864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgis/
--rw-rw-rw-   0        0        0        0 2023-03-31 04:15:33.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgis/__init__.py
--rw-rw-rw-   0        0        0      342 2023-04-21 02:41:09.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgis/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.144866 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/__init__.py
--rw-rw-rw-   0        0        0      446 2023-05-25 07:53:09.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.146864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/django_tenants/
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
--rw-rw-rw-   0        0        0      312 2022-07-01 08:05:12.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/django_tenants/base.py
--rw-rw-rw-   0        0        0      302 2023-04-21 02:41:12.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/mixins.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.147864 django-db-connection-pool-1.2.3/dj_db_conn_pool/compat/
--rw-rw-rw-   0        0        0      302 2022-01-12 07:58:01.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/compat/__init__.py
--rw-rw-rw-   0        0        0      947 2023-04-21 06:02:01.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/compat/jdbc.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.149871 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/
--rw-rw-rw-   0        0        0     1070 2023-04-06 08:30:16.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/__init__.py
--rw-rw-rw-   0        0        0       70 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.151867 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/
--rw-rw-rw-   0        0        0       77 2023-04-06 03:18:16.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-21 07:25:01.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/core.py
--rw-rw-rw-   0        0        0      385 2023-04-06 07:58:20.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/creation.py
--rw-rw-rw-   0        0        0     1293 2023-04-21 08:02:44.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.155867 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      275 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      125 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 08:06:07.157864 django-db-connection-pool-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2255 2023-04-21 06:08:53.000000 django-db-connection-pool-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.956382 django-db-connection-pool-1.2.4/
+-rw-rw-rw-   0        0        0     1067 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     7377 2023-06-10 01:58:53.955380 django-db-connection-pool-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4913 2023-04-20 13:46:44.000000 django-db-connection-pool-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.884674 django-db-connection-pool-1.2.4/dj_db_conn_pool/
+-rw-rw-rw-   0        0        0      391 2023-06-10 01:54:31.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.886675 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.890677 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/
+-rw-rw-rw-   0        0        0     2175 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.893675 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mixins.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.896675 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/__init__.py
+-rw-rw-rw-   0        0        0      574 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.898671 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/__init__.py
+-rw-rw-rw-   0        0        0      703 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.901684 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/base.py
+-rw-rw-rw-   0        0        0      730 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.905039 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/mysql/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/mysql/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/mysql/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.908037 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/__init__.py
+-rw-rw-rw-   0        0        0      682 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/mixins.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.909057 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/
+-rw-rw-rw-   0        0        0        1 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/oracle/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/oracle/__init__.py
+-rw-rw-rw-   0        0        0      365 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/oracle/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/oracle/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/oracle/__init__.py
+-rw-rw-rw-   0        0        0      454 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/oracle/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgis/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgis/__init__.py
+-rw-rw-rw-   0        0        0      342 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgis/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/__init__.py
+-rw-rw-rw-   0        0        0      446 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/django_tenants/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
+-rw-rw-rw-   0        0        0      312 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/django_tenants/base.py
+-rw-rw-rw-   0        0        0      302 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/mixins.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.930864 django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/
+-rw-rw-rw-   0        0        0      295 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/jdbc.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.936922 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/
+-rw-rw-rw-   0        0        0     1070 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.936922 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/
+-rw-rw-rw-   0        0        0       74 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/__init__.py
+-rw-rw-rw-   0        0        0     5046 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/core.py
+-rw-rw-rw-   0        0        0      385 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/creation.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.953392 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/
+-rw-rw-rw-   0        0        0     7377 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1854 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      314 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1520 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 01:58:53.956382 django-db-connection-pool-1.2.4/setup.cfg
```

### Comparing `django-db-connection-pool-1.2.3/LICENSE` & `django-db-connection-pool-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/PKG-INFO` & `django-db-connection-pool-1.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 Metadata-Version: 2.1
 Name: django-db-connection-pool
-Version: 1.2.3
-Summary: Persistent database connection backends for Django
-Home-page: https://github.com/altairbow/django-db-connection-pool
-Download-URL: https://pypi.python.org/pypi/django-db-connection-pool/
-Author: Altair Bow
-Author-email: altair.bow@foxmail.com
-License: MIT
+Version: 1.2.4
+Summary: Database connection pool component library for Django
+Author-email: Altair Bow <altair.bow@foxmail.com>
+License: MIT License
+        
+        Copyright (c) 2019 Altair Bow
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/altairbow/django-db-connection-pool
+Project-URL: repository, https://github.com/altairbow/django-db-connection-pool
 Keywords: django,db,database,persistent,connection,pool,pooling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: jdbc
 Provides-Extra: mysql
 Provides-Extra: odbc
 Provides-Extra: oracle
 Provides-Extra: postgresql
```

### Comparing `django-db-connection-pool-1.2.3/README.md` & `django-db-connection-pool-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/__init__.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import threading
 import jpype
 import jpype.dbapi2
 from dj_db_conn_pool.core.mixins import PersistentDatabaseWrapperMixin
+from dj_db_conn_pool.backends.jdbc.utils import CursorWrapper
 
 import logging
 logger = logging.getLogger(__name__)
 
 jdbc_type_converters = {}
 
 lock_check_jvm_status = threading.Lock()
 
 
 class JDBCDatabaseWrapperMixin(PersistentDatabaseWrapperMixin):
-    _sql_param_style = 'qmark'
-
-    _sql_converter = staticmethod(lambda sql: sql.replace('%s', '?'))
-
     @property
     def jdbc_driver(self):
         raise NotImplementedError()
 
     @property
     def jdbc_url_prefix(self):
         raise NotImplementedError()
@@ -29,14 +26,18 @@
     @property
     def jdbc_url(self):
         return '{prefix}//{HOST}:{PORT}/{NAME}'.format(
             prefix=self.jdbc_url_prefix,
             **self.settings_dict
         )
 
+    def create_cursor(self, name=None):
+        cursor = self.connection.cursor()
+        return CursorWrapper(cursor)
+
     def get_connection_params(self):
         return self.settings_dict.get('OPTIONS', {})
 
     def _get_new_connection(self, conn_params):
         with lock_check_jvm_status:
             if not jpype.isJVMStarted():
                 jpype.startJVM(ignoreUnrecognized=True)
```

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/base.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/base.py`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/mysql/base.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/mysql/base.py`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/mixins.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/mixins.py`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/compat/jdbc.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/jdbc.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import jpype
-
-
-def patch_all():
-    patch_converters()
-
-
-def patch_converters():
-    """
-    patch jpype's jdbc converters
-    """
-    def to_python(value):
-        return value._py()
-
-    def to_number(value):
-        string = str(value.toString())
-
-        if value.scale() > 0:
-            return float(string)
-
-        return int(string)
-
-    @jpype.onJVMStart
-    def register_converters():
-        from dj_db_conn_pool.backends.jdbc import jdbc_type_converters
-
-        jdbc_type_converters[jpype.java.lang.String] = str
-        jdbc_type_converters[jpype.java.sql.Date] = to_python
-        jdbc_type_converters[jpype.java.sql.Time] = to_python
-        jdbc_type_converters[jpype.java.sql.Timestamp] = to_python
-        jdbc_type_converters[jpype.java.math.BigDecimal] = to_number
-        jdbc_type_converters[jpype.JArray(jpype.types.JByte)] = bytes
-        # jdbc_type_converters[type(None)] = lambda v: v
+import jpype
+
+
+def patch_all():
+    patch_converters()
+
+
+def patch_converters():
+    """
+    patch jpype's jdbc converters
+    """
+    def to_python(value):
+        return value._py()
+
+    def to_number(value):
+        string = str(value.toString())
+
+        if value.scale() > 0:
+            return float(string)
+
+        return int(string)
+
+    @jpype.onJVMStart
+    def register_converters():
+        from dj_db_conn_pool.backends.jdbc import jdbc_type_converters
+
+        jdbc_type_converters[jpype.java.lang.String] = str
+        jdbc_type_converters[jpype.java.sql.Date] = to_python
+        jdbc_type_converters[jpype.java.sql.Time] = to_python
+        jdbc_type_converters[jpype.java.sql.Timestamp] = to_python
+        jdbc_type_converters[jpype.java.math.BigDecimal] = to_number
+        jdbc_type_converters[jpype.JArray(jpype.types.JByte)] = bytes
+        # jdbc_type_converters[type(None)] = lambda v: v
```

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/core/__init__.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/core/__init__.py`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/core.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from sqlalchemy import pool
 from dj_db_conn_pool.compat import gettext_lazy as _
 from dj_db_conn_pool.core import pool_container
-from dj_db_conn_pool.core.utils import CursorWrapper
 from dj_db_conn_pool.core.mixins.creation import DatabaseCreationMixin
 
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -39,24 +38,14 @@
                 logger.exception('unable to set autocommit mode of %s(%s) to %s, caused by: %s',
                                  self.vendor, self.alias, autocommit, exc)
                 raise exc from None
 
     def _get_dialect(self):
         return self.SQLAlchemyDialect(dbapi=self.Database)
 
-    _sql_param_style = 'format'
-
-    _sql_converter = staticmethod(lambda sql: sql)
-
-    def create_cursor(self, name=None):
-        # get cursor from django
-        cursor = super().create_cursor(name)
-
-        return CursorWrapper(cursor, self._sql_param_style, self._sql_converter)
-
     def _get_new_connection(self, conn_params):
         return super(PersistentDatabaseWrapperMixin, self).get_new_connection(conn_params)
 
     def get_new_connection(self, conn_params):
         """
         override django.db.backends.<database>.base.DatabaseWrapper.get_new_connection to
         change the default behavior of getting new connection to database, we maintain
```

### Comparing `django-db-connection-pool-1.2.3/dj_db_conn_pool/core/utils.py` & `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,29 @@
 import logging
 import sqlparams
 
 logger = logging.getLogger(__name__)
 
 
 class CursorWrapper:
-    def __init__(self, cursor, style, sql_converter):
-        self._cursor = cursor
+    def __init__(self, cursor):
+        self.cursor = cursor
 
-        self._sql_params_converter = sqlparams.SQLParams('named', style, True, True)
+        self._sql_params_converter = sqlparams.SQLParams('pyformat', 'qmark', True, True)
 
-        self._sql_converter = sql_converter
-
-        self._statement = None
+        self.statement = None
 
     def execute(self, query, parameters=None):
         if isinstance(parameters, dict):
-            _query, _parameters = self._sql_params_converter.format(query, parameters)
+            query, parameters = self._sql_params_converter.format(query, parameters)
         else:
-            _query, _parameters = self._sql_converter(query), parameters
-
-        if query != _query:
-            logger.debug(
-                'SQL (%s), parameters(%s) has been converted to SQL(%s), parameters(%s)',
-                query, parameters, _query, _parameters
-            )
-
-        query, parameters = _query, _parameters
+            query = query.replace('%s', '?')
 
-        try:
-            cursor = self._cursor.cursor
-        except AttributeError:
-            cursor = self._cursor
+        self.statement = query
 
-        self._statement = query
-
-        return cursor.execute(query, parameters or [])
+        return self.cursor.execute(query, parameters)
 
     def __getattr__(self, attr):
-        try:
-            return getattr(self._cursor, attr)
-        except AttributeError:
-            if attr == 'statement':
-                return self._statement
-            raise
+        return getattr(self.cursor, attr)
+
+    def __iter__(self):
+        return iter(self.cursor)
```

### Comparing `django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/PKG-INFO` & `django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 Metadata-Version: 2.1
 Name: django-db-connection-pool
-Version: 1.2.3
-Summary: Persistent database connection backends for Django
-Home-page: https://github.com/altairbow/django-db-connection-pool
-Download-URL: https://pypi.python.org/pypi/django-db-connection-pool/
-Author: Altair Bow
-Author-email: altair.bow@foxmail.com
-License: MIT
+Version: 1.2.4
+Summary: Database connection pool component library for Django
+Author-email: Altair Bow <altair.bow@foxmail.com>
+License: MIT License
+        
+        Copyright (c) 2019 Altair Bow
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/altairbow/django-db-connection-pool
+Project-URL: repository, https://github.com/altairbow/django-db-connection-pool
 Keywords: django,db,database,persistent,connection,pool,pooling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: jdbc
 Provides-Extra: mysql
 Provides-Extra: odbc
 Provides-Extra: oracle
 Provides-Extra: postgresql
```

### Comparing `django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/SOURCES.txt` & `django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
-MANIFEST.in
 README.md
-README_cn.md
-requirements.txt
-setup.py
+pyproject.toml
 dj_db_conn_pool/__init__.py
 dj_db_conn_pool/backends/__init__.py
 dj_db_conn_pool/backends/jdbc/__init__.py
+dj_db_conn_pool/backends/jdbc/utils.py
 dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
 dj_db_conn_pool/backends/jdbc/oceanbase/mixins.py
 dj_db_conn_pool/backends/jdbc/oceanbase/mysql/__init__.py
 dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py
 dj_db_conn_pool/backends/jdbc/oceanbase/oracle/__init__.py
 dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py
 dj_db_conn_pool/backends/jdbc/oracle/__init__.py
@@ -31,15 +29,14 @@
 dj_db_conn_pool/backends/postgresql/mixins.py
 dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
 dj_db_conn_pool/backends/postgresql/django_tenants/base.py
 dj_db_conn_pool/compat/__init__.py
 dj_db_conn_pool/compat/jdbc.py
 dj_db_conn_pool/core/__init__.py
 dj_db_conn_pool/core/exceptions.py
-dj_db_conn_pool/core/utils.py
 dj_db_conn_pool/core/mixins/__init__.py
 dj_db_conn_pool/core/mixins/core.py
 dj_db_conn_pool/core/mixins/creation.py
 django_db_connection_pool.egg-info/PKG-INFO
 django_db_connection_pool.egg-info/SOURCES.txt
 django_db_connection_pool.egg-info/dependency_links.txt
 django_db_connection_pool.egg-info/requires.txt
```

