# Comparing `tmp/subaligner-0.3.2.tar.gz` & `tmp/subaligner-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/subaligner-0.3.2.tar", last modified: Fri Jun  9 08:44:02 2023, max compression
+gzip compressed data, was "subaligner-0.3.3.tar", last modified: Fri Jun  9 18:01:02 2023, max compression
```

## Comparing `subaligner-0.3.2.tar` & `subaligner-0.3.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.924129 subaligner-0.3.2/
--rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.2/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.2/MANIFEST.in
--rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 08:44:02.923299 subaligner-0.3.2/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     9247 2023-04-15 17:31:09.000000 subaligner-0.3.2/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.838080 subaligner-0.3.2/bin/
--rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.2/bin/subaligner
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.2/bin/subaligner_1pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.2/bin/subaligner_2pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.2/bin/subaligner_batch
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.2/bin/subaligner_convert
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.2/bin/subaligner_train
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.2/bin/subaligner_tune
--rw-r--r--   0 macbook    (501) staff       (20)     1185 2023-06-09 08:34:37.000000 subaligner-0.3.2/requirements.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-09 08:44:02.924259 subaligner-0.3.2/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     3748 2023-06-08 23:47:15.000000 subaligner-0.3.2/setup.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.857194 subaligner-0.3.2/subaligner/
--rw-r--r--   0 macbook    (501) staff       (20)      258 2023-03-11 16:33:37.000000 subaligner-0.3.2/subaligner/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.2/subaligner/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)       64 2023-06-08 23:53:14.000000 subaligner-0.3.2/subaligner/_version.py
--rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/embedder.py
--rw-r--r--   0 macbook    (501) staff       (20)      511 2023-03-11 23:58:14.000000 subaligner-0.3.2/subaligner/exception.py
--rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/hparam_tuner.py
--rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/hyperparameters.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.898772 subaligner-0.3.2/subaligner/lib/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/lib/language.py
--rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/lib/to_srt.py
--rw-r--r--   0 macbook    (501) staff       (20)      709 2023-03-19 19:33:51.000000 subaligner-0.3.2/subaligner/llm.py
--rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)    18286 2023-03-17 01:31:21.000000 subaligner-0.3.2/subaligner/media_helper.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.825985 subaligner-0.3.2/subaligner/models/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.826714 subaligner-0.3.2/subaligner/models/training/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.899902 subaligner-0.3.2/subaligner/models/training/config/
--rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/config/hyperparameters.json
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.901364 subaligner-0.3.2/subaligner/models/training/model/
--rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/model/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/model/model.hdf5
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.909729 subaligner-0.3.2/subaligner/models/training/weights/
--rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/weights/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/weights/weights.hdf5
--rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/network.py
--rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/singleton.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.917547 subaligner-0.3.2/subaligner/subaligner_1pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_1pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/subaligner_1pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.918511 subaligner-0.3.2/subaligner/subaligner_2pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_2pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/subaligner_2pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.919743 subaligner-0.3.2/subaligner/subaligner_batch/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_batch/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.2/subaligner/subaligner_batch/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.920607 subaligner-0.3.2/subaligner/subaligner_convert/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_convert/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/subaligner_convert/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.921531 subaligner-0.3.2/subaligner/subaligner_train/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_train/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.2/subaligner/subaligner_train/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.922414 subaligner-0.3.2/subaligner/subaligner_tune/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_tune/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_tune/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-04-15 16:48:57.000000 subaligner-0.3.2/subaligner/subtitle.py
--rw-r--r--   0 macbook    (501) staff       (20)    15876 2023-06-06 00:57:05.000000 subaligner-0.3.2/subaligner/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     4745 2023-06-06 00:48:48.000000 subaligner-0.3.2/subaligner/transcriber.py
--rw-r--r--   0 macbook    (501) staff       (20)    12182 2023-06-06 09:49:57.000000 subaligner-0.3.2/subaligner/translator.py
--rw-r--r--   0 macbook    (501) staff       (20)    33741 2023-03-17 02:05:09.000000 subaligner-0.3.2/subaligner/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.896669 subaligner-0.3.2/subaligner.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1628 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      424 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)     2015 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.260026 subaligner-0.3.3/
+-rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.3/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.3/MANIFEST.in
+-rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 18:01:02.259467 subaligner-0.3.3/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     9247 2023-04-15 17:31:09.000000 subaligner-0.3.3/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.176880 subaligner-0.3.3/bin/
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.3/bin/subaligner
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.3/bin/subaligner_1pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.3/bin/subaligner_2pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.3/bin/subaligner_batch
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.3/bin/subaligner_convert
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.3/bin/subaligner_train
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.3/bin/subaligner_tune
+-rw-r--r--   0 macbook    (501) staff       (20)     1185 2023-06-09 08:34:37.000000 subaligner-0.3.3/requirements.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-09 18:01:02.260151 subaligner-0.3.3/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     3748 2023-06-08 23:47:15.000000 subaligner-0.3.3/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.197970 subaligner-0.3.3/subaligner/
+-rw-r--r--   0 macbook    (501) staff       (20)      258 2023-03-11 16:33:37.000000 subaligner-0.3.3/subaligner/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.3/subaligner/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)       64 2023-06-09 17:58:20.000000 subaligner-0.3.3/subaligner/_version.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/embedder.py
+-rw-r--r--   0 macbook    (501) staff       (20)      511 2023-03-11 23:58:14.000000 subaligner-0.3.3/subaligner/exception.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/hparam_tuner.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/hyperparameters.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.231693 subaligner-0.3.3/subaligner/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/lib/language.py
+-rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/lib/to_srt.py
+-rw-r--r--   0 macbook    (501) staff       (20)      709 2023-03-19 19:33:51.000000 subaligner-0.3.3/subaligner/llm.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)    18286 2023-03-17 01:31:21.000000 subaligner-0.3.3/subaligner/media_helper.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.164770 subaligner-0.3.3/subaligner/models/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.165377 subaligner-0.3.3/subaligner/models/training/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.233276 subaligner-0.3.3/subaligner/models/training/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/config/hyperparameters.json
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.234957 subaligner-0.3.3/subaligner/models/training/model/
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/model/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/model/model.hdf5
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.247728 subaligner-0.3.3/subaligner/models/training/weights/
+-rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/weights/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/weights/weights.hdf5
+-rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/network.py
+-rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/singleton.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.254200 subaligner-0.3.3/subaligner/subaligner_1pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_1pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/subaligner_1pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.255055 subaligner-0.3.3/subaligner/subaligner_2pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_2pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/subaligner_2pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.256216 subaligner-0.3.3/subaligner/subaligner_batch/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_batch/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.3/subaligner/subaligner_batch/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.257204 subaligner-0.3.3/subaligner/subaligner_convert/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_convert/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/subaligner_convert/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.258139 subaligner-0.3.3/subaligner/subaligner_train/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_train/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.3/subaligner/subaligner_train/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.258912 subaligner-0.3.3/subaligner/subaligner_tune/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_tune/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_tune/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-04-15 16:48:57.000000 subaligner-0.3.3/subaligner/subtitle.py
+-rw-r--r--   0 macbook    (501) staff       (20)    15876 2023-06-06 00:57:05.000000 subaligner-0.3.3/subaligner/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4695 2023-06-09 19:42:27.000000 subaligner-0.3.3/subaligner/transcriber.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12182 2023-06-06 09:49:57.000000 subaligner-0.3.3/subaligner/translator.py
+-rw-r--r--   0 macbook    (501) staff       (20)    33741 2023-03-17 02:05:09.000000 subaligner-0.3.3/subaligner/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.228454 subaligner-0.3.3/subaligner.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1628 2023-06-09 18:01:02.000000 subaligner-0.3.3/subaligner.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      424 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)     2015 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/top_level.txt
```

### Comparing `subaligner-0.3.2/LICENSE` & `subaligner-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/PKG-INFO` & `subaligner-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subaligner
-Version: 0.3.2
+Version: 0.3.3
 Summary: Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.
 Home-page: https://subaligner.readthedocs.io/en/latest/
 Author: Xi Bai
 Author-email: xi.bai.ed@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `subaligner-0.3.2/README.md` & `subaligner-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/bin/subaligner` & `subaligner-0.3.3/bin/subaligner`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/bin/subaligner_1pass` & `subaligner-0.3.3/bin/subaligner_1pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/bin/subaligner_2pass` & `subaligner-0.3.3/bin/subaligner_2pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/bin/subaligner_batch` & `subaligner-0.3.3/bin/subaligner_batch`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/bin/subaligner_convert` & `subaligner-0.3.3/bin/subaligner_convert`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/bin/subaligner_train` & `subaligner-0.3.3/bin/subaligner_train`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/bin/subaligner_tune` & `subaligner-0.3.3/bin/subaligner_tune`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/requirements.txt` & `subaligner-0.3.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/setup.py` & `subaligner-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/__main__.py` & `subaligner-0.3.3/subaligner/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/embedder.py` & `subaligner-0.3.3/subaligner/embedder.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/hparam_tuner.py` & `subaligner-0.3.3/subaligner/hparam_tuner.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/hyperparameters.py` & `subaligner-0.3.3/subaligner/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/lib/language.py` & `subaligner-0.3.3/subaligner/lib/language.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/lib/to_srt.py` & `subaligner-0.3.3/subaligner/lib/to_srt.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/llm.py` & `subaligner-0.3.3/subaligner/llm.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/logger.py` & `subaligner-0.3.3/subaligner/logger.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/media_helper.py` & `subaligner-0.3.3/subaligner/media_helper.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/models/training/config/hyperparameters.json` & `subaligner-0.3.3/subaligner/models/training/config/hyperparameters.json`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/models/training/model/model.hdf5` & `subaligner-0.3.3/subaligner/models/training/model/model.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/models/training/weights/weights.hdf5` & `subaligner-0.3.3/subaligner/models/training/weights/weights.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/network.py` & `subaligner-0.3.3/subaligner/network.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/predictor.py` & `subaligner-0.3.3/subaligner/predictor.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/subaligner_1pass/__main__.py` & `subaligner-0.3.3/subaligner/subaligner_1pass/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/subaligner_2pass/__main__.py` & `subaligner-0.3.3/subaligner/subaligner_2pass/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/subaligner_batch/__main__.py` & `subaligner-0.3.3/subaligner/subaligner_batch/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/subaligner_convert/__main__.py` & `subaligner-0.3.3/subaligner/subaligner_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/subaligner_train/__main__.py` & `subaligner-0.3.3/subaligner/subaligner_train/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/subaligner_tune/__main__.py` & `subaligner-0.3.3/subaligner/subaligner_tune/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/subtitle.py` & `subaligner-0.3.3/subaligner/subtitle.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/trainer.py` & `subaligner-0.3.3/subaligner/trainer.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/transcriber.py` & `subaligner-0.3.3/subaligner/transcriber.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             lang = Utils.get_iso_639_alpha_2(language_code)
             if lang not in LANGUAGES:
                 raise TranscriptionException(f'"{language_code}" is not supported by {self.__recipe} ({self.__flavour})')
             audio_file_path = self.__media_helper.extract_audio(video_file_path, True, 16000)
             try:
                 audio = whisper.load_audio(audio_file_path)
                 self.__LOGGER.debug("Start transcribing the audio...")
-                result = self.__model.transcribe(audio, task="transcribe", language=LANGUAGES[lang], logprob_threshold=-1.2, no_speech_threshold=0.16)
+                result = self.__model.transcribe(audio, task="transcribe", language=LANGUAGES[lang])
                 self.__LOGGER.info("Finished transcribing the audio")
                 srt_str = ""
                 for i, segment in enumerate(result["segments"], start=1):
                     srt_str += f"{i}\n" \
                                f"{Utils.format_timestamp(segment['start'])} --> {Utils.format_timestamp(segment['end'])}\n" \
                                f"{segment['text'].strip().replace('-->', '->')}\n" \
                                "\n"
```

### Comparing `subaligner-0.3.2/subaligner/translator.py` & `subaligner-0.3.3/subaligner/translator.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner/utils.py` & `subaligner-0.3.3/subaligner/utils.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner.egg-info/PKG-INFO` & `subaligner-0.3.3/subaligner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subaligner
-Version: 0.3.2
+Version: 0.3.3
 Summary: Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.
 Home-page: https://subaligner.readthedocs.io/en/latest/
 Author: Xi Bai
 Author-email: xi.bai.ed@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `subaligner-0.3.2/subaligner.egg-info/SOURCES.txt` & `subaligner-0.3.3/subaligner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.2/subaligner.egg-info/requires.txt` & `subaligner-0.3.3/subaligner.egg-info/requires.txt`

 * *Files identical despite different names*

