# Comparing `tmp/dvc-data-1.1.0.tar.gz` & `tmp/dvc-data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-data-1.1.0.tar", last modified: Fri Jun  9 23:55:01 2023, max compression
+gzip compressed data, was "dvc-data-1.2.0.tar", last modified: Sat Jun 10 18:24:09 2023, max compression
```

## Comparing `dvc-data-1.1.0.tar` & `dvc-data-1.2.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.005544 dvc-data-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:00.997544 dvc-data-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:00.997544 dvc-data-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-09 23:54:37.000000 dvc-data-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-09 23:54:37.000000 dvc-data-1.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-09 23:54:37.000000 dvc-data-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-09 23:54:37.000000 dvc-data-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 23:55:01.005544 dvc-data-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-09 23:54:37.000000 dvc-data-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-09 23:54:37.000000 dvc-data-1.1.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-09 23:54:37.000000 dvc-data-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-09 23:55:01.005544 dvc-data-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:00.993544 dvc-data-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:00.997544 dvc-data-1.1.0/src/dvc_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.001544 dvc-data-1.1.0/src/dvc_data/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.001544 dvc-data-1.1.0/src/dvc_data/hashfile/db/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/db/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/db/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/db/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/hash_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/hashfile/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.001544 dvc-data-1.1.0/src/dvc_data/index/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/index/view.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-09 23:54:37.000000 dvc-data-1.1.0/src/dvc_data/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:00.997544 dvc-data-1.1.0/src/dvc_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 23:55:00.000000 dvc-data-1.1.0/src/dvc_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-09 23:55:00.000000 dvc-data-1.1.0/src/dvc_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:55:00.000000 dvc-data-1.1.0/src/dvc_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 23:55:00.000000 dvc-data-1.1.0/src/dvc_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:55:00.000000 dvc-data-1.1.0/src/dvc_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-09 23:55:00.000000 dvc-data-1.1.0/src/dvc_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 23:55:00.000000 dvc-data-1.1.0/src/dvc_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.001544 dvc-data-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.001544 dvc-data-1.1.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/benchmarks/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.005544 dvc-data-1.1.0/tests/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_db_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_hash_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/hashfile/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:55:01.005544 dvc-data-1.1.0/tests/index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/index/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/index/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/index/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/index/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 23:54:37.000000 dvc-data-1.1.0/tests/test_dvc_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.511908 dvc-data-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.503908 dvc-data-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.503908 dvc-data-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-10 18:23:47.000000 dvc-data-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-10 18:23:47.000000 dvc-data-1.2.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-10 18:23:47.000000 dvc-data-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-10 18:23:47.000000 dvc-data-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-10 18:24:09.511908 dvc-data-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-10 18:23:47.000000 dvc-data-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-10 18:23:47.000000 dvc-data-1.2.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-10 18:23:47.000000 dvc-data-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-10 18:24:09.511908 dvc-data-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.503908 dvc-data-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.507908 dvc-data-1.2.0/src/dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.507908 dvc-data-1.2.0/src/dvc_data/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.507908 dvc-data-1.2.0/src/dvc_data/hashfile/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/db/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/db/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/db/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/hash_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/hashfile/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.511908 dvc-data-1.2.0/src/dvc_data/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/index/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-10 18:23:47.000000 dvc-data-1.2.0/src/dvc_data/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.507908 dvc-data-1.2.0/src/dvc_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-10 18:24:09.000000 dvc-data-1.2.0/src/dvc_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-10 18:24:09.000000 dvc-data-1.2.0/src/dvc_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:24:09.000000 dvc-data-1.2.0/src/dvc_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 18:24:09.000000 dvc-data-1.2.0/src/dvc_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:24:09.000000 dvc-data-1.2.0/src/dvc_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-10 18:24:09.000000 dvc-data-1.2.0/src/dvc_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 18:24:09.000000 dvc-data-1.2.0/src/dvc_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.511908 dvc-data-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.511908 dvc-data-1.2.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/benchmarks/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.511908 dvc-data-1.2.0/tests/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_db_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_hash_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/hashfile/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:24:09.511908 dvc-data-1.2.0/tests/index/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/index/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/index/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/index/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/index/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 18:23:47.000000 dvc-data-1.2.0/tests/test_dvc_data.py
```

### Comparing `dvc-data-1.1.0/.cruft.json` & `dvc-data-1.2.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/.github/dependabot.yml` & `dvc-data-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/.github/workflows/benchmark.yml` & `dvc-data-1.2.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/.github/workflows/release.yml` & `dvc-data-1.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/.github/workflows/tests.yml` & `dvc-data-1.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/.gitignore` & `dvc-data-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/.pre-commit-config.yaml` & `dvc-data-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/CODE_OF_CONDUCT.rst` & `dvc-data-1.2.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/CONTRIBUTING.rst` & `dvc-data-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/LICENSE` & `dvc-data-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/PKG-INFO` & `dvc-data-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.1.0
+Version: 1.2.0
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.1.0/README.rst` & `dvc-data-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/noxfile.py` & `dvc-data-1.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/pyproject.toml` & `dvc-data-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/setup.cfg` & `dvc-data-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/cli.py` & `dvc-data-1.2.0/src/dvc_data/cli.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/fs.py` & `dvc-data-1.2.0/src/dvc_data/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/__init__.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/_progress.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/build.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/cache.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/checkout.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/db/__init__.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/db/index.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/db/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/db/local.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/db/local.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/db/reference.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/db/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/diff.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/gc.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/hash.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/hash_info.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/hash_info.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/istextfile.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/meta.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/meta.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/state.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/state.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/status.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/status.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/transfer.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/transfer.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/tree.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/hashfile/utils.py` & `dvc-data-1.2.0/src/dvc_data/hashfile/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/__init__.py` & `dvc-data-1.2.0/src/dvc_data/index/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/add.py` & `dvc-data-1.2.0/src/dvc_data/index/add.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/build.py` & `dvc-data-1.2.0/src/dvc_data/index/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/checkout.py` & `dvc-data-1.2.0/src/dvc_data/index/checkout.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from typing import (
     TYPE_CHECKING,
     Callable,
     Collection,
     Dict,
     Iterator,
     List,
+    NamedTuple,
     Optional,
     Tuple,
 )
 
 from dvc_objects.fs.callbacks import DEFAULT_CALLBACK, Callback
 from dvc_objects.fs.generic import transfer
 from dvc_objects.fs.local import LocalFileSystem
 from dvc_objects.fs.utils import exists as batch_exists
 
 from ..hashfile.checkout import CheckoutError
 from ..hashfile.meta import Meta
-from .diff import ADD, DELETE, MODIFY, UNCHANGED, diff
+from .diff import ADD, DELETE, MODIFY, UNCHANGED
+from .diff import diff as idiff
 from .index import FileStorage, ObjectStorage
 
 if TYPE_CHECKING:
     from dvc_objects.fs.base import AnyFSPath, FileSystem
 
     from ..hashfile.state import StateBase
     from .diff import Change
@@ -222,82 +224,76 @@
                 "failed to chmod '%s' '%s'",
                 oct(mode),
                 entry_path,
                 exc_info=True,
             )
 
 
-def checkout(  # noqa: C901
-    index: "BaseDataIndex",
-    path: str,
-    fs: "FileSystem",
-    old: Optional["BaseDataIndex"] = None,
-    delete: bool = False,
-    callback: "Callback" = DEFAULT_CALLBACK,
-    latest_only: bool = True,
-    update_meta: bool = True,
-    jobs: Optional[int] = None,
-    storage: str = "cache",
-    prompt: Optional[Callable] = None,
-    relink: bool = False,
-    force: bool = False,
-    allow_missing: bool = False,
-    state: Optional["StateBase"] = None,
-    **kwargs,
-) -> Dict[str, List["Change"]]:
+class _DiffResult(NamedTuple):
+    changes: Dict[str, list]
+    files_delete: list
+    dirs_delete: list
+    files_create: list
+    dirs_create: list
+    files_chmod: list
 
-    failed = []
 
-    changes = defaultdict(list)
-    files_delete = []
-    dirs_delete = []
-    files_create = []
-    dirs_create = []
-    files_chmod = []
+def _diff(  # noqa: C901
+    old,
+    new,
+    relink: bool = False,
+    delete: bool = False,
+    callback: "Callback" = DEFAULT_CALLBACK,
+):
+    ret = _DiffResult(defaultdict(list), [], [], [], [], [])
 
     def _add_file_create(entry):
         if entry.meta and entry.meta.isexec:
-            files_chmod.append(entry)
+            ret.files_chmod.append(entry)
 
-        files_create.append(entry)
+        ret.files_create.append(entry)
 
     def _add_create(entry):
         if entry.meta and entry.meta.isdir:
-            dirs_create.append(entry)
+            ret.dirs_create.append(entry)
             return
 
         _add_file_create(entry)
 
     def _add_delete(entry):
         if entry.meta and entry.meta.isdir:
-            dirs_delete.append(entry)
+            ret.dirs_delete.append(entry)
             return
 
-        files_delete.append(entry)
+        ret.files_delete.append(entry)
 
     def meta_cmp_key(meta):
         if meta is None:
             return meta
         return (meta.isdir, meta.isexec)
 
-    for change in diff(
-        old, index, with_unchanged=relink, meta_cmp_key=meta_cmp_key
+    for change in idiff(
+        old,
+        new,
+        with_unchanged=relink,
+        meta_cmp_key=meta_cmp_key,
+        callback=callback,
     ):
         if change.typ == ADD:
             _add_create(change.new)
         elif change.typ == DELETE:
             if not delete:
                 continue
 
             _add_delete(change.old)
         elif change.typ == UNCHANGED:
             assert relink
 
             if not change.old.meta or not change.old.meta.isdir:
-                files_delete.append(change.old)
+                ret.files_delete.append(change.old)
 
             if not change.new.meta or not change.new.meta.isdir:
                 _add_file_create(change.new)
 
             continue
         elif change.typ == MODIFY:
             old_hi = change.old.hash_info
@@ -314,59 +310,95 @@
                     # no need to recreate the dir
                     continue
 
                 _add_delete(change.old)
                 _add_create(change.new)
 
             elif old_isexec != new_isexec and not new_isdir:
-                files_chmod.append(change.new)
+                ret.files_chmod.append(change.new)
             else:
                 continue
         else:
             raise AssertionError()
 
-        changes[change.typ].append(change)
+        ret.changes[change.typ].append(change)
+
+    return ret
+
+
+def checkout(
+    index: "BaseDataIndex",
+    path: str,
+    fs: "FileSystem",
+    old: Optional["BaseDataIndex"] = None,
+    delete: bool = False,
+    callback: "Callback" = DEFAULT_CALLBACK,
+    latest_only: bool = True,
+    update_meta: bool = True,
+    jobs: Optional[int] = None,
+    storage: str = "cache",
+    prompt: Optional[Callable] = None,
+    relink: bool = False,
+    force: bool = False,
+    allow_missing: bool = False,
+    state: Optional["StateBase"] = None,
+    **kwargs,
+) -> Dict[str, List["Change"]]:
+
+    failed = []
+
+    if callback == DEFAULT_CALLBACK:
+        cb = callback
+    else:
+        cb = Callback.as_tqdm_callback(desc="Comparing indexes", unit="entry")
+
+    with cb:
+        diff = _diff(old, index, relink=relink, delete=delete, callback=cb)
 
     if fs.version_aware and not latest_only:
         if callback == DEFAULT_CALLBACK:
             cb = callback
         else:
             desc = f"Checking status of existing versions in '{path}'"
             cb = Callback.as_tqdm_callback(desc=desc, unit="file")
         with cb:
-            files_create = list(
-                _prune_existing_versions(files_create, fs, path, callback=cb)
+            diff.files_create = list(
+                _prune_existing_versions(
+                    diff.files_create, fs, path, callback=cb
+                )
             )
 
-    _delete_files(files_delete, index, path, fs, prompt=prompt, force=force)
-    _delete_dirs(dirs_delete, path, fs)
-    _create_dirs(dirs_create, path, fs)
+    _delete_files(
+        diff.files_delete, index, path, fs, prompt=prompt, force=force
+    )
+    _delete_dirs(diff.dirs_delete, path, fs)
+    _create_dirs(diff.dirs_create, path, fs)
 
     def onerror(_src_path, dest_path, _exc):
         failed.append(dest_path)
 
     _create_files(
-        files_create,
+        diff.files_create,
         index,
         path,
         fs,
         onerror=onerror,
         jobs=jobs,
         storage=storage,
         callback=callback,
         update_meta=update_meta,
         state=state,
     )
 
-    _chmod_files(files_chmod, path, fs)
+    _chmod_files(diff.files_chmod, path, fs)
 
     if failed and not allow_missing:
         raise CheckoutError(failed)
 
-    return changes
+    return diff.changes
 
 
 def _prune_existing_versions(
     entries: Collection["DataIndexEntry"],
     fs: "FileSystem",
     path: str,
     callback: "Callback" = DEFAULT_CALLBACK,
```

### Comparing `dvc-data-1.1.0/src/dvc_data/index/diff.py` & `dvc-data-1.2.0/src/dvc_data/index/diff.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import deque
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional
 
 from attrs import define
+from dvc_objects.fs.callbacks import DEFAULT_CALLBACK, Callback
 
 if TYPE_CHECKING:
     from .hashfile.meta import Meta
     from .hashfile.hash_info import HashInfo
     from .index import BaseDataIndex, DataIndexKey
 
 from ..hashfile.tree import TreeError
@@ -162,14 +163,15 @@
     *,
     with_unchanged: Optional[bool] = False,
     with_unknown: Optional[bool] = False,
     hash_only: Optional[bool] = False,
     meta_only: Optional[bool] = False,
     meta_cmp_key: Optional[Callable[["Meta"], Any]] = None,
     shallow: Optional[bool] = False,
+    callback: Callback = DEFAULT_CALLBACK,
 ):
     old_root_items = {}
     new_root_items = {}
 
     if old is not None:
         try:
             old_root_items[()] = old.info(())
@@ -181,15 +183,15 @@
             new_root_items[()] = new.info(())
         except FileNotFoundError:
             pass
 
     todo = deque([(old_root_items, new_root_items, False)])
     while todo:
         old_items, new_items, unknown = todo.popleft()
-        for key in old_items.keys() | new_items.keys():
+        for key in callback.wrap(old_items.keys() | new_items.keys()):
             old_info = old_items.get(key) or {}
             new_info = new_items.get(key) or {}
 
             old_entry = old_info.get("entry")
             new_entry = new_info.get("entry")
 
             typ = _diff_entry(
@@ -288,24 +290,26 @@
     with_renames: Optional[bool] = False,
     with_unchanged: Optional[bool] = False,
     with_unknown: Optional[bool] = False,
     hash_only: Optional[bool] = False,
     meta_only: Optional[bool] = False,
     meta_cmp_key: Optional[Callable[["Meta"], Any]] = None,
     shallow: Optional[bool] = False,
+    callback: Callback = DEFAULT_CALLBACK,
 ):
     changes = _diff(
         old,
         new,
         with_unchanged=with_unchanged,
         with_unknown=with_unknown,
         hash_only=hash_only,
         meta_only=meta_only,
         meta_cmp_key=meta_cmp_key,
         shallow=shallow,
+        callback=callback,
     )
 
     if with_renames and old is not None and new is not None:
         assert not meta_only
         yield from _detect_renames(changes)
     else:
         yield from changes
```

### Comparing `dvc-data-1.1.0/src/dvc_data/index/fetch.py` & `dvc-data-1.2.0/src/dvc_data/index/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/index.py` & `dvc-data-1.2.0/src/dvc_data/index/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/save.py` & `dvc-data-1.2.0/src/dvc_data/index/save.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/serialize.py` & `dvc-data-1.2.0/src/dvc_data/index/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/index/view.py` & `dvc-data-1.2.0/src/dvc_data/index/view.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data/repo.py` & `dvc-data-1.2.0/src/dvc_data/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data.egg-info/PKG-INFO` & `dvc-data-1.2.0/src/dvc_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.1.0
+Version: 1.2.0
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.1.0/src/dvc_data.egg-info/SOURCES.txt` & `dvc-data-1.2.0/src/dvc_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/src/dvc_data.egg-info/requires.txt` & `dvc-data-1.2.0/src/dvc_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/benchmarks/test_checkout.py` & `dvc-data-1.2.0/tests/benchmarks/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_cache.py` & `dvc-data-1.2.0/tests/hashfile/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_db_index.py` & `dvc-data-1.2.0/tests/hashfile/test_db_index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_diff.py` & `dvc-data-1.2.0/tests/hashfile/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_hash.py` & `dvc-data-1.2.0/tests/hashfile/test_hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_hash_stream.py` & `dvc-data-1.2.0/tests/hashfile/test_hash_stream.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_istextfile.py` & `dvc-data-1.2.0/tests/hashfile/test_istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_tree.py` & `dvc-data-1.2.0/tests/hashfile/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/hashfile/test_utils.py` & `dvc-data-1.2.0/tests/hashfile/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/index/conftest.py` & `dvc-data-1.2.0/tests/index/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/index/test_checkout.py` & `dvc-data-1.2.0/tests/index/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/index/test_diff.py` & `dvc-data-1.2.0/tests/index/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.1.0/tests/index/test_index.py` & `dvc-data-1.2.0/tests/index/test_index.py`

 * *Files identical despite different names*

