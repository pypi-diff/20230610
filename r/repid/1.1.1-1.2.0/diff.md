# Comparing `tmp/repid-1.1.1.tar.gz` & `tmp/repid-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.1.1.tar", last modified: Sun Apr 30 00:36:49 2023, max compression
+gzip compressed data, was "repid-1.2.0.tar", last modified: Sat Jun 10 20:58:47 2023, max compression
```

## Comparing `repid-1.1.1.tar` & `repid-1.2.0.tar`

### file list

```diff
@@ -1,74 +1,79 @@
--rw-r--r--   0        0        0     1069 2023-04-30 00:36:20.722967 repid-1.1.1/LICENSE
--rw-r--r--   0        0        0     2589 2023-04-30 00:36:20.722967 repid-1.1.1/README.md
--rw-r--r--   0        0        0     3194 2023-04-30 00:36:49.898706 repid-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      588 2023-04-30 00:36:20.726967 repid-1.1.1/repid/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-30 00:36:20.726967 repid-1.1.1/repid/_asyncify.py
--rw-r--r--   0        0        0     5073 2023-04-30 00:36:20.726967 repid-1.1.1/repid/_processor.py
--rw-r--r--   0        0        0     4061 2023-04-30 00:36:20.730967 repid-1.1.1/repid/_runner.py
--rw-r--r--   0        0        0      509 2023-04-30 00:36:20.730967 repid-1.1.1/repid/actor.py
--rw-r--r--   0        0        0     2316 2023-04-30 00:36:20.730967 repid-1.1.1/repid/config.py
--rw-r--r--   0        0        0     3313 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connection.py
--rw-r--r--   0        0        0      698 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/__init__.py
--rw-r--r--   0        0        0     6594 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/abc.py
--rw-r--r--   0        0        0      158 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0     1472 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/bucket_broker.py
--rw-r--r--   0        0        0     2748 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/consumer.py
--rw-r--r--   0        0        0     3792 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/message_broker.py
--rw-r--r--   0        0        0      860 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/utils.py
--rw-r--r--   0        0        0       90 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     6161 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7091 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      362 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0      910 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0     7593 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     7609 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     3818 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     1944 2023-04-30 00:36:20.730967 repid-1.1.1/repid/converter.py
--rw-r--r--   0        0        0      355 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/__init__.py
--rw-r--r--   0        0        0     2275 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/_buckets.py
--rw-r--r--   0        0        0      819 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/_key.py
--rw-r--r--   0        0        0     5545 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/priorities.py
--rw-r--r--   0        0        0     3873 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/protocols.py
--rw-r--r--   0        0        0     7465 2023-04-30 00:36:20.730967 repid-1.1.1/repid/job.py
--rw-r--r--   0        0        0      546 2023-04-30 00:36:20.730967 repid-1.1.1/repid/logger.py
--rw-r--r--   0        0        0     1655 2023-04-30 00:36:20.730967 repid-1.1.1/repid/main.py
--rw-r--r--   0        0        0      257 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3680 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3647 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2023-04-30 00:36:20.730967 repid-1.1.1/repid/py.typed
--rw-r--r--   0        0        0     1064 2023-04-30 00:36:20.730967 repid-1.1.1/repid/queue.py
--rw-r--r--   0        0        0     1319 2023-04-30 00:36:20.730967 repid-1.1.1/repid/retry_policy.py
--rw-r--r--   0        0        0     5021 2023-04-30 00:36:20.730967 repid-1.1.1/repid/router.py
--rw-r--r--   0        0        0      604 2023-04-30 00:36:20.730967 repid-1.1.1/repid/serializer.py
--rw-r--r--   0        0        0      917 2023-04-30 00:36:20.730967 repid-1.1.1/repid/utils.py
--rw-r--r--   0        0        0     3971 2023-04-30 00:36:20.730967 repid-1.1.1/repid/worker.py
--rw-r--r--   0        0        0        0 2023-04-30 00:36:20.730967 repid-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      743 2023-04-30 00:36:20.730967 repid-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4003 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0      431 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_actor.py
--rw-r--r--   0        0        0     3110 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_config.py
--rw-r--r--   0        0        0     1962 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_connection.py
--rw-r--r--   0        0        0     3818 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10233 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_default_data_models.py
--rw-r--r--   0        0        0     3003 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_job.py
--rw-r--r--   0        0        0      849 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_main.py
--rw-r--r--   0        0        0     7842 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     1484 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_pydantic.py
--rw-r--r--   0        0        0      414 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_queue.py
--rw-r--r--   0        0        0     3194 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_router.py
--rw-r--r--   0        0        0      764 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_serializer.py
--rw-r--r--   0        0        0      685 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_utils_wait_until.py
--rw-r--r--   0        0        0     6887 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_worker.py
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 repid-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-10 20:58:23.725708 repid-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2589 2023-06-10 20:58:23.725708 repid-1.2.0/README.md
+-rw-r--r--   0        0        0     3704 2023-06-10 20:58:47.537941 repid-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      625 2023-06-10 20:58:23.729709 repid-1.2.0/repid/__init__.py
+-rw-r--r--   0        0        0     1552 2023-06-10 20:58:23.729709 repid-1.2.0/repid/_asyncify.py
+-rw-r--r--   0        0        0     5104 2023-06-10 20:58:23.729709 repid-1.2.0/repid/_processor.py
+-rw-r--r--   0        0        0     4061 2023-06-10 20:58:23.729709 repid-1.2.0/repid/_runner.py
+-rw-r--r--   0        0        0      509 2023-06-10 20:58:23.729709 repid-1.2.0/repid/actor.py
+-rw-r--r--   0        0        0     2316 2023-06-10 20:58:23.729709 repid-1.2.0/repid/config.py
+-rw-r--r--   0        0        0     4525 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connection.py
+-rw-r--r--   0        0        0      760 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6594 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/abc.py
+-rw-r--r--   0        0        0      314 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0      260 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/__init__.py
+-rw-r--r--   0        0        0     1823 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/bucket_broker.py
+-rw-r--r--   0        0        0     2765 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/consumer.py
+-rw-r--r--   0        0        0     4093 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/message_broker.py
+-rw-r--r--   0        0        0      860 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/utils.py
+-rw-r--r--   0        0        0       90 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     6161 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7091 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      362 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0      910 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1513 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0     7593 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     7609 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     3818 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     1944 2023-06-10 20:58:23.729709 repid-1.2.0/repid/converter.py
+-rw-r--r--   0        0        0      355 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/__init__.py
+-rw-r--r--   0        0        0     2275 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/_buckets.py
+-rw-r--r--   0        0        0      819 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/_key.py
+-rw-r--r--   0        0        0     5509 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/priorities.py
+-rw-r--r--   0        0        0     3859 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/protocols.py
+-rw-r--r--   0        0        0     7425 2023-06-10 20:58:23.729709 repid-1.2.0/repid/job.py
+-rw-r--r--   0        0        0      546 2023-06-10 20:58:23.729709 repid-1.2.0/repid/logger.py
+-rw-r--r--   0        0        0     1887 2023-06-10 20:58:23.729709 repid-1.2.0/repid/main.py
+-rw-r--r--   0        0        0      257 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3696 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3647 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2023-06-10 20:58:23.729709 repid-1.2.0/repid/py.typed
+-rw-r--r--   0        0        0     1064 2023-06-10 20:58:23.729709 repid-1.2.0/repid/queue.py
+-rw-r--r--   0        0        0     1319 2023-06-10 20:58:23.729709 repid-1.2.0/repid/retry_policy.py
+-rw-r--r--   0        0        0     5021 2023-06-10 20:58:23.729709 repid-1.2.0/repid/router.py
+-rw-r--r--   0        0        0      568 2023-06-10 20:58:23.729709 repid-1.2.0/repid/serializer.py
+-rw-r--r--   0        0        0      844 2023-06-10 20:58:23.729709 repid-1.2.0/repid/testing/__init__.py
+-rw-r--r--   0        0        0     3183 2023-06-10 20:58:23.729709 repid-1.2.0/repid/testing/modifiers.py
+-rw-r--r--   0        0        0     6099 2023-06-10 20:58:23.729709 repid-1.2.0/repid/testing/plugin.py
+-rw-r--r--   0        0        0     1524 2023-06-10 20:58:23.733708 repid-1.2.0/repid/utils.py
+-rw-r--r--   0        0        0     3971 2023-06-10 20:58:23.733708 repid-1.2.0/repid/worker.py
+-rw-r--r--   0        0        0        0 2023-06-10 20:58:23.733708 repid-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      758 2023-06-10 20:58:23.733708 repid-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4003 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0      431 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_actor.py
+-rw-r--r--   0        0        0     3110 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_config.py
+-rw-r--r--   0        0        0     2986 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_connection.py
+-rw-r--r--   0        0        0     3818 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10233 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_default_data_models.py
+-rw-r--r--   0        0        0     3003 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_job.py
+-rw-r--r--   0        0        0     1366 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_main.py
+-rw-r--r--   0        0        0     7842 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     1484 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_pydantic.py
+-rw-r--r--   0        0        0     3819 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      414 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_queue.py
+-rw-r--r--   0        0        0     3194 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_router.py
+-rw-r--r--   0        0        0      764 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_serializer.py
+-rw-r--r--   0        0        0     1038 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     6887 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_worker.py
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 repid-1.2.0/PKG-INFO
```

### Comparing `repid-1.1.1/LICENSE` & `repid-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/README.md` & `repid-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/pyproject.toml` & `repid-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,36 @@
     "typing-extensions>=4.3.0,<5.0.0; python_version < \"3.10\"",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.1.1"
+version = "1.2.0"
 
 [project.license]
 text = "MIT"
 
+[project.entry-points.pytest11]
+repid = "repid.testing.plugin"
+
 [project.optional-dependencies]
 amqp = [
     "aiormq<7.0.0,>=6.4.0",
 ]
 cron = [
     "croniter<2.0.0,>=1.3.4",
 ]
 redis = [
     "redis<5.0.0,>=4.3.3",
 ]
+test = [
+    "pytest",
+    "pytest-asyncio",
+]
 
 [project.urls]
 documentation = "https://repid.aleksul.space"
 funding = "https://github.com/sponsors/aleksul"
 repository = "https://github.com/aleksul/repid"
 tracker = "https://github.com/aleksul/repid/issues"
 
@@ -123,14 +130,30 @@
     "pytest-lazy-fixture",
     "pytest-docker-tools",
     "pytest-cov",
     "hypothesis",
     "pydantic<2.0.0,>=1.10.0",
 ]
 
+[tool.pdm.scripts.test]
+cmd = [
+    "pytest",
+    "--diff-symbols",
+    "--hypothesis-verbosity=normal",
+    "--cov-report=xml",
+    "--cov-report=term-missing",
+    "--cov=repid",
+    "--cov-append",
+]
+
+[tool.pdm.scripts.test.env]
+COV_CORE_SOURCE = "repid"
+COV_CORE_CONFIG = ".coveragerc"
+COV_CORE_DATAFILE = ".coverage.eager"
+
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.ruff]
 ignore = [
     "E501",
     "N999",
@@ -179,13 +202,18 @@
     "FBT",
     "BLE",
     "S101",
 ]
 "repid/connections/__init__.py" = [
     "F401",
 ]
+"repid/testing/__init__.py" = [
+    "F401",
+]
 "benchmarks/*" = [
     "T201",
+    "S603",
+    "S607",
 ]
 "**/__init__.py" = [
     "PLC0414",
 ]
```

### Comparing `repid-1.1.1/repid/_asyncify.py` & `repid-1.2.0/repid/_asyncify.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/_processor.py` & `repid-1.2.0/repid/_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
-import json
 import time
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from repid.actor import ActorData, ActorResult
 from repid.logger import logger
 from repid.middlewares import middleware_wrapper
+from repid.utils import _ArgsBucketInMessageId
 
 if TYPE_CHECKING:
     from repid.connection import Connection
     from repid.data import ParametersT, RoutingKeyT
     from repid.data.protocols import ResultPropertiesT
 
 
@@ -21,17 +21,18 @@
 
     def __init__(self, _conn: Connection) -> None:
         self._conn = _conn
         self.actor_run._repid_signal_emitter = self._conn.middleware.emit_signal
         self._processed = 0
 
     async def get_payload(self, initial_payload: str) -> str:
-        if initial_payload.find("__repid_payload_id", 0, 20) != -1:
-            bucket_id: str = json.loads(initial_payload).get("__repid_payload_id")
-            bucket = await self._conn._ab.get_bucket(bucket_id)
+        if _ArgsBucketInMessageId.check(initial_payload):
+            bucket = await self._conn._ab.get_bucket(
+                _ArgsBucketInMessageId.deconstruct(initial_payload),
+            )
             if bucket is not None:
                 return bucket.data
         return initial_payload
 
     @staticmethod
     @middleware_wrapper
     async def actor_run(
@@ -56,15 +57,15 @@
         logger.info("Running actor '{actor_name}' on message {message_id}.", extra=logger_extra)
         logger.debug("Time limit is set to {time_limit}.", extra=logger_extra)
 
         started_when = time.perf_counter_ns()
 
         try:
             result = await asyncio.wait_for(actor.fn(*args, **kwargs), timeout=time_limit)
-        except Exception as exc:
+        except Exception as exc:  # noqa: BLE001
             exception = exc
             success = False
             logger.exception(
                 "Error inside of an actor '{actor_name}' on message {message_id}.",
                 extra=logger_extra,
             )
         else:
```

### Comparing `repid-1.1.1/repid/_runner.py` & `repid-1.2.0/repid/_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/config.py` & `repid-1.2.0/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connection.py` & `repid-1.2.0/repid/connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import asyncio
+from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Union
 
+from repid.config import Config
 from repid.data.protocols import ResultBucketT
 from repid.middlewares import Middleware
 
 if TYPE_CHECKING:
     from repid.connections import BucketBrokerT, MessageBrokerT
 
 
 @dataclass(frozen=True)
 class Connection:
+    """Connection dataclass represents a combination of connections to a message broker and bucket brokers."""
+
     message_broker: "MessageBrokerT"
     args_bucket_broker: Union["BucketBrokerT", None] = None
     results_bucket_broker: Union["BucketBrokerT", None] = None
     middleware: Middleware = field(default_factory=Middleware, init=False)
     is_open: bool = field(default=False, init=False)
 
     async def connect(self) -> None:
@@ -45,29 +49,41 @@
                 if broker is not None
             ],
         )
         object.__setattr__(self, "is_open", False)  # noqa: FBT003
 
     @property
     def _ab(self) -> "BucketBrokerT":
-        """For internal use. Shortcut to get args bucket broker
-        or raise an error, if it isn't set."""
+        """For internal use.
+
+        Shortcut to get args bucket broker or raise an error, if it isn't set.
+        """
         if self.args_bucket_broker is None:
             raise ValueError("Args bucket broker is not configured.")
         return self.args_bucket_broker
 
     @property
     def _rb(self) -> "BucketBrokerT":
-        """For internal use. Shortcut to get result bucket broker
-        or raise an error, if it isn't set."""
+        """For internal use.
+
+        Shortcut to get result bucket broker or raise an error, if it isn't set.
+        """
         if self.results_bucket_broker is None:
             raise ValueError("Results bucket broker is not configured.")
         return self.results_bucket_broker
 
     def __post_init__(self) -> None:
+        """Magic method that is called after the initialization of the object.
+
+        If `results_bucket_broker` is not `None`, it tries to create an instance of the
+        `BUCKET_CLASS` with some dummy data to check if it is compatible with the `ResultBucketT` class.
+        If it is not compatible, it raises a `ValueError`.
+
+        It then sets middleware signal emitter for every submitted broker.
+        """
         # test result bucket broker has proper BUCKET_CLASS
         if self.results_bucket_broker is not None:
             try:
                 test_subject = self.results_bucket_broker.BUCKET_CLASS(  # type: ignore[call-arg]
                     data="",
                     started_when=123,
                     finished_when=123,
@@ -82,7 +98,19 @@
                 ) from exc
 
         # set _signal_emitter for every submitted protocol
         for broker in [self.message_broker, self.args_bucket_broker, self.results_bucket_broker]:
             if broker is None:
                 continue
             broker._signal_emitter = self.middleware.emit_signal
+
+    def _update_from_config(self) -> None:
+        """For internal use.
+
+        Manually update all brokers from the current Config.
+        """
+        self.message_broker.PARAMETERS_CLASS = deepcopy(Config.PARAMETERS)  # type: ignore[misc]
+        self.message_broker.ROUTING_KEY_CLASS = deepcopy(Config.ROUTING_KEY)  # type: ignore[misc]
+        if self.args_bucket_broker is not None:
+            self.args_bucket_broker.BUCKET_CLASS = deepcopy(Config.BUCKET)
+        if self.results_bucket_broker is not None:
+            self.results_bucket_broker.BUCKET_CLASS = deepcopy(Config.RESULT_BUCKET)
```

### Comparing `repid-1.1.1/repid/connections/__init__.py` & `repid-1.2.0/repid/connections/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from repid.connections.abc import BucketBrokerT, ConsumerT, MessageBrokerT
-from repid.connections.dummy import DummyBucketBroker, DummyMessageBroker
+from repid.connections.in_memory import (
+    DummyBucketBroker,
+    DummyMessageBroker,
+    InMemoryBucketBroker,
+    InMemoryMessageBroker,
+)
+from repid.utils import is_installed
 
 __all__ = [
     "BucketBrokerT",
     "ConsumerT",
     "MessageBrokerT",
     "DummyBucketBroker",
     "DummyMessageBroker",
+    "InMemoryBucketBroker",
+    "InMemoryMessageBroker",
 ]
 
-try:
-    import aiormq
-except ImportError:  # pragma: no cover
-    pass
-else:
+if is_installed("aiormq"):
     from repid.connections.rabbitmq import RabbitMessageBroker
 
     __all__.append("RabbitMessageBroker")
 
-try:
-    import redis
-except ImportError:  # pragma: no cover
-    pass
-else:
+if is_installed("redis"):
     from repid.connections.redis import RedisBucketBroker, RedisMessageBroker
 
     __all__.append("RedisBucketBroker")
     __all__.append("RedisMessageBroker")
```

### Comparing `repid-1.1.1/repid/connections/abc.py` & `repid-1.2.0/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connections/dummy/bucket_broker.py` & `repid-1.2.0/repid/connections/redis/bucket_broker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from __future__ import annotations
 
-import asyncio
 from typing import TYPE_CHECKING
 
+from redis.asyncio.client import Redis
+
 from repid.connections.abc import BucketBrokerT
 from repid.data._buckets import ArgsBucket, ResultBucket
 from repid.logger import logger
 
 if TYPE_CHECKING:
-    from repid.data.protocols import BucketT
+    from repid.data import BucketT
 
 
-class DummyBucketBroker(BucketBrokerT):
-    def __init__(self, *, use_result_bucket: bool = False) -> None:
+class RedisBucketBroker(BucketBrokerT):
+    def __init__(self, dsn: str, *, use_result_bucket: bool = False):
         self.BUCKET_CLASS = ResultBucket if use_result_bucket else ArgsBucket
-        self.__storage: dict[str, BucketT] = {}
+        self.conn: Redis[bytes] = Redis.from_url(dsn)
 
     async def connect(self) -> None:
-        logger.info("Connecting to dummy bucket broker.")
-        await asyncio.sleep(0)
+        await self.conn.ping()
 
     async def disconnect(self) -> None:
-        logger.info("Disconnecting from dummy bucket broker.")
-        await asyncio.sleep(0)
+        await self.conn.close(close_connection_pool=True)
 
     async def get_bucket(self, id_: str) -> BucketT | None:
         logger.debug("Getting bucket with id: {id_}.", extra={"id_": id_})
-        await asyncio.sleep(0)
-        return self.__storage.get(id_, None)
+        data = await self.conn.get(id_)
+        if data is not None:
+            return self.BUCKET_CLASS.decode(data.decode())  # type: ignore[no-any-return]
+        return None
 
     async def store_bucket(self, id_: str, payload: BucketT) -> None:
         logger.debug("Storing bucket with id: {id_}.", extra={"id_": id_})
-        await asyncio.sleep(0)
-        self.__storage[id_] = payload
-        await asyncio.sleep(0)
+        await self.conn.set(
+            id_,
+            payload.encode(),
+            exat=payload.timestamp + payload.ttl if payload.ttl is not None else None,
+        )
 
     async def delete_bucket(self, id_: str) -> None:
         logger.debug("Deleting bucket with id: {id_}.", extra={"id_": id_})
-        await asyncio.sleep(0)
-        self.__storage.pop(id_, None)
-        await asyncio.sleep(0)
+        await self.conn.delete(id_)
```

### Comparing `repid-1.1.1/repid/connections/dummy/consumer.py` & `repid-1.2.0/repid/connections/in_memory/consumer.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from contextlib import suppress
 from datetime import datetime
 from typing import TYPE_CHECKING, Iterable
 
 from repid.connections.abc import ConsumerT
 
 if TYPE_CHECKING:
-    from repid.connections.dummy.message_broker import DummyMessageBroker
-    from repid.connections.dummy.utils import Message
+    from repid.connections.in_memory.message_broker import InMemoryMessageBroker
+    from repid.connections.in_memory.utils import Message
     from repid.data.protocols import ParametersT, RoutingKeyT
 
 
-class _DummyConsumer(ConsumerT):
+class _InMemoryConsumer(ConsumerT):
     def __init__(
         self,
-        broker: DummyMessageBroker,
+        broker: InMemoryMessageBroker,
         queue_name: str,
         topics: Iterable[str] | None,
         max_unacked_messages: int | None = None,  # noqa: ARG002
     ):
         self.broker = broker
         self.queue_name = queue_name
         self._queue = broker.queues[queue_name]
```

### Comparing `repid-1.1.1/repid/connections/dummy/message_broker.py` & `repid-1.2.0/repid/connections/in_memory/message_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING
 
 from repid.connections.abc import MessageBrokerT
-from repid.connections.dummy.consumer import _DummyConsumer
-from repid.connections.dummy.utils import DummyQueue, Message, wait_until
+from repid.connections.in_memory.consumer import _InMemoryConsumer
+from repid.connections.in_memory.utils import DummyQueue, Message, wait_until
 from repid.logger import logger
 
 if TYPE_CHECKING:
     from datetime import datetime
 
     from repid.data.protocols import ParametersT, RoutingKeyT
 
 
-class DummyMessageBroker(MessageBrokerT):
-    CONSUMER_CLASS = _DummyConsumer
+class InMemoryMessageBroker(MessageBrokerT):
+    CONSUMER_CLASS = _InMemoryConsumer
 
     def __init__(self) -> None:
         self.queues: dict[str, DummyQueue] = {}
 
     async def connect(self) -> None:
-        logger.info("Connecting to dummy message broker.")
+        logger.info("Connecting to in-memory message broker.")
         await asyncio.sleep(0)
 
     async def disconnect(self) -> None:
-        logger.info("Disconnecting from dummy message broker.")
+        logger.info("Disconnecting from in-memory message broker.")
         await asyncio.sleep(0)
 
     async def enqueue(
         self,
         key: RoutingKeyT,
         payload: str = "",
         params: ParametersT | None = None,
@@ -116,7 +116,18 @@
     async def queue_delete(self, queue_name: str) -> None:
         logger.debug("Deleting queue '{queue_name}'.", extra={"queue_name": queue_name})
         await asyncio.sleep(0)
 
         self.queues.pop(queue_name, None)
 
         await asyncio.sleep(0)
+
+
+def DummyMessageBroker() -> InMemoryMessageBroker:  # noqa: N802
+    from warnings import warn
+
+    warn(
+        "DummyMessageBroker was renamed to InMemoryMessageBroker.",
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
+    return InMemoryMessageBroker()
```

### Comparing `repid-1.1.1/repid/connections/dummy/utils.py` & `repid-1.2.0/repid/connections/in_memory/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connections/rabbitmq/consumer.py` & `repid-1.2.0/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connections/rabbitmq/message_broker.py` & `repid-1.2.0/repid/connections/rabbitmq/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connections/rabbitmq/utils.py` & `repid-1.2.0/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connections/redis/consumer.py` & `repid-1.2.0/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connections/redis/message_broker.py` & `repid-1.2.0/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/connections/redis/utils.py` & `repid-1.2.0/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/converter.py` & `repid-1.2.0/repid/converter.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/data/_buckets.py` & `repid-1.2.0/repid/data/_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/data/_key.py` & `repid-1.2.0/repid/data/_key.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/data/_parameters.py` & `repid-1.2.0/repid/data/_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import json
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Type, Union
 from uuid import uuid4
 
-from repid.utils import FROZEN_DATACLASS, JSON_ENCODER, SLOTS_DATACLASS
+from repid.utils import FROZEN_DATACLASS, JSON_ENCODER, SLOTS_DATACLASS, is_installed
 
 if TYPE_CHECKING:
     from repid.data.protocols import (
         DelayPropertiesT,
         ResultPropertiesT,
         RetriesPropertiesT,
     )
 
-try:
+if CRON_SUPPORT := is_installed("croniter"):
     from croniter import croniter
 
-    CRON_SUPPORT = True
-except ImportError:  # pragma: no cover
-    CRON_SUPPORT = False
-
 
 @dataclass(**FROZEN_DATACLASS, **SLOTS_DATACLASS)
 class RetriesProperties:
     max_amount: int = 0
     already_tried: int = 0
 
     def encode(self) -> str:
```

### Comparing `repid-1.1.1/repid/data/protocols.py` & `repid-1.2.0/repid/data/protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     @property
     def delay(self) -> DelayPropertiesT:
         ...
 
     def __init__(
         self,
         *,
-        execution_timeout: timedelta = timedelta(minutes=10),  # noqa: B008
+        execution_timeout: timedelta = timedelta(minutes=10),
         result: Union[ResultPropertiesT, None] = None,
         retries: Union[RetriesPropertiesT, None] = None,
         delay: Union[DelayPropertiesT, None] = None,
         timestamp: datetime = datetime.now(),  # noqa: B008
         ttl: Union[timedelta, None] = None,
     ) -> None:
         ...
```

### Comparing `repid-1.1.1/repid/job.py` & `repid-1.2.0/repid/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any
 
 from repid.config import Config
 from repid.data import ParametersT, PrioritiesT, ResultBucketT, RoutingKeyT
 from repid.main import Repid
 from repid.queue import Queue
-from repid.utils import JSON_ENCODER, VALID_ID, VALID_NAME
+from repid.utils import VALID_ID, VALID_NAME, _ArgsBucketInMessageId
 
 if TYPE_CHECKING:
     from repid.connection import Connection
 
 
 class Job:
     __slots__ = (
@@ -65,22 +65,22 @@
         queue: str | Queue = "default",
         priority: PrioritiesT = PrioritiesT.MEDIUM,
         id_: str | None = None,
         deferred_until: datetime | None = None,
         deferred_by: timedelta | None = None,
         cron: str | None = None,
         retries: int = 0,
-        timeout: timedelta = timedelta(minutes=10),  # noqa: B008
+        timeout: timedelta = timedelta(minutes=10),
         ttl: timedelta | None = None,
         args_id: str | None = None,  # default: uuid4
         args_ttl: timedelta | None = None,
         args: Any = None,
         use_args_bucketer: bool | None = None,
         result_id: str | None = None,  # default: uuid4
-        result_ttl: timedelta | None = timedelta(days=1),  # noqa: B008
+        result_ttl: timedelta | None = timedelta(days=1),
         store_result: bool | None = None,
         _connection: Connection | None = None,
     ) -> None:
         self._conn = _connection or Repid.get_magic_connection()
 
         self.name = name
         if not VALID_NAME.fullmatch(self.name):
@@ -172,17 +172,17 @@
             ttl=self.ttl,
         )
 
     async def _construct_args(self) -> str:
         if self.use_args_bucketer and self.args is not None:
             bucket = self._conn._ab.BUCKET_CLASS(data=self.args, ttl=self.args_ttl)
             await self._conn._ab.store_bucket(self.args_id, bucket)
-            return JSON_ENCODER.encode({"__repid_payload_id": self.args_id})
+            return _ArgsBucketInMessageId.construct(self.args_id)
         if self.args_id_set:
-            return JSON_ENCODER.encode({"__repid_payload_id": self.args_id})
+            return _ArgsBucketInMessageId.construct(self.args_id)
         return self.args or ""
 
     async def enqueue(self) -> tuple[RoutingKeyT, str, ParametersT]:
         key = self._construct_routing_key()
         parameters = self._construct_parameters()
         args = await self._construct_args()
         await self._conn.message_broker.enqueue(key, args, parameters)
```

### Comparing `repid-1.1.1/repid/logger.py` & `repid-1.2.0/repid/logger.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/main.py` & `repid-1.2.0/repid/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
         if middlewares is not None:
             for middleware in middlewares:
                 self.connection.middleware.add_middleware(middleware)
 
         if update_config:
             Config.update_all()
+            # In brokers Config is only fetched on initialization, and by the time this is called -
+            # initialization has been already done, so we have to update manually
+            self.connection._update_from_config()
 
     @classmethod
     def get_magic_connection(cls) -> Connection:
         if hasattr(cls.__local, "connection") and isinstance(cls.__local.connection, Connection):
             return cls.__local.connection
         raise ValueError("Default connection isn't set.")
```

### Comparing `repid-1.1.1/repid/middlewares/middleware.py` & `repid-1.2.0/repid/middlewares/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 if key in argspec.args
                 or (key in argspec.defaults if argspec.defaults is not None else False)
             }
             # try to call the function
             try:
                 return await asyncified(**kwargs)
             # ignore the exception and pass it to the logger
-            except Exception:
+            except Exception:  # noqa: BLE001
                 logger.exception(
                     "Subscriber '{fn_name}' ({fn}) raised an exception.",
                     extra=logger_extra,
                 )
 
         # add wrapped subscriber to the dictionary
         if name not in self.subscribers:
```

### Comparing `repid-1.1.1/repid/middlewares/wrapper.py` & `repid-1.2.0/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/queue.py` & `repid-1.2.0/repid/queue.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/retry_policy.py` & `repid-1.2.0/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/router.py` & `repid-1.2.0/repid/router.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/repid/worker.py` & `repid-1.2.0/repid/worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/conftest.py` & `repid-1.2.0/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import asyncio
 from typing import AsyncIterator, Iterator
 
 import pytest
 
-from repid import Connection, DummyBucketBroker, DummyMessageBroker, Repid
+from repid import Connection, InMemoryBucketBroker, InMemoryMessageBroker, Repid
 
 
 @pytest.fixture(scope="session")
 def event_loop() -> Iterator[asyncio.AbstractEventLoop]:
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     yield loop
     loop.close()
 
 
 @pytest.fixture()
 def fake_repid() -> Repid:
     return Repid(
         Connection(
-            DummyMessageBroker(),
-            DummyBucketBroker(),
-            DummyBucketBroker(use_result_bucket=True),
+            InMemoryMessageBroker(),
+            InMemoryBucketBroker(),
+            InMemoryBucketBroker(use_result_bucket=True),
         ),
     )
 
 
 @pytest.fixture()
 async def fake_connection(fake_repid: Repid) -> AsyncIterator[Connection]:
     async with fake_repid.magic(auto_disconnect=True) as conn:
```

### Comparing `repid-1.1.1/tests/integration/conftest.py` & `repid-1.2.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/integration/test_buckets.py` & `repid-1.2.0/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/integration/test_consumer.py` & `repid-1.2.0/tests/integration/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/integration/test_default_flow.py` & `repid-1.2.0/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/integration/test_no_messages_lost.py` & `repid-1.2.0/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_config.py` & `repid-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_connection.py` & `repid-1.2.0/tests/test_connection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,100 @@
 import pytest
 
-from repid import Connection, DummyBucketBroker, DummyMessageBroker
+from repid import Connection, InMemoryBucketBroker, InMemoryMessageBroker
 
 
 def test_result_bucket_check() -> None:
     Connection(
-        DummyMessageBroker(),
-        results_bucket_broker=DummyBucketBroker(use_result_bucket=True),
+        InMemoryMessageBroker(),
+        results_bucket_broker=InMemoryBucketBroker(use_result_bucket=True),
     )
 
     with pytest.raises(ValueError, match="Results bucket"):
         Connection(
-            DummyMessageBroker(),
-            results_bucket_broker=DummyBucketBroker(use_result_bucket=False),
+            InMemoryMessageBroker(),
+            results_bucket_broker=InMemoryBucketBroker(use_result_bucket=False),
         )
 
 
 def test_args_bucket_broker_shortcut() -> None:
     with_args_broker = Connection(
-        DummyMessageBroker(),
-        args_bucket_broker=DummyBucketBroker(),
+        InMemoryMessageBroker(),
+        args_bucket_broker=InMemoryBucketBroker(),
     )
-    with_args_broker._ab
+    with_args_broker._ab  # noqa: B018
 
-    without_args_broker = Connection(DummyMessageBroker())
+    without_args_broker = Connection(InMemoryMessageBroker())
     with pytest.raises(ValueError, match="Args bucket broker"):
-        without_args_broker._ab
+        without_args_broker._ab  # noqa: B018
 
 
 def test_result_bucket_broker_shortcut() -> None:
     with_result_broker = Connection(
-        DummyMessageBroker(),
-        results_bucket_broker=DummyBucketBroker(use_result_bucket=True),
+        InMemoryMessageBroker(),
+        results_bucket_broker=InMemoryBucketBroker(use_result_bucket=True),
     )
-    with_result_broker._rb
+    with_result_broker._rb  # noqa: B018
 
-    without_result_broker = Connection(DummyMessageBroker())
+    without_result_broker = Connection(InMemoryMessageBroker())
     with pytest.raises(ValueError, match="Results bucket broker"):
-        without_result_broker._rb
+        without_result_broker._rb  # noqa: B018
 
 
 async def test_is_open() -> None:
-    conn = Connection(DummyMessageBroker())
+    conn = Connection(InMemoryMessageBroker())
 
     assert not conn.is_open
 
     await conn.connect()
     assert conn.is_open
 
     await conn.disconnect()
     assert not conn.is_open
 
 
 def test_sets_middleware() -> None:
     msg_broker, args_broker, result_broker = (
-        DummyMessageBroker(),
-        DummyBucketBroker(),
-        DummyBucketBroker(use_result_bucket=True),
+        InMemoryMessageBroker(),
+        InMemoryBucketBroker(),
+        InMemoryBucketBroker(use_result_bucket=True),
     )
 
     assert msg_broker._signal_emitter is None
     assert args_broker._signal_emitter is None
     assert result_broker._signal_emitter is None
 
     Connection(msg_broker, args_broker, result_broker)
 
     assert msg_broker._signal_emitter is not None
     assert args_broker._signal_emitter is not None
     assert result_broker._signal_emitter is not None
+
+
+def test_in_memory_renaming_deprecation() -> None:
+    from repid import DummyBucketBroker, DummyMessageBroker
+
+    with pytest.warns(
+        DeprecationWarning,
+        match="DummyBucketBroker was renamed to InMemoryBucketBroker.",
+    ):
+        DummyBucketBroker()
+
+    with pytest.warns(
+        DeprecationWarning,
+        match="DummyBucketBroker was renamed to InMemoryBucketBroker.",
+    ):
+        DummyBucketBroker(use_result_bucket=True)
+
+    with pytest.warns(
+        DeprecationWarning,
+        match="DummyMessageBroker was renamed to InMemoryMessageBroker.",
+    ):
+        DummyMessageBroker()
+
+
+def test_in_memory_module_renaming_deprecation() -> None:
+    with pytest.warns(
+        DeprecationWarning,
+        match="Module repid.connections.dummy was renamed to repid.connections.in_memory",
+    ):
+        from repid.connections.dummy import DummyBucketBroker, DummyMessageBroker  # noqa: F401
```

### Comparing `repid-1.1.1/tests/test_consumer.py` & `repid-1.2.0/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_consumer_abc.py` & `repid-1.2.0/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_default_data_models.py` & `repid-1.2.0/tests/test_default_data_models.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_hypothesis.py` & `repid-1.2.0/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_job.py` & `repid-1.2.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_middleware.py` & `repid-1.2.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_multiprocessing.py` & `repid-1.2.0/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_pydantic.py` & `repid-1.2.0/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_router.py` & `repid-1.2.0/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_serializer.py` & `repid-1.2.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/tests/test_worker.py` & `repid-1.2.0/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.1/PKG-INFO` & `repid-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.1.1
+Version: 1.2.0
 Summary: Repid framework: simple to use, fast to run and extensible to adopt job scheduler
 Author-Email: aleksul <me@aleksul.space>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,17 +18,20 @@
 Project-URL: Repository, https://github.com/aleksul/repid
 Project-URL: Tracker, https://github.com/aleksul/repid/issues
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions<5.0.0,>=4.3.0; python_version < "3.10"
 Requires-Dist: aiormq<7.0.0,>=6.4.0; extra == "amqp"
 Requires-Dist: croniter<2.0.0,>=1.3.4; extra == "cron"
 Requires-Dist: redis<5.0.0,>=4.3.3; extra == "redis"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
 Provides-Extra: amqp
 Provides-Extra: cron
 Provides-Extra: redis
+Provides-Extra: test
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-configure-file { "MD013": { "line_length": 100 } } -->
 <!-- markdownlint-disable MD033 -->
 
 # repid
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: repid Version: 1.1.1 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.2.0 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Typing :: Typed Project-URL: Documentation, https://
 repid.aleksul.space Project-URL: Funding, https://github.com/sponsors/aleksul
 Project-URL: Repository, https://github.com/aleksul/repid Project-URL: Tracker,
 https://github.com/aleksul/repid/issues Requires-Python: >=3.8 Requires-Dist:
 typing-extensions<5.0.0,>=4.3.0; python_version < "3.10" Requires-Dist:
 aiormq<7.0.0,>=6.4.0; extra == "amqp" Requires-Dist: croniter<2.0.0,>=1.3.4;
-extra == "cron" Requires-Dist: redis<5.0.0,>=4.3.3; extra == "redis" Provides-
-Extra: amqp Provides-Extra: cron Provides-Extra: redis Description-Content-
-Type: text/markdown   # repid [Repid's_logo] [![PyPI version](https://
-img.shields.io/pypi/v/repid.svg)](https://pypi.org/project/repid/) [![codecov]
-(https://codecov.io/gh/aleksul/repid/branch/main/graph/
+extra == "cron" Requires-Dist: redis<5.0.0,>=4.3.3; extra == "redis" Requires-
+Dist: pytest; extra == "test" Requires-Dist: pytest-asyncio; extra == "test"
+Provides-Extra: amqp Provides-Extra: cron Provides-Extra: redis Provides-Extra:
+test Description-Content-Type: text/markdown   # repid [Repid's_logo] [![PyPI
+version](https://img.shields.io/pypi/v/repid.svg)](https://pypi.org/project/
+repid/) [![codecov](https://codecov.io/gh/aleksul/repid/branch/main/graph/
 badge.svg?token=IP3Z1VXB1G)](https://codecov.io/gh/aleksul/repid) [![Tests]
 (https://github.com/aleksul/repid/actions/workflows/tests.yaml/badge.svg)]
 (https://github.com/aleksul/repid/actions/workflows/tests.yaml) [![PyPI
 pyversions](https://img.shields.io/pypi/pyversions/repid.svg)](https://
 pypi.python.org/pypi/repid/) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Read
 documentation](https://img.shields.io/badge/read-documentation-
```

