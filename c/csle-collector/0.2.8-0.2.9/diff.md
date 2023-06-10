# Comparing `tmp/csle_collector-0.2.8.tar.gz` & `tmp/csle_collector-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_collector-0.2.8.tar", last modified: Sun Jun  4 08:48:11 2023, max compression
+gzip compressed data, was "csle_collector-0.2.9.tar", last modified: Sun Jun  4 09:08:33 2023, max compression
```

## Comparing `csle_collector-0.2.8.tar` & `csle_collector-0.2.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:11.003833 csle_collector-0.2.8/
--rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-06-04 08:48:11.003833 csle_collector-0.2.8/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     5807 2023-03-28 14:03:22.000000 csle_collector-0.2.8/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-03-28 14:03:22.000000 csle_collector-0.2.8/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1454 2023-06-04 08:48:11.003833 csle_collector-0.2.8/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_collector-0.2.8/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.995833 csle_collector-0.2.8/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.995833 csle_collector-0.2.8/src/csle_collector/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 08:47:59.000000 csle_collector-0.2.8/src/csle_collector/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.995833 csle_collector-0.2.8/src/csle_collector/client_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/client_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9971 2023-06-04 08:31:35.000000 csle_collector-0.2.8/src/csle_collector/client_manager/client_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5660 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/client_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/client_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/client_manager/client_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4316 2023-05-30 09:03:51.000000 csle_collector-0.2.8/src/csle_collector/client_manager/client_population_metrics.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/client_manager/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:40:47.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2379 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9508 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/client.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      340 2023-05-30 13:25:09.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/client_arrival_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2140 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/constant_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2859 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1780 2023-05-30 09:45:21.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/eptmp_rate_function.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2695 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3098 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/sine_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2447 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/spiking_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5539 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/workflow_markov_chain.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5131 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/workflow_service.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5302 2023-06-04 08:47:18.000000 csle_collector-0.2.8/src/csle_collector/client_manager/dao/workflows_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4061 2023-06-04 07:38:33.000000 csle_collector-0.2.8/src/csle_collector/client_manager/query_clients.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/client_manager/threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:20:57.000000 csle_collector-0.2.8/src/csle_collector/client_manager/threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6971 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/threads/arrival_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      971 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/threads/client_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2374 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/client_manager/threads/producer_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    36309 2023-04-18 12:48:07.000000 csle_collector-0.2.8/src/csle_collector/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12394 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13540 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4589 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8801 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3994 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/elk_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/elk_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10740 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5923 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5768 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/elk_manager/query_elk_server.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/host_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      875 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/failed_login_attempt.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    65375 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/host_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13966 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/host_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    28800 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/host_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    33850 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/host_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7783 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/host_metrics.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16572 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/query_host_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1292 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/host_manager/successful_login.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/kafka_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/kafka_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6616 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4116 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1442 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3233 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/kafka_manager/query_kafka_server.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.999833 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2931 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10847 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11386 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7479 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13329 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5377 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:11.003833 csle_collector-0.2.8/src/csle_collector/ryu_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ryu_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ryu_manager/query_ryu_server.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18068 2023-04-18 12:46:51.000000 csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4363 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8368 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2086 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:11.003833 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5787 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7996 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_alert.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11779 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9176 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13005 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8283 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16748 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4288 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:11.003833 csle_collector-0.2.8/src/csle_collector/traffic_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/traffic_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2534 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/traffic_manager/query_traffic_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7492 2023-06-04 07:11:42.000000 csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3087 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1477 2023-03-28 14:03:22.000000 csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:48:10.995833 csle_collector-0.2.8/src/csle_collector.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-06-04 08:48:10.000000 csle_collector-0.2.8/src/csle_collector.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     5103 2023-06-04 08:48:10.000000 csle_collector-0.2.8/src/csle_collector.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 08:48:10.000000 csle_collector-0.2.8/src/csle_collector.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.2.8/src/csle_collector.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      293 2023-06-04 08:48:10.000000 csle_collector-0.2.8/src/csle_collector.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       15 2023-06-04 08:48:10.000000 csle_collector-0.2.8/src/csle_collector.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.605212 csle_collector-0.2.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-06-04 09:08:33.605212 csle_collector-0.2.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5807 2023-03-28 14:03:22.000000 csle_collector-0.2.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-03-28 14:03:22.000000 csle_collector-0.2.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1454 2023-06-04 09:08:33.605212 csle_collector-0.2.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_collector-0.2.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.593211 csle_collector-0.2.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.597211 csle_collector-0.2.9/src/csle_collector/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 09:08:20.000000 csle_collector-0.2.9/src/csle_collector/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.597211 csle_collector-0.2.9/src/csle_collector/client_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/client_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9971 2023-06-04 08:31:35.000000 csle_collector-0.2.9/src/csle_collector/client_manager/client_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5660 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/client_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/client_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/client_manager/client_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4316 2023-05-30 09:03:51.000000 csle_collector-0.2.9/src/csle_collector/client_manager/client_population_metrics.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.597211 csle_collector-0.2.9/src/csle_collector/client_manager/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:40:47.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2379 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9508 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/client.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      340 2023-05-30 13:25:09.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/client_arrival_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2140 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/constant_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2859 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1780 2023-05-30 09:45:21.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/eptmp_rate_function.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2695 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3098 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/sine_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2447 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/spiking_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5540 2023-06-04 09:07:27.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/workflow_markov_chain.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5131 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/workflow_service.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5302 2023-06-04 08:47:18.000000 csle_collector-0.2.9/src/csle_collector/client_manager/dao/workflows_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4061 2023-06-04 07:38:33.000000 csle_collector-0.2.9/src/csle_collector/client_manager/query_clients.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.597211 csle_collector-0.2.9/src/csle_collector/client_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:20:57.000000 csle_collector-0.2.9/src/csle_collector/client_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6971 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/threads/arrival_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      971 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/threads/client_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2374 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/client_manager/threads/producer_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.597211 csle_collector-0.2.9/src/csle_collector/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    36309 2023-04-18 12:48:07.000000 csle_collector-0.2.9/src/csle_collector/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.601211 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12394 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13540 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4589 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8801 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3994 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.601211 csle_collector-0.2.9/src/csle_collector/elk_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/elk_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10740 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5923 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5768 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/elk_manager/query_elk_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.601211 csle_collector-0.2.9/src/csle_collector/host_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      875 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/failed_login_attempt.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    65375 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13966 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/host_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28800 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/host_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33850 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/host_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7783 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/host_metrics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16572 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/query_host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1292 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/host_manager/successful_login.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.601211 csle_collector-0.2.9/src/csle_collector/kafka_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/kafka_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6616 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4116 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1442 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3233 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/kafka_manager/query_kafka_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.601211 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2931 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10847 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11386 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7479 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13329 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5377 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.601211 csle_collector-0.2.9/src/csle_collector/ryu_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ryu_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ryu_manager/query_ryu_server.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18068 2023-04-18 12:46:51.000000 csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4363 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8368 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2086 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.605212 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5787 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7996 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11779 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9176 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13005 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8283 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16748 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4288 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.605212 csle_collector-0.2.9/src/csle_collector/traffic_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/traffic_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2534 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/traffic_manager/query_traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7492 2023-06-04 07:11:42.000000 csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3087 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1477 2023-03-28 14:03:22.000000 csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:08:33.597211 csle_collector-0.2.9/src/csle_collector.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-06-04 09:08:33.000000 csle_collector-0.2.9/src/csle_collector.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5103 2023-06-04 09:08:33.000000 csle_collector-0.2.9/src/csle_collector.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 09:08:33.000000 csle_collector-0.2.9/src/csle_collector.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.2.9/src/csle_collector.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      293 2023-06-04 09:08:33.000000 csle_collector-0.2.9/src/csle_collector.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       15 2023-06-04 09:08:33.000000 csle_collector-0.2.9/src/csle_collector.egg-info/top_level.txt
```

### Comparing `csle_collector-0.2.8/PKG-INFO` & `csle_collector-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_collector
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.2.8/README.md` & `csle_collector-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/pyproject.toml` & `csle_collector-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/setup.cfg` & `csle_collector-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/client_manager.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/client_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/client_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/client_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/client_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/client_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/client_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/client_population_metrics.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/client_population_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/arrival_config.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/client.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/client.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/constant_arrival_config.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/eptmp_arrival_config.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/eptmp_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/eptmp_rate_function.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/eptmp_rate_function.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/sine_arrival_config.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/sine_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/spiking_arrival_config.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/spiking_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/workflow_markov_chain.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/workflow_markov_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,8 +145,8 @@
 
         :param obj: the object to instantiate from
         :return: the instantiated object
         """
         transition_matrix = []
         for i in range(len(obj.transition_matrix.rows)):
             transition_matrix.append(obj.transition_matrix.rows[i].probabilities)
-        return WorkflowMarkovChain(id=obj.id, initial_state=obj.intial_state, transition_matrix=transition_matrix)
+        return WorkflowMarkovChain(id=obj.id, initial_state=obj.initial_state, transition_matrix=transition_matrix)
```

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/workflow_service.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/workflow_service.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/dao/workflows_config.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/dao/workflows_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/query_clients.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/query_clients.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/threads/arrival_thread.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/threads/arrival_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/threads/client_thread.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/threads/client_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/client_manager/threads/producer_thread.py` & `csle_collector-0.2.9/src/csle_collector/client_manager/threads/producer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/constants/constants.py` & `csle_collector-0.2.9/src/csle_collector/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats.py` & `csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_manager.py` & `csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/docker_stats_manager/docker_stats_util.py` & `csle_collector-0.2.9/src/csle_collector/docker_stats_manager/docker_stats_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py` & `csle_collector-0.2.9/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager.py` & `csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/elk_manager/elk_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/elk_manager/elk_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/elk_manager/query_elk_server.py` & `csle_collector-0.2.9/src/csle_collector/elk_manager/query_elk_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/failed_login_attempt.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/failed_login_attempt.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/host_manager.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/host_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/host_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/host_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/host_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/host_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/host_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/host_metrics.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/host_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/query_host_manager.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/query_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/host_manager/successful_login.py` & `csle_collector-0.2.9/src/csle_collector/host_manager/successful_login.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager.py` & `csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/kafka_manager/kafka_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/kafka_manager/kafka_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/kafka_manager/query_kafka_server.py` & `csle_collector-0.2.9/src/csle_collector/kafka_manager/query_kafka_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py` & `csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py` & `csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py` & `csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py` & `csle_collector-0.2.9/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ryu_manager/query_ryu_server.py` & `csle_collector-0.2.9/src/csle_collector/ryu_manager/query_ryu_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager.py` & `csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/ryu_manager/ryu_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/ryu_manager/ryu_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_alert.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py` & `csle_collector-0.2.9/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/traffic_manager/query_traffic_manager.py` & `csle_collector-0.2.9/src/csle_collector/traffic_manager/query_traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager.py` & `csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager_pb2.py` & `csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py` & `csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector/traffic_manager/traffic_manager_util.py` & `csle_collector-0.2.9/src/csle_collector/traffic_manager/traffic_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.8/src/csle_collector.egg-info/PKG-INFO` & `csle_collector-0.2.9/src/csle_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-collector
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.2.8/src/csle_collector.egg-info/SOURCES.txt` & `csle_collector-0.2.9/src/csle_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

