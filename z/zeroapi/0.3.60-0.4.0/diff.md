# Comparing `tmp/zeroapi-0.3.60.tar.gz` & `tmp/zeroapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroapi-0.3.60.tar", last modified: Sat Apr  8 11:59:11 2023, max compression
+gzip compressed data, was "zeroapi-0.4.0.tar", last modified: Sat Jun 10 07:15:42 2023, max compression
```

## Comparing `zeroapi-0.3.60.tar` & `zeroapi-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,74 @@
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.963293 zeroapi-0.3.60/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1076 2023-03-26 09:01:39.000000 zeroapi-0.3.60/LICENSE
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     7325 2023-04-08 11:59:11.963293 zeroapi-0.3.60/PKG-INFO
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     6826 2023-04-08 09:23:27.000000 zeroapi-0.3.60/README.md
--rw-rw-r--   0 ananto    (1000) ananto    (1000)       38 2023-04-08 11:59:11.963293 zeroapi-0.3.60/setup.cfg
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      791 2023-04-08 11:58:50.000000 zeroapi-0.3.60/setup.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.959293 zeroapi-0.3.60/zero/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      255 2023-04-07 20:48:30.000000 zeroapi-0.3.60/zero/__init__.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.959293 zeroapi-0.3.60/zero/client_server/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:04:57.000000 zeroapi-0.3.60/zero/client_server/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)    11147 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/client_server/client.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     6494 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/client_server/server.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3943 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/client_server/worker.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.959293 zeroapi-0.3.60/zero/codegen/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:02.000000 zeroapi-0.3.60/zero/codegen/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3187 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/codegen/codegen.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      277 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/config.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.959293 zeroapi-0.3.60/zero/encoder/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)       64 2023-04-07 21:02:10.000000 zeroapi-0.3.60/zero/encoder/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      214 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/encoder/factory.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      206 2023-04-02 08:45:25.000000 zeroapi-0.3.60/zero/encoder/msgpk.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      213 2023-04-02 08:45:25.000000 zeroapi-0.3.60/zero/encoder/protocols.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      246 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/error.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1617 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/generate_client.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     2213 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/logger.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.959293 zeroapi-0.3.60/zero/pubsub/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:08.000000 zeroapi-0.3.60/zero/pubsub/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1290 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/pubsub/publisher.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3261 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/pubsub/subscriber.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.959293 zeroapi-0.3.60/zero/utils/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:11.000000 zeroapi-0.3.60/zero/utils/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     4236 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/utils/type_util.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     2030 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/utils/util.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.963293 zeroapi-0.3.60/zero/zero_mq/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      157 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/zero_mq/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      935 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/zero_mq/factory.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      712 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/zero_mq/helpers.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1451 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/zero_mq/protocols.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.963293 zeroapi-0.3.60/zero/zero_mq/queue_device/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      118 2023-04-07 21:03:06.000000 zeroapi-0.3.60/zero/zero_mq/queue_device/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      611 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/zero_mq/queue_device/broker.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     4268 2023-04-08 09:13:20.000000 zeroapi-0.3.60/zero/zero_mq/queue_device/client.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1334 2023-04-08 08:04:49.000000 zeroapi-0.3.60/zero/zero_mq/queue_device/worker.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-04-08 11:59:11.963293 zeroapi-0.3.60/zeroapi.egg-info/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     7325 2023-04-08 11:59:11.000000 zeroapi-0.3.60/zeroapi.egg-info/PKG-INFO
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      973 2023-04-08 11:59:11.000000 zeroapi-0.3.60/zeroapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        1 2023-04-08 11:59:11.000000 zeroapi-0.3.60/zeroapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ananto    (1000) ananto    (1000)       14 2023-04-08 11:59:11.000000 zeroapi-0.3.60/zeroapi.egg-info/requires.txt
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        5 2023-04-08 11:59:11.000000 zeroapi-0.3.60/zeroapi.egg-info/top_level.txt
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1076 2023-03-26 09:01:39.000000 zeroapi-0.4.0/LICENSE
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8831 2023-06-10 07:15:42.098272 zeroapi-0.4.0/PKG-INFO
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8333 2023-06-10 07:13:54.000000 zeroapi-0.4.0/README.md
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       38 2023-06-10 07:15:42.098272 zeroapi-0.4.0/setup.cfg
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      790 2023-06-10 07:13:37.000000 zeroapi-0.4.0/setup.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.090273 zeroapi-0.4.0/tests/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      105 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/constants.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.090273 zeroapi-0.4.0/tests/functional/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/__init__.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.090273 zeroapi-0.4.0/tests/functional/multiple_servers/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/multiple_servers/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1012 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/client_inside_server_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      629 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/conftest.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3270 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/multiple_clients_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      303 2023-04-02 19:24:48.000000 zeroapi-0.4.0/tests/functional/multiple_servers/server1.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      823 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/server2.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.094272 zeroapi-0.4.0/tests/functional/single_server/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/single_server/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3171 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/single_server/client_generation_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     2859 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/single_server/client_server_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     5040 2023-05-14 21:11:59.000000 zeroapi-0.4.0/tests/functional/single_server/client_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      370 2023-04-08 08:04:49.000000 zeroapi-0.4.0/tests/functional/single_server/conftest.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3512 2023-04-08 08:04:49.000000 zeroapi-0.4.0/tests/functional/single_server/register_rpc_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1941 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/single_server/server.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      937 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/single_server/server_test.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.094272 zeroapi-0.4.0/tests/unit/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/unit/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8944 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/unit/test_server.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1401 2023-04-08 08:04:49.000000 zeroapi-0.4.0/tests/utils.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      329 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/__init__.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/client_server/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:04:57.000000 zeroapi-0.4.0/zero/client_server/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)    12081 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/client_server/client.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     6612 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/client_server/server.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3943 2023-05-30 19:54:56.000000 zeroapi-0.4.0/zero/client_server/worker.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/codegen/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:02.000000 zeroapi-0.4.0/zero/codegen/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3091 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/codegen/codegen.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      277 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/config.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/encoder/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       64 2023-04-07 21:02:10.000000 zeroapi-0.4.0/zero/encoder/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      215 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/encoder/factory.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      412 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/encoder/msgspc.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      277 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/encoder/protocols.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      246 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/error.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1617 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/generate_client.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     2213 2023-04-08 09:13:20.000000 zeroapi-0.4.0/zero/logger.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/pubsub/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:08.000000 zeroapi-0.4.0/zero/pubsub/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1330 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/pubsub/publisher.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3268 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/pubsub/subscriber.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/utils/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:11.000000 zeroapi-0.4.0/zero/utils/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     4455 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/utils/type_util.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     2030 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/utils/util.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/zero_mq/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      157 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      935 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/factory.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      712 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/helpers.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1451 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/protocols.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/zero_mq/queue_device/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      118 2023-04-07 21:03:06.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      611 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/broker.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     4268 2023-04-08 09:13:20.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/client.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1334 2023-05-14 21:11:59.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/worker.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zeroapi.egg-info/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8831 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1829 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        1 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       14 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/requires.txt
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       11 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/top_level.txt
```

### Comparing `zeroapi-0.3.60/LICENSE` & `zeroapi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/PKG-INFO` & `zeroapi-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: zeroapi
-Version: 0.3.60
-Summary: Zero is a RPC framework to build fast and high performance Python microservices
-Home-page: https://github.com/Ananto30/zero
-Author: Azizul Haque Ananto
-Author-email: azizulhaq.ananto@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
     <img height="300px" src="https://ananto30.github.io/i/1200xCL_TP.png" />
 </p>
 <p align="center">
     <em>Zero is a simple Python framework (RPC like) to build fast and high performance microservices or distributed servers</em>
 </p>
 <p align="center">
@@ -36,115 +21,164 @@
 </p>
 <hr>
 
 **Features**:
 
 *   Zero provides **faster communication** (see [benchmarks](https://github.com/Ananto30/zero#benchmarks-)) between the microservices using [zeromq](https://zeromq.org/) under the hood.
 *   Zero uses messages for communication and traditional **client-server** or **request-reply** pattern is supported.
-*   Support for both **Async** and **sync**.
+*   Support for both **async** and **sync**.
 *   The base server (ZeroServer) **utilizes all cpu cores**.
 *   **Code generation**! See [example](https://github.com/Ananto30/zero#code-generation-) 👇
 
 **Philosophy** behind Zero:
 
-*   **Zero learning curve**: The learning curve is tends to zero. You just add your functions and spin up a server, literally that's it! The framework hides the complexity of messaging pattern that enables faster communication.
+*   **Zero learning curve**: The learning curve is tends to zero. Just add functions and spin up a server, literally that's it! The framework hides the complexity of messaging pattern that enables faster communication.
 *   **ZeroMQ**: An awesome messaging library enables the power of Zero.
 
 Let's get started!
 
 # Getting started 🚀
 
 *Ensure Python 3.8+*
 
     pip install zeroapi
 
 **For Windows**, [tornado](https://pypi.org/project/tornado/) needs to be installed separately (for async operations). It's not included with `zeroapi` because for linux and mac-os, tornado is not needed as they have their own event loops.
 
 *   Create a `server.py`
 
-```python
-from zero import ZeroServer
+    ```python
+    from zero import ZeroServer
 
-app = ZeroServer(port=5559)
+    app = ZeroServer(port=5559)
 
-@app.register_rpc
-def echo(msg: str) -> str:
-    return msg
+    @app.register_rpc
+    def echo(msg: str) -> str:
+        return msg
 
-@app.register_rpc
-async def hello_world() -> str:
-    return "hello world"
-
-
-if __name__ == "__main__":
-    app.run()
-```
+    @app.register_rpc
+    async def hello_world() -> str:
+        return "hello world"
 
-Please note that server **RPC methods are type hinted**. Type hint is **must** in Zero server.
 
-*See the method type async or sync, doesn't matter.* 😃
+    if __name__ == "__main__":
+        app.run()
+    ```
 
-*   Run it
+*   The **RPC functions only support one argument** (`msg`) for now.
 
-<!---->
+*   Also note that server **RPC functions are type hinted**. Type hint is **must** in Zero server. Supported types can be found [here](/zero/utils/type_util.py#L11).
 
+*   Run the server
+    ```shell
     python -m server
+    ```
 
 *   Call the rpc methods
 
-```python
-from zero import ZeroClient
+    ```python
+    from zero import ZeroClient
 
-zero_client = ZeroClient("localhost", 5559)
+    zero_client = ZeroClient("localhost", 5559)
 
-def echo():
-    resp = zero_client.call("echo", "Hi there!")
-    print(resp)
-
-def hello():
-    resp = zero_client.call("hello_world", None)
-    print(resp)
+    def echo():
+        resp = zero_client.call("echo", "Hi there!")
+        print(resp)
 
+    def hello():
+        resp = zero_client.call("hello_world", None)
+        print(resp)
 
-if __name__ == "__main__":
-    echo()
-    hello()
-```
 
-Or using async client -
+    if __name__ == "__main__":
+        echo()
+        hello()
+    ```
+
+*   Or using async client -
+
+    ```python
+    import asyncio
+
+    from zero import AsyncZeroClient
+
+    zero_client = AsyncZeroClient("localhost", 5559)
+
+    async def echo():
+        resp = await zero_client.call("echo", "Hi there!")
+        print(resp)
+
+    async def hello():
+        resp = await zero_client.call("hello_world", None)
+        print(resp)
+
+
+    if __name__ == "__main__":
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(echo())
+        loop.run_until_complete(hello())
+    ```
+
+# Serialization 📦
+
+## Default serializer
+
+[Msgspec](https://jcristharif.com/msgspec/) is the default serializer. So `msgspec.Struct` (for high performance) or `dataclass` or any [supported types](https://jcristharif.com/msgspec/supported-types.html) can be used easily to pass complex arguments, i.e.
 
 ```python
-import asyncio
+from dataclasses import dataclass
+from msgspec import Struct
+from zero import ZeroServer
 
-from zero import AsyncZeroClient
+app = ZeroServer()
 
-zero_client = AsyncZeroClient("localhost", 5559)
+class Person(Struct):
+    name: str
+    age: int
+    dob: datetime
+
+@dataclass
+class Order:
+    id: int
+    amount: float
+    created_at: datetime
 
-async def echo():
-    resp = await zero_client.call("echo", "Hi there!")
-    print(resp)
+@app.register_rpc
+def save_person(person: Person) -> None:
+    # save person to db
+    ...
 
-async def hello():
-    resp = await zero_client.call("hello_world", None)
-    print(resp)
+@app.register_rpc
+def save_order(order: Order) -> None:
+    # save order to db
+    ...
+```
 
+## Return type
 
-if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(echo())
-    loop.run_until_complete(hello())
+The return type of the RPC function can be any of the [supported types](https://jcristharif.com/msgspec/supported-types.html). If `return_type` is set in the client `call` method, then the return type will be converted to that type.
+
+```python
+@dataclass
+class Order:
+    id: int
+    amount: float
+    created_at: datetime
+
+def get_order(id: str) -> Order:
+    return zero_client.call("get_order", id, return_type=Order)
 ```
 
-# Code Generation! 🙌
+# Code Generation 🤖
 
-You can also use our code generation tool to generate Python client code!
+Easy to use code generation tool is also provided!
 
-After running the server, like above, you can call the server to get the client code.
+After running the server, like above, call the server to get the client code. This makes it easy to know what functions are available in the local or remote server.
 
-Using `zero.generate_client` you can generate client code for even remote servers using the `--host` and `--port` options. You don't need access to the code 😃
+Using `zero.generate_client` generate client code for even remote servers using the `--host` and `--port` options.
 
 ```shell
 python -m zero.generate_client --host localhost --port 5559 --overwrite-dir ./my_client
 ```
 
 It will generate client like this -
 
@@ -178,22 +212,24 @@
 if __name__ == "__main__":
     client.echo("Hi there!")
     client.hello_world(None)
 ```
 
 Currently, the code generation tool supports only `ZeroClient` and not `AsyncZeroClient`.
 
+*WIP - Generate models from server code.*
+
 # Important notes 📝
 
 *   `ZeroServer` should always be run under `if __name__ == "__main__":`, as it uses multiprocessing.
-*   The methods which are under `register_rpc()` in `ZeroServer` should have **type hinting**, like `def echo(msg: str):`
+*   The methods which are under `register_rpc()` in `ZeroServer` should have **type hinting**, like `def echo(msg: str) -> str:`
 
-# Let's do some benchmarking 🤘
+# Let's do some benchmarking! 🏎
 
-Zero is talking about inter service communication. In most real life scenarios, we need to call another microservice.
+Zero is all about inter service communication. In most real life scenarios, we need to call another microservice.
 
 So we will be testing a gateway calling another server for some data. Check the [benchmark/dockerize](https://github.com/Ananto30/zero/tree/main/benchmarks/dockerize) folder for details.
 
 There are two endpoints in every tests,
 
 *   `/hello`: Just call for a hello world response 😅
 *   `/order`: Save a Order object in redis
@@ -213,17 +249,17 @@
 fastApi     | 9590.96               | 18.31            | 6669.81            | 24.41
 sanic       | 18790.49              | 8.69             | 12259.29           | 13.52
 zero(sync)  | 24805.61              | 4.57             | 16498.83           | 7.80
 zero(async) | 22716.84              | 5.61             | 17446.19           | 7.24
 
 # Roadmap 🗺
 
-*   \[ ] Make msgspec as default serializer
-*   \[ ] Add support for async server (currently the sync server runs async functions in the eventloop, which is blocking)
-*   \[ ] Add pub/sub support
+*   [x] Make msgspec as default serializer
+*   [ ] Add support for async server (currently the sync server runs async functions in the eventloop, which is blocking)
+*   [ ] Add pub/sub support
 
 # Contribution
 
 Contributors are welcomed 🙏
 
 **Please leave a star ⭐ if you like Zero!**
```

### Comparing `zeroapi-0.3.60/README.md` & `zeroapi-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: zeroapi
+Version: 0.4.0
+Summary: Zero is a RPC framework to build fast and high performance Python microservices
+Home-page: https://github.com/Ananto30/zero
+Author: Azizul Haque Ananto
+Author-email: azizulhaq.ananto@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
     <img height="300px" src="https://ananto30.github.io/i/1200xCL_TP.png" />
 </p>
 <p align="center">
     <em>Zero is a simple Python framework (RPC like) to build fast and high performance microservices or distributed servers</em>
 </p>
 <p align="center">
@@ -21,115 +36,164 @@
 </p>
 <hr>
 
 **Features**:
 
 *   Zero provides **faster communication** (see [benchmarks](https://github.com/Ananto30/zero#benchmarks-)) between the microservices using [zeromq](https://zeromq.org/) under the hood.
 *   Zero uses messages for communication and traditional **client-server** or **request-reply** pattern is supported.
-*   Support for both **Async** and **sync**.
+*   Support for both **async** and **sync**.
 *   The base server (ZeroServer) **utilizes all cpu cores**.
 *   **Code generation**! See [example](https://github.com/Ananto30/zero#code-generation-) 👇
 
 **Philosophy** behind Zero:
 
-*   **Zero learning curve**: The learning curve is tends to zero. You just add your functions and spin up a server, literally that's it! The framework hides the complexity of messaging pattern that enables faster communication.
+*   **Zero learning curve**: The learning curve is tends to zero. Just add functions and spin up a server, literally that's it! The framework hides the complexity of messaging pattern that enables faster communication.
 *   **ZeroMQ**: An awesome messaging library enables the power of Zero.
 
 Let's get started!
 
 # Getting started 🚀
 
 *Ensure Python 3.8+*
 
     pip install zeroapi
 
 **For Windows**, [tornado](https://pypi.org/project/tornado/) needs to be installed separately (for async operations). It's not included with `zeroapi` because for linux and mac-os, tornado is not needed as they have their own event loops.
 
 *   Create a `server.py`
 
-```python
-from zero import ZeroServer
+    ```python
+    from zero import ZeroServer
 
-app = ZeroServer(port=5559)
+    app = ZeroServer(port=5559)
 
-@app.register_rpc
-def echo(msg: str) -> str:
-    return msg
+    @app.register_rpc
+    def echo(msg: str) -> str:
+        return msg
 
-@app.register_rpc
-async def hello_world() -> str:
-    return "hello world"
-
-
-if __name__ == "__main__":
-    app.run()
-```
+    @app.register_rpc
+    async def hello_world() -> str:
+        return "hello world"
 
-Please note that server **RPC methods are type hinted**. Type hint is **must** in Zero server.
 
-*See the method type async or sync, doesn't matter.* 😃
+    if __name__ == "__main__":
+        app.run()
+    ```
 
-*   Run it
+*   The **RPC functions only support one argument** (`msg`) for now.
 
-<!---->
+*   Also note that server **RPC functions are type hinted**. Type hint is **must** in Zero server. Supported types can be found [here](/zero/utils/type_util.py#L11).
 
+*   Run the server
+    ```shell
     python -m server
+    ```
 
 *   Call the rpc methods
 
-```python
-from zero import ZeroClient
+    ```python
+    from zero import ZeroClient
 
-zero_client = ZeroClient("localhost", 5559)
+    zero_client = ZeroClient("localhost", 5559)
 
-def echo():
-    resp = zero_client.call("echo", "Hi there!")
-    print(resp)
-
-def hello():
-    resp = zero_client.call("hello_world", None)
-    print(resp)
+    def echo():
+        resp = zero_client.call("echo", "Hi there!")
+        print(resp)
 
+    def hello():
+        resp = zero_client.call("hello_world", None)
+        print(resp)
 
-if __name__ == "__main__":
-    echo()
-    hello()
-```
 
-Or using async client -
+    if __name__ == "__main__":
+        echo()
+        hello()
+    ```
+
+*   Or using async client -
+
+    ```python
+    import asyncio
+
+    from zero import AsyncZeroClient
+
+    zero_client = AsyncZeroClient("localhost", 5559)
+
+    async def echo():
+        resp = await zero_client.call("echo", "Hi there!")
+        print(resp)
+
+    async def hello():
+        resp = await zero_client.call("hello_world", None)
+        print(resp)
+
+
+    if __name__ == "__main__":
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(echo())
+        loop.run_until_complete(hello())
+    ```
+
+# Serialization 📦
+
+## Default serializer
+
+[Msgspec](https://jcristharif.com/msgspec/) is the default serializer. So `msgspec.Struct` (for high performance) or `dataclass` or any [supported types](https://jcristharif.com/msgspec/supported-types.html) can be used easily to pass complex arguments, i.e.
 
 ```python
-import asyncio
+from dataclasses import dataclass
+from msgspec import Struct
+from zero import ZeroServer
 
-from zero import AsyncZeroClient
+app = ZeroServer()
 
-zero_client = AsyncZeroClient("localhost", 5559)
+class Person(Struct):
+    name: str
+    age: int
+    dob: datetime
+
+@dataclass
+class Order:
+    id: int
+    amount: float
+    created_at: datetime
 
-async def echo():
-    resp = await zero_client.call("echo", "Hi there!")
-    print(resp)
+@app.register_rpc
+def save_person(person: Person) -> None:
+    # save person to db
+    ...
 
-async def hello():
-    resp = await zero_client.call("hello_world", None)
-    print(resp)
+@app.register_rpc
+def save_order(order: Order) -> None:
+    # save order to db
+    ...
+```
 
+## Return type
 
-if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(echo())
-    loop.run_until_complete(hello())
+The return type of the RPC function can be any of the [supported types](https://jcristharif.com/msgspec/supported-types.html). If `return_type` is set in the client `call` method, then the return type will be converted to that type.
+
+```python
+@dataclass
+class Order:
+    id: int
+    amount: float
+    created_at: datetime
+
+def get_order(id: str) -> Order:
+    return zero_client.call("get_order", id, return_type=Order)
 ```
 
-# Code Generation! 🙌
+# Code Generation 🤖
 
-You can also use our code generation tool to generate Python client code!
+Easy to use code generation tool is also provided!
 
-After running the server, like above, you can call the server to get the client code.
+After running the server, like above, call the server to get the client code. This makes it easy to know what functions are available in the local or remote server.
 
-Using `zero.generate_client` you can generate client code for even remote servers using the `--host` and `--port` options. You don't need access to the code 😃
+Using `zero.generate_client` generate client code for even remote servers using the `--host` and `--port` options.
 
 ```shell
 python -m zero.generate_client --host localhost --port 5559 --overwrite-dir ./my_client
 ```
 
 It will generate client like this -
 
@@ -163,22 +227,24 @@
 if __name__ == "__main__":
     client.echo("Hi there!")
     client.hello_world(None)
 ```
 
 Currently, the code generation tool supports only `ZeroClient` and not `AsyncZeroClient`.
 
+*WIP - Generate models from server code.*
+
 # Important notes 📝
 
 *   `ZeroServer` should always be run under `if __name__ == "__main__":`, as it uses multiprocessing.
-*   The methods which are under `register_rpc()` in `ZeroServer` should have **type hinting**, like `def echo(msg: str):`
+*   The methods which are under `register_rpc()` in `ZeroServer` should have **type hinting**, like `def echo(msg: str) -> str:`
 
-# Let's do some benchmarking 🤘
+# Let's do some benchmarking! 🏎
 
-Zero is talking about inter service communication. In most real life scenarios, we need to call another microservice.
+Zero is all about inter service communication. In most real life scenarios, we need to call another microservice.
 
 So we will be testing a gateway calling another server for some data. Check the [benchmark/dockerize](https://github.com/Ananto30/zero/tree/main/benchmarks/dockerize) folder for details.
 
 There are two endpoints in every tests,
 
 *   `/hello`: Just call for a hello world response 😅
 *   `/order`: Save a Order object in redis
@@ -198,17 +264,17 @@
 fastApi     | 9590.96               | 18.31            | 6669.81            | 24.41
 sanic       | 18790.49              | 8.69             | 12259.29           | 13.52
 zero(sync)  | 24805.61              | 4.57             | 16498.83           | 7.80
 zero(async) | 22716.84              | 5.61             | 17446.19           | 7.24
 
 # Roadmap 🗺
 
-*   \[ ] Make msgspec as default serializer
-*   \[ ] Add support for async server (currently the sync server runs async functions in the eventloop, which is blocking)
-*   \[ ] Add pub/sub support
+*   [x] Make msgspec as default serializer
+*   [ ] Add support for async server (currently the sync server runs async functions in the eventloop, which is blocking)
+*   [ ] Add pub/sub support
 
 # Contribution
 
 Contributors are welcomed 🙏
 
 **Please leave a star ⭐ if you like Zero!**
```

### Comparing `zeroapi-0.3.60/setup.py` & `zeroapi-0.4.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zeroapi",
-    version="0.3.60",
+    version="0.4.0",
     author="Azizul Haque Ananto",
     author_email="azizulhaq.ananto@gmail.com",
     license="MIT",
     url="https://github.com/Ananto30/zero",
     description="Zero is a RPC framework to build fast and high performance Python microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `zeroapi-0.3.60/zero/client_server/client.py` & `zeroapi-0.4.0/zero/client_server/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import asyncio
 import logging
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Tuple, Type, TypeVar, Union
 
 from zero import config
 from zero.encoder import Encoder, get_encoder
 from zero.error import MethodNotFoundException, RemoteException, TimeoutException
 from zero.utils import util
 from zero.zero_mq import AsyncZeroMQClient, ZeroMQClient, get_async_client, get_client
 from zero.zero_mq.helpers import zpipe_async
 
+T = TypeVar("T")
+
 
 class ZeroClient:
     def __init__(
         self,
         host: str,
         port: int,
         default_timeout: int = 2000,
@@ -38,30 +40,31 @@
 
         default_timeout: int
             Default timeout for the ZeroClient for all calls.
             Default is 2000 ms.
 
         encoder: Optional[Encoder]
             Encoder to encode/decode messages from/to client.
-            Default is msgpack.
+            Default is msgspec.
             If any other encoder is used, the server should use the same encoder.
             Implement custom encoder by inheriting from `zero.encoder.Encoder`.
         """
         self._address = f"tcp://{host}:{port}"
         self._default_timeout = default_timeout
-        self.encdr = encoder or get_encoder(config.ENCODER)
+        self._encoder = encoder or get_encoder(config.ENCODER)
 
         self.zmqc: ZeroMQClient = None  # type: ignore
 
     def call(
         self,
         rpc_func_name: str,
         msg: Union[int, float, str, dict, list, tuple, None],
         timeout: Optional[int] = None,
-    ) -> Any:
+        return_type: Optional[Type[T]] = None,
+    ) -> T:
         """
         Call the rpc function resides on the ZeroServer.
 
         Parameters
         ----------
         rpc_func_name: str
             Function name should be string.
@@ -71,14 +74,18 @@
             The only argument of the rpc function.
             This should be of the same type as the rpc function's argument.
 
         timeout: Optional[int]
             Timeout for the call. In milliseconds.
             Default is 2000 milliseconds.
 
+        return_type: Optional[Type[T]]
+            The return type of the rpc function.
+            If return_type is set, the response will be parsed to the return_type.
+
         Returns
         -------
         Any
             The return value of the rpc function.
 
         Raises
         ------
@@ -100,32 +107,38 @@
 
         def _poll_data():
             if not self.zmqc.poll(_timeout):
                 raise TimeoutException(
                     f"Timeout while sending message at {self._address}"
                 )
 
-            resp_id, resp_data = self.encdr.decode(self.zmqc.recv())
+            resp_id, resp_data = (
+                self._encoder.decode(self.zmqc.recv())
+                if return_type is None
+                else self._encoder.decode_type(
+                    self.zmqc.recv(), Tuple[str, return_type]
+                )
+            )
             return resp_id, resp_data
 
         req_id = util.unique_id()
         frames = [req_id, rpc_func_name, "" if msg is None else msg]
-        self.zmqc.send(self.encdr.encode(frames))
+        self.zmqc.send(self._encoder.encode(frames))
 
         resp_id, resp_data = None, None
         # as the client is synchronous, we know that the response will be available any next poll
         # we try to get the response until timeout because a previous call might be timed out
         # and the response is still in the socket,
         # so we poll until we get the response for this call
         while resp_id != req_id:
             resp_id, resp_data = _poll_data()
 
         check_response(resp_data)
 
-        return resp_data
+        return resp_data  # type: ignore
 
     def close(self):
         if self.zmqc is not None:
             self.zmqc.close()
             self.zmqc = None
 
     def _ensure_connected(self):
@@ -137,16 +150,16 @@
 
     def _init(self):
         self.zmqc = get_client(config.ZEROMQ_PATTERN, self._default_timeout)
         self.zmqc.connect(self._address)
 
     def _try_connect(self):
         frames = [util.unique_id(), "connect", ""]
-        self.zmqc.send(self.encdr.encode(frames))
-        self.encdr.decode(self.zmqc.recv())
+        self.zmqc.send(self._encoder.encode(frames))
+        self._encoder.decode(self.zmqc.recv())
         logging.info("Connected to server at %s", self._address)
 
 
 class AsyncZeroClient:
     def __init__(
         self,
         host: str,
@@ -177,15 +190,15 @@
 
         default_timeout: int
             Default timeout for the AsyncZeroClient for all calls.
             Default is 2000 ms.
 
         encoder: Optional[Encoder]
             Encoder to encode/decode messages from/to client.
-            Default is msgpack.
+            Default is msgspec.
             If any other encoder is used, the server should use the same encoder.
             Implement custom encoder by inheriting from `zero.encoder.Encoder`.
         """
         self._address = f"tcp://{host}:{port}"
         self._default_timeout = default_timeout
         self._encoder = encoder or get_encoder(config.ENCODER)
         self._resp_map: Dict[str, Any] = {}
@@ -194,15 +207,16 @@
         self.peer1 = self.peer2 = None
 
     async def call(
         self,
         rpc_func_name: str,
         msg: Union[int, float, str, dict, list, tuple, None],
         timeout: Optional[int] = None,
-    ) -> Any:
+        return_type: Optional[Type[T]] = None,
+    ) -> T:
         """
         Call the rpc function resides on the ZeroServer.
 
         Parameters
         ----------
         rpc_func_name: str
             Function name should be string.
@@ -212,18 +226,23 @@
             The only argument of the rpc function.
             This should be of the same type as the rpc function's argument.
 
         timeout: Optional[int]
             Timeout for the call. In milliseconds.
             Default is 2000 milliseconds.
 
+        return_type: Optional[Type[T]]
+            The return type of the rpc function.
+            If return_type is set, the response will be parsed to the return_type.
+
         Returns
         -------
-        Any
+        T
             The return value of the rpc function.
+            If return_type is set, the response will be parsed to the return_type.
 
         Raises
         ------
         TimeoutException
             If the call times out or the connection is dropped.
 
         MethodNotFoundException
@@ -242,15 +261,19 @@
 
         async def _poll_data():
             # TODO async has issue with poller, after 3-4 calls, it returns empty
             # if not await self.zmq_client.poll(_timeout):
             #     raise TimeoutException(f"Timeout while sending message at {self._address}")
 
             resp = await self.zmqc.recv()
-            resp_id, resp_data = self._encoder.decode(resp)
+            resp_id, resp_data = (
+                self._encoder.decode(resp)
+                if return_type is None
+                else self._encoder.decode_type(resp, Tuple[str, return_type])
+            )
             self._resp_map[resp_id] = resp_data
 
             # TODO try to use pipe instead of sleep
             # await self.peer1.send(b"")
 
         req_id = util.unique_id()
         frames = [req_id, rpc_func_name, "" if msg is None else msg]
```

### Comparing `zeroapi-0.3.60/zero/client_server/server.py` & `zeroapi-0.4.0/zero/client_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         ----------
         host: str
             Host of the ZeroServer.
         port: int
             Port of the ZeroServer.
         encoder: Optional[Encoder]
             Encoder to encode/decode messages from/to client.
-            Default is msgpack.
+            Default is msgspec.
             If any other encoder is used, the client should use the same encoder.
             Implement custom encoder by inheriting from `zero.encoder.Encoder`.
         """
         self._broker: ZeroMQBroker = None  # type: ignore
         self._device_comm_channel: str = None  # type: ignore
         self._pool: Pool = None  # type: ignore
         self._device_ipc: str = None  # type: ignore
@@ -179,15 +179,19 @@
             self._broker.close()
         self._terminate_pool()
         self._remove_ipc()
         sys.exit(0)
 
     @util.log_error
     def _remove_ipc(self):
-        if os.name == "posix":
+        if (
+            os.name == "posix"
+            and self._device_ipc is not None
+            and os.path.exists(self._device_ipc)
+        ):
             os.remove(self._device_ipc)
 
     @util.log_error
     def _terminate_pool(self):
         self._pool.terminate()
         self._pool.close()
         self._pool.join()
```

### Comparing `zeroapi-0.3.60/zero/client_server/worker.py` & `zeroapi-0.4.0/zero/client_server/worker.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/codegen/codegen.py` & `zeroapi-0.4.0/zero/codegen/codegen.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
         self._rpc_router = rpc_router
         self._rpc_input_type_map = rpc_input_type_map
         self._rpc_return_type_map = rpc_return_type_map
         self._typing_imports = set()
 
     def generate_code(self, host="localhost", port=5559):
         code = f"""# Generated by Zero
-import typing  # remove this if not needed
-from typing import List, Dict, Union, Optional, Tuple  # remove this if not needed
+# import types as per needed
+
 from zero import ZeroClient
 
 
 zero_client = ZeroClient("{host}", {port})
 
 
 class RpcClient:
```

### Comparing `zeroapi-0.3.60/zero/generate_client.py` & `zeroapi-0.4.0/zero/generate_client.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/logger.py` & `zeroapi-0.4.0/zero/logger.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/pubsub/publisher.py` & `zeroapi-0.4.0/zero/pubsub/publisher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import msgpack
+import msgspec
 import zmq
 import zmq.asyncio
 
 from zero.utils.type_util import verify_allowed_type
 
 
 class ZeroPublisher:  # pragma: no cover
@@ -29,12 +29,14 @@
 
     def _set_socket_opt(self):
         # self.__socket.setsockopt(zmq.RCVTIMEO, 2000)
         self.__socket.setsockopt(zmq.LINGER, 0)
 
     def publish(self, topic, msg):
         verify_allowed_type(msg)
-        self.__socket.send_multipart([topic.encode(), msgpack.packb(msg)])
+        self.__socket.send_multipart([topic.encode(), msgspec.msgpack.encode(msg)])
 
     async def publish_async(self, topic, msg):
         verify_allowed_type(msg)
-        await self.__socket.send_multipart([topic.encode(), msgpack.packb(msg)])
+        await self.__socket.send_multipart(
+            [topic.encode(), msgspec.msgpack.encode(msg)]
+        )
```

### Comparing `zeroapi-0.3.60/zero/pubsub/subscriber.py` & `zeroapi-0.4.0/zero/pubsub/subscriber.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 import sys
 from multiprocessing import Process
 from typing import Callable, Dict
 
-import msgpack
+import msgspec
 import zmq
 import zmq.asyncio
 
 
 class ZeroSubscriber:  # pragma: no cover
     def __init__(self, host: str = "127.0.0.1", port: int = 5558):
         self._host = host
@@ -99,10 +99,10 @@
 
         while True:
             topic, msg = await socket.recv_multipart()
             if topic.decode() != self._topic:
                 continue
 
             try:
-                await self._func(msgpack.unpackb(msg))
+                await self._func(msgspec.msgpack.decode(msg))
             except Exception as exc:  # pylint: disable=broad-except
                 logging.error(exc)
```

### Comparing `zeroapi-0.3.60/zero/utils/type_util.py` & `zeroapi-0.4.0/zero/utils/type_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,61 @@
-from typing import (
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    get_origin,
-    get_type_hints,
-)
+import dataclasses
+import datetime
+import decimal
+import enum
+import typing
+import uuid
+from typing import Callable, Optional, get_origin, get_type_hints
 
-basic_types: List[type] = [
+import msgspec
+
+builtin_types: typing.List = [
+    None,
+    bool,
     int,
     float,
     str,
-    bool,
+    bytes,
+    bytearray,
+    tuple,
+    typing.Tuple,
     list,
+    typing.List,
     dict,
-    tuple,
+    typing.Dict,
     set,
+    typing.Set,
+    frozenset,
+    typing.FrozenSet,
 ]
-typing_types: List[type] = [
-    List,
-    Dict,
+
+std_lib_types: typing.List = [
+    datetime.datetime,
+    datetime.date,
+    datetime.time,
+    uuid.UUID,
+    decimal.Decimal,
+    enum.Enum,
+    enum.IntEnum,
+    dataclasses.dataclass,
 ]
-special_types: List[type] = [
-    Union,  # type: ignore
-    Optional,  # type: ignore
-    Tuple,  # type: ignore
+
+typing_types: typing.List = [
+    typing.Any,
+    typing.Union,
+    typing.Optional,
+]
+
+msgspec_types: typing.List = [
+    msgspec.Struct,
+    msgspec.Raw,
 ]
 
 
-allowed_types = basic_types + typing_types + special_types
+allowed_types = builtin_types + std_lib_types + typing_types
 
 
 def verify_function_args(func: Callable) -> None:
     arg_count = func.__code__.co_argcount
     if arg_count < 1:
         return
     if arg_count > 1:
@@ -81,40 +102,44 @@
 def get_function_return_class(func: Callable):
     types = get_type_hints(func)
     return types.get("return")
 
 
 def verify_function_input_type(func: Callable):
     input_type = get_function_input_class(func)
-    if input_type is None:
-        return
-    if input_type in basic_types:
+    if input_type in allowed_types:
         return
-    if get_origin(input_type) in basic_types:
-        return
-    if get_origin(input_type) in special_types:
+
+    origin_type = get_origin(input_type)
+    if origin_type is not None and origin_type in allowed_types:
         return
 
+    for mtype in msgspec_types:
+        if input_type is not None and issubclass(input_type, mtype):
+            return
+
     raise TypeError(
         f"{func.__name__} has type {input_type} which is not allowed; "
         "allowed types are: \n" + "\n".join([str(t) for t in allowed_types])
     )
 
 
 def verify_function_return_type(func: Callable):
     return_type = get_function_return_class(func)
-    if return_type is None:
-        return
-    if return_type in basic_types:
+    if return_type in allowed_types:
         return
-    if get_origin(return_type) in basic_types:
-        return
-    if get_origin(return_type) in special_types:
+
+    origin_type = get_origin(return_type)
+    if origin_type is not None and origin_type in allowed_types:
         return
 
+    for t in msgspec_types:
+        if issubclass(return_type, t):
+            return
+
     raise TypeError(
         f"{func.__name__} has return type {return_type} which is not allowed; "
         "allowed types are: \n" + "\n".join([str(t) for t in allowed_types])
     )
 
 
 def verify_allowed_type(msg, rpc_method: Optional[str] = None):
@@ -129,28 +154,19 @@
 def verify_incoming_rpc_call_input_type(
     msg, rpc_method: str, rpc_input_type_map: dict
 ):  # pragma: no cover
     input_type = rpc_input_type_map[rpc_method]
     if input_type is None:
         return
 
-    if input_type in basic_types:
+    if input_type in builtin_types:
         if input_type != type(msg):
             raise TypeError(
                 f"{msg} is not allowed for method `{rpc_method}`; allowed type: {input_type}"
             )
 
     origin_type = get_origin(input_type)
-    if origin_type in basic_types:
+    if origin_type in builtin_types:
         if origin_type != type(msg):
             raise TypeError(
                 f"{msg} is not allowed for method `{rpc_method}`; allowed type: {input_type}"
             )
-
-
-# def is_pydantic(cls):
-#     if cls not in basic_types:
-#         if get_origin(cls) not in basic_types:
-#             if get_origin(cls) not in special_types:
-#                 if issubclass(cls, tuple(pydantic_types)):
-#                     return True
-#     return False
```

### Comparing `zeroapi-0.3.60/zero/utils/util.py` & `zeroapi-0.4.0/zero/utils/util.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/zero_mq/factory.py` & `zeroapi-0.4.0/zero/zero_mq/factory.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/zero_mq/helpers.py` & `zeroapi-0.4.0/zero/zero_mq/helpers.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/zero_mq/protocols.py` & `zeroapi-0.4.0/zero/zero_mq/protocols.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/zero_mq/queue_device/broker.py` & `zeroapi-0.4.0/zero/zero_mq/queue_device/broker.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/zero_mq/queue_device/client.py` & `zeroapi-0.4.0/zero/zero_mq/queue_device/client.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zero/zero_mq/queue_device/worker.py` & `zeroapi-0.4.0/zero/zero_mq/queue_device/worker.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.3.60/zeroapi.egg-info/PKG-INFO` & `zeroapi-0.4.0/zeroapi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroapi
-Version: 0.3.60
+Version: 0.4.0
 Summary: Zero is a RPC framework to build fast and high performance Python microservices
 Home-page: https://github.com/Ananto30/zero
 Author: Azizul Haque Ananto
 Author-email: azizulhaq.ananto@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -36,115 +36,164 @@
 </p>
 <hr>
 
 **Features**:
 
 *   Zero provides **faster communication** (see [benchmarks](https://github.com/Ananto30/zero#benchmarks-)) between the microservices using [zeromq](https://zeromq.org/) under the hood.
 *   Zero uses messages for communication and traditional **client-server** or **request-reply** pattern is supported.
-*   Support for both **Async** and **sync**.
+*   Support for both **async** and **sync**.
 *   The base server (ZeroServer) **utilizes all cpu cores**.
 *   **Code generation**! See [example](https://github.com/Ananto30/zero#code-generation-) 👇
 
 **Philosophy** behind Zero:
 
-*   **Zero learning curve**: The learning curve is tends to zero. You just add your functions and spin up a server, literally that's it! The framework hides the complexity of messaging pattern that enables faster communication.
+*   **Zero learning curve**: The learning curve is tends to zero. Just add functions and spin up a server, literally that's it! The framework hides the complexity of messaging pattern that enables faster communication.
 *   **ZeroMQ**: An awesome messaging library enables the power of Zero.
 
 Let's get started!
 
 # Getting started 🚀
 
 *Ensure Python 3.8+*
 
     pip install zeroapi
 
 **For Windows**, [tornado](https://pypi.org/project/tornado/) needs to be installed separately (for async operations). It's not included with `zeroapi` because for linux and mac-os, tornado is not needed as they have their own event loops.
 
 *   Create a `server.py`
 
-```python
-from zero import ZeroServer
+    ```python
+    from zero import ZeroServer
 
-app = ZeroServer(port=5559)
+    app = ZeroServer(port=5559)
 
-@app.register_rpc
-def echo(msg: str) -> str:
-    return msg
+    @app.register_rpc
+    def echo(msg: str) -> str:
+        return msg
 
-@app.register_rpc
-async def hello_world() -> str:
-    return "hello world"
+    @app.register_rpc
+    async def hello_world() -> str:
+        return "hello world"
 
 
-if __name__ == "__main__":
-    app.run()
-```
-
-Please note that server **RPC methods are type hinted**. Type hint is **must** in Zero server.
+    if __name__ == "__main__":
+        app.run()
+    ```
 
-*See the method type async or sync, doesn't matter.* 😃
+*   The **RPC functions only support one argument** (`msg`) for now.
 
-*   Run it
-
-<!---->
+*   Also note that server **RPC functions are type hinted**. Type hint is **must** in Zero server. Supported types can be found [here](/zero/utils/type_util.py#L11).
 
+*   Run the server
+    ```shell
     python -m server
+    ```
 
 *   Call the rpc methods
 
-```python
-from zero import ZeroClient
+    ```python
+    from zero import ZeroClient
 
-zero_client = ZeroClient("localhost", 5559)
+    zero_client = ZeroClient("localhost", 5559)
 
-def echo():
-    resp = zero_client.call("echo", "Hi there!")
-    print(resp)
-
-def hello():
-    resp = zero_client.call("hello_world", None)
-    print(resp)
+    def echo():
+        resp = zero_client.call("echo", "Hi there!")
+        print(resp)
 
+    def hello():
+        resp = zero_client.call("hello_world", None)
+        print(resp)
 
-if __name__ == "__main__":
-    echo()
-    hello()
-```
 
-Or using async client -
+    if __name__ == "__main__":
+        echo()
+        hello()
+    ```
+
+*   Or using async client -
+
+    ```python
+    import asyncio
+
+    from zero import AsyncZeroClient
+
+    zero_client = AsyncZeroClient("localhost", 5559)
+
+    async def echo():
+        resp = await zero_client.call("echo", "Hi there!")
+        print(resp)
+
+    async def hello():
+        resp = await zero_client.call("hello_world", None)
+        print(resp)
+
+
+    if __name__ == "__main__":
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(echo())
+        loop.run_until_complete(hello())
+    ```
+
+# Serialization 📦
+
+## Default serializer
+
+[Msgspec](https://jcristharif.com/msgspec/) is the default serializer. So `msgspec.Struct` (for high performance) or `dataclass` or any [supported types](https://jcristharif.com/msgspec/supported-types.html) can be used easily to pass complex arguments, i.e.
 
 ```python
-import asyncio
+from dataclasses import dataclass
+from msgspec import Struct
+from zero import ZeroServer
 
-from zero import AsyncZeroClient
+app = ZeroServer()
 
-zero_client = AsyncZeroClient("localhost", 5559)
+class Person(Struct):
+    name: str
+    age: int
+    dob: datetime
+
+@dataclass
+class Order:
+    id: int
+    amount: float
+    created_at: datetime
 
-async def echo():
-    resp = await zero_client.call("echo", "Hi there!")
-    print(resp)
+@app.register_rpc
+def save_person(person: Person) -> None:
+    # save person to db
+    ...
 
-async def hello():
-    resp = await zero_client.call("hello_world", None)
-    print(resp)
+@app.register_rpc
+def save_order(order: Order) -> None:
+    # save order to db
+    ...
+```
 
+## Return type
 
-if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(echo())
-    loop.run_until_complete(hello())
+The return type of the RPC function can be any of the [supported types](https://jcristharif.com/msgspec/supported-types.html). If `return_type` is set in the client `call` method, then the return type will be converted to that type.
+
+```python
+@dataclass
+class Order:
+    id: int
+    amount: float
+    created_at: datetime
+
+def get_order(id: str) -> Order:
+    return zero_client.call("get_order", id, return_type=Order)
 ```
 
-# Code Generation! 🙌
+# Code Generation 🤖
 
-You can also use our code generation tool to generate Python client code!
+Easy to use code generation tool is also provided!
 
-After running the server, like above, you can call the server to get the client code.
+After running the server, like above, call the server to get the client code. This makes it easy to know what functions are available in the local or remote server.
 
-Using `zero.generate_client` you can generate client code for even remote servers using the `--host` and `--port` options. You don't need access to the code 😃
+Using `zero.generate_client` generate client code for even remote servers using the `--host` and `--port` options.
 
 ```shell
 python -m zero.generate_client --host localhost --port 5559 --overwrite-dir ./my_client
 ```
 
 It will generate client like this -
 
@@ -178,22 +227,24 @@
 if __name__ == "__main__":
     client.echo("Hi there!")
     client.hello_world(None)
 ```
 
 Currently, the code generation tool supports only `ZeroClient` and not `AsyncZeroClient`.
 
+*WIP - Generate models from server code.*
+
 # Important notes 📝
 
 *   `ZeroServer` should always be run under `if __name__ == "__main__":`, as it uses multiprocessing.
-*   The methods which are under `register_rpc()` in `ZeroServer` should have **type hinting**, like `def echo(msg: str):`
+*   The methods which are under `register_rpc()` in `ZeroServer` should have **type hinting**, like `def echo(msg: str) -> str:`
 
-# Let's do some benchmarking 🤘
+# Let's do some benchmarking! 🏎
 
-Zero is talking about inter service communication. In most real life scenarios, we need to call another microservice.
+Zero is all about inter service communication. In most real life scenarios, we need to call another microservice.
 
 So we will be testing a gateway calling another server for some data. Check the [benchmark/dockerize](https://github.com/Ananto30/zero/tree/main/benchmarks/dockerize) folder for details.
 
 There are two endpoints in every tests,
 
 *   `/hello`: Just call for a hello world response 😅
 *   `/order`: Save a Order object in redis
@@ -213,17 +264,17 @@
 fastApi     | 9590.96               | 18.31            | 6669.81            | 24.41
 sanic       | 18790.49              | 8.69             | 12259.29           | 13.52
 zero(sync)  | 24805.61              | 4.57             | 16498.83           | 7.80
 zero(async) | 22716.84              | 5.61             | 17446.19           | 7.24
 
 # Roadmap 🗺
 
-*   \[ ] Make msgspec as default serializer
-*   \[ ] Add support for async server (currently the sync server runs async functions in the eventloop, which is blocking)
-*   \[ ] Add pub/sub support
+*   [x] Make msgspec as default serializer
+*   [ ] Add support for async server (currently the sync server runs async functions in the eventloop, which is blocking)
+*   [ ] Add pub/sub support
 
 # Contribution
 
 Contributors are welcomed 🙏
 
 **Please leave a star ⭐ if you like Zero!**
```

