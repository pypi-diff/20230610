# Comparing `tmp/fusion-engine-client-1.20.0rc1.tar.gz` & `tmp/fusion-engine-client-1.20.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.20.0rc1.tar", last modified: Fri Jun  2 20:03:05 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.20.0rc2.tar", last modified: Wed Jun  7 03:33:19 2023, max compression
```

## Comparing `fusion-engine-client-1.20.0rc1.tar` & `fusion-engine-client-1.20.0rc2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    14038 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   110311 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.521266 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56191 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.521266 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.521266 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.800689 fusion-engine-client-1.20.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-07 03:33:19.796688 fusion-engine-client-1.20.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.784688 fusion-engine-client-1.20.0rc2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14038 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.784688 fusion-engine-client-1.20.0rc2/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.788689 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110311 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.792688 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56695 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.792688 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.796688 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.784688 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:33:19.800689 fusion-engine-client-1.20.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.796688 fusion-engine-client-1.20.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.20.0rc1/PKG-INFO` & `fusion-engine-client-1.20.0rc2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc1
+Version: 1.20.0rc2
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc1/README.md` & `fusion-engine-client-1.20.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/bin/p1_extract` & `fusion-engine-client-1.20.0rc2/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/bin/p1_print` & `fusion-engine-client-1.20.0rc2/bin/p1_print`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import Any, Iterable, NamedTuple, Optional, List, Union, Tuple
 
 import construct
 from construct import (Struct, Padding, this, Flag, Bytes, Array,
-                       Float32l, Float64l, Int64ul, Int32ul, Int16ul, Int8ul, Int64sl, Int32sl, Int16sl, Int8sl)
+                       Float32l, Float64l, Int64ul, Int32ul, Int16ul, Int8ul, Int64sl, Int32sl, Int16sl, Int8sl, PaddedString)
 
 from ..utils.construct_utils import NamedTupleAdapter, AutoEnum, construct_message_to_string
 from ..utils.enum_utils import IntEnum
 from .defs import *
 
 
 ################################################################################
@@ -38,14 +38,15 @@
     TROPOSPHERE_CONFIG = 55
     INTERFACE_CONFIG = 200
     UART1_BAUD = 256
     UART2_BAUD = 257
     UART1_OUTPUT_DIAGNOSTICS_MESSAGES = 258
     UART2_OUTPUT_DIAGNOSTICS_MESSAGES = 259
     ENABLE_WATCHDOG_TIMER = 300
+    USER_DEVICE_ID = 301
 
 
 class InterfaceConfigType(IntEnum):
   INVALID = 0
   OUTPUT_DIAGNOSTICS_MESSAGES = 1
   BAUD_RATE = 2
   REMOTE_ADDRESS = 3
@@ -399,14 +400,26 @@
         value: bool = False
 
     # Construct to serialize 8 bit boolean types.
     BoolConstruct = Struct(
         "value" / Flag,
     )
 
+    class StringVal(NamedTuple):
+        """!
+        @brief String value specifier.
+        """
+        value: str = ""
+
+    @staticmethod
+    def StringConstruct(max_len):
+        return Struct(
+            "value" / PaddedString(max_len, 'utf8'),
+        )
+
     class SatelliteTypeMaskVal(IntegerVal):
         """!
         @brief Bitmask specifying enabled @ref SatelliteType%s.
         """
         def __new__(cls, *args, **kwargs):
             # Check if the user specified a single SatelliteType or a list of values, and convert to a mask.
             if len(args) == 1:
@@ -747,14 +760,22 @@
 class WatchdogTimerEnabled(_conf_gen.BoolVal):
     """!
     @brief Enable watchdog timer to restart device after fatal errors.
     """
     pass
 
 
+@_conf_gen.create_config_class(ConfigType.USER_DEVICE_ID, _conf_gen.StringConstruct(32))
+class UserDeviceID(_conf_gen.StringVal):
+    """!
+    @brief A string for identifying a device.
+    """
+    pass
+
+
 @_conf_gen.create_config_class(ConfigType.DEVICE_COARSE_ORIENTATION, _conf_gen.CoarseOrientationConstruct)
 class DeviceCourseOrientationConfig(_conf_gen.CoarseOrientation):
     """!
     @brief The orientation of a device with respect to the vehicle body axes.
 
     A device's orientation is defined by specifying how the +x and +z axes of its
     IMU are aligned with the vehicle body axes. For example, in a car:
```

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,29 +456,29 @@
     def unpack(self, buffer: bytes, offset: int = 0, message_version: int = MessagePayload._UNSPECIFIED_VERSION) -> int:
         parsed = self.DeviceIDMessageConstruct.parse(buffer[offset:])
         self.__dict__.update(parsed)
         return parsed._io.tell()
 
     @staticmethod
     def _get_str(msg: bytes) -> str:
-        is_printable = all(b in DeviceIDMessage.__PRINTABLE_CHARS for b in msg)
+        is_printable = all(b in DeviceIDMessage._PRINTABLE_CHARS for b in msg)
         if is_printable:
             return msg.decode('ascii')
         else:
             return '[' + ' '.join(f'{b:02X}' for b in msg) + ']'
 
     def __repr__(self):
         result = super().__repr__()[:-1]
         result += f'type={self.device_type}, hw={self._get_str(self.hw_id_data)}, user={self._get_str(self.user_id_data)},\
             rx={self._get_str(self.receiver_id_data)}'
         return result
 
     def __str__(self):
         string = f'Device ID Info @ %s\n' % system_time_to_str(self.system_time_ns)
-        string += f'  Device Type: {device_type}\n'
+        string += f'  Device Type: {self.device_type}\n'
         string += f'  HW ID: {self._get_str(self.hw_id_data)}\n'
         string += f'  User ID: {self._get_str(self.user_id_data)}\n'
         string += f'  Receiver ID: {self._get_str(self.receiver_id_data)}'
         return string
 
     def calcsize(self) -> int:
         return len(self.pack())
```

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc1
+Version: 1.20.0rc2
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/setup.py` & `fusion-engine-client-1.20.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_config.py` & `fusion-engine-client-1.20.0rc2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_construct_utils.py` & `fusion-engine-client-1.20.0rc2/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_data_loader.py` & `fusion-engine-client-1.20.0rc2/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_decoder.py` & `fusion-engine-client-1.20.0rc2/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_encoder.py` & `fusion-engine-client-1.20.0rc2/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_enum_utils.py` & `fusion-engine-client-1.20.0rc2/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_file_index.py` & `fusion-engine-client-1.20.0rc2/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_message_defs.py` & `fusion-engine-client-1.20.0rc2/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.20.0rc2/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc1/tests/test_time_range.py` & `fusion-engine-client-1.20.0rc2/tests/test_time_range.py`

 * *Files identical despite different names*

