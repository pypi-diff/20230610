# Comparing `tmp/labmate-0.6.1.tar.gz` & `tmp/labmate-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labmate-0.6.1.tar", last modified: Sun May 14 17:35:11 2023, max compression
+gzip compressed data, was "labmate-0.7.0.tar", last modified: Sat Jun 10 13:56:26 2023, max compression
```

## Comparing `labmate-0.6.1.tar` & `labmate-0.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.763683 labmate-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-14 17:34:57.000000 labmate-0.6.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-14 17:34:57.000000 labmate-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-14 17:35:11.763683 labmate-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 17:34:57.000000 labmate-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.755683 labmate-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/acquisition_notebook.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/acquisition_and_analysis_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/examples/files/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/dummy_config1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/dummy_config2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/dummy_config3.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/init_analyse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/examples/more/
--rw-r--r--   0 runner    (1001) docker     (123)   111306 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/more/h5nparray.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/more/loop_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/smart_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/h5nparray.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/releases/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.4.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.5.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.6.0.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.6.1.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/acquisition_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/acquisition_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/acquisition_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/analysis_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/analysis_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/acquisition_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition_notebook/acquisition_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition_notebook/acquisition_magic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/attrdict/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/attrdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/attrdict/attrdict_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/json/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/path/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/path/path_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/plot_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/plot_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/plot_utils/random_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/plt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/syncdata/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata/h5py_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata/syncdata_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/syncdata_types/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata_types/h5_np_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.763683 labmate-0.6.1/labmate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 17:34:57.000000 labmate-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:35:11.763683 labmate-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-14 17:34:57.000000 labmate-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-10 13:56:18.000000 labmate-0.7.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-10 13:56:18.000000 labmate-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-10 13:56:26.544299 labmate-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-10 13:56:18.000000 labmate-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.540298 labmate-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/acquisition_notebook.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.540298 labmate-0.7.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/acquisition_and_analysis_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.540298 labmate-0.7.0/docs/examples/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/files/dummy_config1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/files/dummy_config2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/files/dummy_config3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/files/init_analyse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.540298 labmate-0.7.0/docs/examples/more/
+-rw-r--r--   0 runner    (1001) docker     (123)   111306 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/more/h5nparray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/more/loop_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/examples/smart_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/h5nparray.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.540298 labmate-0.7.0/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/releases/0.4.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/releases/0.5.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/releases/0.6.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/releases/0.6.1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-10 13:56:18.000000 labmate-0.7.0/docs/releases/0.7.0.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.540298 labmate-0.7.0/labmate/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/acquisition_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/acquisition_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/acquisition_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/analysis_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/analysis_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/acquisition_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition_notebook/acquisition_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/acquisition_notebook/acquisition_magic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/attrdict/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/attrdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/attrdict/attrdict_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/json/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/json/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/path/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/path/path_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/plt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/syncdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/syncdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/syncdata/function_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/syncdata/h5py_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/syncdata/syncdata_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/syncdata_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/syncdata_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/syncdata_types/h5_np_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.544299 labmate-0.7.0/labmate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/utils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/utils/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-10 13:56:18.000000 labmate-0.7.0/labmate/utils/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:56:26.540298 labmate-0.7.0/labmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-10 13:56:26.000000 labmate-0.7.0/labmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-10 13:56:26.000000 labmate-0.7.0/labmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:56:26.000000 labmate-0.7.0/labmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-10 13:56:26.000000 labmate-0.7.0/labmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 13:56:26.000000 labmate-0.7.0/labmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-10 13:56:18.000000 labmate-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:56:26.544299 labmate-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-10 13:56:18.000000 labmate-0.7.0/setup.py
```

### Comparing `labmate-0.6.1/LICENCE` & `labmate-0.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/PKG-INFO` & `labmate-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: labmate
-Version: 0.6.1
+Version: 0.7.0
 Summary: Data management library to save data and plots to hdf5 files
 Home-page: https://github.com/kyrylo-gr/labmate
 Author: LKB-OMQ
 Author-email: cryo.paris.su@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENCE
 
 ## Install
 
 `pip install labmate`
```

### Comparing `labmate-0.6.1/docs/examples/acquisition_and_analysis_notebook.ipynb` & `labmate-0.7.0/docs/examples/acquisition_and_analysis_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/examples/files/init_analyse.py` & `labmate-0.7.0/docs/examples/files/init_analyse.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb` & `labmate-0.7.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/examples/more/h5nparray.ipynb` & `labmate-0.7.0/docs/examples/more/h5nparray.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/examples/more/loop_example.ipynb` & `labmate-0.7.0/docs/examples/more/loop_example.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/h5nparray.md` & `labmate-0.7.0/docs/h5nparray.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/releases/0.4.0.md` & `labmate-0.7.0/docs/releases/0.4.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/releases/0.5.0.md` & `labmate-0.7.0/docs/releases/0.5.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/docs/releases/0.6.0.md` & `labmate-0.7.0/docs/releases/0.6.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/acquisition/acquisition_data.py` & `labmate-0.7.0/labmate/acquisition/acquisition_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,21 @@
         self['useful'] = True
 
         if not self._save_files:
             return
         self.save_cell()
         self.save_configs()
 
+    def save_acquisition(self, **kwds) -> 'NotebookAcquisitionData':
+        self.update(**kwds)
+        self.save_additional_info()
+        if self.save_on_edit is False:
+            self.save()
+        return self
+
 
 def read_config_files(config_files: List[str]) -> Dict[str, str]:
     configs: Dict[str, str] = {}
     for config_file in config_files:
         config_file_name = os.path.basename(config_file)
         if config_file_name in configs:
             raise ValueError(
```

### Comparing `labmate-0.6.1/labmate/acquisition/acquisition_loop.py` & `labmate-0.7.0/labmate/acquisition/acquisition_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,17 +142,16 @@
             if len(self._iteration)-1 > level:
                 self._iteration.pop()
             self._level -= 1
 
         return GenerToIter(
             loop_iter(iterable, level=level), length)
 
-    def enum(self, iterable: Iterable, level=None):
-        return enumerate(self.iter(
-            iterable=iterable, level=level))
+    def enum(self, *args, iterable: Optional[Iterable] = None):
+        return enumerate(self(*args, iterable=iterable))  # type: ignore
 
 
 class AcquisitionLoopOld:
     """Acquisition loop allow to save data during for loops.
 
     - Example 1 that saves list of squares till 10:
     ```
@@ -276,15 +275,15 @@
         for key, data_flatten in self._data_flatten.items():
             data_flatten = np.array(data_flatten).flatten()
             expected_len = np.prod(self._reshape_tuple(key))
             if expected_len < len(data_flatten):
                 # print(key, expected_len, len(data_flatten))
                 data_flatten = data_flatten[-expected_len:]
 
-            data_reshape[key] = np.pad(data_flatten, (0, expected_len-len(data_flatten))).reshape(
+            data_reshape[key] = np.pad(data_flatten, (0, expected_len-len(data_flatten))).reshape(  # type: ignore
                 self._reshape_tuple(key))
         return data_reshape
 
     def asdict(self):
         data = self.data
         data['__loop_shape__'] = self.loop_shape
         return data
```

### Comparing `labmate-0.6.1/labmate/acquisition/acquisition_manager.py` & `labmate-0.7.0/labmate/acquisition/acquisition_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,14 +152,42 @@
         self.acquisition_tmp_data = dic
 
         self._current_acquisition = self.get_acquisition(replace=True,
                                                          save_on_edit=save_on_edit)
 
         return self.current_acquisition
 
+    def create_acquisition(self,
+                           name: str,
+                           cell: Optional[str] = None,
+                           save_on_edit: Optional[bool] = None
+                           ) -> NotebookAcquisitionData:
+        """Create a new acquisition with the given experiment name."""
+        configs = read_config_files(self.config_files)
+
+        if self.config_files_eval:
+            configs = eval_config_files(configs, self.config_files_eval)
+
+        dic = AcquisitionTmpData(experiment_name=name,
+                                 time_stamp=get_timestamp(),
+                                 configs=configs,
+                                 directory=self.data_directory)
+
+        filepath = self.create_path_from_tmp_data(dic)
+        configs = configs if configs else None
+        save_on_edit = save_on_edit if save_on_edit is not None else self._save_on_edit
+
+        return NotebookAcquisitionData(
+            filepath=str(filepath),
+            configs=configs,
+            cell=cell or self.cell,
+            overwrite=False,
+            save_on_edit=save_on_edit,
+            save_files=self._save_files)
+
     @ property
     def current_acquisition(self) -> NotebookAcquisitionData:
         if self._current_acquisition is None:
             self._current_acquisition = self.get_acquisition()
         return self._current_acquisition
 
     @ property
```

### Comparing `labmate-0.6.1/labmate/acquisition/analysis_data.py` & `labmate-0.7.0/labmate/acquisition/analysis_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from typing import List, Literal, Optional, Protocol, Tuple, Union
 
 
 from .analysis_loop import AnalysisLoop
 
 from ..syncdata import SyncData
-from ..attrdict import AttrDict
+from .config_file import ConfigFile
 from ..path import Path
 from .. import utils
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
@@ -56,18 +56,18 @@
 
         super().__init__(filepath=str(filepath), overwrite=False,
                          read_only=False, save_on_edit=save_on_edit)
         self.lock_data()
 
         self._save_files = save_files
 
-        if save_fig_inside_h5 is True:
-            raise NotImplementedError(
-                """We stop using pickle as it's not consistent between systems.
-                before the better solution found this functionality is deprecated.""")
+        # if save_fig_inside_h5 is True:
+        #     raise NotImplementedError(
+        #         """We stop using pickle as it's not consistent between systems.
+        #         before the better solution found this functionality is deprecated.""")
         self._save_fig_inside_h5 = save_fig_inside_h5
 
         self._default_config_files: Tuple[str, ...] = tuple()
 
         self.reset_am()
 
         for key, value in self.items():
@@ -120,33 +120,33 @@
         If name is None, use (...)_FIG1, (...)_FIG2.
         pdf is used by default if no extension is provided in name
         """
         self._figure_last_name = str(name).lstrip('_') if name is not None else None
 
         fig_name = self.get_fig_name(name)
         full_fig_name = f'{self.filepath}_{fig_name}'
-
-        if fig is not None:
-            # if self._save_fig_inside_h5 and kwargs.get("pickle", True):
-            #     try:
-            #         import pickle
-            #         import codecs
-            #         pickled = codecs.encode(pickle.dumps(fig), "base64").decode()
-            #         self[f"figures/{fig_name}"] = pickled
-            #         self.save([f"figures/{fig_name}"])
-            #     except Exception as error:
-            #         logger.warning("Failed to pickle the figure due to %s", error)
-            if tight_layout and hasattr(fig, "tight_layout"):
-                fig.tight_layout()  # type: ignore
-            fig.savefig(full_fig_name, **kwargs)
-        else:
+        if fig is None:
             from matplotlib import pyplot as plt
-            if tight_layout:
-                plt.tight_layout()
-            plt.savefig(full_fig_name, **kwargs)
+            fig = plt.gcf()
+
+        if (self._save_fig_inside_h5 and kwargs.get("inside_h5", True)) or \
+                kwargs.get("inside_h5", False):
+            try:
+                # import pickle
+                # import codecs
+                # pickled = codecs.encode(pickle.dumps(fig), "base64").decode()
+                import pltsave
+                data = pltsave.dumps(fig).to_json()
+                self[f"figures/{fig_name}"] = data
+                self.save([f"figures/{fig_name}"])
+            except Exception as error:
+                logger.exception("Failed to save the figure inside h5 file due to %s", error)
+        if tight_layout and hasattr(fig, "tight_layout"):
+            fig.tight_layout()  # type: ignore
+        fig.savefig(full_fig_name, **kwargs)
 
         self._figure_saved = True
 
     def get_fig_name(self, name: Optional[Union[str, int]] = None) -> str:
         """Get the name of the figure depending on the suffix.
 
         If name is not specified, suffix is `FIG1.pdf`, `FIG2.pdf`, etc.
@@ -167,41 +167,48 @@
                 name = name + ".pdf"
 
         return 'FIG' + name
 
     def parse_config(
             self,
             config_files: Optional[Tuple[str, ...]] = None
-    ) -> AttrDict:
+    ) -> ConfigFile:
         # if isinstance(config_files, str):
         #     logging.warning("""Function `parse_config` changed its behavior.
         #                     Old parse_config function now calls `parse_config_file`.""")
         #     return self.parse_config_file(config_files)  # type: ignore
 
         config_files = config_files or self._default_config_files
 
         if not isinstance(config_files, tuple):
             config_files = tuple(config_files)
         if hash(config_files) in self._parsed_configs:
             return self._parsed_configs[hash(config_files)]
 
         config_data = sum(
-            (self.parse_config_file(config_file) for config_file in config_files), AttrDict())
+            (self.parse_config_file(config_file) for config_file in config_files),
+            ConfigFile())
 
         self._parsed_configs[hash(config_files)] = config_data
 
         return config_data
 
+    @property
+    def cfg(self) -> 'ConfigFile':
+        return self.parse_config()
+
     def parse_config_values(
             self,
             keys: List[str],
             config_files: Optional[Tuple[str, ...]] = None
     ) -> List[utils.parse.ValueForPrint]:
 
         config_data = self.parse_config(config_files=config_files)
+        if not isinstance(keys, (list, tuple)):
+            raise ValueError("Keys must be a list of strings.")
         keys_with_values = []
         for key in keys:
             key_value, key_units, key_format = utils.parse.parse_get_format(key)
             if key_value == "filename" or key_value == "file" or key_value == "f":
                 filename = os.path.split(self.filepath)[-1]
                 keys_with_values.append(utils.parse.ValueForPrint(
                     key_value, filename, key_units, key_format))
@@ -215,25 +222,25 @@
                 logger.warning("key %s not found and cannot be parsed", key_value)
 
         return keys_with_values
 
     def parse_config_str(
             self,
             values: List[str],
-            max_length: Optional[int] = None,
+            max_length: Optional[int] = 60,
             config_files: Optional[Tuple[str, ...]] = None
     ) -> str:
         """Parse the configuration files.
 
         Returns: key1=value1, key2=value2, ...
         """
         keys_with_values = self.parse_config_values(values, config_files=config_files)
         return utils.parse.format_title(keys_with_values, max_length=max_length)
 
-    def parse_config_file(self, config_file_name: str, /) -> AttrDict:
+    def parse_config_file(self, config_file_name: str, /) -> ConfigFile:
         if config_file_name in self._parsed_configs:
             return self._parsed_configs[config_file_name]
 
         if 'configs' not in self:
             raise KeyError("The is no config files saved within AnalysisManager")
 
         if config_file_name not in self['configs']:
@@ -251,15 +258,16 @@
                 self._parsed_configs[original_config_name] = self._parsed_configs[config_file_name]
                 return self._parsed_configs[config_file_name]
 
         else:
             original_config_name = None
 
         from ..utils.parse import parse_str
-        config_data = AttrDict(parse_str(self['configs'][config_file_name]))
+        file_content = self['configs'][config_file_name]
+        config_data = ConfigFile(parse_str(file_content), file_content)
         self._parsed_configs[config_file_name] = config_data
         if original_config_name is not None:
             self._parsed_configs[original_config_name] = config_data
 
         # print("e", self._parsed_configs.keys())
 
         return config_data
@@ -275,24 +283,33 @@
             raise ValueError(
                 f"There is no field 'analysis_cells' inside the data file. "
                 f"Possible keys are {tuple(self.keys())}.")
 
         # if isinstance(code, bytes):
         #     code = code.decode()
         if name not in code:
-            raise KeyError(f"Cannot get cell '{name}'. Possible cells are: {tuple(code.key())}")
+            raise KeyError(f"Cannot get cell '{name}'. Possible cells are: {tuple(code.keys())}")
 
         code_str: str = code[name]
         if update_code:
             code_str = code_str.replace("aqm.analysis_cell()", f"aqm.analysis_cell('{self.filepath}')")
         return code_str
 
     def open_figs(self) -> list:
-        raise NotImplementedError(
-            "Not implemented for the moment. If you want to open an old figure. Use open_old_figs function")
+        figures = []
+
+        for figure_key in self.get("figures", []):
+            import pltsave
+            figure_code = self['figures'][figure_key]
+            figure = pltsave.loads(figure_code)
+            figures.append(figure)
+        return figures
+
+        # raise NotImplementedError(
+        # "Not implemented for the moment. If you want to open an old figure. Use open_old_figs function")
 
     def open_old_figs(self) -> list:
         figures = []
         # print(self.get("figures"))
 
         for figure_key in self.get("figures", []):  # pylint: disable=E1133
             # print(figure_key)
```

### Comparing `labmate-0.6.1/labmate/acquisition/analysis_loop.py` & `labmate-0.7.0/labmate/acquisition/analysis_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             child_kwds = {}
             for key, value in self._data.items():
                 if key[:1] == '_':
                     continue
 
                 # if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
                 if not hasattr(value, "__getitem__") or \
-                        isinstance(value, (str, bytes, int, float)):
+                        isinstance(value, (str, bytes, int, float, complex)):
                     child_kwds[key] = value
                 elif len(value) == 1:
                     child_kwds[key] = value[0]
                 else:
                     child_kwds[key] = value[index]
 
                 val = child_kwds[key]
```

### Comparing `labmate-0.6.1/labmate/acquisition/lint.py` & `labmate-0.7.0/labmate/acquisition/lint.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/acquisition_notebook/acquisition_analysis_manager.py` & `labmate-0.7.0/labmate/acquisition_notebook/acquisition_analysis_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import logging
 import time
 from ..acquisition import AcquisitionManager, AnalysisData
 from .. import utils
 if TYPE_CHECKING:
     from ..acquisition import FigureProtocol
-    from ..attrdict import AttrDict
+    from ..acquisition.config_file import ConfigFile
     from ..path import Path
 
 # from ..syncdata import SyncData
 
 logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.INFO)
 logger = logging.getLogger(__name__)
 handler = logging.StreamHandler()
@@ -85,15 +85,15 @@
             save_on_edit_analysis (bool. Defaults to same as save_on_edit):
                 save_on_edit parameter for AnalysisManager i.e. data inside analysis_cell
             shell (InteractiveShell | None, optional. Defaults to True):
                 could be provided or explicitly set to None. Defaults to get_ipython().
         """
         if shell is False or shell is True:  # behavior by default shell
             try:
-                from IPython import get_ipython
+                from IPython.core.getipython import get_ipython
                 self.shell = get_ipython()
             except ImportError:
                 self.shell = None
         else:  # if any shell is provided. even None
             self.shell = shell
 
         if use_magic:
@@ -183,51 +183,57 @@
         self.save_fig_only(fig=fig, name=name, **kwds)
         self.save_analysis_cell(name=name, cell=cell)
         return self
 
     def __setitem__(self, __key: str, __value: Any) -> None:
         if self._analysis_data is not None:
             raise ValueError(
-                "This is the way to save acquisition data. But analysis data was loaded."
-                "So you possibly run it inside analysis_cell")
+                "This is the way to save acquisition data. But analysis data was loaded. "
+                "So you possibly run it outside of acquisition_cell")
         acq_data = self.current_acquisition
         if acq_data is None:
             raise ValueError(
                 "Cannot save data to acquisition as current acquisition is None."
                 "Possibly because you have never run `acquisition_cell(..)` or it's an old data")
         acq_data[__key] = __value
 
     def save_acquisition(self, **kwds) -> 'AcquisitionAnalysisManager':
         acquisition_finished = time.time()
         kwds.update({"info": {"acquisition_duration": acquisition_finished-self._acquisition_started}})
         super().save_acquisition(**kwds)
-        self.load_analysis_data()
+        self._load_analysis_data()
         return self
 
-    def load_analysis_data(self, filepath: Optional[str] = None):
+    def _load_analysis_data(self, filepath: Optional[str] = None):
         filepath = filepath or str(self.current_filepath)
 
-        if not os.path.exists(filepath if filepath.endswith('.h5') else filepath + '.h5'):
-            raise ValueError(
-                f"Cannot load data from {filepath}. As file does not exist.")
+        self._analysis_data = self.load_file(filepath)
+
+        if self._save_on_edit_analysis is False:
+            self._analysis_data.save()
+
+        return self._analysis_data
 
-        self._analysis_data = AnalysisData(
-            filepath=filepath,
+    def load_file(self, filename) -> 'AnalysisData':
+        filename = self.get_full_filename(str(filename))
+        if not os.path.exists(filename if filename.endswith('.h5') else filename + '.h5'):
+            raise ValueError(f"File {filename} cannot be found")
+
+        data = AnalysisData(
+            filepath=filename,
             save_files=self._save_files, save_on_edit=self._save_on_edit_analysis,
             save_fig_inside_h5=self._save_fig_inside_h5)
 
-        self._analysis_data.unlock_data('useful').update(**{'useful': True}).lock_data('useful')
-
-        if self._save_on_edit_analysis is False:
-            self._analysis_data.save()
+        if not data.get('useful', True):
+            data.unlock_data('useful').update(**{'useful': True}).lock_data('useful')
 
         if self._default_config_files:
-            self._analysis_data.set_default_config_files(self._default_config_files)
+            data.set_default_config_files(self._default_config_files)
 
-        return self._analysis_data
+        return data
 
     def acquisition_cell(
             self,
             name: str,
             cell: Optional[str] = None,
             prerun: Optional[Union[_CallableWithNoArgs, List[_CallableWithNoArgs]]] = None,
             save_on_edit: Optional[bool] = None
@@ -263,15 +269,15 @@
             self._is_old_data = True
             if self.shell is not None:
                 try:
                     from IPython import display
                     html = """<div style="
                     background-color:#ec7413; padding: .5em; text-align:center"
                     >Old data analysis</div>"""
-                    display.display(display.HTML(str(html)))
+                    display.display(display.HTML(str(html)))  # type: ignore
                 except ImportError:
                     logger.warning("Old data analysis")
             filename = str(filepath or self.get_full_filename(str(filename)))  # type: ignore
             filename = (filename.rsplit('.h5', 1)[0]) \
                 if filename.endswith('.h5') else filename
 
         else:
@@ -294,15 +300,15 @@
             if ('acquisition_cell(' in self.shell.last_execution_result.info.raw_cell and
                     not self.shell.last_execution_result.success):
                 raise ChildProcessError(
                     "Last executed cell was probably an `acquisition_cell` and failed to run. "
                     "Check if everything is ok and executive again")
 
         if os.path.exists(filename + '.h5'):
-            self.load_analysis_data(filename)
+            self._load_analysis_data(filename)
         else:
             if self._is_old_data:
                 raise ValueError(f"Cannot load data from {filename}")
             self._analysis_data = None
 
         if cell is not None:
             self.save_analysis_cell(cell=cell)
@@ -338,24 +344,24 @@
 
         name_with_prefix = utils.lstrip_int(filename)
         if name_with_prefix:
             suffix = name_with_prefix[1]
             return os.path.join(self.data_directory, suffix, filename)
         return filename
 
-    def parse_config_file(self, config_file_name: str, /) -> 'AttrDict':
+    def parse_config_file(self, config_file_name: str, /) -> 'ConfigFile':
         return self.data.parse_config_file(config_file_name)
 
     def parse_config(
             self,
-            config_files: Optional[Tuple[str, ...]] = None) -> 'AttrDict':
+            config_files: Optional[Tuple[str, ...]] = None) -> 'ConfigFile':
         return self.data.parse_config(config_files=(config_files or self._default_config_files))
 
     @property
-    def cfg(self) -> 'AttrDict':
+    def cfg(self) -> 'ConfigFile':
         return self.parse_config()
 
     def parse_config_str(
         self,
         values: List[str], /,
         max_length: Optional[int] = None,
     ) -> str:
```

### Comparing `labmate-0.6.1/labmate/acquisition_notebook/acquisition_magic_class.py` & `labmate-0.7.0/labmate/acquisition_notebook/acquisition_magic_class.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/json/decoders.py` & `labmate-0.7.0/labmate/json/decoders.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/json/open.py` & `labmate-0.7.0/labmate/json/open.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/json_utils.py` & `labmate-0.7.0/labmate/json_utils.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/path/path_class.py` & `labmate-0.7.0/labmate/path/path_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     - sum 2 path or path and str. Action: sum 2 str
     - makedirs. Action: os.makedirs
     - make_extension
     - dirname
     - basename
     """
 
-    def __add__(self, other: str):
+    def __add__(self, other: Union['Path', str]):
         """Sum 2 str."""
         if not isinstance(other, str):
             other = str(other)
         return type(self)(self.as_posix() + other)
 
     def makedirs(self, mode=0o777, exist_ok=False):
         """Create a directories if needed.
@@ -51,14 +51,18 @@
     def dirname(self) -> 'Path':
         return type(self)(os.path.dirname(self))
 
     @property
     def basename(self) -> 'Path':
         return type(self)(os.path.basename(self))
 
+    @property
+    def str(self) -> str:
+        return str(self)
+
 
 def get_file_path(file_name: Union[str, Path], *,
                   path: Optional[Union[str, Path]] = None,
                   extension: Optional[str] = None) -> Path:
     file_name = Path(file_name)
     if extension:
         file_name.make_extension(extension)
```

### Comparing `labmate-0.6.1/labmate/plt.py` & `labmate-0.7.0/labmate/plt.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/syncdata/h5py_utils.py` & `labmate-0.7.0/labmate/syncdata/h5py_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 import h5py
-from typing import Dict, Literal, Optional, Protocol, Set, Union
+from typing import Callable, Dict, Literal, Optional, Protocol, Set, Union
 from ..utils.errors import FileLockedError
 
 import numpy as np
 
 
 class ClassWithAsdict(Protocol):
     """Any class with predefined `_asdict` attribute.
@@ -48,18 +48,34 @@
             os.remove(self.lock_filename)
         #     print("lock del", time.time())
         # else:
         #     print("exit without lock file", time.time())
 
 
 DICT_OR_LIST_LIKE = Optional[Union[dict, list, np.ndarray, ClassWithAsdict, ClassWithAsarray,
-                                   np.int_, np.float_, float, int, str]]
+                                   np.int_, np.float_, float, int, str, Callable]]
 RIGHT_DATA_TYPE = Union[dict, np.ndarray, np.int_, np.float_, float, int]
 
 
+def np_array_check(lst, size: Optional[int] = None) -> int:
+    if isinstance(lst, (list, np.ndarray)):
+        if size is not None and size != len(lst):
+            return -1
+        for lst_elm in lst:
+            check = np_array_check(lst_elm, size)
+            if check >= 0:
+                size = check
+            else:
+                return -1
+        return len(lst)
+    if isinstance(lst, (np.number)):
+        return 0
+    return -1
+
+
 def transform_to_possible_formats(data: DICT_OR_LIST_LIKE) -> DICT_OR_LIST_LIKE:
     if hasattr(data, '__should_not_be_converted__') \
             and data.__should_not_be_converted__ is True:  # type: ignore
         return data
 
     if hasattr(data, 'asdict'):
         data = data.asdict()  # type: ignore
@@ -67,40 +83,54 @@
     if hasattr(data, 'asarray'):
         data = data.asarray()  # type: ignore
 
     if isinstance(data, dict):
         for key, value in data.items():
             data[key] = transform_to_possible_formats(value)
         return data
+
     if isinstance(data, (tuple, set)):
         data = list(data)
+
     if isinstance(data, list):
-        data_array = np.array(data)
-        if 'U' in str(data_array.dtype) or \
-                'object' in str(data_array.dtype):
+        if np_array_check(data) < 0:
             return data
-        return data_array
     return data
 
 
 def transform_on_open(value):
     if isinstance(value, bytes):
         value = value.decode()
     if isinstance(value, str) and value.startswith('__json__'):
         return json.loads(value[8:])
-
+    if isinstance(value, str) and value.startswith('__function__'):
+        from . import function_save
+        return function_save.Function(value[12:])
     return value
 
 
-def transform_list_on_save(value):
-    value_np = np.array(value)
-    if 'U' in str(value_np.dtype) or \
-            'object' in str(value_np.dtype):
-        return '__json__' + json.dumps(value)
-    return value_np
+def transform_list_on_save(value, level=0):
+    if isinstance(value, np.ndarray):
+        if level == 0:
+            return value
+        return value.tolist()
+
+    if isinstance(value, (list)):
+        if np_array_check(value) < 0:
+            try:
+                return '__json__' + json.dumps(value)
+            except TypeError:
+                value_transformed = [transform_list_on_save(v) for v in value]
+                return '__json__' + json.dumps(value_transformed)
+
+    if isinstance(value, Callable):
+        from . import function_save
+        return '__function__' + function_save.function_to_str(value)
+
+    return value
 
 
 def save_sub_dict(
     group: Union[h5py.File, h5py.Group],
     data: Union[dict, list, np.ndarray, ClassWithAsdict],
     key: str,
     use_compression: Optional[Union[Literal[True], str]] = None
@@ -110,17 +140,17 @@
     if hasattr(data, 'asarray'):
         data = data.asarray()  # type: ignore
     if isinstance(data, dict):
         g = group.create_group(key)
         for k, v in data.items():
             save_sub_dict(g, v, k, use_compression=use_compression)
     elif (key is not None) and (data is not None):
+        data = transform_list_on_save(data)  # type: ignore
         if isinstance(data, (np.ndarray, list)):
             use_compression = "gzip" if use_compression is True else use_compression
-            data = transform_list_on_save(data)  # type: ignore
             group.create_dataset(key, data=data, compression=use_compression)  # compression="gzip"
         else:
             group.create_dataset(key, data=data)
 
 
 def save_dict(
     filename: str,
```

### Comparing `labmate-0.6.1/labmate/syncdata/syncdata_class.py` & `labmate-0.7.0/labmate/syncdata/syncdata_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Iterable, Optional, Set, TypeVar, Union, overload
+from typing import Any, Dict, Iterable, Literal, Optional, Set, TypeVar, Union, overload
 import logging
 import os
 from pathlib import Path
 from functools import wraps
 from . import h5py_utils
 
 
@@ -58,15 +58,16 @@
     _raise_file_locked_error: bool = False
     _retry_on_file_locked_error: int = 5
     _last_time_data_checked: float = 0
     _file_modified_time: float = 0
     __should_not_be_converted__ = True
 
     def __init__(self,
-                 filepath_or_data: Optional[Union[str, dict, Path]] = None, /, *,
+                 filepath_or_data: Optional[Union[str, dict, Path]] = None, /,
+                 mode: Optional[Literal['r', 'w', 'a']] = None, *,
                  filepath: Optional[Union[str, Path]] = None,
                  save_on_edit: bool = False,
                  read_only: Optional[Union[bool, Set[str]]] = None,
                  overwrite: Optional[bool] = None,
                  data: Optional[dict] = None,
                  open_on_init: Optional[bool] = None,
                  **kwds):
@@ -82,14 +83,23 @@
                 If file exists, it should be explicitly precised.
                 By default raises an error if file exist.
             data (Optional[dict], optional):
                 Data to load. If data provided, file . Defaults to None.
             open_on_init (Optional[bool], optional): open_on_init. Defaults to True.
 
         """
+        if mode == 'w':
+            read_only = False
+            overwrite = True
+        elif mode == 'a':
+            read_only = False
+            overwrite = False
+        elif mode == 'r':
+            read_only = True
+
         if filepath_or_data is not None and hasattr(filepath_or_data, "keys"):
             if not isinstance(filepath_or_data, dict):
                 filepath_or_data = {key: filepath_or_data[key] for key in filepath_or_data.keys()}  # type: ignore
             data = data or filepath_or_data
 
         if isinstance(filepath_or_data, (str, Path)):
             filepath = filepath or filepath_or_data
@@ -241,33 +251,33 @@
         self.__del_key(key)
         # self.pull(auto=True)
         if key not in self._unopened_keys:
             self._data.pop(key)
             return self
 
     @overload
-    def get_dict(self, __key: str) -> Optional[Any]:
+    def get_dict(self, __key: str) -> Any:
         """Return element as a dict. Return None if not found."""
 
     @overload
     def get_dict(self, __key: str, __default: _T) -> Union[Any, _T]:
         """With default value provided."""
 
-    def get_dict(self, key: str, default: Optional[Any] = None):
+    def get_dict(self, key: str, default: Any = None):
         return self.__get_data__(key, default)
 
     @overload
-    def get(self, __key: str) -> Optional[Any]:
+    def get(self, __key: str) -> Any:
         """Return element as a SyncData class if it's dict. Return None if not found."""
 
     @overload
     def get(self, __key: str, __default: _T) -> Union[Any, _T]:
         """With default value provided."""
 
-    def get(self, key: str, default: Optional[Any] = None):
+    def get(self, key: str, default: Any = None):
         data = self.__get_data__(key, default)
         if isinstance(data, dict) and data:
             return SyncData(filepath=self._filepath, data=data, key_prefix=key)
         return data
 
     def __getitem__(self, __key: Union[str, tuple]):
         if isinstance(__key, tuple):
@@ -334,15 +344,15 @@
     def __get_data__(self, __key: str) -> Optional[None]:
         """Return None if the data doesn't contain key."""
 
     @overload
     def __get_data__(self, __key: str, __default: _T) -> Union[Any, _T]:
         """Return default value if the data doesn't contain key."""
 
-    def __get_data__(self, __key: str, __default: Optional[Any] = None):
+    def __get_data__(self, __key: str, __default: Any = None):
         if __key in self._unopened_keys:
             self._load_from_h5(key=__key)
         data = self._data.get(__key, __default)
         if isinstance(data, NotLoaded):
             self._load_from_h5(key=__key)
             data = self._data.get(__key, __default)
         return data
@@ -410,15 +420,20 @@
 
     def __contains__(self, item):
         return (item in self._data) or (item in self._unopened_keys)
 
     def __dir__(self) -> Iterable[str]:
         return list(self._keys) + self._default_attr
 
-    def save(self, just_update: Union[bool, Iterable[str]] = False, filepath: Optional[str] = None):
+    def save(self,
+             just_update: Union[bool, Iterable[str]] = False,
+             filepath: Optional[str] = None,
+             force: Optional[bool] = None):
+        if just_update is False and force is True:
+            just_update = False
         # print(f"saving globally with {just_update=}")
         if self._read_only is True:
             raise ValueError("Cannot save opened in a read-only mode. Should reopen the file")
         if isinstance(just_update, Iterable):
             last_update = self._last_update.intersection(just_update)
             self._last_update = self._last_update.difference(just_update)
         else:
@@ -492,14 +507,21 @@
     @filepath.setter
     def filepath(self, value: str):
         if not isinstance(value, str):
             value = str(value)
         self._filepath = value if value.endswith('.h5') else value + '.h5'
 
     @property
+    def filename(self) -> Optional[str]:
+        filepath = self.filepath
+        if filepath is None:
+            return None
+        return os.path.basename(filepath)
+
+    @property
     def save_on_edit(self):
         return self._save_on_edit
 
     # def _asdict(self):
     #     return self._data
 
     def asdict(self):
```

### Comparing `labmate-0.6.1/labmate/syncdata_types/h5_np_array.py` & `labmate-0.7.0/labmate/syncdata_types/h5_np_array.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate/utils/random_utils.py` & `labmate-0.7.0/labmate/utils/random_utils.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.1/labmate.egg-info/PKG-INFO` & `labmate-0.7.0/labmate.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: labmate
-Version: 0.6.1
+Version: 0.7.0
 Summary: Data management library to save data and plots to hdf5 files
 Home-page: https://github.com/kyrylo-gr/labmate
 Author: LKB-OMQ
 Author-email: cryo.paris.su@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENCE
 
 ## Install
 
 `pip install labmate`
```

### Comparing `labmate-0.6.1/labmate.egg-info/SOURCES.txt` & `labmate-0.7.0/labmate.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,43 +15,44 @@
 docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
 docs/examples/more/h5nparray.ipynb
 docs/examples/more/loop_example.ipynb
 docs/releases/0.4.0.md
 docs/releases/0.5.0.md
 docs/releases/0.6.0.md
 docs/releases/0.6.1.md
+docs/releases/0.7.0.md
 labmate/__init__.py
 labmate/json_utils.py
 labmate/plt.py
 labmate.egg-info/PKG-INFO
 labmate.egg-info/SOURCES.txt
 labmate.egg-info/dependency_links.txt
 labmate.egg-info/requires.txt
 labmate.egg-info/top_level.txt
 labmate/acquisition/__init__.py
 labmate/acquisition/acquisition_data.py
 labmate/acquisition/acquisition_loop.py
 labmate/acquisition/acquisition_manager.py
 labmate/acquisition/analysis_data.py
 labmate/acquisition/analysis_loop.py
+labmate/acquisition/config_file.py
 labmate/acquisition/lint.py
 labmate/acquisition_notebook/__init__.py
 labmate/acquisition_notebook/acquisition_analysis_manager.py
 labmate/acquisition_notebook/acquisition_magic_class.py
 labmate/attrdict/__init__.py
 labmate/attrdict/attrdict_class.py
 labmate/json/__init__.py
 labmate/json/decoders.py
 labmate/json/encoders.py
 labmate/json/open.py
 labmate/path/__init__.py
 labmate/path/path_class.py
-labmate/plot_utils/__init__.py
-labmate/plot_utils/random_utils.py
 labmate/syncdata/__init__.py
+labmate/syncdata/function_save.py
 labmate/syncdata/h5py_utils.py
 labmate/syncdata/syncdata_class.py
 labmate/syncdata_types/__init__.py
 labmate/syncdata_types/h5_np_array.py
 labmate/utils/__init__.py
 labmate/utils/async_utils.py
 labmate/utils/autoreload.py
```

### Comparing `labmate-0.6.1/setup.py` & `labmate-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='labmate',
-    version="0.6.1",
+    version="0.7.0",
     author="LKB-OMQ",
     author_email="cryo.paris.su@gmail.com",
     description="Data management library to save data and plots to hdf5 files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kyrylo-gr/labmate",
     packages=setuptools.find_packages(exclude=['tests', 'tests.*']),
@@ -20,14 +20,20 @@
     ],
     python_requires='>=3.8',
     install_requires=[
         "numpy",
         "h5py",
     ],
     extras_require={
+        "all": [
+            "matplotlib",
+            "pltsave"
+        ],
         "dev": [
             "matplotlib",
             "pytest",
             "check-manifest",
+            "sphinx",
+            "sphinx_rtd_theme",
         ]
     }
 )
```

