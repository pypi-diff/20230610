# Comparing `tmp/zeroapi-0.4.0.tar.gz` & `tmp/zeroapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroapi-0.4.0.tar", last modified: Sat Jun 10 07:15:42 2023, max compression
+gzip compressed data, was "zeroapi-0.4.1.tar", last modified: Sat Jun 10 07:29:50 2023, max compression
```

## Comparing `zeroapi-0.4.0.tar` & `zeroapi-0.4.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1076 2023-03-26 09:01:39.000000 zeroapi-0.4.0/LICENSE
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     8831 2023-06-10 07:15:42.098272 zeroapi-0.4.0/PKG-INFO
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     8333 2023-06-10 07:13:54.000000 zeroapi-0.4.0/README.md
--rw-rw-r--   0 ananto    (1000) ananto    (1000)       38 2023-06-10 07:15:42.098272 zeroapi-0.4.0/setup.cfg
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      790 2023-06-10 07:13:37.000000 zeroapi-0.4.0/setup.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.090273 zeroapi-0.4.0/tests/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      105 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/constants.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.090273 zeroapi-0.4.0/tests/functional/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/__init__.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.090273 zeroapi-0.4.0/tests/functional/multiple_servers/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/multiple_servers/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1012 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/client_inside_server_test.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      629 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/conftest.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3270 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/multiple_clients_test.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      303 2023-04-02 19:24:48.000000 zeroapi-0.4.0/tests/functional/multiple_servers/server1.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      823 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/multiple_servers/server2.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.094272 zeroapi-0.4.0/tests/functional/single_server/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/single_server/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3171 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/single_server/client_generation_test.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     2859 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/single_server/client_server_test.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     5040 2023-05-14 21:11:59.000000 zeroapi-0.4.0/tests/functional/single_server/client_test.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      370 2023-04-08 08:04:49.000000 zeroapi-0.4.0/tests/functional/single_server/conftest.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3512 2023-04-08 08:04:49.000000 zeroapi-0.4.0/tests/functional/single_server/register_rpc_test.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1941 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/functional/single_server/server.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      937 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/functional/single_server/server_test.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.094272 zeroapi-0.4.0/tests/unit/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.0/tests/unit/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     8944 2023-06-10 07:13:54.000000 zeroapi-0.4.0/tests/unit/test_server.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1401 2023-04-08 08:04:49.000000 zeroapi-0.4.0/tests/utils.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      329 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/__init__.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/client_server/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:04:57.000000 zeroapi-0.4.0/zero/client_server/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)    12081 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/client_server/client.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     6612 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/client_server/server.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3943 2023-05-30 19:54:56.000000 zeroapi-0.4.0/zero/client_server/worker.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/codegen/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:02.000000 zeroapi-0.4.0/zero/codegen/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3091 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/codegen/codegen.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      277 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/config.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/encoder/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)       64 2023-04-07 21:02:10.000000 zeroapi-0.4.0/zero/encoder/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      215 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/encoder/factory.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      412 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/encoder/msgspc.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      277 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/encoder/protocols.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      246 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/error.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1617 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/generate_client.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     2213 2023-04-08 09:13:20.000000 zeroapi-0.4.0/zero/logger.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/pubsub/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:08.000000 zeroapi-0.4.0/zero/pubsub/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1330 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/pubsub/publisher.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     3268 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/pubsub/subscriber.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/utils/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:11.000000 zeroapi-0.4.0/zero/utils/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     4455 2023-06-10 07:13:54.000000 zeroapi-0.4.0/zero/utils/type_util.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     2030 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/utils/util.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/zero_mq/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      157 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      935 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/factory.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      712 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/helpers.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1451 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/protocols.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zero/zero_mq/queue_device/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      118 2023-04-07 21:03:06.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/__init__.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)      611 2023-04-08 08:04:49.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/broker.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     4268 2023-04-08 09:13:20.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/client.py
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1334 2023-05-14 21:11:59.000000 zeroapi-0.4.0/zero/zero_mq/queue_device/worker.py
-drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:15:42.098272 zeroapi-0.4.0/zeroapi.egg-info/
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     8831 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/PKG-INFO
--rw-rw-r--   0 ananto    (1000) ananto    (1000)     1829 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ananto    (1000) ananto    (1000)        1 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ananto    (1000) ananto    (1000)       14 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/requires.txt
--rw-rw-r--   0 ananto    (1000) ananto    (1000)       11 2023-06-10 07:15:42.000000 zeroapi-0.4.0/zeroapi.egg-info/top_level.txt
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1076 2023-03-26 09:01:39.000000 zeroapi-0.4.1/LICENSE
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8831 2023-06-10 07:29:50.372708 zeroapi-0.4.1/PKG-INFO
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8333 2023-06-10 07:13:54.000000 zeroapi-0.4.1/README.md
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       38 2023-06-10 07:29:50.372708 zeroapi-0.4.1/setup.cfg
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      790 2023-06-10 07:28:17.000000 zeroapi-0.4.1/setup.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.368709 zeroapi-0.4.1/tests/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      105 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/constants.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.368709 zeroapi-0.4.1/tests/functional/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.1/tests/functional/__init__.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.368709 zeroapi-0.4.1/tests/functional/multiple_servers/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.1/tests/functional/multiple_servers/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1012 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/functional/multiple_servers/client_inside_server_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      629 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/functional/multiple_servers/conftest.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3270 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/functional/multiple_servers/multiple_clients_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      303 2023-04-02 19:24:48.000000 zeroapi-0.4.1/tests/functional/multiple_servers/server1.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      823 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/functional/multiple_servers/server2.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.368709 zeroapi-0.4.1/tests/functional/single_server/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.1/tests/functional/single_server/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3171 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/functional/single_server/client_generation_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     2859 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/functional/single_server/client_server_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     5040 2023-05-14 21:11:59.000000 zeroapi-0.4.1/tests/functional/single_server/client_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      370 2023-04-08 08:04:49.000000 zeroapi-0.4.1/tests/functional/single_server/conftest.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3512 2023-04-08 08:04:49.000000 zeroapi-0.4.1/tests/functional/single_server/register_rpc_test.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1941 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/functional/single_server/server.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      937 2023-04-02 08:45:25.000000 zeroapi-0.4.1/tests/functional/single_server/server_test.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.368709 zeroapi-0.4.1/tests/unit/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 08:45:25.000000 zeroapi-0.4.1/tests/unit/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8944 2023-06-10 07:13:54.000000 zeroapi-0.4.1/tests/unit/test_server.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1401 2023-04-08 08:04:49.000000 zeroapi-0.4.1/tests/utils.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.368709 zeroapi-0.4.1/zero/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      329 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/__init__.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zero/client_server/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:04:57.000000 zeroapi-0.4.1/zero/client_server/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)    12081 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/client_server/client.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     6612 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/client_server/server.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3943 2023-05-30 19:54:56.000000 zeroapi-0.4.1/zero/client_server/worker.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zero/codegen/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:02.000000 zeroapi-0.4.1/zero/codegen/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3091 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/codegen/codegen.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      277 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/config.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zero/encoder/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       64 2023-04-07 21:02:10.000000 zeroapi-0.4.1/zero/encoder/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      215 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/encoder/factory.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      412 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/encoder/msgspc.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      277 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/encoder/protocols.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      246 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/error.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1617 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/generate_client.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     2213 2023-04-08 09:13:20.000000 zeroapi-0.4.1/zero/logger.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zero/pubsub/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:08.000000 zeroapi-0.4.1/zero/pubsub/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1330 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/pubsub/publisher.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     3268 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/pubsub/subscriber.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zero/utils/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        0 2023-04-02 09:05:11.000000 zeroapi-0.4.1/zero/utils/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     4455 2023-06-10 07:13:54.000000 zeroapi-0.4.1/zero/utils/type_util.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     2030 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/utils/util.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zero/zero_mq/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      157 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/zero_mq/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      935 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/zero_mq/factory.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      712 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/zero_mq/helpers.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1451 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/zero_mq/protocols.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zero/zero_mq/queue_device/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      118 2023-04-07 21:03:06.000000 zeroapi-0.4.1/zero/zero_mq/queue_device/__init__.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)      611 2023-04-08 08:04:49.000000 zeroapi-0.4.1/zero/zero_mq/queue_device/broker.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     4268 2023-04-08 09:13:20.000000 zeroapi-0.4.1/zero/zero_mq/queue_device/client.py
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1334 2023-05-14 21:11:59.000000 zeroapi-0.4.1/zero/zero_mq/queue_device/worker.py
+drwxrwxr-x   0 ananto    (1000) ananto    (1000)        0 2023-06-10 07:29:50.372708 zeroapi-0.4.1/zeroapi.egg-info/
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     8831 2023-06-10 07:29:50.000000 zeroapi-0.4.1/zeroapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)     1829 2023-06-10 07:29:50.000000 zeroapi-0.4.1/zeroapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)        1 2023-06-10 07:29:50.000000 zeroapi-0.4.1/zeroapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       14 2023-06-10 07:29:50.000000 zeroapi-0.4.1/zeroapi.egg-info/requires.txt
+-rw-rw-r--   0 ananto    (1000) ananto    (1000)       11 2023-06-10 07:29:50.000000 zeroapi-0.4.1/zeroapi.egg-info/top_level.txt
```

### Comparing `zeroapi-0.4.0/LICENSE` & `zeroapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/PKG-INFO` & `zeroapi-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Zero is a RPC framework to build fast and high performance Python microservices
 Home-page: https://github.com/Ananto30/zero
 Author: Azizul Haque Ananto
 Author-email: azizulhaq.ananto@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zeroapi-0.4.0/README.md` & `zeroapi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/setup.py` & `zeroapi-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zeroapi",
-    version="0.4.0",
+    version="0.4.1",
     author="Azizul Haque Ananto",
     author_email="azizulhaq.ananto@gmail.com",
     license="MIT",
     url="https://github.com/Ananto30/zero",
     description="Zero is a RPC framework to build fast and high performance Python microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -17,9 +17,9 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
     package_dir={"": "."},
-    install_requires=["pyzmq", "msgpack"],
+    install_requires=["pyzmq", "msgspec"],
 )
```

### Comparing `zeroapi-0.4.0/tests/functional/multiple_servers/client_inside_server_test.py` & `zeroapi-0.4.1/tests/functional/multiple_servers/client_inside_server_test.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/multiple_servers/conftest.py` & `zeroapi-0.4.1/tests/functional/multiple_servers/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/multiple_servers/multiple_clients_test.py` & `zeroapi-0.4.1/tests/functional/multiple_servers/multiple_clients_test.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/multiple_servers/server2.py` & `zeroapi-0.4.1/tests/functional/multiple_servers/server2.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/single_server/client_generation_test.py` & `zeroapi-0.4.1/tests/functional/single_server/client_generation_test.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/single_server/client_server_test.py` & `zeroapi-0.4.1/tests/functional/single_server/client_server_test.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/single_server/client_test.py` & `zeroapi-0.4.1/tests/functional/single_server/client_test.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/single_server/register_rpc_test.py` & `zeroapi-0.4.1/tests/functional/single_server/register_rpc_test.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/single_server/server.py` & `zeroapi-0.4.1/tests/functional/single_server/server.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/functional/single_server/server_test.py` & `zeroapi-0.4.1/tests/functional/single_server/server_test.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/unit/test_server.py` & `zeroapi-0.4.1/tests/unit/test_server.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/tests/utils.py` & `zeroapi-0.4.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/client_server/client.py` & `zeroapi-0.4.1/zero/client_server/client.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/client_server/server.py` & `zeroapi-0.4.1/zero/client_server/server.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/client_server/worker.py` & `zeroapi-0.4.1/zero/client_server/worker.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/codegen/codegen.py` & `zeroapi-0.4.1/zero/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/generate_client.py` & `zeroapi-0.4.1/zero/generate_client.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/logger.py` & `zeroapi-0.4.1/zero/logger.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/pubsub/publisher.py` & `zeroapi-0.4.1/zero/pubsub/publisher.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/pubsub/subscriber.py` & `zeroapi-0.4.1/zero/pubsub/subscriber.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/utils/type_util.py` & `zeroapi-0.4.1/zero/utils/type_util.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/utils/util.py` & `zeroapi-0.4.1/zero/utils/util.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/zero_mq/factory.py` & `zeroapi-0.4.1/zero/zero_mq/factory.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/zero_mq/helpers.py` & `zeroapi-0.4.1/zero/zero_mq/helpers.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/zero_mq/protocols.py` & `zeroapi-0.4.1/zero/zero_mq/protocols.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/zero_mq/queue_device/broker.py` & `zeroapi-0.4.1/zero/zero_mq/queue_device/broker.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/zero_mq/queue_device/client.py` & `zeroapi-0.4.1/zero/zero_mq/queue_device/client.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zero/zero_mq/queue_device/worker.py` & `zeroapi-0.4.1/zero/zero_mq/queue_device/worker.py`

 * *Files identical despite different names*

### Comparing `zeroapi-0.4.0/zeroapi.egg-info/PKG-INFO` & `zeroapi-0.4.1/zeroapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Zero is a RPC framework to build fast and high performance Python microservices
 Home-page: https://github.com/Ananto30/zero
 Author: Azizul Haque Ananto
 Author-email: azizulhaq.ananto@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zeroapi-0.4.0/zeroapi.egg-info/SOURCES.txt` & `zeroapi-0.4.1/zeroapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

