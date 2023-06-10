# Comparing `tmp/sqlite3-to-mysql-1.4.9.tar.gz` & `tmp/sqlite3_to_mysql-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite3-to-mysql-1.4.9.tar", last modified: Sun Dec 19 22:12:53 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sqlite3-to-mysql-1.4.9.tar` & `sqlite3_to_mysql-2.0.0.tar`

### file list

```diff
@@ -1,42 +1,26 @@
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.733608 sqlite3-to-mysql-1.4.9/
--rw-r--r--   0 klemen     (501) staff       (20)     5513 2021-09-19 12:10:28.000000 sqlite3-to-mysql-1.4.9/CODE-OF-CONDUCT.md
--rw-r--r--   0 klemen     (501) staff       (20)     1069 2021-02-13 11:00:12.000000 sqlite3-to-mysql-1.4.9/LICENSE
--rw-r--r--   0 klemen     (501) staff       (20)      166 2020-07-19 22:13:21.000000 sqlite3-to-mysql-1.4.9/MANIFEST.in
--rw-r--r--   0 klemen     (501) staff       (20)     5850 2021-12-19 22:12:53.734417 sqlite3-to-mysql-1.4.9/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)     4449 2021-09-19 12:11:52.000000 sqlite3-to-mysql-1.4.9/README.md
--rw-r--r--   0 klemen     (501) staff       (20)      288 2019-08-31 11:17:29.000000 sqlite3-to-mysql-1.4.9/pytest.ini
--rw-r--r--   0 klemen     (501) staff       (20)      729 2021-10-10 13:00:57.000000 sqlite3-to-mysql-1.4.9/requirements_dev.txt
--rw-r--r--   0 klemen     (501) staff       (20)      191 2021-12-19 22:12:53.736088 sqlite3-to-mysql-1.4.9/setup.cfg
--rw-r--r--   0 klemen     (501) staff       (20)     2492 2021-10-10 12:17:53.000000 sqlite3-to-mysql-1.4.9/setup.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.682585 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/
--rw-r--r--   0 klemen     (501) staff       (20)       96 2019-08-30 23:56:58.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)      363 2021-12-19 22:11:54.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/__version__.py
--rw-r--r--   0 klemen     (501) staff       (20)     5267 2021-09-15 21:38:13.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     2369 2021-04-18 12:23:41.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/click_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)     3387 2020-08-31 11:57:01.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/debug_info.py
--rw-r--r--   0 klemen     (501) staff       (20)     2969 2021-09-18 22:11:02.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/mysql_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)      378 2020-08-31 11:51:56.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/sixeptions.py
--rw-r--r--   0 klemen     (501) staff       (20)     1337 2021-09-15 13:46:49.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/sqlite_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)    26206 2021-12-19 22:06:09.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/transporter.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.691244 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/
--rw-r--r--   0 klemen     (501) staff       (20)     5850 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)      906 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 klemen     (501) staff       (20)       77 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/entry_points.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2019-08-29 21:34:48.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/not-zip-safe
--rw-r--r--   0 klemen     (501) staff       (20)      346 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/requires.txt
--rw-r--r--   0 klemen     (501) staff       (20)       17 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/top_level.txt
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.710607 sqlite3-to-mysql-1.4.9/tests/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.9/tests/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    12906 2021-12-19 22:12:07.000000 sqlite3-to-mysql-1.4.9/tests/conftest.py
--rw-r--r--   0 klemen     (501) staff       (20)     1260 2019-09-02 14:03:22.000000 sqlite3-to-mysql-1.4.9/tests/database.py
--rw-r--r--   0 klemen     (501) staff       (20)     4023 2021-10-10 13:39:09.000000 sqlite3-to-mysql-1.4.9/tests/factories.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.723615 sqlite3-to-mysql-1.4.9/tests/func/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.9/tests/func/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    19781 2021-10-10 13:16:37.000000 sqlite3-to-mysql-1.4.9/tests/func/sqlite3_to_mysql_test.py
--rw-r--r--   0 klemen     (501) staff       (20)    12717 2021-04-18 12:43:07.000000 sqlite3-to-mysql-1.4.9/tests/func/test_cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     5974 2021-04-17 20:58:11.000000 sqlite3-to-mysql-1.4.9/tests/models.py
--rw-r--r--   0 klemen     (501) staff       (20)      246 2019-08-27 07:59:34.000000 sqlite3-to-mysql-1.4.9/tests/sixeptions.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.730085 sqlite3-to-mysql-1.4.9/tests/unit/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.9/tests/unit/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    13223 2021-09-18 20:05:05.000000 sqlite3-to-mysql-1.4.9/tests/unit/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/requirements_dev.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/__init__.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/cli.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/click_utils.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/debug_info.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/py.typed
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/sqlite_utils.py
+-rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/transporter.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    11208 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/database.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/factories.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/func/__init__.py
+-rw-r--r--   0        0        0    24132 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/func/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/unit/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/README.md
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/PKG-INFO
```

### Comparing `sqlite3-to-mysql-1.4.9/CODE-OF-CONDUCT.md` & `sqlite3_to_mysql-2.0.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.9/LICENSE` & `sqlite3_to_mysql-2.0.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Klemen Tusar
+Copyright (c) 2023 Klemen Tusar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sqlite3-to-mysql-1.4.9/PKG-INFO` & `sqlite3_to_mysql-2.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,12 @@
-Metadata-Version: 2.1
-Name: sqlite3-to-mysql
-Version: 1.4.9
-Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
-Home-page: https://github.com/techouse/sqlite3-to-mysql
-Author: Klemen Tusar
-Author-email: techouse@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Database
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI](https://img.shields.io/pypi/v/sqlite3-to-mysql)](https://pypi.org/project/sqlite3-to-mysql/)
 [![Downloads](https://pepy.tech/badge/sqlite3-to-mysql)](https://pepy.tech/project/sqlite3-to-mysql)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlite3-to-mysql)](https://pypi.org/project/sqlite3-to-mysql/)
 [![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
-[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
+[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6|+10.11&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
 [![GitHub license](https://img.shields.io/github/license/techouse/sqlite3-to-mysql)](https://github.com/techouse/sqlite3-to-mysql/blob/master/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/d33b59d35b924711aae9418741a923ae)](https://www.codacy.com/manual/techouse/sqlite3-to-mysql?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/sqlite3-to-mysql&amp;utm_campaign=Badge_Grade)
 [![Build Status](https://github.com/techouse/sqlite3-to-mysql/workflows/Test/badge.svg)](https://github.com/techouse/sqlite3-to-mysql/actions?query=workflow%3ATest)
 [![codecov](https://codecov.io/gh/techouse/sqlite3-to-mysql/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/sqlite3-to-mysql)
 [![GitHub stars](https://img.shields.io/github/stars/techouse/sqlite3-to-mysql.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/sqlite3-to-mysql/stargazers)
@@ -65,39 +32,53 @@
 ### Usage
 ```
 Usage: sqlite3mysql [OPTIONS]
 
   Transfer SQLite to MySQL using the provided CLI options.
 
 Options:
-  -f, --sqlite-file PATH       SQLite3 database file  [required]
-  -t, --sqlite-tables TUPLE    Transfer only these specific tables (space
-                               separated table names). Implies --without-
-                               foreign-keys which inhibits the transfer of
-                               foreign keys.
-  -X, --without-foreign-keys   Do not transfer foreign keys.
-  -d, --mysql-database TEXT    MySQL database name  [required]
-  -u, --mysql-user TEXT        MySQL user  [required]
-  -p, --prompt-mysql-password  Prompt for MySQL password
-  --mysql-password TEXT        MySQL password
-  -h, --mysql-host TEXT        MySQL host. Defaults to localhost.
-  -P, --mysql-port INTEGER     MySQL port. Defaults to 3306.
-  -S, --skip-ssl               Disable MySQL connection encryption.
-  --mysql-integer-type TEXT    MySQL default integer field type. Defaults to
-                               INT(11).
-  --mysql-string-type TEXT     MySQL default string field type. Defaults to
-                               VARCHAR(255).
-  --mysql-charset TEXT         MySQL database and table character set
-                               [default: utf8mb4]
-  --mysql-collation TEXT       MySQL database and table collation
-  -T, --use-fulltext           Use FULLTEXT indexes on TEXT columns. Will
-                               throw an error if your MySQL version does not
-                               support InnoDB FULLTEXT indexes!
-  --with-rowid                 Transfer rowid columns.
-  -c, --chunk INTEGER          Chunk reading/writing SQL records
-  -l, --log-file PATH          Log file
-  -q, --quiet                  Quiet. Display only errors.
-  --version                    Show the version and exit.
-  --help                       Show this message and exit.
+  -f, --sqlite-file PATH          SQLite3 database file  [required]
+  -t, --sqlite-tables TUPLE       Transfer only these specific tables (space
+                                  separated table names). Implies --without-
+                                  foreign-keys which inhibits the transfer of
+                                  foreign keys.
+  -X, --without-foreign-keys      Do not transfer foreign keys.
+  -W, --ignore-duplicate-keys     Ignore duplicate keys. The default behavior
+                                  is to create new ones with a numerical
+                                  suffix, e.g. 'exising_key' ->
+                                  'existing_key_1'
+  -d, --mysql-database TEXT       MySQL database name  [required]
+  -u, --mysql-user TEXT           MySQL user  [required]
+  -p, --prompt-mysql-password     Prompt for MySQL password
+  --mysql-password TEXT           MySQL password
+  -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
+  -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
+  -S, --skip-ssl                  Disable MySQL connection encryption.
+  -i, --mysql-insert-method [UPDATE|IGNORE|DEFAULT]
+                                  MySQL insert method. DEFAULT will throw
+                                  errors when encountering duplicate records;
+                                  UPDATE will update existing rows; IGNORE
+                                  will ignore insert errors. Defaults to
+                                  IGNORE.
+  -E, --mysql-truncate-tables     Truncates existing tables before inserting
+                                  data.
+  --mysql-integer-type TEXT       MySQL default integer field type. Defaults
+                                  to INT(11).
+  --mysql-string-type TEXT        MySQL default string field type. Defaults to
+                                  VARCHAR(255).
+  --mysql-text-type [MEDIUMTEXT|TEXT|TINYTEXT|LONGTEXT]
+                                  MySQL default text field type. Defaults to
+                                  TEXT.
+  --mysql-charset TEXT            MySQL database and table character set
+                                  [default: utf8mb4]
+  --mysql-collation TEXT          MySQL database and table collation
+  -T, --use-fulltext              Use FULLTEXT indexes on TEXT columns. Will
+                                  throw an error if your MySQL version does
+                                  not support InnoDB FULLTEXT indexes!
+  --with-rowid                    Transfer rowid columns.
+  -c, --chunk INTEGER             Chunk reading/writing SQL records
+  -l, --log-file PATH             Log file
+  -q, --quiet                     Quiet. Display only errors.
+  --debug                         Debug mode. Will throw exceptions.
+  --version                       Show the version and exit.
+  --help                          Show this message and exit.
 ```
-
-
```

### Comparing `sqlite3-to-mysql-1.4.9/setup.py` & `sqlite3_to_mysql-2.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,125 @@
-from codecs import open
-from os.path import abspath, dirname, join
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "sqlite3-to-mysql"
+description = "A simple Python tool to transfer data from SQLite 3 to MySQL"
+readme = "README.md"
+license = { text = "MIT" }
+requires-python = ">=3.7"
+authors = [
+    { name = "Klemen Tusar", email = "techouse@gmail.com" },
+]
+urls = { Source = "https://github.com/techouse/sqlite3-to-mysql" }
+keywords = [
+    "sqlite3",
+    "mysql",
+    "transfer",
+    "data",
+    "migrate",
+    "migration",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: Database",
+]
+dependencies = [
+    "Click>=8.1.3",
+    "mysql-connector-python>=8.0.33",
+    "pytimeparse2",
+    "simplejson>=3.19.1",
+    "tqdm>=4.65.0",
+    "packaging>=23.1",
+    "tabulate",
+    "Unidecode>=1.3.6",
+    "typing_extensions",
+]
+dynamic = ["version"]
 
-from setuptools import setup
+[tool.hatch.version]
+path = "sqlite3_to_mysql/__init__.py"
 
-here = abspath(dirname(__file__))
+[tool.hatch.build.targets.sdist]
+include = [
+    "sqlite3_to_mysql",
+    "tests",
+    "README.md",
+    "CODE-OF-CONDUCT.md",
+    "LICENSE",
+    "requirements_dev.txt",
+]
 
-packages = ["sqlite3_to_mysql"]
+[project.scripts]
+sqlite3mysql = "sqlite3_to_mysql.cli:cli"
 
-requires = [
-    "Click>=7.0,<8.0.0 ; python_version<'3.6'",
-    "Click>=7.0 ; python_version>='3.6'",
-    "mysql-connector-python>=8.0.18,<8.0.24 ; python_version<'3.6'",
-    "mysql-connector-python>=8.0.18 ; python_version>='3.6'",
-    "pytimeparse>=1.1.8",
-    "six>=1.12.0",
-    "simplejson>=3.16.0",
-    "tqdm>=4.35.0",
-    "packaging>=20.3",
-    "tabulate<0.8.6 ; python_version<'3.5'",
-    "tabulate ; python_version>='3.5'",
-    "Unidecode<=1.2.0 ; python_version<'3.5'",
-    "Unidecode>=1.2.0 ; python_version>='3.5'",
-]
-
-about = {}
-with open(join(here, "sqlite3_to_mysql", "__version__.py"), "r", "utf-8") as fh:
-    exec(fh.read(), about)
-
-with open(join(here, "README.md"), "r", "utf-8") as fh:
-    readme = fh.read()
-
-setup(
-    name=about["__title__"],
-    version=about["__version__"],
-    description=about["__description__"],
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    author=about["__author__"],
-    author_email=about["__author_email__"],
-    url=about["__url__"],
-    packages=packages,
-    include_package_data=True,
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
-    install_requires=requires,
-    license=about["__license__"],
-    zip_safe=False,
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Console",
-        "Intended Audience :: End Users/Desktop",
-        "Intended Audience :: Developers",
-        "Intended Audience :: System Administrators",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Topic :: Database",
-    ],
-    project_urls={"Source": about["__url__"]},
-    entry_points="""
-        [console_scripts]
-        sqlite3mysql=sqlite3_to_mysql.cli:cli
-    """,
+[tool.black]
+line-length = 120
+target-version = ["py37", "py38", "py39", "py310", "py311"]
+include = '\.pyi?$'
+exclude = '''
+(
+    /(
+        \.eggs
+        | \.git
+        | \.hg
+        | \.mypy_cache
+        | \.tox
+        | \.venv
+        | _build
+        | buck-out
+        | build
+        | dist
+    )/
+    | foo.py
 )
+'''
+
+[tool.isort]
+line_length = 120
+profile = "black"
+lines_after_imports = 2
+known_first_party = "sqlite3_to_mysql"
+skip_gitignore = true
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+norecursedirs = [".*", "venv", "env", "*.egg", "dist", "build"]
+minversion = "7.3.1"
+addopts = "-rsxX -l --tb=short --strict-markers"
+timeout = 300
+markers = [
+    "init: Run the initialisation test functions",
+    "transfer: Run the main transfer test functions",
+    "cli: Run the cli test functions",
+]
+
+[tool.mypy]
+python_version = "3.7"
+exclude = [
+    "tests",
+    "build",
+    "dist",
+    "venv",
+    "env",
+]
+warn_return_any = true
+warn_unused_configs = true
+
+[[tool.mypy.overrides]]
+module = "pytimeparse2.*,factory.*,docker.*"
+ignore_missing_imports = true
```

### Comparing `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/cli.py` & `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """The command line interface of SQLite3toMySQL."""
-
+import os
 import sys
+import typing as t
 
 import click
 from mysql.connector import CharacterSet
 from tabulate import tabulate
 
 from . import SQLite3toMySQL
 from .click_utils import OptionEatAll, prompt_password
 from .debug_info import info
-from .mysql_utils import mysql_supported_character_sets
+from .mysql_utils import MYSQL_INSERT_METHOD, MYSQL_TEXT_COLUMN_TYPES, mysql_supported_character_sets
 
 
 @click.command()
 @click.option(
     "-f",
     "--sqlite-file",
     type=click.Path(exists=True),
@@ -25,50 +26,67 @@
     "-t",
     "--sqlite-tables",
     type=tuple,
     cls=OptionEatAll,
     help="Transfer only these specific tables (space separated table names). "
     "Implies --without-foreign-keys which inhibits the transfer of foreign keys.",
 )
+@click.option("-X", "--without-foreign-keys", is_flag=True, help="Do not transfer foreign keys.")
 @click.option(
-    "-X", "--without-foreign-keys", is_flag=True, help="Do not transfer foreign keys."
-)
-@click.option(
-    "-d", "--mysql-database", default=None, help="MySQL database name", required=True
+    "-W",
+    "--ignore-duplicate-keys",
+    is_flag=True,
+    help="Ignore duplicate keys. The default behavior is to create new ones with a numerical suffix, e.g. "
+    "'exising_key' -> 'existing_key_1'",
 )
+@click.option("-d", "--mysql-database", default=None, help="MySQL database name", required=True)
 @click.option("-u", "--mysql-user", default=None, help="MySQL user", required=True)
 @click.option(
     "-p",
     "--prompt-mysql-password",
     is_flag=True,
     default=False,
     callback=prompt_password,
     help="Prompt for MySQL password",
 )
 @click.option("--mysql-password", default=None, help="MySQL password")
-@click.option(
-    "-h", "--mysql-host", default="localhost", help="MySQL host. Defaults to localhost."
-)
-@click.option(
-    "-P", "--mysql-port", type=int, default=3306, help="MySQL port. Defaults to 3306."
+@click.option("-h", "--mysql-host", default="localhost", help="MySQL host. Defaults to localhost.")
+@click.option("-P", "--mysql-port", type=int, default=3306, help="MySQL port. Defaults to 3306.")
+@click.option("-S", "--skip-ssl", is_flag=True, help="Disable MySQL connection encryption.")
+@click.option(
+    "-i",
+    "--mysql-insert-method",
+    type=click.Choice(MYSQL_INSERT_METHOD, case_sensitive=False),
+    default="IGNORE",
+    help="MySQL insert method. DEFAULT will throw errors when encountering duplicate records; "
+    "UPDATE will update existing rows; IGNORE will ignore insert errors. Defaults to IGNORE.",
 )
 @click.option(
-    "-S", "--skip-ssl", is_flag=True, help="Disable MySQL connection encryption."
+    "-E",
+    "--mysql-truncate-tables",
+    is_flag=True,
+    help="Truncates existing tables before inserting data.",
 )
 @click.option(
     "--mysql-integer-type",
     default="INT(11)",
     help="MySQL default integer field type. Defaults to INT(11).",
 )
 @click.option(
     "--mysql-string-type",
     default="VARCHAR(255)",
     help="MySQL default string field type. Defaults to VARCHAR(255).",
 )
 @click.option(
+    "--mysql-text-type",
+    type=click.Choice(MYSQL_TEXT_COLUMN_TYPES, case_sensitive=False),
+    default="TEXT",
+    help="MySQL default text field type. Defaults to TEXT.",
+)
+@click.option(
     "--mysql-charset",
     metavar="TEXT",
     type=click.Choice(list(CharacterSet.get_supported()), case_sensitive=False),
     default="utf8mb4",
     show_default=True,
     help="MySQL database and table character set",
 )
@@ -86,81 +104,83 @@
     "-T",
     "--use-fulltext",
     is_flag=True,
     help="Use FULLTEXT indexes on TEXT columns. "
     "Will throw an error if your MySQL version does not support InnoDB FULLTEXT indexes!",
 )
 @click.option("--with-rowid", is_flag=True, help="Transfer rowid columns.")
-@click.option(
-    "-c", "--chunk", type=int, default=None, help="Chunk reading/writing SQL records"
-)
+@click.option("-c", "--chunk", type=int, default=None, help="Chunk reading/writing SQL records")
 @click.option("-l", "--log-file", type=click.Path(), help="Log file")
 @click.option("-q", "--quiet", is_flag=True, help="Quiet. Display only errors.")
-@click.version_option(
-    message=tabulate(info(), headers=["software", "version"], tablefmt="github")
-)
+@click.option("--debug", is_flag=True, help="Debug mode. Will throw exceptions.")
+@click.version_option(message=tabulate(info(), headers=["software", "version"], tablefmt="github"))
 def cli(
-    sqlite_file,
-    sqlite_tables,
-    without_foreign_keys,
-    mysql_user,
-    prompt_mysql_password,
-    mysql_password,
-    mysql_database,
-    mysql_host,
-    mysql_port,
-    skip_ssl,
-    mysql_integer_type,
-    mysql_string_type,
-    mysql_charset,
-    mysql_collation,
-    use_fulltext,
-    with_rowid,
-    chunk,
-    log_file,
-    quiet,
-):
+    sqlite_file: t.Union[str, "os.PathLike[t.Any]"],
+    sqlite_tables: t.Optional[t.Sequence[str]],
+    without_foreign_keys: bool,
+    ignore_duplicate_keys: bool,
+    mysql_user: str,
+    prompt_mysql_password: bool,
+    mysql_password: str,
+    mysql_database: str,
+    mysql_host: str,
+    mysql_port: int,
+    skip_ssl: bool,
+    mysql_insert_method: str,
+    mysql_truncate_tables: bool,
+    mysql_integer_type: str,
+    mysql_string_type: str,
+    mysql_text_type: str,
+    mysql_charset: str,
+    mysql_collation: str,
+    use_fulltext: bool,
+    with_rowid: bool,
+    chunk: int,
+    log_file: t.Union[str, "os.PathLike[t.Any]"],
+    quiet: bool,
+    debug: bool,
+) -> None:
     """Transfer SQLite to MySQL using the provided CLI options."""
     try:
         if mysql_collation:
-            charset_collations = tuple(
-                cs.collation
-                for cs in mysql_supported_character_sets(mysql_charset.lower())
+            charset_collations: t.Tuple[str, ...] = tuple(
+                cs.collation for cs in mysql_supported_character_sets(mysql_charset.lower())
             )
             if mysql_collation not in set(charset_collations):
                 raise click.ClickException(
-                    "Error: Invalid value for '--collation' of charset '{charset}': '{collation}' is not one of "
-                    "{collations}.".format(
-                        collation=mysql_collation,
-                        charset=mysql_charset,
-                        collations="'" + "', '".join(charset_collations) + "'",
-                    )
+                    f"""Error: Invalid value for '--collation' of charset '{mysql_charset}': '{mysql_collation}' is not one of {"'" + "', '".join(charset_collations) + "'"}."""
                 )
 
-        converter = SQLite3toMySQL(
+        SQLite3toMySQL(
             sqlite_file=sqlite_file,
-            sqlite_tables=sqlite_tables,
-            without_foreign_keys=without_foreign_keys
-            or (sqlite_tables is not None and len(sqlite_tables) > 0),
+            sqlite_tables=sqlite_tables or tuple(),
+            without_foreign_keys=without_foreign_keys or (sqlite_tables is not None and len(sqlite_tables) > 0),
             mysql_user=mysql_user,
             mysql_password=mysql_password or prompt_mysql_password,
             mysql_database=mysql_database,
             mysql_host=mysql_host,
             mysql_port=mysql_port,
             mysql_ssl_disabled=skip_ssl,
+            mysql_insert_method=mysql_insert_method,
+            mysql_truncate_tables=mysql_truncate_tables,
             mysql_integer_type=mysql_integer_type,
             mysql_string_type=mysql_string_type,
+            mysql_text_type=mysql_text_type,
             mysql_charset=mysql_charset.lower() if mysql_charset else "utf8mb4",
             mysql_collation=mysql_collation.lower() if mysql_collation else None,
+            ignore_duplicate_keys=ignore_duplicate_keys,
             use_fulltext=use_fulltext,
             with_rowid=with_rowid,
             chunk=chunk,
             log_file=log_file,
             quiet=quiet,
-        )
-        converter.transfer()
+        ).transfer()
     except KeyboardInterrupt:
+        if debug:
+            raise
         click.echo("\nProcess interrupted. Exiting...")
         sys.exit(1)
     except Exception as err:  # pylint: disable=W0703
+        if debug:
+            raise
         click.echo(err)
         sys.exit(1)
```

### Comparing `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/click_utils.py` & `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/click_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Click utilities."""
 
+import typing as t
+
 import click
 
 
 class OptionEatAll(click.Option):
     """Taken from https://stackoverflow.com/questions/48391777/nargs-equivalent-for-options-in-click#answer-48394004."""  # noqa: ignore=E501 pylint: disable=C0301
 
     def __init__(self, *args, **kwargs):
         """Override."""
         self.save_other_options = kwargs.pop("save_other_options", True)
         nargs = kwargs.pop("nargs", -1)
         if nargs != -1:
-            raise ValueError("nargs, if set, must be -1 not {}".format(nargs))
+            raise ValueError(f"nargs, if set, must be -1 not {nargs}")
         super(OptionEatAll, self).__init__(*args, **kwargs)
         self._previous_parser_process = None
         self._eat_all_parser = None
 
-    def add_to_parser(self, parser, ctx):
+    def add_to_parser(self, parser, ctx) -> None:
         """Override."""
 
-        def parser_process(value, state):
+        def parser_process(value, state) -> None:
             # method to hook to the parser.process
-            done = False
+            done: bool = False
             value = [value]
             if self.save_other_options:
                 # grab everything up to the next option
                 while state.rargs and not done:
                     for prefix in self._eat_all_parser.prefixes:
                         if state.rargs[0].startswith(prefix):
                             done = True
@@ -36,29 +38,27 @@
                 value += state.rargs
                 state.rargs[:] = []
             value = tuple(value)
 
             # call the actual process
             self._previous_parser_process(value, state)
 
-        retval = super(OptionEatAll, self).add_to_parser(  # pylint: disable=E1111
-            parser, ctx
-        )
+        retval = super(OptionEatAll, self).add_to_parser(parser, ctx)  # pylint: disable=E1111
         for name in self.opts:
             # pylint: disable=W0212
             our_parser = parser._long_opt.get(name) or parser._short_opt.get(name)
             if our_parser:
                 self._eat_all_parser = our_parser
                 self._previous_parser_process = our_parser.process
                 our_parser.process = parser_process
                 break
         return retval
 
 
-def prompt_password(ctx, param, use_password):  # pylint: disable=W0613
+def prompt_password(ctx: click.core.Context, param: t.Any, use_password: bool):  # pylint: disable=W0613
     """Prompt for password."""
     if use_password:
         mysql_password = ctx.params.get("mysql_password")
         if not mysql_password:
             mysql_password = click.prompt("MySQL password", hide_input=True)
 
         return mysql_password
```

### Comparing `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/debug_info.py` & `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/debug_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,91 @@
 """Module containing bug report helper(s).
 
 Adapted from https://github.com/psf/requests/blob/master/requests/help.py
 """
 
-from __future__ import print_function
-
 import platform
 import sqlite3
 import sys
-from distutils.spawn import find_executable
+import typing as t
+from distutils.spawn import find_executable  # pylint: disable=W0402
 from subprocess import check_output
 
 import click
 import mysql.connector
-import pytimeparse
+import pytimeparse2
 import simplejson
-import six
 import tabulate
 import tqdm
 
 from . import __version__ as package_version
 
 
-def _implementation():
+def _implementation() -> str:
     """Return a dict with the Python implementation and version.
 
     Provide both the name and the version of the Python implementation
     currently running. For example, on CPython 2.7.5 it will return
     {'name': 'CPython', 'version': '2.7.5'}.
 
     This function works best on CPython and PyPy: in particular, it probably
     doesn't work for Jython or IronPython. Future investigation should be done
     to work out the correct shape of the code for those platforms.
     """
-    implementation = platform.python_implementation()
+    implementation: str = platform.python_implementation()
 
     if implementation == "CPython":
         implementation_version = platform.python_version()
     elif implementation == "PyPy":
         implementation_version = "%s.%s.%s" % (
-            sys.pypy_version_info.major,  # noqa: ignore=E1101 pylint: disable=E1101
-            sys.pypy_version_info.minor,  # noqa: ignore=E1101 pylint: disable=E1101
-            sys.pypy_version_info.micro,  # noqa: ignore=E1101 pylint: disable=E1101
-        )
-        rel = (
-            sys.pypy_version_info.releaselevel  # noqa: ignore=E1101 pylint: disable=E1101
+            sys.pypy_version_info.major,  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
+            sys.pypy_version_info.minor,  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
+            sys.pypy_version_info.micro,  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
         )
+        rel = sys.pypy_version_info.releaselevel  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
         if rel != "final":
             implementation_version = "".join([implementation_version, rel])
     elif implementation == "Jython":
         implementation_version = platform.python_version()  # Complete Guess
     elif implementation == "IronPython":
         implementation_version = platform.python_version()  # Complete Guess
     else:
         implementation_version = "Unknown"
 
-    return "{implementation} {implementation_version}".format(
-        implementation=implementation, implementation_version=implementation_version
-    )
+    return f"{implementation} {implementation_version}"
 
 
-def _mysql_version():
+def _mysql_version() -> str:
     if find_executable("mysql"):
         try:
-            mysql_version = check_output(["mysql", "-V"])
+            mysql_version: t.Union[str, bytes] = check_output(["mysql", "-V"])
             try:
-                return mysql_version.decode().strip()
+                return mysql_version.decode().strip()  # type: ignore
             except (UnicodeDecodeError, AttributeError):
-                return mysql_version
+                return str(mysql_version)
         except Exception:  # nosec pylint: disable=W0703
             pass
     return "MySQL client not found on the system"
 
 
-def info():
+def info() -> t.List[t.List[str]]:
     """Generate information for a bug report."""
     try:
-        platform_info = "{system} {release}".format(
-            system=platform.system(),
-            release=platform.release(),
-        )
+        platform_info = f"{platform.system()} {platform.release()}"
     except IOError:
         platform_info = "Unknown"
 
     return [
-        ["sqlite3-to-mysql", package_version.__version__],
+        ["sqlite3-to-mysql", package_version],
         ["", ""],
         ["Operating System", platform_info],
         ["Python", _implementation()],
         ["MySQL", _mysql_version()],
         ["SQLite", sqlite3.sqlite_version],
         ["", ""],
         ["click", click.__version__],
         ["mysql-connector-python", mysql.connector.__version__],
-        ["pytimeparse", pytimeparse.__version__],
-        ["simplejson", simplejson.__version__],
-        ["six", six.__version__],
+        ["pytimeparse2", pytimeparse2.__version__],
+        ["simplejson", simplejson.__version__],  # type: ignore
         ["tabulate", tabulate.__version__],
         ["tqdm", tqdm.__version__],
     ]
```

### Comparing `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/transporter.py` & `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/transporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,147 +1,151 @@
 """Use to transfer an SQLite 3 database to MySQL."""
 
-from __future__ import division
-
 import logging
+import os
 import re
 import sqlite3
+import typing as t
 from datetime import timedelta
 from decimal import Decimal
+from itertools import chain
 from math import ceil
 from os.path import isfile, realpath
 from sys import stdout
 
 import mysql.connector
-import six
-from mysql.connector import CharacterSet, errorcode
+import typing_extensions as tx
+from mysql.connector import CharacterSet
+from mysql.connector import __version__ as mysql_connector_version_string
+from mysql.connector import errorcode
+from packaging import version
 from tqdm import tqdm, trange
 
 from sqlite3_to_mysql.sqlite_utils import (
     adapt_decimal,
     adapt_timedelta,
-    convert_blob,
+    check_sqlite_table_xinfo_support,
+    convert_date,
     convert_decimal,
     convert_timedelta,
     unicase_compare,
 )
 
 from .mysql_utils import (
+    MYSQL_BLOB_COLUMN_TYPES,
     MYSQL_COLUMN_TYPES,
+    MYSQL_COLUMN_TYPES_WITHOUT_DEFAULT,
+    MYSQL_INSERT_METHOD,
+    MYSQL_TEXT_COLUMN_TYPES,
+    MYSQL_TEXT_COLUMN_TYPES_WITH_JSON,
     check_mysql_fulltext_support,
     check_mysql_json_support,
     safe_identifier_length,
 )
-
-if six.PY2:
-    from .sixeptions import *  # pylint: disable=W0622,W0401,W0614
+from .types import SQLite3toMySQLAttributes, SQLite3toMySQLParams
 
 
-class SQLite3toMySQL:
+class SQLite3toMySQL(SQLite3toMySQLAttributes):
     """Use this class to transfer an SQLite 3 database to MySQL."""
 
-    COLUMN_PATTERN = re.compile(r"^[^(]+")
-    COLUMN_LENGTH_PATTERN = re.compile(r"\(\d+\)$")
+    COLUMN_PATTERN: t.Pattern[str] = re.compile(r"^[^(]+")
+    COLUMN_LENGTH_PATTERN: t.Pattern[str] = re.compile(r"\(\d+\)$")
+
+    MYSQL_CONNECTOR_VERSION: version.Version = version.parse(mysql_connector_version_string)
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: tx.Unpack[SQLite3toMySQLParams]):
         """Constructor."""
-        if not kwargs.get("sqlite_file"):
+        if kwargs.get("sqlite_file") is None:
             raise ValueError("Please provide an SQLite file")
-
-        if not isfile(kwargs.get("sqlite_file")):
+        elif not isfile(str(kwargs.get("sqlite_file"))):
             raise FileNotFoundError("SQLite file does not exist")
+        else:
+            self._sqlite_file = realpath(str(kwargs.get("sqlite_file")))
 
-        if not kwargs.get("mysql_user"):
+        if kwargs.get("mysql_user") is not None:
+            self._mysql_user = str(kwargs.get("mysql_user"))
+        else:
             raise ValueError("Please provide a MySQL user")
 
-        self._sqlite_file = realpath(kwargs.get("sqlite_file"))
+        self._mysql_password = str(kwargs.get("mysql_password")) or None
 
-        self._sqlite_tables = (
-            tuple(kwargs.get("sqlite_tables"))
-            if kwargs.get("sqlite_tables") is not None
-            else tuple()
-        )
-
-        self._without_foreign_keys = (
-            True
-            if len(self._sqlite_tables) > 0
-            else (kwargs.get("without_foreign_keys") or False)
-        )
+        self._mysql_host = kwargs.get("mysql_host") or "localhost"
 
-        self._mysql_user = str(kwargs.get("mysql_user"))
-
-        self._mysql_password = (
-            str(kwargs.get("mysql_password")) if kwargs.get("mysql_password") else None
-        )
+        self._mysql_port = kwargs.get("mysql_port") or 3306
 
-        self._mysql_host = str(kwargs.get("mysql_host") or "localhost")
+        self._sqlite_tables = kwargs.get("sqlite_tables") or tuple()
 
-        self._mysql_port = int(kwargs.get("mysql_port") or 3306)
+        self._without_foreign_keys = len(self._sqlite_tables) > 0 or kwargs.get("without_foreign_keys") or False
 
         self._mysql_ssl_disabled = kwargs.get("mysql_ssl_disabled") or False
 
-        self._chunk_size = int(kwargs.get("chunk")) if kwargs.get("chunk") else None
+        self._chunk_size = kwargs.get("chunk") or None
 
         self._quiet = kwargs.get("quiet") or False
 
-        self._logger = self._setup_logger(
-            log_file=kwargs.get("log_file") or None, quiet=self._quiet
-        )
+        self._logger = self._setup_logger(log_file=kwargs.get("log_file") or None, quiet=self._quiet)
+
+        self._mysql_database = kwargs.get("mysql_database") or "transfer"
+
+        self._mysql_insert_method = str(kwargs.get("mysql_integer_type") or "IGNORE").upper()
+        if self._mysql_insert_method not in MYSQL_INSERT_METHOD:
+            self._mysql_insert_method = "IGNORE"
+
+        self._mysql_truncate_tables = kwargs.get("mysql_truncate_tables") or False
+
+        self._mysql_integer_type = str(kwargs.get("mysql_integer_type") or "INT(11)").upper()
 
-        self._mysql_database = str(kwargs.get("mysql_database") or "transfer")
+        self._mysql_string_type = str(kwargs.get("mysql_string_type") or "VARCHAR(255)").upper()
 
-        self._mysql_integer_type = str(
-            kwargs.get("mysql_integer_type") or "INT(11)"
-        ).upper()
-
-        self._mysql_string_type = str(
-            kwargs.get("mysql_string_type") or "VARCHAR(255)"
-        ).upper()
+        self._mysql_text_type = str(kwargs.get("mysql_text_type") or "TEXT").upper()
+        if self._mysql_text_type not in MYSQL_TEXT_COLUMN_TYPES:
+            self._mysql_text_type = "TEXT"
 
         self._mysql_charset = kwargs.get("mysql_charset") or "utf8mb4"
 
         self._mysql_collation = (
-            kwargs.get("mysql_collation")
-            or CharacterSet.get_default_collation(self._mysql_charset.lower())[0]
+            kwargs.get("mysql_collation") or CharacterSet.get_default_collation(self._mysql_charset.lower())[0]
         )
-        if (
-            not kwargs.get("mysql_collation")
-            and self._mysql_collation == "utf8mb4_0900_ai_ci"
-        ):
+        if not kwargs.get("mysql_collation") and self._mysql_collation == "utf8mb4_0900_ai_ci":
             self._mysql_collation = "utf8mb4_general_ci"
 
+        self._ignore_duplicate_keys = kwargs.get("ignore_duplicate_keys") or False
+
         self._use_fulltext = kwargs.get("use_fulltext") or False
 
         self._with_rowid = kwargs.get("with_rowid") or False
 
         sqlite3.register_adapter(Decimal, adapt_decimal)
         sqlite3.register_converter("DECIMAL", convert_decimal)
         sqlite3.register_adapter(timedelta, adapt_timedelta)
+        sqlite3.register_converter("DATE", convert_date)
         sqlite3.register_converter("TIME", convert_timedelta)
 
-        if six.PY2:
-            sqlite3.register_converter("BLOB", convert_blob)
-
-        self._sqlite = sqlite3.connect(
-            realpath(self._sqlite_file), detect_types=sqlite3.PARSE_DECLTYPES
-        )
+        self._sqlite = sqlite3.connect(realpath(self._sqlite_file), detect_types=sqlite3.PARSE_DECLTYPES)
         self._sqlite.row_factory = sqlite3.Row
         self._sqlite.create_collation("unicase", unicase_compare)
 
         self._sqlite_cur = self._sqlite.cursor()
 
+        self._sqlite_version = self._get_sqlite_version()
+        self._sqlite_table_xinfo_support = check_sqlite_table_xinfo_support(self._sqlite_version)
+
         try:
-            self._mysql = mysql.connector.connect(
+            _mysql_connection = mysql.connector.connect(
                 user=self._mysql_user,
                 password=self._mysql_password,
                 host=self._mysql_host,
                 port=self._mysql_port,
                 ssl_disabled=self._mysql_ssl_disabled,
                 use_pure=True,
             )
+            if isinstance(_mysql_connection, mysql.connector.MySQLConnection):
+                self._mysql = _mysql_connection
+            else:
+                raise ConnectionError("Unable to connect to MySQL")
             if not self._mysql.is_connected():
                 raise ConnectionError("Unable to connect to MySQL")
 
             self._mysql_cur = self._mysql.cursor(prepared=True)
 
             try:
                 self._mysql.database = self._mysql_database
@@ -150,31 +154,27 @@
                     self._create_database()
                 else:
                     self._logger.error(err)
                     raise
 
             self._mysql_version = self._get_mysql_version()
             self._mysql_json_support = check_mysql_json_support(self._mysql_version)
-            self._mysql_fulltext_support = check_mysql_fulltext_support(
-                self._mysql_version
-            )
+            self._mysql_fulltext_support = check_mysql_fulltext_support(self._mysql_version)
 
             if self._use_fulltext and not self._mysql_fulltext_support:
-                raise ValueError(
-                    "Your MySQL version does not support InnoDB FULLTEXT indexes!"
-                )
+                raise ValueError("Your MySQL version does not support InnoDB FULLTEXT indexes!")
         except mysql.connector.Error as err:
             self._logger.error(err)
             raise
 
     @classmethod
-    def _setup_logger(cls, log_file=None, quiet=False):
-        formatter = logging.Formatter(
-            fmt="%(asctime)s %(levelname)-8s %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
-        )
+    def _setup_logger(
+        cls, log_file: t.Optional[t.Union[str, "os.PathLike[t.Any]"]] = None, quiet: bool = False
+    ) -> logging.Logger:
+        formatter = logging.Formatter(fmt="%(asctime)s %(levelname)-8s %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
         logger = logging.getLogger(cls.__name__)
         logger.setLevel(logging.DEBUG)
 
         if not quiet:
             screen_handler = logging.StreamHandler(stream=stdout)
             screen_handler.setFormatter(formatter)
             logger.addHandler(screen_handler)
@@ -182,243 +182,270 @@
         if log_file:
             file_handler = logging.FileHandler(realpath(log_file), mode="w")
             file_handler.setFormatter(formatter)
             logger.addHandler(file_handler)
 
         return logger
 
-    def _get_mysql_version(self):
+    def _get_mysql_version(self) -> str:
         try:
             self._mysql_cur.execute("SHOW VARIABLES LIKE 'version'")
-            return self._mysql_cur.fetchone()[1]
+            row = self._mysql_cur.fetchone()
+            if row:
+                return str(row[1])
+            else:
+                self._logger.error("MySQL failed checking for InnoDB version")
+                raise mysql.connector.Error("MySQL failed checking for InnoDB version")
         except (IndexError, mysql.connector.Error) as err:
             self._logger.error(
                 "MySQL failed checking for InnoDB version: %s",
                 err,
             )
             raise
 
-    def _sqlite_table_has_rowid(self, table):
+    def _get_sqlite_version(self) -> str:
+        try:
+            self._sqlite_cur.execute("SELECT sqlite_version()")
+            return str(self._sqlite_cur.fetchone()[0])
+        except (IndexError, sqlite3.Error) as err:
+            self._logger.error(
+                "SQLite failed checking for InnoDB version: %s",
+                err,
+            )
+            raise
+
+    def _sqlite_table_has_rowid(self, table: str) -> bool:
         try:
-            self._sqlite_cur.execute("""SELECT rowid FROM "{}" LIMIT 1""".format(table))
+            self._sqlite_cur.execute(f'SELECT rowid FROM "{table}" LIMIT 1')
             self._sqlite_cur.fetchall()
             return True
         except sqlite3.OperationalError:
             return False
 
-    def _create_database(self):
+    def _create_database(self) -> None:
         try:
             self._mysql_cur.execute(
-                """
-                CREATE DATABASE IF NOT EXISTS `{database}`
-                DEFAULT CHARACTER SET {charset}
-                DEFAULT COLLATE {collation}
-            """.format(
-                    database=self._mysql_database,
-                    charset=self._mysql_charset,
-                    collation=self._mysql_collation,
-                )
+                f"""
+                CREATE DATABASE IF NOT EXISTS `{self._mysql_database}`
+                DEFAULT CHARACTER SET {self._mysql_charset}
+                DEFAULT COLLATE {self._mysql_collation}
+            """
             )
             self._mysql_cur.close()
             self._mysql.commit()
             self._mysql.database = self._mysql_database
-            self._mysql_cur = self._mysql.cursor(prepared=True)
+            self._mysql_cur = self._mysql.cursor(prepared=True)  # pylint: disable=W0201
         except mysql.connector.Error as err:
             self._logger.error(
                 "MySQL failed creating databse %s: %s",
                 self._mysql_database,
                 err,
             )
             raise
 
     @classmethod
-    def _valid_column_type(cls, column_type):
+    def _valid_column_type(cls, column_type: str) -> t.Optional[t.Match[str]]:
         return cls.COLUMN_PATTERN.match(column_type.strip())
 
-    def _translate_type_from_sqlite_to_mysql(self, column_type):
+    def _translate_type_from_sqlite_to_mysql(self, column_type: str) -> str:
         """This could be optimized even further, however is seems adequate."""
-        full_column_type = column_type.upper()
-        match = self._valid_column_type(column_type)
+        full_column_type: str = column_type.upper()
+        match: t.Optional[t.Match[str]] = self._valid_column_type(column_type)
         if not match:
             raise ValueError("Invalid column_type!")
 
-        data_type = match.group(0).upper()
+        data_type: str = match.group(0).upper()
         if data_type in {"TEXT", "CLOB", "STRING"}:
-            return "TEXT"
+            return self._mysql_text_type
         if data_type in {"CHARACTER", "NCHAR", "NATIVE CHARACTER"}:
             return "CHAR" + self._column_type_length(column_type)
         if data_type in {"VARYING CHARACTER", "NVARCHAR", "VARCHAR"}:
-            if self._mysql_string_type == "TEXT":
+            if self._mysql_string_type in MYSQL_TEXT_COLUMN_TYPES:
                 return self._mysql_string_type
             length = self._column_type_length(column_type)
             if not length:
                 return self._mysql_string_type
             match = self._valid_column_type(self._mysql_string_type)
-            return match.group(0).upper() + length
+            if match:
+                return match.group(0).upper() + length
         if data_type == "DOUBLE PRECISION":
             return "DOUBLE"
         if data_type == "UNSIGNED BIG INT":
             return "BIGINT" + self._column_type_length(column_type) + " UNSIGNED"
         if data_type in {"INT1", "INT2"}:
             return self._mysql_integer_type
         if data_type in {"INTEGER", "INT"}:
             length = self._column_type_length(column_type)
             if not length:
                 return self._mysql_integer_type
             match = self._valid_column_type(self._mysql_integer_type)
-            if self._mysql_integer_type.endswith("UNSIGNED"):
-                return match.group(0).upper() + length + " UNSIGNED"
-            return match.group(0).upper() + length
+            if match:
+                if self._mysql_integer_type.endswith("UNSIGNED"):
+                    return match.group(0).upper() + length + " UNSIGNED"
+                return match.group(0).upper() + length
         if data_type in {"INT64", "NUMERIC"}:
             return "BIGINT" + self._column_type_length(column_type, 19)
+        if data_type == "BOOLEAN":
+            return "TINYINT(1)"
         if data_type not in MYSQL_COLUMN_TYPES:
             return self._mysql_string_type
         return full_column_type
 
     @classmethod
-    def _column_type_length(cls, column_type, default=None):
-        suffix = cls.COLUMN_LENGTH_PATTERN.search(column_type)
+    def _column_type_length(cls, column_type: str, default: t.Optional[t.Union[str, int, float]] = None) -> str:
+        suffix: t.Optional[t.Match[str]] = cls.COLUMN_LENGTH_PATTERN.search(column_type)
         if suffix:
             return suffix.group(0)
         if default:
-            return "({})".format(default)
+            return f"({default})"
         return ""
 
-    def _create_table(self, table_name, transfer_rowid=False):
-        primary_keys = []
+    def _create_table(self, table_name: str, transfer_rowid: bool = False) -> None:
+        primary_keys: t.List[t.Dict[str, str]] = []
 
-        sql = "CREATE TABLE IF NOT EXISTS `{}` ( ".format(
-            safe_identifier_length(table_name)
-        )
+        sql: str = f"CREATE TABLE IF NOT EXISTS `{safe_identifier_length(table_name)}` ( "
 
         if transfer_rowid:
             sql += " `rowid` BIGINT NOT NULL, "
 
-        self._sqlite_cur.execute('PRAGMA table_info("{}")'.format(table_name))
+        if self._sqlite_table_xinfo_support:
+            self._sqlite_cur.execute(f'PRAGMA table_xinfo("{table_name}")')
+        else:
+            self._sqlite_cur.execute(f'PRAGMA table_info("{table_name}")')
+
+        rows: t.List[t.Any] = self._sqlite_cur.fetchall()
+        compound_primary_key: bool = len(tuple(True for row in rows if dict(row)["pk"] > 0)) > 1
 
-        rows = self._sqlite_cur.fetchall()
-        compound_primary_key = (
-            len(tuple(True for row in rows if dict(row)["pk"] > 0)) > 1
-        )
         for row in rows:
-            column = dict(row)
-            sql += " `{name}` {type} {notnull} {dflt} {auto_increment}, ".format(
-                name=safe_identifier_length(column["name"]),
-                type=self._translate_type_from_sqlite_to_mysql(column["type"]),
+            column: t.Dict[str, t.Any] = dict(row)
+            mysql_safe_name: str = safe_identifier_length(column["name"])
+            column_type: str = self._translate_type_from_sqlite_to_mysql(column["type"])
+
+            # The "hidden" value is 0 for visible columns, 1 for "hidden" columns,
+            # 2 for computed virtual columns and 3 for computed stored columns.
+            # Read more on hidden columns here https://www.sqlite.org/pragma.html#pragma_table_xinfo
+            if "hidden" in column and column["hidden"] == 1:
+                continue
+
+            sql += " `{name}` {type} {notnull} {default} {auto_increment}, ".format(
+                name=mysql_safe_name,
+                type=column_type,
                 notnull="NOT NULL" if column["notnull"] or column["pk"] else "NULL",
                 auto_increment="AUTO_INCREMENT"
-                if column["pk"] > 0
-                and self._translate_type_from_sqlite_to_mysql(
-                    column["type"]
-                ).startswith(("INT", "BIGINT"))
-                and not compound_primary_key
+                if column["pk"] > 0 and column_type.startswith(("INT", "BIGINT")) and not compound_primary_key
+                else "",
+                default="DEFAULT " + column["dflt_value"]
+                if column["dflt_value"] and column_type not in MYSQL_COLUMN_TYPES_WITHOUT_DEFAULT
                 else "",
-                dflt="DEFAULT " + column["dflt_value"] if column["dflt_value"] else "",
             )
+
             if column["pk"] > 0:
-                primary_key = {
-                    "column": safe_identifier_length(column["name"]),
+                primary_key: t.Dict[str, str] = {
+                    "column": mysql_safe_name,
                     "length": "",
                 }
                 # In case we have a non-numeric primary key
-                column_type = self._translate_type_from_sqlite_to_mysql(column["type"])
-                if column_type in {"TEXT", "BLOB"} or column_type.startswith(
-                    ("CHAR", "VARCHAR")
-                ):
+                if column_type in (
+                    MYSQL_TEXT_COLUMN_TYPES_WITH_JSON + MYSQL_BLOB_COLUMN_TYPES
+                ) or column_type.startswith(("CHAR", "VARCHAR")):
                     primary_key["length"] = self._column_type_length(column_type, 255)
                 primary_keys.append(primary_key)
 
         sql = sql.rstrip(", ")
+
         if len(primary_keys) > 0:
             sql += ", PRIMARY KEY ({columns})".format(
-                columns=", ".join(
-                    "`{column}`{length}".format(**primary_key)
-                    for primary_key in primary_keys
-                )
+                columns=", ".join("`{column}`{length}".format(**primary_key) for primary_key in primary_keys)
             )
+
         if transfer_rowid:
-            sql += ", CONSTRAINT `{}_rowid` UNIQUE (`rowid`)".format(
-                safe_identifier_length(table_name)
-            )
-        sql += " ) ENGINE=InnoDB DEFAULT CHARSET={charset} COLLATE={collation}".format(
-            charset=self._mysql_charset,
-            collation=self._mysql_collation,
-        )
+            sql += f", CONSTRAINT `{safe_identifier_length(table_name)}_rowid` UNIQUE (`rowid`)"
+
+        sql += f" ) ENGINE=InnoDB DEFAULT CHARSET={self._mysql_charset} COLLATE={self._mysql_collation}"
 
         try:
             self._mysql_cur.execute(sql)
             self._mysql.commit()
         except mysql.connector.Error as err:
             self._logger.error(
                 "MySQL failed creating table %s: %s",
                 safe_identifier_length(table_name),
                 err,
             )
             raise
 
-    def _add_indices(self, table_name):
-        self._sqlite_cur.execute('PRAGMA table_info("{}")'.format(table_name))
-        table_columns = {}
+    def _truncate_table(self, table_name: str) -> None:
+        self._mysql_cur.execute(
+            """
+            SELECT `TABLE_NAME`
+            FROM `INFORMATION_SCHEMA`.`TABLES`
+            WHERE `TABLE_SCHEMA` = %s
+            AND `TABLE_NAME` = %s
+            LIMIT 1
+            """,
+            (self._mysql_database, safe_identifier_length(table_name)),
+        )
+        if len(self._mysql_cur.fetchall()) > 0:
+            self._logger.info("Truncating table %s", safe_identifier_length(table_name))
+            self._mysql_cur.execute(f"TRUNCATE TABLE `{safe_identifier_length(table_name)}`")
+
+    def _add_indices(self, table_name: str) -> None:
+        self._sqlite_cur.execute(f'PRAGMA table_info("{table_name}")')
+        table_columns: t.Dict[str, str] = {}
         for row in self._sqlite_cur.fetchall():
-            column = dict(row)
+            column: t.Dict[str, t.Any] = dict(row)
             table_columns[column["name"]] = column["type"]
 
-        self._sqlite_cur.execute('PRAGMA index_list("{}")'.format(table_name))
-        indices = tuple(dict(row) for row in self._sqlite_cur.fetchall())
+        self._sqlite_cur.execute(f'PRAGMA index_list("{table_name}")')
+        indices: t.Tuple[t.Dict[str, t.Any], ...] = tuple(dict(row) for row in self._sqlite_cur.fetchall())
 
         for index in indices:
             if index["origin"] == "pk":
                 continue
 
-            self._sqlite_cur.execute('PRAGMA index_info("{}")'.format(index["name"]))
-            index_infos = tuple(dict(row) for row in self._sqlite_cur.fetchall())
+            self._sqlite_cur.execute(f'PRAGMA index_info("{index["name"]}")')
+            index_infos: t.Tuple[t.Dict[str, t.Any], ...] = tuple(dict(row) for row in self._sqlite_cur.fetchall())
 
-            index_type = "UNIQUE" if int(index["unique"]) == 1 else "INDEX"
+            index_type: str = "UNIQUE" if int(index["unique"]) == 1 else "INDEX"
 
             if any(
-                table_columns[index_info["name"]].upper() == "TEXT"
+                table_columns[index_info["name"]].upper() in MYSQL_TEXT_COLUMN_TYPES_WITH_JSON
                 for index_info in index_infos
             ):
                 if self._use_fulltext and self._mysql_fulltext_support:
                     # Use fulltext if requested and available
                     index_type = "FULLTEXT"
-                    index_columns = ",".join(
-                        "`{}`".format(safe_identifier_length(index_info["name"]))
-                        for index_info in index_infos
+                    index_columns: str = ",".join(
+                        f'`{safe_identifier_length(index_info["name"])}`' for index_info in index_infos
                     )
                 else:
                     # Limit the max TEXT field index length to 255
                     index_columns = ", ".join(
                         "`{column}`{length}".format(
                             column=safe_identifier_length(index_info["name"]),
-                            length="({})".format(255)
-                            if table_columns[index_info["name"]].upper() == "TEXT"
+                            length="(255)"
+                            if table_columns[index_info["name"]].upper() in MYSQL_TEXT_COLUMN_TYPES_WITH_JSON
                             else "",
                         )
                         for index_info in index_infos
                     )
             else:
-                column_list = []
+                column_list: t.List[str] = []
                 for index_info in index_infos:
-                    index_length = ""
+                    index_length: str = ""
                     # Limit the max BLOB field index length to 255
-                    if table_columns[index_info["name"]].upper() == "BLOB":
-                        index_length = "({})".format(255)
+                    if table_columns[index_info["name"]].upper() in MYSQL_BLOB_COLUMN_TYPES:
+                        index_length = "(255)"
                     else:
-                        suffix = self.COLUMN_LENGTH_PATTERN.search(
+                        suffix: t.Optional[t.Match[str]] = self.COLUMN_LENGTH_PATTERN.search(
                             table_columns[index_info["name"]]
                         )
                         if suffix:
                             index_length = suffix.group(0)
-                    column_list.append(
-                        "`{column}`{length}".format(
-                            column=safe_identifier_length(index_info["name"]),
-                            length=index_length,
-                        )
-                    )
+                    column_list.append(f'`{safe_identifier_length(index_info["name"])}`{index_length}')
                 index_columns = ", ".join(column_list)
 
             try:
                 self._add_index(
                     table_name=table_name,
                     index_type=index_type,
                     index=index,
@@ -431,100 +458,102 @@
                     self._add_index(
                         table_name=table_name,
                         index_type="UNIQUE" if int(index["unique"]) == 1 else "INDEX",
                         index=index,
                         index_columns=", ".join(
                             "`{column}`{length}".format(
                                 column=safe_identifier_length(index_info["name"]),
-                                length="({})".format(255)
-                                if table_columns[index_info["name"]].upper() == "TEXT"
+                                length="(255)"
+                                if table_columns[index_info["name"]].upper() in MYSQL_TEXT_COLUMN_TYPES_WITH_JSON
                                 else "",
                             )
                             for index_info in index_infos
                         ),
                         index_infos=index_infos,
                     )
                 else:
                     raise
 
     def _add_index(
         self,
-        table_name,
-        index_type,
-        index,
-        index_columns,
-        index_infos,
-        index_iteration=0,
-    ):
-        sql = """
+        table_name: str,
+        index_type: str,
+        index: t.Dict[str, t.Any],
+        index_columns: str,
+        index_infos: t.Tuple[t.Dict[str, t.Any], ...],
+        index_iteration: int = 0,
+    ) -> None:
+        sql: str = """
             ALTER TABLE `{table}`
             ADD {index_type} `{name}`({columns})
         """.format(
             table=safe_identifier_length(table_name),
             index_type=index_type,
             name=safe_identifier_length(index["name"])
             if index_iteration == 0
-            else "{name}_{index_iteration}".format(
-                name=safe_identifier_length(index["name"], max_length=60),
-                index_iteration=index_iteration,
-            ),
+            else f'{safe_identifier_length(index["name"], max_length=60)}_{index_iteration}',
             columns=index_columns,
         )
 
         try:
             self._logger.info(
                 """Adding %s to column "%s" in table %s""",
                 "unique index" if int(index["unique"]) == 1 else "index",
-                ", ".join(
-                    safe_identifier_length(index_info["name"])
-                    for index_info in index_infos
-                ),
+                ", ".join(safe_identifier_length(index_info["name"]) for index_info in index_infos),
                 safe_identifier_length(table_name),
             )
             self._mysql_cur.execute(sql)
             self._mysql.commit()
         except mysql.connector.Error as err:
             if err.errno == errorcode.ER_DUP_KEYNAME:
-                # handle a duplicate key name
-                self._add_index(
-                    table_name=table_name,
-                    index_type=index_type,
-                    index=index,
-                    index_columns=index_columns,
-                    index_infos=index_infos,
-                    index_iteration=index_iteration + 1,
-                )
+                if not self._ignore_duplicate_keys:
+                    # handle a duplicate key name
+                    self._add_index(
+                        table_name=table_name,
+                        index_type=index_type,
+                        index=index,
+                        index_columns=index_columns,
+                        index_infos=index_infos,
+                        index_iteration=index_iteration + 1,
+                    )
+                    self._logger.warning(
+                        """Duplicate key "%s" in table %s detected! Trying to create new key "%s_%s" ...""",
+                        safe_identifier_length(index["name"]),
+                        safe_identifier_length(table_name),
+                        safe_identifier_length(index["name"]),
+                        index_iteration + 1,
+                    )
+                else:
+                    self._logger.warning(
+                        """Ignoring duplicate key "%s" in table %s!""",
+                        safe_identifier_length(index["name"]),
+                        safe_identifier_length(table_name),
+                    )
             elif err.errno == errorcode.ER_BAD_FT_COLUMN:
                 # handle bad FULLTEXT index
                 self._logger.warning(
                     """Failed adding FULLTEXT index to column "%s" in table %s. Retrying without FULLTEXT ...""",
-                    ", ".join(
-                        safe_identifier_length(index_info["name"])
-                        for index_info in index_infos
-                    ),
+                    ", ".join(safe_identifier_length(index_info["name"]) for index_info in index_infos),
                     safe_identifier_length(table_name),
                 )
                 raise
             else:
                 self._logger.error(
                     """MySQL failed adding index to column "%s" in table %s: %s""",
-                    ", ".join(
-                        safe_identifier_length(index_info["name"])
-                        for index_info in index_infos
-                    ),
+                    ", ".join(safe_identifier_length(index_info["name"]) for index_info in index_infos),
                     safe_identifier_length(table_name),
                     err,
                 )
                 raise
 
-    def _add_foreign_keys(self, table_name):
-        self._sqlite_cur.execute('PRAGMA foreign_key_list("{}")'.format(table_name))
+    def _add_foreign_keys(self, table_name: str) -> None:
+        self._sqlite_cur.execute(f'PRAGMA foreign_key_list("{table_name}")')
 
         for row in self._sqlite_cur.fetchall():
-            foreign_key = dict(row)
+            foreign_key: t.Dict[str, t.Any] = dict(row)
             sql = """
                 ALTER TABLE `{table}`
                 ADD CONSTRAINT `{table}_FK_{id}_{seq}`
                 FOREIGN KEY (`{column}`)
                 REFERENCES `{ref_table}`(`{ref_column}`)
                 ON DELETE {on_delete}
                 ON UPDATE {on_update}
@@ -560,53 +589,46 @@
                     safe_identifier_length(foreign_key["from"]),
                     safe_identifier_length(foreign_key["table"]),
                     safe_identifier_length(foreign_key["to"]),
                     err,
                 )
                 raise
 
-    def _transfer_table_data(self, sql, total_records=0):
+    def _transfer_table_data(self, sql: str, total_records: int = 0) -> None:
         if self._chunk_size is not None and self._chunk_size > 0:
-            for _ in trange(
-                0, int(ceil(total_records / self._chunk_size)), disable=self._quiet
-            ):
+            for _ in trange(0, int(ceil(total_records / self._chunk_size)), disable=self._quiet):
                 self._mysql_cur.executemany(
                     sql,
-                    (
-                        tuple(row)
-                        for row in self._sqlite_cur.fetchmany(self._chunk_size)
-                    ),
+                    (tuple(row) for row in self._sqlite_cur.fetchmany(self._chunk_size)),  # type: ignore
                 )
         else:
             self._mysql_cur.executemany(
                 sql,
-                (
+                (  # type: ignore
                     tuple(row)
                     for row in tqdm(
                         self._sqlite_cur.fetchall(),
                         total=total_records,
                         disable=self._quiet,
                     )
                 ),
             )
         self._mysql.commit()
 
-    def transfer(self):
+    def transfer(self) -> None:
         """The primary and only method with which we transfer all the data."""
         if len(self._sqlite_tables) > 0:
             # transfer only specific tables
             self._sqlite_cur.execute(
-                """
+                f"""
                 SELECT name FROM sqlite_master
                 WHERE type='table'
                 AND name NOT LIKE 'sqlite_%'
-                AND name IN({placeholders})
-                """.format(
-                    placeholders=("?, " * len(self._sqlite_tables)).rstrip(" ,")
-                ),
+                AND name IN({("?, " * len(self._sqlite_tables)).rstrip(" ,")})
+                """,
                 self._sqlite_tables,
             )
         else:
             # transfer all tables
             self._sqlite_cur.execute(
                 """
                 SELECT name FROM sqlite_master
@@ -614,55 +636,68 @@
                 AND name NOT LIKE 'sqlite_%'
                 """
             )
         try:
             self._mysql_cur.execute("SET FOREIGN_KEY_CHECKS=0")
 
             for row in self._sqlite_cur.fetchall():
-                table = dict(row)
+                table: t.Dict[str, t.Any] = dict(row)
 
                 # check if we're transferring rowid
-                transfer_rowid = self._with_rowid and self._sqlite_table_has_rowid(
-                    table["name"]
-                )
+                transfer_rowid: bool = self._with_rowid and self._sqlite_table_has_rowid(table["name"])
 
                 # create the table
                 self._create_table(table["name"], transfer_rowid=transfer_rowid)
 
+                # truncate the table on request
+                if self._mysql_truncate_tables:
+                    self._truncate_table(table["name"])
+
                 # get the size of the data
-                self._sqlite_cur.execute(
-                    'SELECT COUNT(*) AS total_records FROM "{}"'.format(table["name"])
-                )
+                self._sqlite_cur.execute(f'SELECT COUNT(*) AS total_records FROM "{table["name"]}"')
                 total_records = int(dict(self._sqlite_cur.fetchone())["total_records"])
 
                 # only continue if there is anything to transfer
                 if total_records > 0:
                     # populate it
                     self._logger.info("Transferring table %s", table["name"])
                     self._sqlite_cur.execute(
-                        """
-                        SELECT {rowid} * FROM "{table_name}"
-                    """.format(
+                        '''SELECT {rowid} * FROM "{table_name}"'''.format(
                             rowid='rowid as "rowid",' if transfer_rowid else "",
                             table_name=table["name"],
                         )
                     )
-                    columns = [
-                        safe_identifier_length(column[0])
-                        for column in self._sqlite_cur.description
+                    columns: t.List[str] = [
+                        safe_identifier_length(column[0]) for column in self._sqlite_cur.description
                     ]
-                    sql = """
-                        INSERT IGNORE
-                        INTO `{table}` ({fields})
-                        VALUES ({placeholders})
-                    """.format(
-                        table=safe_identifier_length(table["name"]),
-                        fields=("`{}`, " * len(columns)).rstrip(" ,").format(*columns),
-                        placeholders=("%s, " * len(columns)).rstrip(" ,"),
-                    )
+                    if self._mysql_insert_method.upper() == "UPDATE":
+                        sql: str = """
+                            INSERT
+                            INTO `{table}` ({fields})
+                            VALUES ({placeholders}) AS `__new__`
+                            ON DUPLICATE KEY UPDATE {field_updates}
+                        """.format(
+                            table=safe_identifier_length(table["name"]),
+                            fields=("`{}`, " * len(columns)).rstrip(" ,").format(*columns),
+                            placeholders=("%s, " * len(columns)).rstrip(" ,"),
+                            field_updates=("`{}`=`__new__`.`{}`, " * len(columns))
+                            .rstrip(" ,")
+                            .format(*list(chain.from_iterable((column, column) for column in columns))),
+                        )
+                    else:
+                        sql = """
+                            INSERT {ignore}
+                            INTO `{table}` ({fields})
+                            VALUES ({placeholders})
+                        """.format(
+                            ignore="IGNORE" if self._mysql_insert_method.upper() == "IGNORE" else "",
+                            table=safe_identifier_length(table["name"]),
+                            fields=("`{}`, " * len(columns)).rstrip(" ,").format(*columns),
+                            placeholders=("%s, " * len(columns)).rstrip(" ,"),
+                        )
                     try:
                         self._transfer_table_data(sql=sql, total_records=total_records)
                     except mysql.connector.Error as err:
                         self._logger.error(
                             "MySQL transfer failed inserting data into table %s: %s",
                             safe_identifier_length(table["name"]),
                             err,
```

### Comparing `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/PKG-INFO` & `sqlite3_to_mysql-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 Metadata-Version: 2.1
 Name: sqlite3-to-mysql
-Version: 1.4.9
+Version: 2.0.0
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
-Home-page: https://github.com/techouse/sqlite3-to-mysql
-Author: Klemen Tusar
-Author-email: techouse@gmail.com
-License: MIT
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
-Platform: UNKNOWN
+Author-email: Klemen Tusar <techouse@gmail.com>
+License: MIT
+License-File: LICENSE
+Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
+Requires-Dist: click>=8.1.3
+Requires-Dist: mysql-connector-python>=8.0.33
+Requires-Dist: packaging>=23.1
+Requires-Dist: pytimeparse2
+Requires-Dist: simplejson>=3.19.1
+Requires-Dist: tabulate
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: typing-extensions
+Requires-Dist: unidecode>=1.3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/sqlite3-to-mysql)](https://pypi.org/project/sqlite3-to-mysql/)
 [![Downloads](https://pepy.tech/badge/sqlite3-to-mysql)](https://pepy.tech/project/sqlite3-to-mysql)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlite3-to-mysql)](https://pypi.org/project/sqlite3-to-mysql/)
 [![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
-[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
+[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6|+10.11&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
 [![GitHub license](https://img.shields.io/github/license/techouse/sqlite3-to-mysql)](https://github.com/techouse/sqlite3-to-mysql/blob/master/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/d33b59d35b924711aae9418741a923ae)](https://www.codacy.com/manual/techouse/sqlite3-to-mysql?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/sqlite3-to-mysql&amp;utm_campaign=Badge_Grade)
 [![Build Status](https://github.com/techouse/sqlite3-to-mysql/workflows/Test/badge.svg)](https://github.com/techouse/sqlite3-to-mysql/actions?query=workflow%3ATest)
 [![codecov](https://codecov.io/gh/techouse/sqlite3-to-mysql/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/sqlite3-to-mysql)
 [![GitHub stars](https://img.shields.io/github/stars/techouse/sqlite3-to-mysql.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/sqlite3-to-mysql/stargazers)
@@ -65,39 +69,53 @@
 ### Usage
 ```
 Usage: sqlite3mysql [OPTIONS]
 
   Transfer SQLite to MySQL using the provided CLI options.
 
 Options:
-  -f, --sqlite-file PATH       SQLite3 database file  [required]
-  -t, --sqlite-tables TUPLE    Transfer only these specific tables (space
-                               separated table names). Implies --without-
-                               foreign-keys which inhibits the transfer of
-                               foreign keys.
-  -X, --without-foreign-keys   Do not transfer foreign keys.
-  -d, --mysql-database TEXT    MySQL database name  [required]
-  -u, --mysql-user TEXT        MySQL user  [required]
-  -p, --prompt-mysql-password  Prompt for MySQL password
-  --mysql-password TEXT        MySQL password
-  -h, --mysql-host TEXT        MySQL host. Defaults to localhost.
-  -P, --mysql-port INTEGER     MySQL port. Defaults to 3306.
-  -S, --skip-ssl               Disable MySQL connection encryption.
-  --mysql-integer-type TEXT    MySQL default integer field type. Defaults to
-                               INT(11).
-  --mysql-string-type TEXT     MySQL default string field type. Defaults to
-                               VARCHAR(255).
-  --mysql-charset TEXT         MySQL database and table character set
-                               [default: utf8mb4]
-  --mysql-collation TEXT       MySQL database and table collation
-  -T, --use-fulltext           Use FULLTEXT indexes on TEXT columns. Will
-                               throw an error if your MySQL version does not
-                               support InnoDB FULLTEXT indexes!
-  --with-rowid                 Transfer rowid columns.
-  -c, --chunk INTEGER          Chunk reading/writing SQL records
-  -l, --log-file PATH          Log file
-  -q, --quiet                  Quiet. Display only errors.
-  --version                    Show the version and exit.
-  --help                       Show this message and exit.
+  -f, --sqlite-file PATH          SQLite3 database file  [required]
+  -t, --sqlite-tables TUPLE       Transfer only these specific tables (space
+                                  separated table names). Implies --without-
+                                  foreign-keys which inhibits the transfer of
+                                  foreign keys.
+  -X, --without-foreign-keys      Do not transfer foreign keys.
+  -W, --ignore-duplicate-keys     Ignore duplicate keys. The default behavior
+                                  is to create new ones with a numerical
+                                  suffix, e.g. 'exising_key' ->
+                                  'existing_key_1'
+  -d, --mysql-database TEXT       MySQL database name  [required]
+  -u, --mysql-user TEXT           MySQL user  [required]
+  -p, --prompt-mysql-password     Prompt for MySQL password
+  --mysql-password TEXT           MySQL password
+  -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
+  -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
+  -S, --skip-ssl                  Disable MySQL connection encryption.
+  -i, --mysql-insert-method [UPDATE|IGNORE|DEFAULT]
+                                  MySQL insert method. DEFAULT will throw
+                                  errors when encountering duplicate records;
+                                  UPDATE will update existing rows; IGNORE
+                                  will ignore insert errors. Defaults to
+                                  IGNORE.
+  -E, --mysql-truncate-tables     Truncates existing tables before inserting
+                                  data.
+  --mysql-integer-type TEXT       MySQL default integer field type. Defaults
+                                  to INT(11).
+  --mysql-string-type TEXT        MySQL default string field type. Defaults to
+                                  VARCHAR(255).
+  --mysql-text-type [MEDIUMTEXT|TEXT|TINYTEXT|LONGTEXT]
+                                  MySQL default text field type. Defaults to
+                                  TEXT.
+  --mysql-charset TEXT            MySQL database and table character set
+                                  [default: utf8mb4]
+  --mysql-collation TEXT          MySQL database and table collation
+  -T, --use-fulltext              Use FULLTEXT indexes on TEXT columns. Will
+                                  throw an error if your MySQL version does
+                                  not support InnoDB FULLTEXT indexes!
+  --with-rowid                    Transfer rowid columns.
+  -c, --chunk INTEGER             Chunk reading/writing SQL records
+  -l, --log-file PATH             Log file
+  -q, --quiet                     Quiet. Display only errors.
+  --debug                         Debug mode. Will throw exceptions.
+  --version                       Show the version and exit.
+  --help                          Show this message and exit.
 ```
-
-
```

### Comparing `sqlite3-to-mysql-1.4.9/tests/conftest.py` & `sqlite3_to_mysql-2.0.0/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
+import json
 import socket
+import typing as t
 from codecs import open
-from collections import namedtuple
-from contextlib import contextmanager, closing
-from os.path import join, isfile, realpath, dirname, abspath
+from contextlib import contextmanager
+from os.path import abspath, dirname, isfile, join, realpath
+from pathlib import Path
 from time import sleep
 
 import docker
 import mysql.connector
 import pytest
-import six
-import json
+from _pytest._py.path import LocalPath
+from _pytest.config import Config
+from _pytest.config.argparsing import Parser
+from _pytest.legacypath import TempdirFactory
 from click.testing import CliRunner
+from docker import DockerClient
 from docker.errors import NotFound
-from mysql.connector import errorcode
+from docker.models.containers import Container
+from faker import Faker
+from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
+from mysql.connector.pooling import PooledMySQLConnection
 from requests import HTTPError
 from sqlalchemy import create_engine
+from sqlalchemy.engine import Engine
 from sqlalchemy.exc import IntegrityError
+from sqlalchemy.orm import Session
 from sqlalchemy_utils import database_exists, drop_database
 
 from .database import Database
-from .factories import (
-    ArticleFactory,
-    AuthorFactory,
-    ImageFactory,
-    MiscFactory,
-    TagFactory,
-    MediaFactory,
-)
+from .factories import ArticleFactory, AuthorFactory, ImageFactory, MediaFactory, MiscFactory, TagFactory
 
-if six.PY2:
-    from sixeptions import *
 
-
-def pytest_addoption(parser):
+def pytest_addoption(parser: "Parser") -> None:
     parser.addoption(
         "--sqlite-file",
         dest="sqlite_file",
         default=None,
         help="SQLite database file. Defaults to none and generates one internally.",
     )
 
@@ -91,211 +91,157 @@
         default="mysql:latest",
         help="Run the tests against a specific MySQL Docker image. Defaults to mysql:latest. "
         "Check all supported versions here https://hub.docker.com/_/mysql",
     )
 
 
 @pytest.fixture(scope="session", autouse=True)
-def cleanup_hanged_docker_containers():
+def cleanup_hanged_docker_containers() -> None:
     try:
-        client = docker.from_env()
+        client: DockerClient = docker.from_env()
         for container in client.containers.list():
             if container.name == "pytest_sqlite3_to_mysql":
                 container.kill()
                 break
     except Exception:
         pass
 
 
-def pytest_keyboard_interrupt():
+def pytest_keyboard_interrupt() -> None:
     try:
-        client = docker.from_env()
+        client: DockerClient = docker.from_env()
         for container in client.containers.list():
             if container.name == "pytest_sqlite3_to_mysql":
                 container.kill()
                 break
     except Exception:
         pass
 
 
 class Helpers:
     @staticmethod
     @contextmanager
-    def not_raises(exception):
+    def not_raises(exception: t.Type[Exception]) -> t.Generator:
         try:
             yield
         except exception:
-            raise pytest.fail("DID RAISE {0}".format(exception))
+            raise pytest.fail(f"DID RAISE {exception}")
 
     @staticmethod
     @contextmanager
-    def session_scope(db):
+    def session_scope(db: Database) -> t.Generator:
         """Provide a transactional scope around a series of operations."""
-        session = db.Session()
+        session: Session = db.Session()
         try:
             yield session
             session.commit()
         except Exception:
             session.rollback()
             raise
         finally:
             session.close()
 
 
 @pytest.fixture
-def helpers():
+def helpers() -> t.Type[Helpers]:
     return Helpers
 
 
-if six.PY2:
-
-    @pytest.fixture(scope="session")
-    def sqlite_database(pytestconfig, faker, tmpdir_factory):
-        db_file = pytestconfig.getoption("sqlite_file")
-        if db_file:
-            if not isfile(realpath(db_file)):
-                pytest.fail("{} does not exist".format(db_file))
-                raise FileNotFoundError("{} does not exist".format(db_file))
-            return realpath(db_file)
-
-        temp_data_dir = tmpdir_factory.mktemp("data")
-        temp_image_dir = tmpdir_factory.mktemp("images")
-        db_file = temp_data_dir.join("db.sqlite3")
-        db = Database("sqlite:///{}".format(str(db_file)))
-
-        with Helpers.session_scope(db) as session:
-            for _ in range(faker.pyint(min_value=12, max_value=24)):
-                article = ArticleFactory()
-                article.authors.append(AuthorFactory())
-                article.tags.append(TagFactory())
-                article.misc.append(MiscFactory())
-                article.media.append(MediaFactory())
-                for _ in range(faker.pyint(min_value=1, max_value=4)):
-                    article.images.append(
-                        ImageFactory(
-                            path=join(
-                                str(temp_image_dir),
-                                faker.year(),
-                                faker.month(),
-                                faker.day_of_month(),
-                                faker.file_name(extension="jpg"),
-                            )
-                        )
-                    )
-                session.add(article)
-            try:
-                session.commit()
-            except IntegrityError:
-                session.rollback()
-
-        return str(db_file)
-
-
-else:
-
-    @pytest.fixture(scope="session")
-    def sqlite_database(pytestconfig, _session_faker, tmpdir_factory):
-        db_file = pytestconfig.getoption("sqlite_file")
-        if db_file:
-            if not isfile(realpath(db_file)):
-                pytest.fail("{} does not exist".format(db_file))
-                raise FileNotFoundError("{} does not exist".format(db_file))
-            return realpath(db_file)
-
-        temp_data_dir = tmpdir_factory.mktemp("data")
-        temp_image_dir = tmpdir_factory.mktemp("images")
-        db_file = temp_data_dir.join("db.sqlite3")
-        db = Database("sqlite:///{}".format(str(db_file)))
-
-        with Helpers.session_scope(db) as session:
-            for _ in range(_session_faker.pyint(min_value=12, max_value=24)):
-                article = ArticleFactory()
-                article.authors.append(AuthorFactory())
-                article.tags.append(TagFactory())
-                article.misc.append(MiscFactory())
-                article.media.append(MediaFactory())
-                for _ in range(_session_faker.pyint(min_value=1, max_value=4)):
-                    article.images.append(
-                        ImageFactory(
-                            path=join(
-                                str(temp_image_dir),
-                                _session_faker.year(),
-                                _session_faker.month(),
-                                _session_faker.day_of_month(),
-                                _session_faker.file_name(extension="jpg"),
-                            )
+@pytest.fixture(scope="session")
+def sqlite_database(pytestconfig: Config, _session_faker: Faker, tmpdir_factory: TempdirFactory) -> str:
+    db_file: LocalPath = pytestconfig.getoption("sqlite_file")
+    if db_file:
+        if not isfile(realpath(db_file)):
+            pytest.fail(f"{db_file} does not exist")
+        return str(realpath(db_file))
+
+    temp_data_dir: LocalPath = tmpdir_factory.mktemp("data")
+    temp_image_dir: LocalPath = tmpdir_factory.mktemp("images")
+    db_file = temp_data_dir.join(Path("db.sqlite3"))
+    db: Database = Database(f"sqlite:///{db_file}")
+
+    with Helpers.session_scope(db) as session:
+        for _ in range(_session_faker.pyint(min_value=12, max_value=24)):
+            article = ArticleFactory()
+            article.authors.append(AuthorFactory())
+            article.tags.append(TagFactory())
+            article.misc.append(MiscFactory())
+            article.media.append(MediaFactory())
+            for _ in range(_session_faker.pyint(min_value=1, max_value=4)):
+                article.images.append(
+                    ImageFactory(
+                        path=join(
+                            str(temp_image_dir),
+                            _session_faker.year(),
+                            _session_faker.month(),
+                            _session_faker.day_of_month(),
+                            _session_faker.file_name(extension="jpg"),
                         )
                     )
-                session.add(article)
-            try:
-                session.commit()
-            except IntegrityError:
-                session.rollback()
+                )
+            session.add(article)
+        try:
+            session.commit()
+        except IntegrityError:
+            session.rollback()
 
-        return str(db_file)
+    return str(db_file)
 
 
-def is_port_in_use(port, host="0.0.0.0"):
-    if six.PY2:
-        with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
-            return s.connect_ex((host, port)) == 0
-    else:
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-            return s.connect_ex((host, port)) == 0
+def is_port_in_use(port: int, host: str = "0.0.0.0") -> bool:
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        return s.connect_ex((host, port)) == 0
 
 
-@pytest.fixture(scope="session")
-def mysql_credentials(pytestconfig):
-    MySQLCredentials = namedtuple(
-        "MySQLCredentials", ["user", "password", "host", "port", "database"]
-    )
+class MySQLCredentials(t.NamedTuple):
+    """MySQL credentials."""
 
-    db_credentials_file = abspath(join(dirname(__file__), "db_credentials.json"))
+    user: str
+    password: str
+    host: str
+    port: int
+    database: str
+
+
+@pytest.fixture(scope="session")
+def mysql_credentials(pytestconfig: Config) -> MySQLCredentials:
+    db_credentials_file: str = abspath(join(dirname(__file__), "db_credentials.json"))
     if isfile(db_credentials_file):
         with open(db_credentials_file, "r", "utf-8") as fh:
-            db_credentials = json.load(fh)
+            db_credentials: t.Dict[str, t.Any] = json.load(fh)
             return MySQLCredentials(
                 user=db_credentials["mysql_user"],
                 password=db_credentials["mysql_password"],
                 database=db_credentials["mysql_database"],
                 host=db_credentials["mysql_host"],
                 port=db_credentials["mysql_port"],
             )
 
-    port = pytestconfig.getoption("mysql_port") or 3306
+    port: int = pytestconfig.getoption("mysql_port") or 3306
     if pytestconfig.getoption("use_docker"):
         while is_port_in_use(port, pytestconfig.getoption("mysql_host")):
-            if port >= 2 ** 16 - 1:
-                pytest.fail(
-                    "No ports appear to be available on the host {}".format(
-                        pytestconfig.getoption("mysql_host")
-                    )
-                )
-                raise ConnectionError(
-                    "No ports appear to be available on the host {}".format(
-                        pytestconfig.getoption("mysql_host")
-                    )
-                )
+            if port >= 2**16 - 1:
+                pytest.fail(f'No ports appear to be available on the host {pytestconfig.getoption("mysql_host")}')
             port += 1
 
     return MySQLCredentials(
         user=pytestconfig.getoption("mysql_user") or "tester",
         password=pytestconfig.getoption("mysql_password") or "testpass",
         database=pytestconfig.getoption("mysql_database") or "test_db",
         host=pytestconfig.getoption("mysql_host") or "0.0.0.0",
         port=port,
     )
 
 
 @pytest.fixture(scope="session")
-def mysql_instance(mysql_credentials, pytestconfig):
-    container = None
-    mysql_connection = None
-    mysql_available = False
-    mysql_connection_retries = 15  # failsafe
+def mysql_instance(mysql_credentials: MySQLCredentials, pytestconfig: Config) -> t.Iterator[MySQLConnection]:
+    container: t.Optional[Container] = None
+    mysql_connection: t.Optional[t.Union[PooledMySQLConnection, MySQLConnection, CMySQLConnection]] = None
+    mysql_available: bool = False
+    mysql_connection_retries: int = 15  # failsafe
 
     db_credentials_file = abspath(join(dirname(__file__), "db_credentials.json"))
     if isfile(db_credentials_file):
         use_docker = False
     else:
         use_docker = pytestconfig.getoption("use_docker")
 
@@ -303,35 +249,31 @@
         """Connecting to a MySQL server within a Docker container is quite tricky :P
         Read more on the issue here https://hub.docker.com/_/mysql#no-connections-until-mysql-init-completes
         """
         try:
             client = docker.from_env()
         except Exception as err:
             pytest.fail(str(err))
-            raise
 
-        docker_mysql_image = (
-            pytestconfig.getoption("docker_mysql_image") or "mysql:latest"
-        )
+        docker_mysql_image = pytestconfig.getoption("docker_mysql_image") or "mysql:latest"
 
         if not any(docker_mysql_image in image.tags for image in client.images.list()):
-            print("Attempting to download Docker image {}'".format(docker_mysql_image))
+            print(f"Attempting to download Docker image {docker_mysql_image}'")
             try:
                 client.images.pull(docker_mysql_image)
             except (HTTPError, NotFound) as err:
                 pytest.fail(str(err))
-                raise
 
         container = client.containers.run(
             image=docker_mysql_image,
             name="pytest_sqlite3_to_mysql",
             ports={
                 "3306/tcp": (
                     mysql_credentials.host,
-                    "{}/tcp".format(mysql_credentials.port),
+                    f"{mysql_credentials.port}/tcp",
                 )
             },
             environment={
                 "MYSQL_RANDOM_ROOT_PASSWORD": "yes",
                 "MYSQL_USER": mysql_credentials.user,
                 "MYSQL_PASSWORD": mysql_credentials.password,
                 "MYSQL_DATABASE": mysql_credentials.database,
@@ -361,38 +303,30 @@
         finally:
             mysql_connection_retries -= 1
             if mysql_connection and mysql_connection.is_connected():
                 mysql_available = True
                 mysql_connection.close()
     else:
         if not mysql_available and mysql_connection_retries <= 0:
-            raise ConnectionAbortedError(
-                "Maximum MySQL connection retries exhausted! Are you sure MySQL is running?"
-            )
+            raise ConnectionAbortedError("Maximum MySQL connection retries exhausted! Are you sure MySQL is running?")
 
-    yield
+    yield  # type: ignore[misc]
 
-    if use_docker:
+    if use_docker and container is not None:
         container.kill()
 
 
 @pytest.fixture()
-def mysql_database(mysql_instance, mysql_credentials):
-    yield
+def mysql_database(mysql_instance: t.Generator, mysql_credentials: MySQLCredentials) -> t.Iterator[Engine]:
+    yield  # type: ignore[misc]
 
-    engine = create_engine(
-        "mysql+pymysql://{user}:{password}@{host}:{port}/{database}".format(
-            user=mysql_credentials.user,
-            password=mysql_credentials.password,
-            host=mysql_credentials.host,
-            port=mysql_credentials.port,
-            database=mysql_credentials.database,
-        )
+    engine: Engine = create_engine(
+        f"mysql+pymysql://{mysql_credentials.user}:{mysql_credentials.password}@{mysql_credentials.host}:{mysql_credentials.port}/{mysql_credentials.database}"
     )
 
     if database_exists(engine.url):
         drop_database(engine.url)
 
 
 @pytest.fixture()
-def cli_runner():
+def cli_runner() -> t.Iterator[CliRunner]:
     yield CliRunner()
```

### Comparing `sqlite3-to-mysql-1.4.9/tests/database.py` & `sqlite3_to_mysql-2.0.0/tests/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,42 @@
+import typing as t
 from datetime import datetime, timedelta
 from decimal import Decimal
 
 import simplejson as json
 from sqlalchemy import create_engine
+from sqlalchemy.engine import Engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy_utils import database_exists
 
 from .models import Base
 
 
 class Database:
-    engine = None
-    Session = None
+    engine: Engine
+    Session: sessionmaker
 
     def __init__(self, database_uri):
         self.Session = sessionmaker()
-        self.engine = create_engine(
-            database_uri, json_serializer=self.dumps, json_deserializer=json.loads
-        )
+        self.engine = create_engine(database_uri, json_serializer=self.dumps, json_deserializer=json.loads)
         if not database_exists(database_uri):
             self._create_db_tables()
         self.Session.configure(bind=self.engine)
 
-    def _create_db_tables(self):
+    def _create_db_tables(self) -> None:
         Base.metadata.create_all(self.engine)
 
     @classmethod
-    def dumps(cls, data):
+    def dumps(cls, data: t.Any) -> str:
         return json.dumps(data, default=cls.json_serializer)
 
     @staticmethod
-    def json_serializer(data):
+    def json_serializer(data: t.Any) -> t.Optional[str]:
         if isinstance(data, datetime):
             return data.isoformat()
         if isinstance(data, Decimal):
             return str(data)
         if isinstance(data, timedelta):
             hours, remainder = divmod(data.total_seconds(), 3600)
             minutes, seconds = divmod(remainder, 60)
             return "{:02}:{:02}:{:02}".format(int(hours), int(minutes), int(seconds))
+        return None
```

### Comparing `sqlite3-to-mysql-1.4.9/tests/factories.py` & `sqlite3_to_mysql-2.0.0/tests/factories.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,80 @@
+import typing as t
 from os import environ
 
 import factory
-import six
+from factory import Faker
 
 from . import models
+from .models import Article, Author, Image, Media, Misc, Tag
 
 
 class AuthorFactory(factory.Factory):
     class Meta:
-        model = models.Author
+        model: t.Type[Author] = models.Author
 
-    name = factory.Faker("name")
+    name: Faker = factory.Faker("name")
 
 
 class ImageFactory(factory.Factory):
     class Meta:
-        model = models.Image
+        model: t.Type[Image] = models.Image
 
-    path = factory.Faker("file_path", depth=3, extension="jpg")
-    description = factory.Faker("sentence", nb_words=12, variable_nb_words=True)
+    path: Faker = factory.Faker("file_path", depth=3, extension="jpg")
+    description: Faker = factory.Faker("sentence", nb_words=12, variable_nb_words=True)
 
 
 class TagFactory(factory.Factory):
     class Meta:
-        model = models.Tag
+        model: t.Type[Tag] = models.Tag
 
-    name = factory.Faker("sentence", nb_words=3, variable_nb_words=True)
+    name: Faker = factory.Faker("sentence", nb_words=3, variable_nb_words=True)
 
 
 class MiscFactory(factory.Factory):
     class Meta:
-        model = models.Misc
+        model: t.Type[Misc] = models.Misc
 
-    big_integer_field = factory.Faker("pyint", max_value=10 ** 9)
-    blob_field = factory.Faker("binary", length=1024 * 10)
-    boolean_field = factory.Faker("boolean")
-    char_field = factory.Faker("text", max_nb_chars=255)
-    date_field = factory.Faker("date_this_decade")
-    date_time_field = factory.Faker("date_time_this_century")
-    decimal_field = factory.Faker("pydecimal", left_digits=8, right_digits=2)
-    float_field = factory.Faker("pyfloat", left_digits=8, right_digits=4)
-    integer_field = factory.Faker("pyint", min_value=-(2 ** 31), max_value=2 ** 31 - 1)
-    if environ.get("LEGACY_DB", "0") == "0" and six.PY3:
+    big_integer_field: Faker = factory.Faker("pyint", max_value=10**9)
+    blob_field: Faker = factory.Faker("binary", length=1024 * 10)
+    boolean_field: Faker = factory.Faker("boolean")
+    char_field: Faker = factory.Faker("text", max_nb_chars=255)
+    date_field: Faker = factory.Faker("date_this_decade")
+    date_time_field: Faker = factory.Faker("date_time_this_century")
+    decimal_field: Faker = factory.Faker("pydecimal", left_digits=8, right_digits=2)
+    float_field: Faker = factory.Faker("pyfloat", left_digits=8, right_digits=4)
+    integer_field: Faker = factory.Faker("pyint", min_value=-(2**31), max_value=2**31 - 1)
+    if environ.get("LEGACY_DB", "0") == "0":
         json_field = factory.Faker(
             "pydict",
             nb_elements=10,
             variable_nb_elements=True,
             value_types=["str", "int", "float", "boolean", "date_time"],
         )
-    numeric_field = factory.Faker("pyfloat", left_digits=8, right_digits=4)
-    real_field = factory.Faker("pyfloat", left_digits=8, right_digits=4)
-    small_integer_field = factory.Faker(
-        "pyint", min_value=-(2 ** 15), max_value=2 ** 15 - 1
-    )
-    string_field = factory.Faker("text", max_nb_chars=255)
-    text_field = factory.Faker("text", max_nb_chars=1024)
-    time_field = factory.Faker("time_object")
-    varchar_field = factory.Faker("text", max_nb_chars=255)
-    timestamp_field = factory.Faker("date_time_this_century")
-    my_type_field = factory.Faker("text", max_nb_chars=255)
+    numeric_field: Faker = factory.Faker("pyfloat", left_digits=8, right_digits=4)
+    real_field: Faker = factory.Faker("pyfloat", left_digits=8, right_digits=4)
+    small_integer_field: Faker = factory.Faker("pyint", min_value=-(2**15), max_value=2**15 - 1)
+    string_field: Faker = factory.Faker("text", max_nb_chars=255)
+    text_field: Faker = factory.Faker("text", max_nb_chars=1024)
+    time_field: Faker = factory.Faker("time_object")
+    varchar_field: Faker = factory.Faker("text", max_nb_chars=255)
+    timestamp_field: Faker = factory.Faker("date_time_this_century")
+    my_type_field: Faker = factory.Faker("text", max_nb_chars=255)
 
 
 class ArticleFactory(factory.Factory):
     class Meta:
-        model = models.Article
+        model: t.Type[Article] = models.Article
 
-    hash = factory.Faker("md5")
-    title = factory.Faker("sentence", nb_words=6)
-    slug = factory.Faker("slug")
-    content = factory.Faker("text", max_nb_chars=1024)
-    status = factory.Faker("pystr", max_chars=1)
-    published = factory.Faker("date_between", start_date="-1y", end_date="-1d")
+    hash: Faker = factory.Faker("md5")
+    title: Faker = factory.Faker("sentence", nb_words=6)
+    slug: Faker = factory.Faker("slug")
+    content: Faker = factory.Faker("text", max_nb_chars=1024)
+    status: Faker = factory.Faker("pystr", max_chars=1)
+    published: Faker = factory.Faker("date_between", start_date="-1y", end_date="-1d")
 
     @factory.post_generation
     def authors(self, create, extracted, **kwargs):
         if not create:
             # Simple build, do nothing.
             return
 
@@ -115,12 +115,12 @@
             # A list of authors were passed in, use them
             for misc in extracted:
                 self.misc.add(misc)
 
 
 class MediaFactory(factory.Factory):
     class Meta:
-        model = models.Media
+        model: t.Type[Media] = models.Media
 
-    id = factory.Faker("sha256", raw_output=False)
-    title = factory.Faker("sentence", nb_words=6)
-    description = factory.Faker("sentence", nb_words=12, variable_nb_words=True)
+    id: Faker = factory.Faker("sha256", raw_output=False)
+    title: Faker = factory.Faker("sentence", nb_words=6)
+    description: Faker = factory.Faker("sentence", nb_words=12, variable_nb_words=True)
```

### Comparing `sqlite3-to-mysql-1.4.9/tests/unit/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.0.0/tests/unit/sqlite3_to_mysql_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,358 +1,329 @@
 import logging
 import re
+import typing as t
 from random import choice
 
 import mysql.connector
 import pytest
+from _pytest.logging import LogCaptureFixture
+from faker import Faker
 from mysql.connector import errorcode
-from sqlalchemy import create_engine, inspect
+from pytest_mock import MockerFixture, MockFixture
+from sqlalchemy import Connection, CursorResult, Engine, Inspector, TextClause, create_engine, inspect, text
 from sqlalchemy.dialects.sqlite import __all__ as sqlite_column_types
 
 from sqlite3_to_mysql import SQLite3toMySQL
+from tests.conftest import MySQLCredentials
 
 
 @pytest.mark.usefixtures("sqlite_database", "mysql_instance")
 class TestSQLite3toMySQL:
     @pytest.mark.parametrize("quiet", [False, True])
     def test_translate_type_from_sqlite_to_mysql_invalid_column_type(
-        self, sqlite_database, mysql_database, mysql_credentials, mocker, quiet
-    ):
-        proc = SQLite3toMySQL(
+        self,
+        sqlite_database: str,
+        mysql_database: Engine,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        quiet: bool,
+    ) -> None:
+        proc: SQLite3toMySQL = SQLite3toMySQL(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             quiet=quiet,
         )
         with pytest.raises(ValueError) as excinfo:
             mocker.patch.object(proc, "_valid_column_type", return_value=False)
             proc._translate_type_from_sqlite_to_mysql("text")
         assert "Invalid column_type!" in str(excinfo.value)
 
     @pytest.mark.parametrize(
-        "mysql_integer_type, mysql_string_type",
+        "mysql_integer_type, mysql_string_type, mysql_text_type",
         [
-            ("INT(11)", "VARCHAR(300)"),
-            ("BIGINT(19)", "TEXT"),
-            ("BIGINT(20) UNSIGNED", "CHAR(100)"),
+            ("INT(11)", "VARCHAR(300)", "TEXT"),
+            ("BIGINT(19)", "TEXT", "MEDIUMTEXT"),
+            ("BIGINT(19)", "MEDIUMTEXT", "TINYTEXT"),
+            ("BIGINT(20) UNSIGNED", "CHAR(100)", "LONGTEXT"),
         ],
     )
     def test_translate_type_from_sqlite_to_mysql_all_valid_columns(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        faker,
-        mysql_integer_type,
-        mysql_string_type,
-    ):
-        proc = SQLite3toMySQL(
+        sqlite_database: str,
+        mysql_database: Engine,
+        mysql_credentials: MySQLCredentials,
+        faker: Faker,
+        mysql_integer_type: str,
+        mysql_string_type: str,
+        mysql_text_type: str,
+    ) -> None:
+        proc: SQLite3toMySQL = SQLite3toMySQL(  # type: ignore
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             mysql_integer_type=mysql_integer_type,
             mysql_string_type=mysql_string_type,
+            mysql_text_type=mysql_text_type,
         )
 
         for column in sqlite_column_types + ("INT64",):
             if column in {"Insert", "insert", "dialect"}:
                 continue
             elif column == "VARCHAR":
-                assert (
-                    proc._translate_type_from_sqlite_to_mysql(column)
-                    == proc._mysql_string_type
-                )
+                assert proc._translate_type_from_sqlite_to_mysql(column) == proc._mysql_string_type
             elif column in {"INTEGER", "INT"}:
-                assert (
-                    proc._translate_type_from_sqlite_to_mysql(column)
-                    == proc._mysql_integer_type
-                )
+                assert proc._translate_type_from_sqlite_to_mysql(column) == proc._mysql_integer_type
             elif column in {"INT64", "NUMERIC"}:
                 assert proc._translate_type_from_sqlite_to_mysql(column) == "BIGINT(19)"
+            elif column in {"TINYTEXT", "TEXT", "MEDIUMTEXT", "LONGTEXT"}:
+                assert proc._translate_type_from_sqlite_to_mysql(column) == proc._mysql_text_type
+            elif column == "BOOLEAN":
+                assert proc._translate_type_from_sqlite_to_mysql(column) == "TINYINT(1)"
             else:
                 assert proc._translate_type_from_sqlite_to_mysql(column) == column
-        assert proc._translate_type_from_sqlite_to_mysql("TEXT") == "TEXT"
-        assert proc._translate_type_from_sqlite_to_mysql("CLOB") == "TEXT"
+        assert proc._translate_type_from_sqlite_to_mysql("TEXT") == proc._mysql_text_type
+        assert proc._translate_type_from_sqlite_to_mysql("CLOB") == proc._mysql_text_type
         assert proc._translate_type_from_sqlite_to_mysql("CHARACTER") == "CHAR"
-        length = faker.pyint(min_value=1, max_value=99)
-        assert proc._translate_type_from_sqlite_to_mysql(
-            "CHARACTER({})".format(length)
-        ) == "CHAR({})".format(length)
+        length: int = faker.pyint(min_value=1, max_value=99)
+        assert proc._translate_type_from_sqlite_to_mysql(f"CHARACTER({length})") == f"CHAR({length})"
         assert proc._translate_type_from_sqlite_to_mysql("NCHAR") == "CHAR"
         length = faker.pyint(min_value=1, max_value=99)
-        assert proc._translate_type_from_sqlite_to_mysql(
-            "NCHAR({})".format(length)
-        ) == "CHAR({})".format(length)
+        assert proc._translate_type_from_sqlite_to_mysql(f"NCHAR({length})") == f"CHAR({length})"
         assert proc._translate_type_from_sqlite_to_mysql("NATIVE CHARACTER") == "CHAR"
         length = faker.pyint(min_value=1, max_value=99)
-        assert proc._translate_type_from_sqlite_to_mysql(
-            "NATIVE CHARACTER({})".format(length)
-        ) == "CHAR({})".format(length)
-        assert (
-            proc._translate_type_from_sqlite_to_mysql("VARCHAR")
-            == proc._mysql_string_type
-        )
+        assert proc._translate_type_from_sqlite_to_mysql(f"NATIVE CHARACTER({length})") == f"CHAR({length})"
+        assert proc._translate_type_from_sqlite_to_mysql("VARCHAR") == proc._mysql_string_type
         length = faker.pyint(min_value=1, max_value=255)
-        assert proc._translate_type_from_sqlite_to_mysql(
-            "VARCHAR({})".format(length)
-        ) == re.sub(r"\d+", str(length), proc._mysql_string_type)
-        assert proc._translate_type_from_sqlite_to_mysql("DOUBLE PRECISION") == "DOUBLE"
-        assert (
-            proc._translate_type_from_sqlite_to_mysql("UNSIGNED BIG INT")
-            == "BIGINT UNSIGNED"
+        assert proc._translate_type_from_sqlite_to_mysql(f"VARCHAR({length})") == re.sub(
+            r"\d+", str(length), proc._mysql_string_type
         )
+        assert proc._translate_type_from_sqlite_to_mysql("DOUBLE PRECISION") == "DOUBLE"
+        assert proc._translate_type_from_sqlite_to_mysql("UNSIGNED BIG INT") == "BIGINT UNSIGNED"
         length = faker.pyint(min_value=1000000000, max_value=99999999999999999999)
-        assert proc._translate_type_from_sqlite_to_mysql(
-            "UNSIGNED BIG INT({})".format(length)
-        ) == "BIGINT({}) UNSIGNED".format(length)
-        assert (
-            proc._translate_type_from_sqlite_to_mysql("INT1")
-            == proc._mysql_integer_type
+        assert proc._translate_type_from_sqlite_to_mysql(f"UNSIGNED BIG INT({length})") == f"BIGINT({length}) UNSIGNED"
+        assert proc._translate_type_from_sqlite_to_mysql("INT1") == proc._mysql_integer_type
+        assert proc._translate_type_from_sqlite_to_mysql("INT2") == proc._mysql_integer_type
+        length = faker.pyint(min_value=1, max_value=11)
+        assert proc._translate_type_from_sqlite_to_mysql(f"INT({length})") == re.sub(
+            r"\d+", str(length), proc._mysql_integer_type
         )
+        for column in {"META", "FOO", "BAR"}:
+            assert proc._translate_type_from_sqlite_to_mysql(column) == proc._mysql_string_type
+        precision: int = faker.pyint(min_value=3, max_value=19)
+        scale: int = faker.pyint(min_value=0, max_value=precision - 1)
         assert (
-            proc._translate_type_from_sqlite_to_mysql("INT2")
-            == proc._mysql_integer_type
+            proc._translate_type_from_sqlite_to_mysql(f"DECIMAL({precision},{scale})")
+            == f"DECIMAL({precision},{scale})"
         )
-        length = faker.pyint(min_value=1, max_value=11)
-        assert proc._translate_type_from_sqlite_to_mysql(
-            "INT({})".format(length)
-        ) == re.sub(r"\d+", str(length), proc._mysql_integer_type)
-        for column in {"META", "FOO", "BAR"}:
-            assert (
-                proc._translate_type_from_sqlite_to_mysql(column)
-                == proc._mysql_string_type
-            )
-        precision = faker.pyint(min_value=3, max_value=19)
-        scale = faker.pyint(min_value=0, max_value=precision - 1)
-        assert proc._translate_type_from_sqlite_to_mysql(
-            "DECIMAL({precision},{scale})".format(precision=precision, scale=scale)
-        ) == "DECIMAL({precision},{scale})".format(precision=precision, scale=scale)
 
     @pytest.mark.parametrize("quiet", [False, True])
     def test_create_database_connection_error(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        mocker,
-        faker,
-        caplog,
-        quiet,
-    ):
-        proc = SQLite3toMySQL(
+        sqlite_database: str,
+        mysql_database: Engine,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        faker: Faker,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc: SQLite3toMySQL = SQLite3toMySQL(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             quiet=quiet,
         )
 
         class FakeCursor:
-            def execute(self, statement):
-                raise mysql.connector.Error(
-                    msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR
-                )
+            def execute(self, statement: t.Any) -> None:
+                raise mysql.connector.Error(msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR)
 
         mocker.patch.object(proc, "_mysql_cur", FakeCursor())
 
         with pytest.raises(mysql.connector.Error) as excinfo:
             caplog.set_level(logging.DEBUG)
             proc._create_database()
         assert str(errorcode.CR_UNKNOWN_ERROR) in str(excinfo.value)
-        assert any(
-            str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages
-        )
+        assert any(str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages)
 
     @pytest.mark.parametrize("quiet", [False, True])
     def test_create_table_cursor_error(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        mocker,
-        faker,
-        caplog,
-        quiet,
-    ):
-        proc = SQLite3toMySQL(
+        sqlite_database: str,
+        mysql_database: Engine,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        faker: Faker,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc = SQLite3toMySQL(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             quiet=quiet,
         )
 
         class FakeCursor:
             def execute(self, statement):
-                raise mysql.connector.Error(
-                    msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR
-                )
+                raise mysql.connector.Error(msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR)
 
         mocker.patch.object(proc, "_mysql_cur", FakeCursor())
 
-        sqlite_engine = create_engine(
-            "sqlite:///{database}".format(database=sqlite_database)
-        )
-        sqlite_inspect = inspect(sqlite_engine)
-        sqlite_tables = sqlite_inspect.get_table_names()
+        sqlite_engine: Engine = create_engine(f"sqlite:///{sqlite_database}")
+        sqlite_inspect: Inspector = inspect(sqlite_engine)
+        sqlite_tables: t.List[str] = sqlite_inspect.get_table_names()
 
         with pytest.raises(mysql.connector.Error) as excinfo:
             caplog.set_level(logging.DEBUG)
             proc._create_table(choice(sqlite_tables))
         assert str(errorcode.CR_UNKNOWN_ERROR) in str(excinfo.value)
-        assert any(
-            str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages
-        )
+        assert any(str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages)
+
+        sqlite_engine.dispose()
 
     @pytest.mark.parametrize("quiet", [False, True])
     def test_process_cursor_error(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        mocker,
-        faker,
-        caplog,
-        quiet,
-    ):
-        proc = SQLite3toMySQL(
+        sqlite_database: str,
+        mysql_database: Engine,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        faker: Faker,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc = SQLite3toMySQL(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             quiet=quiet,
         )
 
         def fake_transfer_table_data(sql, total_records=0):
-            raise mysql.connector.Error(
-                msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR
-            )
+            raise mysql.connector.Error(msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR)
 
         mocker.patch.object(proc, "_transfer_table_data", fake_transfer_table_data)
 
         with pytest.raises(mysql.connector.Error) as excinfo:
             caplog.set_level(logging.DEBUG)
             proc.transfer()
         assert str(errorcode.CR_UNKNOWN_ERROR) in str(excinfo.value)
-        assert any(
-            str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages
-        )
+        assert any(str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages)
 
     @pytest.mark.parametrize("quiet", [False, True])
     def test_add_indices_error(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        mocker,
-        faker,
-        caplog,
-        quiet,
-    ):
-        proc = SQLite3toMySQL(
+        sqlite_database: str,
+        mysql_database: Engine,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        faker: Faker,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc = SQLite3toMySQL(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             quiet=quiet,
         )
 
-        sqlite_engine = create_engine(
-            "sqlite:///{database}".format(database=sqlite_database)
-        )
-        sqlite_inspect = inspect(sqlite_engine)
-        sqlite_tables = sqlite_inspect.get_table_names()
+        sqlite_engine: Engine = create_engine(f"sqlite:///{sqlite_database}")
+        sqlite_inspect: Inspector = inspect(sqlite_engine)
+        sqlite_tables: t.List[str] = sqlite_inspect.get_table_names()
 
-        tables_with_indices = []
+        tables_with_indices: t.List[str] = []
         for table in sqlite_tables:
             if sqlite_inspect.get_indexes(table):
                 tables_with_indices.append(table)
 
-        table_name = choice(tables_with_indices)
+        table_name: str = choice(tables_with_indices)
         proc._create_table(table_name)
 
         class FakeCursor:
             def execute(self, statement):
-                raise mysql.connector.Error(
-                    msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR
-                )
+                raise mysql.connector.Error(msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR)
 
         mocker.patch.object(proc, "_mysql_cur", FakeCursor())
 
         with pytest.raises(mysql.connector.Error) as excinfo:
             caplog.set_level(logging.DEBUG)
             proc._add_indices(table_name)
         assert str(errorcode.CR_UNKNOWN_ERROR) in str(excinfo.value)
-        assert any(
-            str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages
-        )
+        assert any(str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages)
+
+        sqlite_engine.dispose()
 
     @pytest.mark.parametrize("quiet", [False, True])
     def test_add_foreign_keys_error(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        mocker,
-        faker,
-        caplog,
-        quiet,
-    ):
-        proc = SQLite3toMySQL(
+        sqlite_database: str,
+        mysql_database: Engine,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockFixture,
+        faker: Faker,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc = SQLite3toMySQL(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             quiet=quiet,
         )
 
-        sqlite_engine = create_engine(
-            "sqlite:///{database}".format(database=sqlite_database)
-        )
-        sqlite_inspect = inspect(sqlite_engine)
-        sqlite_tables = sqlite_inspect.get_table_names()
+        sqlite_engine: Engine = create_engine(f"sqlite:///{sqlite_database}")
+        sqlite_inspect: Inspector = inspect(sqlite_engine)
+        sqlite_cnx: Connection = sqlite_engine.connect()
+        sqlite_tables: t.List[str] = sqlite_inspect.get_table_names()
 
-        tables_with_foreign_keys = []
+        tables_with_foreign_keys: t.List[str] = []
 
         for table in sqlite_tables:
-            sqlite_fk_stmt = 'PRAGMA foreign_key_list("{table}")'.format(table=table)
-            sqlite_fk_result = sqlite_engine.execute(sqlite_fk_stmt)
+            sqlite_fk_stmt: TextClause = text(f'PRAGMA foreign_key_list("{table}")')
+            sqlite_fk_result: CursorResult[t.Any] = sqlite_cnx.execute(sqlite_fk_stmt)
             if sqlite_fk_result.returns_rows:
                 for _ in sqlite_fk_result:
                     tables_with_foreign_keys.append(table)
                     break
 
-        table_name = choice(tables_with_foreign_keys)
+        table_name: str = choice(tables_with_foreign_keys)
 
         proc._create_table(table_name)
 
         class FakeCursor:
             def execute(self, statement):
-                raise mysql.connector.Error(
-                    msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR
-                )
+                raise mysql.connector.Error(msg="Unknown MySQL error", errno=errorcode.CR_UNKNOWN_ERROR)
 
         mocker.patch.object(proc, "_mysql_cur", FakeCursor())
 
         with pytest.raises(mysql.connector.Error) as excinfo:
             caplog.set_level(logging.DEBUG)
             proc._add_foreign_keys(table_name)
         assert str(errorcode.CR_UNKNOWN_ERROR) in str(excinfo.value)
-        assert any(
-            str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages
-        )
+        assert any(str(errorcode.CR_UNKNOWN_ERROR) in message for message in caplog.messages)
+
+        sqlite_cnx.close()
+        sqlite_engine.dispose()
```

